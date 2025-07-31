# local_networktool_kit
🔧 A modular Python toolkit for LAN reconnaissance, MITM, and packet sniffing. Built with PyQt5 and Scapy, it features live host discovery, ARP spoofing, and real-time packet capture in a clean tabbed GUI. Designed for ethical hacking and network analysis.


# 🔧 Local Network Toolkit (LAN Recon & MITM Suite)

A professional-grade, modular Python application for **LAN reconnaissance**, **MITM attacks**, and **network analysis**, built with **PyQt5**, **Scapy**, and **python-nmap**. Designed for ethical hacking, lab simulations, and learning network security principles through hands-on tools.

## 🚀 Features

* 🔍 **Live Host Discovery**
  Scan your LAN using ICMP pings and detect active devices with real-time results.

* 🧠 **Port Scanning with Service Detection** *(Coming Soon)*
  Identify open ports and running services using `python-nmap`.

* 🌐 **ARP Spoofing / MITM (Man-in-the-Middle)**
  Intercept traffic between a target and the gateway (via Scapy).

* 📦 **Network Packet Sniffing**
  Capture, inspect, and display real-time packets on your interface.

* 📑 **Report Generation** *(HTML/PDF export planned)*
  Create summaries of your recon/sniff/MITM sessions.

* ⚙️ **Scan Profiles & Settings Storage**
  JSON-based configuration for reusable scan preferences.

* 🖥️ **Tabbed GUI (PyQt5)**
  Modern, responsive UI with dedicated tabs for each feature.

* 🧩 **Modular Architecture**
  Easily add new tools without breaking existing functionality.

---

## 🛠️ Tech Stack

* Python 3.x
* PyQt5 (GUI)
* Scapy (Packet sniffing, ARP spoofing)
* python-nmap (Port scanning)
* ReportLab or HTML (report output)
* Threading, Subprocess, IP/Socket libraries

---

## 📁 Project Structure

```
📦 local-network-toolkit/
├── core/            # Scanning, sniffing, spoofing logic
│   ├── scanner.py
│   ├── sniffer.py
│   └── mitm.py
├── gui/             # GUI tabs using PyQt5
│   ├── recon_tab.py
│   ├── mitm_tab.py
│   └── sniffer_tab.py
├── config/          # JSON profiles and settings
│   └── default_profile.json
├── reports/         # Generated output (PDF/HTML)
├── run.py           # Entry point
├── requirements.txt
└── README.md
```

---
## 🔧 Installation

### 🔹 1. Clone the repository

```bash
git clone https://github.com/yourusername/local-network-toolkit.git
cd local-network-toolkit
```

### 🔹 2. Install dependencies

```bash
pip install -r requirements.txt
```


## ▶️ Running the App

```bash
python run.py
```

> Use `sudo` or run as admin **if sniffing or spoofing** (required by Scapy).

--
## 🧪 Example Use Cases

* Discover devices on your local network
* Intercept device traffic in lab environments
* Analyze packet-level behavior
* Test IDS/IPS defenses in a simulated LAN
## ⚠️ Disclaimer

This tool is intended **for educational and ethical use only**.
Do not use on unauthorized networks. Always have explicit permission

## 📌 To-Do / Roadmap

 [ ] Multithreaded ping scan (for faster scanning)
 [ ] Port scanning tab (nmap + banner grabbing)
 [ ] OS fingerprinting
 [ ] Export results as PDF/HTML
 [ ] Dark theme toggle
 [ ] Notifications/log pane

## 🤝 Contributions Welcome!

Open to PRs, ideas, and improvements. Help build this into a full-featured network toolkit.

## 📜 License
MIT License

