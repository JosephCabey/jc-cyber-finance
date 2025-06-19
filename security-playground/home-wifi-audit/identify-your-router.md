# 🖥️ How to Identify Your Home Router

Knowing your router's brand and model is the first step in understanding its capabilities, vulnerabilities, and how to secure it. Here are several methods to identify your router:

---

## 🖥️ 1. Check the Router Label (Physical Inspection)

Flip your router over or look at the back panel. You’ll typically find:

- **Brand** (e.g., Netgear, TP-Link, Asus, Spectrum)
- **Model number** (e.g., Archer C7, R6700, etc.)
- **Default IP address** (e.g., `192.168.0.1` or `192.168.1.1`)
- **Login credentials** (e.g., `admin` / `password`)  
  > ⚠️ These should be changed immediately after setup!

---

## 🌐 2. Log Into the Router Dashboard (Browser Method)

1. Connect to your Wi-Fi network or plug in via Ethernet.
2. Open a browser and type one of the following IP addresses:
http://192.168.0.1
http://192.168.1.1
http://192.168.1.254
Or try http://10.0.0.1 for Xfinity routers

4. Enter the router’s **admin username and password** (found on the label or previously configured).
5. Once inside, you should see:
   - **Router brand and model**
   - **Firmware version**
   - **Wireless and network settings**

---

## 💻 3. Use the Command Line (Windows, Mac, or Linux)

### 🔹 On **Windows**
1. Open **Command Prompt**
2. Run:
   ```bash
   ipconfig
3. Look for the Default Gateway — this is your router’s IP address.
4. Enter that IP into a web browser to access your router dashboard.
**On macOS/Linux**
1. Open Terminal
2. Run one of the following commands:
   
netstat -nr | grep default
or
ip route | grep default
3. Use the displayed IP address in a browser to log into your router.

## 🛠️ 4. Use a Network Scanner (Optional)

You can also use network tools to identify your router:

🔧 nmap
nmap -O 192.168.0.1
Tries to detect the operating system and fingerprint the router

🔧 arp
arp -a
Lists all devices on your local network — your router is usually the first one listed.

📱 Mobile App: Fing (Android/iOS)
Fing scans your network and automatically identifies the router’s brand and model along with all connected devices.

## 📌 Quick Tip

Once you identify the **model number**, Google it (e.g., `TP-Link Archer A6`) to find:

- 🧾 User manuals and setup guides  
- 🔐 Known security vulnerabilities  
- 🔄 Firmware updates  
- ⚙️ Steps for enabling security features  
