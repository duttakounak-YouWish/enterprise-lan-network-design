# IP Addressing Table

Network Details

| Parameter | Value |
|---|---|
| Network | `192.168.10.0/24` |
| Subnet mask | `255.255.255.0` |
| Usable host range | `192.168.10.1` – `192.168.10.254` |
| Broadcast address | `192.168.10.255` |
| Default gateway | `192.168.10.1` |
| VLAN | VLAN 1 (default access LAN) |

Infrastructure

| Device | Interface | IP address | Subnet mask | Default gateway |
|---|---|---:|---|---:|
| Router | GigabitEthernet0/0 | `192.168.10.1` | `255.255.255.0` |
| Switch 1 | VLAN 1  | `192.168.10.2` | `255.255.255.0` | `192.168.10.1` |
| Switch 2 | VLAN 1  | `192.168.10.3` | `255.255.255.0` | `192.168.10.1` |

End Devices

| Department / Device | Hostname | IP address | Subnet mask | Default gateway |
|---|---|---:|---|---:|
| HR | HR-PC1 | `192.168.10.11` | `255.255.255.0` | `192.168.10.1` |
| HR | HR-PC2 | `192.168.10.12` | `255.255.255.0` | `192.168.10.1` |
| HR | HR-PC3 | `192.168.10.13` | `255.255.255.0` | `192.168.10.1` |
| Finance | FIN-PC4 | `192.168.10.21` | `255.255.255.0` | `192.168.10.1` |
| Finance | FIN-PC5 | `192.168.10.22` | `255.255.255.0` | `192.168.10.1` |
| Finance | FIN-PC6 | `192.168.10.23` | `255.255.255.0` | `192.168.10.1` |
| IT | IT-PC7 | `192.168.10.31` | `255.255.255.0` | `192.168.10.1` |
| IT | IT-PC8 | `192.168.10.32` | `255.255.255.0` | `192.168.10.1` |
| IT | IT-PC9 | `192.168.10.33` | `255.255.255.0` | `192.168.10.1` |
| Server | SERVER1 | `192.168.10.100` | `255.255.255.0` | `192.168.10.1` |

- All listed devices use the same `/24` subnet.
- Configure the listed gateway on every PC and on the server.
- Switch management IPs are configured on the VLAN 1 switched virtual interface (SVI).
- VLAN 2 is not used in this final single-subnet design.
- Assign each end-device IP to the matching device in Packet Tracer. Hostnames in this table are suggested labels; retain the labels used in your actual topology if they differ.
