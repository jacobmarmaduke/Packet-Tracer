# Lab 05 – DHCP Configuration

## Overview
This lab demonstrates how to configure a Cisco router as a DHCP server to automatically assign IP addresses and network settings to client devices.

The router provides DHCP services for two separate LANs, allowing PCs to obtain their network configurations automatically instead of requiring manual IP configuration.

## Network Topology
- 1 Cisco 1941 Router
- 2 Cisco 2960 Switches
- 4 PCs

## IP Addressing

| Device | Interface | IP Address | Subnet Mask |
|---|---|---|---|
| R1 | G0/0 | 192.168.10.1 | 255.255.255.0 |
| R1 | G0/1 | 192.168.20.1 | 255.255.255.0 |
| PC1 | DHCP | Automatic | Automatic |
| PC2 | DHCP | Automatic | Automatic |
| PC3 | DHCP | Automatic | Automatic |
| PC4 | DHCP | Automatic | Automatic |

### Network Details

| Network | Subnet | Default Gateway |
|---|---|---|
| LAN 1 | 192.168.10.0/24 | 192.168.10.1 |
| LAN 2 | 192.168.20.0/24 | 192.168.20.1 |

## Configuration
The router is configured with two DHCP pools:

- **LAN1-POOL:** Assigns IP addresses to devices on the 192.168.10.0/24 network.
- **LAN2-POOL:** Assigns IP addresses to devices on the 192.168.20.0/24 network.

The configuration also includes:
- Excluded IP addresses reserved for network infrastructure.
- Default gateway assignments through DHCP.
- DNS server configuration.
- Router interfaces configured with static IP addresses.

## Verification and Testing
The following commands and tests were used to verify DHCP functionality:

- Display DHCP pool information `show ip dhcp pool`
- Display addresses assigned to clients `show ip dhcp binding`
- Display DHCP server statistics `show ip dhcp server statistics`
- Display the IP configuration assigned to a PC`ipconfig`

## Skills Demonstrated
- Cisco IOS DHCP configuration
- DHCP address pools
- Excluded IP address ranges
- Default gateway and DNS configuration
- Automatic IP address assignment
- Network connectivity testing
- DHCP troubleshooting
