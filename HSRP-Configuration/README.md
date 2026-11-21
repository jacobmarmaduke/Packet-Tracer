# HSRP Configuration – Cisco Packet Tracer Lab

## Objective
Configure Hot Standby Router Protocol (HSRP) between two Cisco routers to provide default gateway redundancy and improve network availability.

## Network Equipment
- 2 Cisco 1941 Routers
- 2 Cisco 2960 Switches
- 4 PCs

## Skills Demonstrated
- HSRP configuration
- First Hop Redundancy Protocols (FHRP)
- Virtual IP address configuration
- Active and Standby router roles
- Router priority configuration
- HSRP preemption
- Gateway redundancy
- Network failover testing

## IP Addressing

| Device | Interface | IP Address |
|---|---|---|
| R1 | G0/1 | 192.168.10.2 |
| R2 | G0/1 | 192.168.10.3 |
| HSRP Virtual IP | — | 192.168.10.1 |
| PCs | NIC | 192.168.10.x |

Subnet Mask: `255.255.255.0`

Default Gateway for all PCs: `192.168.10.1`

## HSRP Configuration

| Setting | Value |
|---|---|
| HSRP Group | 1 |
| Virtual IP | 192.168.10.1 |
| R1 Priority | 110 |
| R2 Priority | 100 |
| Active Router | R1 |
| Standby Router | R2 |

## Cisco Technologies
- HSRP
- First Hop Redundancy Protocol (FHRP)
- Virtual IP addressing
- Router priority and preemption
- High availability

## Testing and Verification
- Verify HSRP status using `show standby brief`.
- View detailed HSRP information using `show standby`.
- Verify router interfaces using `show ip interface brief`.
- Ping the virtual IP address from all PCs.
- Shut down R1's interface to simulate a router failure.
- Verify R2 takes over as the Active router.
- Restore R1 and verify preemption.

## Conclusion
This lab demonstrates how HSRP provides network redundancy by allowing two routers to share a virtual default gateway. If the Active router fails, the Standby router automatically takes over, helping maintain network connectivity.

