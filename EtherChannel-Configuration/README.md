# EtherChannel Configuration – Cisco Packet Tracer Lab

## Objective
Configure EtherChannel between two Cisco switches using Link Aggregation Control Protocol (LACP) to combine multiple physical connections into one logical link.

This lab demonstrates how EtherChannel increases available bandwidth and provides link redundancy between switches.

## Network Equipment
- 2 Cisco 2960 Switches
- 4 PCs

## Network Topology
- PC1 and PC2 connect to SW1.
- PC3 and PC4 connect to SW2.
- SW1 Fa0/23 connects to SW2 Fa0/23.
- SW1 Fa0/24 connects to SW2 Fa0/24.
- Both physical links are combined into Port-Channel 1.

## Skills Demonstrated
- EtherChannel configuration
- Link Aggregation Control Protocol (LACP)
- Port-Channel configuration
- Switch-to-switch connectivity
- Link redundancy
- Increased network bandwidth
- EtherChannel troubleshooting

## Cisco Technologies
- EtherChannel
- LACP (IEEE 802.1AX)
- Port-Channel interfaces
- Cisco Catalyst 2960 switches

## Testing and Verification
- Verify EtherChannel using `show etherchannel summary`.
- Verify LACP neighbors using `show lacp neighbor`.
- Verify Port-Channel interfaces using `show interfaces port-channel 1`.
- Verify switch interfaces using `show interfaces status`.
- Test connectivity between PCs on different switches.
- Disconnect one physical EtherChannel link and verify connectivity remains operational.
- Confirm the remaining physical link continues forwarding traffic.

## Conclusion
This lab demonstrates how EtherChannel combines multiple physical switch connections into a single logical link using LACP. By increasing available bandwidth and providing link redundancy, EtherChannel improves network performance and reliability.

