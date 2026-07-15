# Cisco Packet Tracer — Enterprise Network Design Project

A multi-block enterprise network built and configured in Cisco Packet Tracer, covering core switching, routing, and services concepts: DHCP, DNS, HTTP/HTTPS, SMTP, VLANs with VTP, EtherChannel, port security, ACLs, and dynamic routing with redistribution.

## Topology Overview
The network is split into 8 functional blocks, each targeting a specific networking concept:

| Block | Focus |
|---|---|
| 1 | Two switches; DHCP server for automatic IP assignment; HTTP/HTTPS web server with custom index page; SMTP server with working email send/receive; DNS server resolving a custom domain |
| 2 | Three switches; LACP EtherChannel to bond links for increased bandwidth; port security restricting a switch port to a single connected device |
| 3 | Three switches using VLAN Trunking Protocol (VTP) — Server / Transparent / Client roles; four VLANs (Students, Faculty, Admin, IT) with inter-VLAN routing; management IPs configured for remote Telnet access from the IT VLAN |
| 4 | Access Control List (ACL) on a router to selectively permit one PC and deny another |
| 5 | RIP routing configured across four routers |
| 6 | OSPF routing configured across a separate set of routers |
| 7 | Route redistribution between RIP and OSPF domains |
| 8 | Remote Telnet access verified from a client PC to a router, including enable-mode authentication |

## Key Concepts Demonstrated
- Subnetting with only two usable host addresses per inter-router link
- DHCP, DNS, HTTP/HTTPS, and SMTP server configuration
- VLAN creation, trunking, and inter-VLAN routing via VTP
- LACP EtherChannel and port security
- Standard ACLs for traffic filtering
- RIP and OSPF configuration and mutual redistribution
- Remote device management via Telnet

## Files
| File | Description |
|---|---|
| `network_proj.pkt` | The Cisco Packet Tracer project file — open in Packet Tracer to explore the full topology and device configs |
| `project_documentation.pdf` | Screenshots and command-line output showing each block working (DHCP/email test, port security status, VLAN/trunk verification, ACL rules, OSPF neighbor tables, Telnet session, etc.) |

## How to View
1. Install [Cisco Packet Tracer] (free with a Cisco Networking Academy account).
2. Open `network_proj.pkt`.
3. Click into individual devices' **CLI** or **Desktop** tabs to inspect configurations, or refer to `project_documentation.pdf` for a walkthrough with verified outputs.
