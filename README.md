# Multi-site-VPN-using-Juniper-SRX
A secure multisite VPN network project using Juniper SRX firewalls to connect HQ (Lagos) with two branches (Abuja and Port Harcourt). Each site is segmented by VLANs for departmental isolation (Engineering, Finance, HR), and connected via IPsec VPN tunnels to ensure encrypted, reliable communication. 

## Topology
- 3 sites: Lagos (HQ), Abuja, Port Harcourt
- IPsec VPN for secure communication
- VLAN-based segmentation per site

Objectives

Ensure secure, encrypted communication between HQ and remote branches.

Enable inter-VLAN routing and inter-branch communication.

Implement structured IP addressing and subnetting for departmental segregation.

Use Juniper SRX devices for site security and routing.

Network Topology Summary

Headquarters (Lagos)

VLAN10 - Engineering: 172.16.1.0/26

VLAN20 - Finance: 172.16.1.64/27

VLAN30 - HR: 172.16.1.96/28

SRX loopback: 1.1.1.1

VPN links:

Lagos to Abuja: 100.100.100.0/30

Lagos to Port Harcourt: 100.100.100.4/30

Abuja Branch

VLAN10 - Engineering: 172.16.2.0/26

VLAN20 - Finance: 172.16.2.64/27

VLAN30 - HR: 172.16.2.96/28

SRX loopback: 2.2.2.2

Port Harcourt Branch

VLAN10 - Engineering: 172.16.3.0/26

VLAN20 - Finance: 172.16.3.64/27

VLAN30 - HR: 172.16.3.96/28

SRX loopback: 3.3.3.3

Technologies Used

Juniper SRX Series Gateways (firewall + routing)

IPsec VPN Tunnels

Inter-VLAN routing via iRBs

Layer 2 and Layer 3 switching

Private WAN addressing for tunnel connectivity

Features

Secure IPsec tunnels for Lagos-Abuja and Lagos-Port Harcourt

Logical VLAN assignment for departmental separation

Loopback interfaces for tunnel stability and reachability

## Configuration Files
Configuration snippets for each SRX device are in the `/configs` folder.

## Diagram
Network topology is available in `/multisite-topology.png`

## Author
Ephraim Ameh
