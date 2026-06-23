# 01 — DNS Lookup (Name → IP)

## Goal

Show what DNS looks like on the network.

DNS is how your computer turns a website name (like `example.com`) into an IP address.

---

## What I Did

* Opened Wireshark and started a capture on my active interface (Wi-Fi).
* Triggered a DNS lookup by visiting a website or running a lookup command.
* Stopped the capture and filtered to DNS traffic.
* Saved the capture and screenshot for evidence.

---

## Wireshark Filters Used

### Show DNS Packets

```plaintext
dns
```

### Show DNS Traffic on Common Ports

```plaintext
udp.port == 53
```

(Most common)

```plaintext
tcp.port == 53
```

(Sometimes used)

---

## What I Observed

* I observed a DNS query where my computer asked:
  > "What is the IP address associated with this domain?"

* I then observed a DNS response where the DNS server returned one or more IP addresses associated with the requested domain.

### Common DNS Record Types

| Record Type | Purpose |
|---|---|
| A | IPv4 Address |
| AAAA | IPv6 Address |
| CNAME | Alias that points to another domain |

---

## How To Find The Website In DNS

1. Click a DNS packet.
2. Expand:

```plaintext
Domain Name System (query)
```

3. Review:

### Queries

Displays the domain name being requested.

Example:

```plaintext
example.com
```

### Answers

Displays the returned IP address(es).

Example:

```plaintext
93.184.216.34
```

---

## Evidence Collected

### Capture File

```plaintext
captures/dns_lookup.pcapng
```

### Screenshot

```plaintext
screenshots/dns_lookup.png
```

### Notes

```plaintext
notes/01_dns.md
```

---

## Why This Matters

DNS is typically the first network activity that occurs before a connection is established to a website or service.

Understanding DNS traffic allows analysts to:

* Identify domain lookups performed by devices
* Investigate suspicious domains
* Correlate domains to IP addresses
* Support threat hunting and incident response investigations

DNS logs are frequently reviewed during malware investigations because malicious software often performs DNS lookups before communicating with external infrastructure.

---

## Key Takeaways

* DNS translates domain names into IP addresses.
* Most web traffic begins with a DNS lookup.
* DNS records provide valuable investigative context.
* Analysts frequently use DNS activity to investigate suspicious infrastructure.
* Understanding DNS behavior is foundational for network monitoring and incident response.

---

## Privacy Note

I used non-sensitive browsing during capture and only recorded DNS resolution behavior within a controlled lab environment.
