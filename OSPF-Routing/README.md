# OSPF Routing – Cisco Packet Tracer Lab

## Objective
Configure Open Shortest Path First (OSPF) across three Cisco routers to dynamically exchange routing information and allow communication between multiple LAN networks.

## Network Equipment
- 3 Cisco 1941 Routers
- 2 Cisco 2960 Switches
- 4 PCs

## Network Addressing

| Device | Interface | IP Address |
|---|---|---|
| R1 | G0/0 | 10.0.0.1/30 |
| R1 | G0/1 | 192.168.10.1/24 |
| R2 | G0/0 | 10.0.0.2/30 |
| R2 | G0/1 | 10.0.0.5/30 |
| R3 | G0/0 | 192.168.20.1/24 |
| R3 | G0/1 | 10.0.0.6/30 |

## PC Addressing

| Device | IP Address | Default Gateway |
|---|---|---|
| PC1 | 192.168.10.11 | 192.168.10.1 |
| PC2 | 192.168.10.12 | 192.168.10.1 |
| PC3 | 192.168.20.11 | 192.168.20.1 |
| PC4 | 192.168.20.12 | 192.168.20.1 |

Subnet mask for PCs: 255.255.255.0

## Skills Demonstrated
- OSPF configuration
- Dynamic routing
- OSPF neighbor relationships
- OSPF Area 0
- Network advertisement
- Routing table verification
- Multi-router communication
- Connectivity testing

## Cisco Technologies
- OSPF
- IPv4
- Dynamic routing
- Routing tables

## Testing and Verification
- Verify interfaces using `show ip interface brief`.
- Verify OSPF neighbors using `show ip ospf neighbor`.
- Verify OSPF routes using `show ip route`.
- Verify OSPF configuration using `show ip protocols`.
- Test connectivity between all PCs across different networks.

## Conclusion
This lab demonstrates how OSPF dynamically exchanges routing information between multiple routers, allowing different networks to communicate without manually configuring static routes.
