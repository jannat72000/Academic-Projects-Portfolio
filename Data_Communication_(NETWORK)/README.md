# 🌐 Data Communication & Network Simulation (EIGRP)

This project focuses on designing and implementing a robust network infrastructure using dynamic routing protocols to ensure seamless data communication across multiple subnets.

---

## 📌 Project Summary
The project involved building a hierarchical network topology designed for small to medium-sized organizations. The architecture connects six workstations (PCs) across three distinct local area networks (LANs), bridged by three routers and three switches.

### **Core Components & Technologies Used:**

* **Network Topology:** A hierarchical design using **3 Routers, 3 Switches, and 6 PCs**.
* **Routing Protocol:** **EIGRP (Enhanced Interior Gateway Routing Protocol)** was implemented (AS 10) to facilitate efficient dynamic routing and fast convergence between subnets.
* **IP Addressing:** A structured **Class C IP addressing** scheme was applied across six logical segments (3 LANs and 3 WAN interconnections).
* **Simulation Tool:** **Cisco Packet Tracer** was used for designing the environment, configuring the hardware interfaces, and simulating real-time traffic.

---

## 🚀 Key Accomplishments

* **Subnetting & Gateway Setup:** Configured distinct network addresses (`192.168.1.0` through `192.168.6.0`) with dedicated gateways for each departmental segment.
* **Dynamic Path Selection:** Enabled routers to automatically share routing tables and determine the most efficient paths for data packets.
* **End-to-End Connectivity:** Successfully validated communication across the entire network, specifically verifying a 100% success rate for **PING operations** between devices on non-adjacent routers (e.g., PC1 to PC6).
* **Performance Verification:** Achieved stable data transfer with minimal latency (average round-trip time of **1ms**).

---

## 📂 Repository Contents
* `Network_Design.pkt`: The original Cisco Packet Tracer simulation file.
* `Project_Report.pdf`: Full documentation covering the network problem statement and technical objectives.
* `Screenshots/`: Visual proof of successful PING operations and the finalized network topology.

---

**Contributor:** **Jannatul Ferdous Salma** | Dept. of CSE, **East West University** Course: Data Communication
