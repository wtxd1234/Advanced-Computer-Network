# Advanced Computer Networks (NET3014) – 2025

## 1. Overview of the Internet

- **Internet as a "Network of Networks":**  
  - The Internet is not a single network but a vast, interconnected collection of networks.  
  - It connects **mobile networks**, **home networks**, **enterprise networks**, **regional/local ISPs**, **national/global ISPs**, **datacenter networks**, and **content provider networks**.

- **Core Components:**
  - **Packet Switches:** Devices (e.g., routers and switches) that **forward packets**—chunks of data.
  - **Communication Links:** Include **fiber-optic cables**, **copper**, **radio waves**, and **satellite links**. They determine the **transmission rate** (or bandwidth).
  - **Hosts:** Billions of computing devices (end systems) at the Internet’s edge running various network applications.

---

## 2. The Two Perspectives on the Internet

### A. The "Nuts and Bolts" View
- Focuses on the *physical structure* and *hardware components* of the Internet.
- **Important Elements:**
  - **Access Networks:** The starting point for connectivity; examples include:
    - **Mobile Network**
    - **Home Network**
    - **Enterprise Network**
  - **Intermediate Networks:** ISPs at various scales:
    - **Local/Regional ISPs**
    - **National/Global ISPs**
  - **Data Center Networks and Content Provider Networks:**  
    - Providers like **Google, Microsoft, Akamai** operate their private networks to deliver content quickly to end users.
- **Exam Tip:** Remember the layered view—from edge (hosts) to the core (routers and interconnections).

### B. The "Service" View
- Emphasizes the **services and applications** built on top of the network infrastructure.
- **Key Points:**
  - **Application Services:** The foundation for Web browsing, **streaming video**, **email**, **multimedia teleconferencing**, **e-commerce**, and **social media**.
  - **Programming Interfaces (APIs):** Provide "hooks" for distributed applications to connect and use the underlying Internet transport services.

---

## 3. Internet Structure and Scalability

### A. Stepwise Build-Up of the Internet
- **Network Edge:**
  - **Hosts:** Comprised of clients (end-user devices) and servers (often within data centers).
  - **Access Networks:** Use both **wired** and **wireless communication links**.
  
- **Network Core:**
  - **Interconnected Routers:** Form the backbone that ties multiple networks together into a cohesive whole.
  - **Scalability Challenge:**  
    - Directly connecting millions of access ISPs would lead to an **O(N²)** complexity, making such an approach impractical.

### B. Strategies to Overcome Scalability
- **Global Transit ISP Model:**  
  - **Concept:** Let every access ISP connect to one global transit ISP.  
  - **Challenge:** If economically viable, multiple competitors would arise, complicating the model.
  
- **Internet Exchange Points (IXPs):**  
  - **Role:** Allow ISPs to establish **peering links** and interconnect more efficiently without the need for each one to connect directly to every other.
  - **Additional Layer:** Regional networks can further connect local ISPs to larger transit networks.
  
- **Exam Tip:** Understand the economic and logistical reasons behind choosing IXPs over a fully meshed model.

---

## 4. Protocols, Standards, and the OSI Model

### A. Protocols in the Internet
- **Definition:** Protocols control how information is sent and received over the Internet.
- **Key Protocols Include:**  
  - **HTTP** (used in web browsing)  
  - **Streaming Protocols** (used for streaming video)  
  - **Skype Protocols** (for VoIP)  
  - **TCP/IP** (the fundamental protocols of the Internet)  
  - **WiFi and 4G** (for wireless communication)  
  - **Ethernet** (common in wired networks)
- **Standards Organizations:**
  - **RFC (Request for Comments):** Documents that describe methods, behaviors, research, or innovations applicable to the Internet.
  - **IETF (Internet Engineering Task Force):** Develops and promotes voluntary Internet standards.

### B. The OSI Model (Open Systems Interconnection)
- **Purpose:** A conceptual model used to understand and design network communications so that different systems can interoperate.
- **Seven Layers (Mnemonic Aid):**  
  - **Application Layer** – *All*
  - **Presentation Layer** – *People*
  - **Session Layer** – *Seem*
  - **Transport Layer** – *To*
  - **Network Layer** – *Need*
  - **Data Link Layer** – *Data*
  - **Physical Layer** – *Processing*
- **Exam Tip:** Be ready to explain the function of each layer and why the OSI model is important for network design.

---

## 5. Special Topics and Emerging Areas

- **Advanced Network Architectures:**
  - **Tier-1 ISPs:**  
    - Large commercial networks such as **Level 3, Sprint, AT&T,** and **NTT** that provide national and international connectivity.
  - **Content Provider Networks:**  
    - Companies like **Google** and **Facebook** often establish private networks to bypass traditional ISPs for performance and cost benefits.
  
- **Diverse Network Areas:**  
  - **Wireless Sensor Networks (WSN)**
  - **Body Area Networks (BAN)**
  - **Personal Area Networks (PAN)**
  - **Wired Networks** (such as those employing **5G**)
  - **Security Measures:** Overview of **Intrusion Prevention Systems (IPS)** and **Intrusion Detection Systems (IDS)**.
  
- **Emerging Concerns:**  
  - The integration of **Machine Learning (ML)** and **Security** in network management.
  - **Exam Tip:** Focus on how classical models are evolving with emerging network technologies.

---

## 6. Summary of Exam-Essential Points

- **Internet Structure:**  
  - Understand both the hardware ("nuts and bolts") and service perspectives of the Internet.
  
- **Core Components & Connectivity:**  
  - **Hosts, Packet Switches, Communication Links.**  
  - **Scalability Problems:** Why a full mesh among millions of ISPs is not practical; the role of **IXPs**.

- **Protocols and Standards:**  
  - Familiarize yourself with the key protocols (e.g., TCP/IP, HTTP) and the role of the **IETF** and **RFCs**.

- **OSI Model:**  
  - Memorize and be able to discuss each of the **seven layers**.

- **Economic and Organizational Models:**  
  - Understand the economic agreements between customer and provider ISPs, regional ISP roles, and the influence of national policies.

---

## Further Exploration

- **Deep Dive into Packet Switching:** Explore how modern routers and switches handle data.
- **Case Studies on ISP Interconnection:** Look into real-world examples of how regional and global ISPs form their networks.
- **Emerging Technologies in Networking:** Study the developments in Software Defined Networking (SDN) and how they might impact traditional network structures.
