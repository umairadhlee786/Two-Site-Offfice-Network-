# Two-Site-Offfice-Network
A Cisco Packet tracer simulation of a two-site office network 

This project demonstrates the design and implementation of a secure and scalable enterprise network connecting a Branch office and Headquarters (HQ) using Cisco networking technologies.

Overview
The network supports VLAN segmentation, inter-VLAN routing, dynamic routing with OSPFv2, Internet connectivity via static routing, DHCP (server and relay), NAT (static and PAT), wireless LAN (WLAN), and access control through ACLs.
The design uses VLSM-based IP addressing across 192.168.0.0/24 (Branch) and 172.10.0.0/24 (HQ) to efficiently allocate address space.

Key Features
VLANs and Inter-VLAN Routing
VLAN 10 (students), VLAN 20 (staff), and VLAN 99 (management) are configured. Inter-VLAN routing is implemented using a router-on-a-stick approach.

Routing
OSPFv2 is configured across all routers in Area 0 with proper router ID assignment and default route propagation. Static routing is used at the network edge to enable Internet access.

NAT
Static NAT is configured to allow external access to an internal host. Dynamic PAT (overload) is implemented to enable multiple internal users to share a public IP for Internet access.

DHCP
A centralized DHCP server is configured at HQ, with DHCP relay enabled on branch networks to ensure automatic IP address assignment across VLANs.

WLAN
A wireless network is configured with SSID “LANE” using WPA2-AES security. Wireless clients receive IP addresses dynamically and have full network and Internet connectivity.

Security (ACLs)
Access Control Lists are used to restrict unauthorized remote access and control traffic flow between internal networks.

Validation and Testing
Full end-to-end connectivity was successfully verified across all VLANs, LANs, and WLAN clients. Internet access was confirmed, external access to the internal server via static NAT was validated, OSPF routing was stable, and all ACL policies were enforced as required.

Troubleshooting
During implementation, several issues were identified and resolved, including OSPF neighbor state problems, NAT misconfigurations, missing DHCP relay settings, VLAN mismatches, and wireless connectivity issues.
Repository Contents
The repository includes the Cisco Packet Tracer (.pkt) file containing the complete network configuration and a high level topology diagram. 

Learning Outcomes
This project demonstrates practical skills in enterprise network design, routing and switching, network security, and troubleshooting. It reflects the ability to build and validate a fully functional, secure, and scalable network solution.
