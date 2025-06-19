# 🔐 Router & IoT Device Hardening Guide

This guide outlines best practices to secure your home router and IoT (Internet of Things) devices against common threats. These steps help reduce your network’s attack surface and improve overall security.

---

## 📡 Router Hardening

### 1. Change Default Credentials
- Replace default admin username and password.
- Use a strong, unique password with a mix of letters, numbers, and symbols.

### 2. Update Firmware Regularly
- Check your router dashboard for firmware updates.
- Apply patches to fix known vulnerabilities.

### 3. Use Strong Encryption
- Set Wi-Fi security to **WPA2** or **WPA3**.
- Avoid WEP and WPA (they are insecure and easily cracked).

### 4. Disable WPS (Wi-Fi Protected Setup)
- WPS is vulnerable to brute-force attacks.
- Turn it off to prevent unauthorized device pairing.

### 5. Turn Off Remote Management
- Disable remote access unless absolutely necessary.
- Only allow local configuration access via Ethernet or secure Wi-Fi.

### 6. Disable Unused Services
- UPnP (Universal Plug and Play)  
- Telnet  
- FTP  
These services can open unwanted ports or expose control to outside devices.

### 7. Set a Guest Network (Optional)
- Isolate IoT devices or guests from your main network.
- Limit their access to sensitive devices or file shares.

### 8. Change the Default Network Name (SSID)
- Avoid using names that reveal your router model or personal info.
- Example: Avoid `NETGEAR123` or `JohnsWiFiHome`.

---

## 📱 IoT Device Hardening

### 1. Update Device Firmware
- Keep smart plugs, cameras, thermostats, etc. up to date.
- Use manufacturer apps or portals to check for updates.

### 2. Change Default Passwords
- Most IoT devices ship with weak, predictable logins.
- Use a password manager to assign unique credentials per device.

### 3. Isolate IoT Devices
- Use a **separate VLAN** or **guest network** if your router supports it.
- Prevent them from accessing computers, NAS drives, or private files.

### 4. Disable Unused Features
- Turn off unused cloud integration, voice assistants, or remote access.
- Reduce the number of internet-facing features whenever possible.

### 5. Monitor Device Behavior
- Periodically check what IPs your devices are connecting to.
- Use router logs or tools like `nmap` and `Wireshark` to analyze traffic.

---

## 🧠 General Best Practices

- Enable a **firewall** on your router (usually on by default).
- Turn off router **SSID broadcasting** if you want to limit visibility (optional).
- Periodically audit your network with tools from this project.
- Consider setting up **device alerts** if new hardware connects to your network.

---

> ⚠️ **Note:** IoT devices are often built with minimal security — treat them as untrusted and segment your network when possible.

---

## 📎 References

- [OWASP IoT Security Guidelines](https://owasp.org/www-project-internet-of-things/)
- [US-CERT Home Network Security Tips](https://www.cisa.gov/news-events/news/home-network-security)
- [RouterSecurity.org](https://routersecurity.org)


