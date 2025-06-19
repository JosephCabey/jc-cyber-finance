# 🔐 Router & IoT Device Hardening Guide

This guide provides best practices for securing home routers and IoT (Internet of Things) devices. These steps help reduce the attack surface and protect your network from common threats.

---

## 📡 Router Hardening

### 1. Change Default Credentials
- Replace the default admin username and password immediately.
- Use a strong, unique password with a mix of letters, numbers, and symbols.

### 2. Update Firmware Regularly
- Log in to your router dashboard and check for firmware updates.
- Apply patches to fix known vulnerabilities as soon as they're available.

### 3. Use Strong Encryption
- Set your Wi-Fi security to **WPA2** or **WPA3**.
- Avoid outdated standards like **WEP** and **WPA**, which are easily cracked.

### 4. Disable WPS (Wi-Fi Protected Setup)
- WPS is vulnerable to brute-force attacks.
- Turn it off to prevent unauthorized device pairing.

### 5. Turn Off Remote Management
- Disable remote access unless absolutely necessary.
- Only allow configuration changes from devices connected locally via Ethernet or secured Wi-Fi.

### 6. Disable Unused Services
Turn off services that are not required, such as:
- **UPnP (Universal Plug and Play)**
- **Telnet**
- **FTP**

These can expose your router to unnecessary risk and open unexpected ports.

### 7. Set Up a Guest Network (Optional)
- Use a separate guest network for IoT devices and visitors.
- This isolates untrusted devices from your primary home network and sensitive systems.

### 8. Change the Default Network Name (SSID)
- Avoid using a network name that reveals your router brand or personal information.
- For example, avoid `NETGEAR123`, `JohnsWiFiHome`, or `MercedesGuestWiFi`.
- **Why?** Identifiable SSIDs can make it easier for attackers to:
  - Determine your router model (and known vulnerabilities)
  - Guess your password pattern
  - Target your home based on perceived wealth

---

## 📱 IoT Device Hardening

### 1. Update Device Firmware
- Regularly update firmware on smart plugs, cameras, thermostats, etc.
- Use the manufacturer’s app or web portal to check for updates.

### 2. Change Default Passwords
- IoT devices often ship with generic credentials like `admin/admin`.
- Change these immediately and use a password manager to store secure, unique passwords.

### 3. Isolate IoT Devices
- Place IoT devices on a **guest network** or **separate VLAN** if supported.
- Prevent them from accessing computers, servers, or other private devices on your network.

### 4. Disable Unused Features
- Turn off unnecessary cloud services, voice assistants, and remote access options.
- Fewer features = fewer ways for attackers to get in.

### 5. Monitor Device Behavior
- Periodically check which IP addresses your devices are connecting to.
- Use tools like `nmap`, your router’s admin panel, or `Wireshark` to review traffic.

---

## 🧠 General Best Practices

- ✅ Enable your router’s built-in firewall (should be on by default).
- 🚫 Turn off SSID broadcasting if you want to limit visibility (optional).
- 🕵️‍♂️ Periodically scan your network using tools from the [Home Wi-Fi Audit](./README.md).
- 📳 Enable alerts for when new devices connect to your network, if supported by your router.

---

> ⚠️ **Note:** IoT devices often prioritize convenience over security. Always treat them as potentially untrusted and keep them separated from critical systems.

---

## 📎 References

- [OWASP IoT Security Guidelines](https://owasp.org/www-project-internet-of-things/)
- [US-CERT Home Network Security Tips](https://www.cisa.gov/news-events/news/home-network-security)
- [RouterSecurity.org](https://routersecurity.org)

