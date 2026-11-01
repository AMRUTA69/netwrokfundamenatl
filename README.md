# Cyber Security Internship: Networking Tasks

**Intern:** Amruta Deshmukh
**Company:** Veda Technology
**Track:** Cyber Security (Level 1)

This repository contains my reports for the networking tasks completed during the internship.

## Tasks

| Task | Topic | Tool | Report |
|---|---|---|---|
| Task 11 (Day 11) | Networking Fundamentals | Cisco Packet Tracer | [Networking_Fundamentals_Report.docx](Networking_Fundamentals_Report.docx) |
| Task 13 (Day 13) | TCP and UDP Comparison | Wireshark | [TCP_vs_UDP_Report.docx](TCP_vs_UDP_Report.docx) |

## Task 11: Networking Fundamentals

**Objective:** Build a basic network topology, understand how devices connect, assign IP addresses and observe packet flow.

- Built a topology with 2 PCs, 1 switch and 1 router in Cisco Packet Tracer
- Assigned static IPv4 addresses in the 192.168.1.0/24 subnet
- Configured the router interface (192.168.1.1) via CLI
- Verified connectivity with a successful ping from PC0 to PC1
- Covered interview topics: IP address, MAC address and ports

## Task 13: TCP and UDP Comparison

**Objective:** Understand transport-layer protocols by capturing and comparing real traffic.

- Captured live traffic on Wi-Fi using Wireshark
- Observed the TCP three-way handshake (SYN, SYN-ACK, ACK), FIN teardown and retransmissions
- Observed UDP behaviour through DNS queries and QUIC traffic on port 443
- Compared TCP and UDP headers (TCP 20 to 60 bytes, UDP 8 bytes)
- Covered use cases and the security angle (SYN flood, DNS amplification)

### Wireshark filters used

```
tcp.flags.syn == 1
tcp.stream eq 3
tcp.flags.fin == 1
dns
udp.port == 443
```

### TCP vs UDP at a glance

| Feature | TCP | UDP |
|---|---|---|
| Connection | Connection-oriented | Connectionless |
| Reliability | Guaranteed delivery | No guarantee |
| Header size | 20 to 60 bytes | 8 bytes |
| Speed | Slower | Faster |
| Examples | HTTPS, SSH, FTP | DNS, VoIP, gaming, QUIC |

## Tools Used

- Cisco Packet Tracer 9.0.1
- Wireshark 4.6.9
- Web browser

## Repository Structure

```
.
├── README.md
├── Networking_Fundamentals_Report.docx
└── TCP_vs_UDP_Report.docx
```

## Author

**Amruta Deshmukh**
Cyber Security Intern, Veda Technology
