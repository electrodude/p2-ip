# Internet Protocol stack for the Parallax Propeller 2

Tested with ManAtWork's included MAC/PHY driver for the LAN8720A.  It should be possible to make it work with any other MAC/PHY.

## Current Functionality

- Replies to ARP requests
- Replies to ICMP pings
- Sends replies to UDP packets provided by a user-supplied callback
- Actively refuses all TCP connections

## Planned Work

- Use fewer than three cogs
	- E.g. one for both TX and RX and another (possibly using LUT sharing, possibly using XBYTE) for most of IP
- Refactor into more Spin objects
- Send packets on our own, not just in response to received packets
- ARP
	- Properly probe for an address before claiming it
	- Send ARP probes for nodes we're trying to contact
- IPv4
- IPv6
- ICMPv4 features besides ping
- ICMPv6 features besides ping
	- Most importantly, NDP
- Hosts table
	- Associates IP addresses, MAC addresses, and hostnames
- DHCP client
- DNS resolver
- mDNS
- TCP
	- Scary...
