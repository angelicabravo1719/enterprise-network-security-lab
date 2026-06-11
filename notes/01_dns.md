# Enterprise Network Security Lab

## Overview

This repository documents hands-on network security analysis performed using Wireshark and packet capture (PCAP) files. The objective of these labs is to develop a practical understanding of network communications, protocol behavior, and packet analysis techniques commonly used by network engineers, SOC analysts, cybersecurity analysts, and incident responders.

Through these exercises, I captured and analyzed real network traffic to better understand how devices communicate across modern networks and how security professionals investigate network activity.

---

## Scope of Work

The labs in this repository focus on:

* DNS name resolution
* TCP three-way handshakes
* HTTP communications
* HTTPS and TLS encryption
* Packet capture analysis
* Network troubleshooting fundamentals
* Security implications of network protocols

---

## Skills Demonstrated

### Network Fundamentals

* IP addressing
* Ports and protocols
* Client-server communications
* Packet flow analysis

### Traffic Analysis

* Wireshark packet inspection
* Protocol identification
* Packet filtering
* Traffic interpretation

### Security Analysis

* Understanding cleartext vs encrypted communications
* Identifying DNS requests and responses
* Examining TLS handshake behavior
* Recognizing protocol metadata exposure
* Understanding how analysts investigate network activity

### Documentation

* Technical note-taking
* Evidence collection
* Screenshot documentation
* Analyst-style reporting

---

## Lab Summary

| Lab | Topic                   | Skill Demonstrated                |
| --- | ----------------------- | --------------------------------- |
| 01  | DNS Analysis            | Name Resolution Investigation     |
| 02  | TCP Three-Way Handshake | Connection Establishment Analysis |
| 03  | HTTP Analysis           | Cleartext Traffic Analysis        |
| 04  | HTTPS / TLS Analysis    | Encrypted Communication Analysis  |

---

## Lab Progression

### Lab 01 – DNS Analysis

**Objective:** Understand how domain names are translated into IP addresses.

Topics covered:

* DNS queries
* DNS responses
* Name resolution process
* Client-server communication

Files:

* `captures/dns_lookup.pcapng`
* `notes/01_dns.md`
* `screenshots/dns_lookup.png`

---

### Lab 02 – TCP Three-Way Handshake

**Objective:** Analyze the process used to establish TCP connections.

Topics covered:

* SYN packets
* SYN-ACK responses
* ACK completion
* Connection establishment

Files:

* `captures/tcp_handshake.pcapng`
* `notes/02_tcp_handshake.md`
* `screenshots/tcp_handshake.png`

---

### Lab 03 – HTTP Analysis

**Objective:** Examine unencrypted web communications.

Topics covered:

* HTTP requests
* HTTP responses
* Headers
* Cleartext communications

Files:

* `captures/http_request_cleartext.pcapng`
* `notes/03_HTTP.md`
* `screenshots/http_request.png`

---

### Lab 04 – HTTPS and TLS Handshake Analysis

**Objective:** Understand how encrypted web sessions are established.

Topics covered:

* TLS handshake
* Server certificates
* Session establishment
* Encryption fundamentals

Files:

* `captures/https_tls_handshake.pcapng`
* `notes/04_HTTPS (TLS).md`
* `screenshots/https_tls_handshake.png`

---

## SOC Applications

The skills demonstrated throughout this repository directly support:

* Security Operations Center (SOC) Analysis
* Network Security Monitoring
* Incident Response
* Threat Hunting
* Malware Investigations
* Traffic Analysis
* Security Event Triage

Understanding network communications is a foundational skill for cybersecurity professionals because nearly all modern attacks involve some form of network activity.

---

## Repository Structure

```plaintext
enterprise-network-security-lab/

├── captures/
│   ├── dns_lookup.pcapng
│   ├── tcp_handshake.pcapng
│   ├── http_request_cleartext.pcapng
│   └── https_tls_handshake.pcapng
│
├── notes/
│   ├── 01_dns.md
│   ├── 02_tcp_handshake.md
│   ├── 03_HTTP.md
│   └── 04_HTTPS (TLS).md
│
├── screenshots/
│   ├── dns_lookup.png
│   ├── tcp_handshake.png
│   ├── http_request.png
│   └── https_tls_handshake.png
│
└── README.md
```

---

## Technologies Used

* Wireshark
* Windows
* TCP/IP
* DNS
* HTTP
* HTTPS
* TLS

---

## Learning Objectives

The purpose of this repository is to develop practical experience analyzing network traffic while building skills directly applicable to cybersecurity operations.

Key learning objectives include:

* Understanding how common network protocols function
* Learning to identify protocol behavior in packet captures
* Developing packet analysis skills using Wireshark
* Understanding the security implications of network communications
* Building foundational knowledge for SOC analysis and incident response

