# Multi-site-VPN-using-Juniper-SRX
A secure multisite VPN network project using Juniper SRX firewalls to connect HQ (Lagos) with two branches (Abuja and Port Harcourt). Each site is segmented by VLANs for departmental isolation (Engineering, Finance, HR), and connected via IPsec VPN tunnels to ensure encrypted, reliable communication. 

## Topology
- 3 sites: Lagos (HQ), Abuja, Port Harcourt
- IPsec VPN for secure communication
- VLAN-based segmentation per site

## Configuration Files
Configuration snippets for each SRX device are in the `/configs` folder.

## Diagram
Network topology is available in `/diagrams/multisite-topology.png`

## Author
[Your Name]
