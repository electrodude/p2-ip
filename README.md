# Internet Protocol stack for the Parallax Propeller 2

Tested with ManAtWork's included MAC/PHY driver for the LAN8720A.  It should be possible to make it work with any other MAC/PHY.

## Current Functionality

- Echos Ethernet frames received from ManAtWork's driver

## Planned Work

- Ethernet frames
- ARP
- IPv4
- IPv6
- ICMPv4
- ICMPv6
- Hosts table
	- Associates IP addresses, MAC addresses, and hostnames
- UDP
- DHCP client
- DNS resolver
- mDNS
- TCP
	- Scary...
