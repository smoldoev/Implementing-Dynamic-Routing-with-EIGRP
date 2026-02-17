# Enterprise WAN Network with EIGRP (Cisco Packet Tracer)

## Project Overview
This project demonstrates a WAN network topology connecting a Headquarters (HQ) and a Branch Office through an ISP router using the EIGRP dynamic routing protocol.

The main goal of this project is to show how EIGRP enables communication between remote networks even when traffic must traverse intermediate routers.

## Network Topology

The topology includes:
- 3 Routers (HQ Router, Branch Router, ISP Router)
- 2 LAN Networks (HQ and Branch)
- Serial WAN connections
- End devices for connectivity testing

HQ Network: 192.168.10.0/24  
Branch Network: 192.168.30.0/24  

## Technologies Used
- EIGRP (Enhanced Interior Gateway Routing Protocol)
- Serial WAN Links
- IP Addressing & Subnetting
- Router-to-Router communication
- End-to-End connectivity testing (ICMP / ping)

## Project Objectives
- Configure dynamic routing using EIGRP
- Establish WAN communication between two geographically separated offices
- Verify routing tables
- Demonstrate successful end-to-end connectivity using ping
- Show how EIGRP automatically shares routes between routers

## How It Works

1. EIGRP is enabled on all three routers.
2. Each router advertises its directly connected networks.
3. Routers exchange routing information dynamically.
4. HQ users can successfully ping Branch users through the ISP router.
5. This proves that EIGRP correctly builds routing tables and selects the best path.

## 📡 Verification

- `show ip route`
- `show ip eigrp neighbors`
- `ping 192.168.30.10` from HQ
- `ping 192.168.10.10` from Branch

Successful ICMP replies confirm proper EIGRP operation.

## Learning Outcome

This project demonstrates:
- Practical WAN routing configuration
- Understanding of dynamic routing protocols
- EIGRP neighbor relationship establishment
- Real-world enterprise network design principles

## Author
Sabyr Moldoev  
Cybersecurity Student | Networking Enthusiast
