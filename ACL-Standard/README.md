# ACL (Standard) Configuration – Cisco Packet Tracer Lab

## Objective
Configure a numbered standard Access Control List (ACL) on a Cisco router to block traffic from a specific source IP address while allowing other network traffic.

This lab demonstrates how standard ACLs filter traffic based on source IP addresses.

## Network Equipment
- 1 Cisco 1941 Router
- 2 Cisco 2960 Switches
- 3 PCs

## Network Topology
- R1 G0/0 connects to SW1.
- R1 G0/1 connects to SW2.
- PC1 and PC2 connect to SW1.
- PC3 connects to SW2.

## IP Addressing

| Device | Interface | IP Address |
|---|---|---|
| R1 | G0/0 | 192.168.10.1 |
| R1 | G0/1 | 192.168.20.1 |
| PC1 | NIC | 192.168.10.11 |
| PC2 | NIC | 192.168.10.12 |
| PC3 | NIC | 192.168.20.11 |

Subnet Mask: `255.255.255.0`

## Access Control Policy
- Block all traffic originating from PC3 (192.168.20.10).
- Allow PC1 and PC2 to communicate normally.
- Use a standard ACL to filter traffic based on source IP address.

## Cisco Technologies
- Standard Access Control Lists (ACLs)
- Numbered ACLs
- Wildcard masks
- Permit and deny statements
- Inbound and outbound ACL application

## Testing and Verification
- Verify router interfaces using `show ip interface brief`.
- Display configured ACLs using `show access-lists`.
- Verify ACL application using `show running-config`.
- Test connectivity between PC1 and PC2.
- Test connectivity from PC3 to PC1 and PC2.
- Verify that PC3's traffic is denied.

## Conclusion
This lab demonstrates how standard ACLs control network traffic using source IP addresses. By denying a specific source IP address, a router can prevent traffic from that device from passing through the network while allowing other devices to communicate normally.

