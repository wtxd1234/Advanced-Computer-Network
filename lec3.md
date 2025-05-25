# Data Center Networking and Terminologies

## Part A Recap

(See previous notes for foundational concepts: definitions, topologies, types, importance, challenges, trends.)

---

## Part B: Detailed Data Center Components & Design Principles

### 1. Data Center Definition

* **Data Center (Datacenter/Data Centre):** A facility composed of networked computers, storage systems, and computing infrastructure used to **assemble, process, store, and disseminate** large amounts of data. It includes the physical building(s), power and cooling systems, and security measures. ⭐

### 2. Types of Data Centers

* **Enterprise Data Center:** Owned and operated by a single organization.
* **Colocation Data Center:** Multiple customers share space, power, cooling, and security.
* **Hyperscale Data Center:** Operated by large cloud providers (e.g., AWS, Google, Azure) with massive scale.
* **Edge/Container-Based Data Center:** Modular units for rapid deployment or disaster recovery (e.g., trailers with built-in cooling and power). ⭐

### 3. Switch Classes & Port Speeds

* **Access/Leaf Switches:** Typically **48×25G** or **48×100G** server-facing ports plus **8×400G** uplinks.
* **Aggregation/Spine Switches:** **32–64×400G/800G** high-speed ports.
* **Super-Spine/Director-Class Switches:** Emerging **1.6T-ready** chassis with up to **128×800G** ports (e.g., Juniper PTX10008). ⭐ Memorize typical port counts for each class.

### 4. Data Center Networking Layers

1. **Core Layer:** High-speed backbone; runs routing protocols like **OSPF/BGP**; no single point of failure (SPOF). Core switches route packets at maximum speed. ⭐
2. **Aggregation/Distribution Layer:** Layer 2/3 demarcation; processes north-south and east-west traffic; categorizes and forwards to correct workgroups.
3. **Access Layer:** Server connectivity; includes Top-of-Rack (ToR) and blade chassis switches; provides Layer 2 connectivity for end systems.

### 5. Power over Ethernet (PoE)

* **Definition:** Supplies power and data over the same cable; ideal for IP phones and wireless APs.
* **Benefit:** Flexibility in endpoint placement without separate power outlets. ⭐

### 6. Container-Based Data Centers

* **Description:** Pre-fabricated modules (trailers) with built-in cooling, power, and networking.
* **Use Cases:** Rapid deployment, disaster recovery in remote sites.
* **Vendors:** Cisco, IBM, SGI, Oracle. ⭐

### 7. Design Principles

* **Resiliency:** No single point of failure; redundant core and aggregation paths.
* **Scalability:** Modular expansion via additional spine/leaf modules.
* **Manageability:** Simplified cabling (e.g., structured pods), standardized configurations.

### 8. Standards & Best Practices

* **TIA-942:** Data center design standard defining Tier 1–4 availability:

  * **Tier I:** Basic capacity, 99.671% uptime.
  * **Tier II:** Redundant components, 99.741% uptime.
  * **Tier III:** Concurrent maintainability, 99.982% uptime.
  * **Tier IV:** Fault tolerant, 99.995% uptime. ⭐ Know the four tiers and their features.

### 9. Common Issues

* **Congestion & Backpressure:** Packet buildup when buffers fill; resolved by high-capacity core switches.
* **Cooling & Power:** Significant energy and heat; requires efficient HVAC and UPS systems.
* **Security:** Physical access controls, network segmentation, IDS/IPS systems.

### 10. Future Trends

* **Higher Data Rates:** Moving from **400G** to **800G** and **1.6T** fabrics.
* **AI/ML-Driven Management:** Automated traffic optimization and fault prediction.
* **Software-Defined Data Centers (SDDC):** Virtualization of compute, storage, and networking resources. ⭐

---

*Keep these notes handy for exam revision—focus on starred (⭐) items!*
