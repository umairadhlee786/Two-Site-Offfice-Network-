# Two-Site-Offfice-Network
A Cisco Packet tracer simulation of a two-site office network 

This project implements a secure and scalable network connecting a Branch and Headquarters (HQ) environment using Cisco Packet Tracer.

Overview

The network is designed to support segmented LANs, dynamic routing, secure Internet access, and centralized services. It uses VLSM-based addressing across separate Branch and HQ networks.


Core Components

  VLANs with inter-VLAN routing (router-on-a-stick)

OSPFv2 (Area 0) for dynamic routing across all routers

Static routing for Internet connectivity

NAT (Static and PAT) for internal-to-external communication

Centralized DHCP with relay for multi-network support

Secure WLAN with WPA2 encryption

ACLs for traffic filtering and access control


Key Outcomes

Full end-to-end connectivity across Branch, HQ, and WLAN

Internet access for all internal networks

External access to internal server via static NAT

Stable routing and enforced security policies


Repository Contents

Cisco Packet Tracer (.pkt) file with full network configuration

Project report (PDF) with detailed design and implementation
