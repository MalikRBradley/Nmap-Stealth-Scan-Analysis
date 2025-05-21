# Nmap Stealth Scan Analysis – Network Traffic Detection with Wireshark

This project simulates attacker reconnaissance behavior using an Nmap TCP SYN scan and captures network traffic using Wireshark. The goal is to detect pre-connection activity and analyze the stealth scan behavior at the packet level in a 3-VM lab setup.

---

## 🧪 Lab Setup

- 💻 Host: M3 MacBook Pro (ARM64) using VMware
- 🐱‍💻 VMs: Kali Linux (attacker), Windows 11 (target), Ubuntu (monitor)
- 🔧 Tools Used:
  - Nmap
  - Wireshark
  - VMware

---

## 📌 Key Objectives

- Simulate stealth scan activity (TCP SYN scan)
- Capture real-time packets on Ubuntu using Wireshark
- Inspect SYN packets using filters (`tcp.flags.syn == 1 and tcp.flags.ack == 0`)
- Save and analyze `.pcapng` traffic
- Identify open ports and attacker footprinting techniques

---

## 🧠 Skills Demonstrated

- ✅ Nmap scanning and packet crafting
- ✅ Wireshark traffic analysis
- ✅ Packet-level TCP inspection
- ✅ Detecting reconnaissance activity
- ✅ GitHub project documentation

---

## 📸 Screenshots

| Description | Screenshot |
|------------|------------|
| 1️⃣ Kali terminal running the Nmap scan | ![Nmap Scan](images/nmap-scan-kali-terminal.png) |
| 2️⃣ SYN packet from Nmap in Wireshark | ![SYN Packet](images/syn-packet-analysis.png) |
| 3️⃣ Full capture of DNS, ARP, MDNS traffic | ![Wireshark Full](images/wireshark-full-packetview.png) |

---

## 📂 PCAP File

The full capture is included:  
**`Nmap-Stealth-Scan.pcapng`**

You can open this in Wireshark and apply display filters to follow along with the analysis.

---

## 🔐 Defender’s Perspective

This analysis helps blue teamers recognize stealth scan patterns and pre-connection behavior early in an attack kill chain.

---

## 🧠 Thinking like an attacker. Analyzing like a defender.
