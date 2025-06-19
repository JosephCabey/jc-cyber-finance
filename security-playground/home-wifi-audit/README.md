# 🛡️ Home Wi-Fi Security Audit

This project simulates a basic home Wi-Fi network security audit using open-source tools and security analyst methodology. It aims to identify common vulnerabilities in a typical home network and promote responsible cybersecurity practices without launching active attacks or exploiting systems.

---

## 🧭 Project Scope

This audit focuses on:
- Detecting connected devices on the network
- Identifying open ports and exposed services
- Reviewing router security settings (e.g., encryption, firmware, credentials)
- Examining DNS behavior and potential misconfigurations
- Capturing and analyzing unencrypted packet data responsibly

---

## 🔍 Key Audit Steps

1. **Enumerate Devices on the Network**
   - Use `nmap` to scan your local IP range and list all connected devices.
   ```bash
   nmap -sn 192.168.0.0/24
2. Scan for Open Ports and Running Services

Identify which ports are open on your router or another device.

nmap -sV 192.168.0.1

3. Check Network Connections on Your Machine

Use netstat or ss to review all open connections.

netstat -tulnp

4. Inspect DNS and IP Configuration

Look up IP and DNS info to verify if anything seems misconfigured or suspicious.

whois example.com
dig example.com
traceroute example.com
arp -a
5. Review Your Router Settings (Manually via Dashboard)

Login to your router (typically http://192.168.0.1 or http://192.168.1.1) and check for:

Default login credentials (change them!)

Weak or outdated encryption (use WPA2/WPA3)

UPnP enabled (disable if not needed)

Outdated firmware (update if available)

6. Analyze Traffic (Optional – for learning only)

Open Wireshark and capture some packets from your Wi-Fi interface.

Filter by protocols like HTTP, DNS, or ARP to analyze patterns.

Do not capture other people’s private data — stay ethical.

⚙️ Tools Used
nmap – for network and port scanning

netstat / ss – for viewing local open connections

whois, dig, traceroute, arp – for DNS and IP diagnostics

Router Web UI – for config inspection

Wireshark – for optional, ethical packet analysis

🧠 What I Learned
How to scan and map devices on a local network

The importance of strong router passwords and updated firmware

How to interpret port scan and DNS query results

How unencrypted traffic can reveal sensitive information

The difference between reconnaissance and exploitation in security audits

