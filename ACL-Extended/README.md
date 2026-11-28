# Extended ACL Configuration – Cisco Packet Tracer Lab

## Objective
Configure an Extended Access Control List (ACL) to control communication between specific devices on different VLANs. The goal is to prevent PC1 and PC2 from reaching PC4 while allowing other network traffic.

## Network Equipment
- 1 Cisco 1941 Router
- 2 Cisco 2960 Switches
- 4 PCs

## Skills Demonstrated
- VLAN configuration
- Inter-VLAN routing
- Router subinterfaces
- 802.1Q trunking
- Extended ACL configuration
- Traffic filtering by source and destination IP address
- Network troubleshooting

## VLAN Configuration

| VLAN | Network | Default Gateway |
|---|---|---|
| VLAN 10 | 192.168.10.0/24 | 192.168.10.1 |
| VLAN 20 | 192.168.20.0/24 | 192.168.20.1 |
| VLAN 30 | 192.168.30.0/24 | 192.168.30.1 |

## IP Addressing

| Device | IP Address | VLAN |
|---|---|---|
| PC1 | 192.168.10.10 | 10 |
| PC2 | 192.168.10.11 | 10 |
| PC3 | 192.168.20.10 | 20 |
| PC4 | 192.168.30.10 | 30 |

Subnet Mask: 255.255.255.0

## Cisco Technologies
- VLANs 10, 20, and 30
- Inter-VLAN Routing
- Router Subinterfaces
- 802.1Q Trunking
- Extended ACL (Access Control List)

## Testing and Verification
- Verified communication between devices before applying the ACL.
- Verified all PCs could reach their default gateways.
- Tested communication between VLANs.
- Configured an Extended ACL to block PC1 and PC2 from reaching PC4.
- Verified other network communication remained permitted.
- Used `show access-lists` to verify ACL matches.

## Conclusion
Successfully configured inter-VLAN routing and an Extended ACL to control traffic between specific source and destination IP addresses. This lab demonstrates how network administrators can restrict access to individual devices without blocking all communication between VLANs.

