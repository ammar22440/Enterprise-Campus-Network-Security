# Enterprise Campus Network & Security Infrastructure

An enterprise-level network infrastructure designed and simulated using Cisco Packet Tracer. Features dynamic routing, high availability, inter-VLAN routing, and access control security policies.

![Topology Network Diagram](topology.png)

## Core Network Architecture & Features

- **Multi-Zone Network Segmentation:** Configured 4 isolated VLANs (Admin, Staff, Guest, DMZ Server Farm) with Router-on-a-Stick inter-VLAN routing.
- **High Availability & Link Aggregation:** Implemented **LACP EtherChannel** between core switches to double link bandwidth and provide fault tolerance.
- **Dynamic Routing Protocol:** Configured **OSPF Area 0** across WAN links between HQ and Branch sites.
- **Access Control & Security (Zero-Trust):** Applied **Extended Access Control Lists (ACLs)** to block Guest VLAN access to Admin and Server subnets.
- **Access Layer Security:** Enabled **Sticky Port Security** on access ports to prevent unauthorized device access.

## Verification & Testing
- ICMP End-to-End connectivity verified from Admin PC to DMZ Server (`192.168.40.10`).
- Extended ACL verification: Guest PC traffic restricted from sensitive infrastructure subnets with 100% enforcement.
