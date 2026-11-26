Enterprise LAN Network Design

Project Overview
This project demonstrates the design and configuration of a small enterprise LAN using Cisco Packet Tracer. The network connects HR, Finance and IT workstations, a server, two access switches and one router.

Objectives
- Build a connected LAN using Cisco router and switch devices.
- Configure IPv4 addressing for end devices and network infrastructure.
- Configure switch management interfaces.
- Verify end-to-end connectivity using ICMP ping.
- Inspect switch MAC address tables to confirm Layer 2 learning.

Network Topology
| Device | Model | Hostname / Role |
|---|---|---|
| Router | Cisco 2911 | R1 |
| Switch 1 | Cisco 2960 | SW1 |
| Switch 2 | Cisco 2960 | SW2 |
| End devices | PCs | 3 HR, 3 Finance, 3 IT |
| Server | Server-PT | Enterprise server |

Physical connections
- R1 GigabitEthernet0/0 connects to SW1 GigabitEthernet0/1.
- SW1 GigabitEthernet0/2 connects to SW2 GigabitEthernet0/1.
- PCs and the server connect to the access switches.

IP Addressing
The project uses one IPv4 subnet: `192.168.10.0/24`.

- Network address: `192.168.10.0`
- Subnet mask: `255.255.255.0`
- Default gateway: `192.168.10.1`
- Broadcast address: `192.168.10.255`

See [ip-addressing-table.md] for the complete addressing plan.

Configuration command references are provided in:
- [router-configuration.txt](router-configuration.txt)
- [switch1-configuration.txt](switch1-configuration.txt)
- [switch2-configuration.txt](switch2-configuration.txt)

These files document the intended final single-subnet design.
Verification
Used the following checks in Packet Tracer:

1. Confirmed router `GigabitEthernet0/0` is up/up.
2. Confirmed Switch 1 and Switch 2 management SVIs are up/up.
3. From PC, ping the default gateway (`192.168.10.1`).
4. Ping the server (`192.168.10.100`) from a PC.

For this project, all devices are in the same `192.168.10.0/24` subnet and use the default access VLAN (VLAN 1).

## Project Status
The Packet Tracer simulation and screenshots are maintained separately in this repository. The configuration files are documentation of the intended final setup;
