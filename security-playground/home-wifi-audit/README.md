# 🛡️ Home Wi-Fi Security Audit

This project simulates a basic home Wi-Fi network security audit using open-source tools and cybersecurity analyst methodology. The goal is to identify common vulnerabilities, assess the overall hygiene of the network, and demonstrate responsible analysis techniques — without engaging in any intrusive or malicious activity.

---

## 🔍 Key Focus Areas

- Enumeration of connected devices using `nmap`
- Port scanning and service fingerprinting
- Router configuration review (WPA2/3 usage, default credentials, UPnP exposure)
- DNS and IP address inspection using `whois`, `dig`, and `traceroute`
- Basic packet capture and interpretation using Wireshark
- Open connection checks using `netstat` or `ss`

---

## ⚙️ Tools & Sample Commands

```bash
# Scan the local network for connected devices
nmap -sP 192.168.0.0/24

# Scan router for open ports and running services
nmap -sV 192.168.0.1

# Check active TCP/UDP connections
netstat -tulnp

# DNS and IP information
whois example.com
dig example.com
traceroute example.com
arp -a

