# Multi-Campus-Educational-Institution-Network-Design
<b><h3>Multi-Campus Educational Institution network design using Cisco Packet Tracer</b></h3>

<h3> <b> Background </b></h3>
A private educational institution operates from a Head Office (Main Campus) and two Branch Campuses (Branch 01 and Branch 02). 
Due to the increase in student intake, academic departments, and administrative staff, the institution requires a robust, scalable, 
and centrally managed enterprise network.<br><br>

<b>The organization must ensure:</b>

Secure separation of departments
Centralized services
Reliable inter-campus connectivity
Internet access through an ISP

**This project demonstrates:**
- VLAN configuration
- Inter-VLAN routing
- DHCP
- WAN connectivity between Head Office and Branches

<h3> <b> Network Architecture Overview </b></h3>
  
<h2> <b>1. Head Office (Main Campus) </b> </h2>

The Head Office functions as the core network hub and hosts centralized services.

Departments at Head Office:

- IT & Server Room<br>
- HR & Finance<br>
- Lecture Rooms<br>
- Student Labs<br>
- Administrative Offices<br>


Infrastructure:

- Core Router connected to ISP<br>
- Multilayer Switch for inter-VLAN routing<br>
- Multiple Access Switches per department<br>
- PCs, printers, and wireless laptops<br>

Functions:

- Inter-VLAN routing<br>
- Central DHCP services<br>
- Routing between campuses<br>
- Internet gateway access<br>

<h2> <b>2. Branch Office 01 </b> </h2>

Branch 01 supports academic and office operations.

Departments:
- Lecture Hall A
- Lecture Hall B
- Office Section

VLAN Implementation:

- VLAN 90 – Lecture Hall A (192.168.9.0/24)
- VLAN 100 – Lecture Hall B (192.168.10.0/24)

Infrastructure:

- Branch Router connected to Head Office
- Multilayer Switch
- Access Switches
- End devices (PCs, printers, laptops)

  <h2> <b>3. Branch Office 02 </b></h2>

Branch 02 focuses mainly on student practical labs and offices.

Departments:

- Student Lab 02
- Student Lab 03
- Office Section

VLAN Implementation:

- VLAN 70 – Student Lab 02 (192.168.7.0/24)
- VLAN 80 – Student Lab 03 (192.168.8.0/24)

Infrastructure:

- Branch Router connected via WAN
- Multilayer Switch
- Access Switches
- Wired and wireless end devices

 <h2> <b>WAN & ISP Connectivity </b></h2>

- All campuses are interconnected using WAN point-to-point links.
- The Head Office router acts as the central routing node.
- An ISP Cloud provides Internet access.
- A public-facing server is connected near the ISP for external services.

 <h3> <b>WAN IP addressing:</b></h3>

10.10.10.0/30<br>
10.10.10.4/30<br>
10.10.10.8/30<br>
10.10.10.12/30<br>

 <h2> <b>Routing & Network Services</b></h2>
 <h3> <b>Routing</b></h3>

- - Dynamic routing protocol is used to ensure:
- Automatic route learning
- Scalability
- Fault tolerance
- - (RIP v2 or OSPF suitable for this topology) --><b> In this Case I used RIP version 2</b>

<h3> <b>Services</b></h3>

- DHCP for all VLANs
- Centralized routing at Head Office
- End-to-end connectivity verified using ICMP (ping)

   <h2> <b>Security & Performance Benefits</b></h2>

- VLAN segmentation reduces broadcast traffic
- Department isolation improves security
- Centralized control simplifies management
- WAN routing ensures reliable inter-campus communication

  <h2> <b>Project Objectives</b></h2>

- Design a scalable multi-site enterprise network
- Implement VLANs and inter-VLAN routing
- Enable centralized services
- Ensure full connectivity across campuses
- Simulate real-world enterprise networking practices

  <h2> <b> Technologies Used</b></h2>

- Cisco Packet Tracer
- VLANs
- Multilayer Switching
- Dynamic Routing
- DHCP
- WAN Networking
- ISP Connectivity

  
Tool: Cisco Packet Tracer

<img width="1919" height="1079" alt="Project 5" src="https://github.com/user-attachments/assets/c3b0c517-7567-4906-8f0f-81eba7399bdf" />



