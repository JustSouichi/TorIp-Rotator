# 🌐 Tor IP Rotator

**Automatically change your IP address every 3 seconds using Tor!** 🕵️‍♂️🔄

## 🚀 Features
- **Automatic IP Rotation** every 3 seconds
- **Privacy Boost** by routing traffic through the Tor network
- **Seamless Integration** with Firefox
- **Open Source & Easy to Use**

---

## 📌 Installation Guide

### 🔧 Install Tor
```bash
sudo apt update && sudo apt install tor
```

### ▶️ Start Tor Service
```bash
sudo systemctl start tor
```

✅ **Check if Tor is running:**
```bash
sudo systemctl status tor
```

### 🐍 Install Python & Tornet
```bash
sudo apt install python3-pip
sudo pip install tornet  # or use --break-system-packages if needed
```

### 🌍 Verify Tor is Working
1. Close all active Firefox tabs.
2. Run the following command to open a Tor session with Firefox:
   ```bash
   sudo tornet --interval 3 --count 0
   ```
3. Visit [Tor Check](https://check.torproject.org/) to confirm it's working!

---

## 🔥 Configure Firefox for Tor

1. Open **Firefox Settings** ⚙️
2. Scroll down to **Network Settings** -> Click **Settings**
3. Under **Configure Proxy Access to the Internet**, select **Manual Proxy Configuration**
4. Set the following:
   - **SOCKS v5**
   - **SOCKS Host:** `127.0.0.1`
   - **Port:** `9050`
   - ✅ Enable **Proxy DNS when using SOCKS v5**
5. Apply the settings & test your IP at [DNS Leak Test](https://www.dnsleaktest.com/)

---

## 🛑 Stopping TorNet & Restoring Firefox Settings

When you're done using TorNet:
```bash
sudo systemctl stop tor
```

🔄 Reset Firefox Proxy Settings:
- Go to **Firefox Settings**
- Under **Network Settings**, select **Auto-detect proxy settings for this network**
- Save & restart Firefox

---

## 📜 License
This project is licensed under the [MIT License](LICENSE).

## 🤝 Code of Conduct
Please read our [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) before contributing!

---

🚀 **Enjoy anonymous browsing & enhanced privacy with Tor IP Rotator!** 🕶️🌍

