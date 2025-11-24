# Nmap Lab

This section covers essential Nmap commands used for network scanning, host discovery, service detection, OS fingerprinting, and enumeration. These commands are suitable for beginners as well as those practicing OSCP-style scanning.

---

## 🔍 Basic Host Scan
```bash
nmap 192.168.1.10
nmap -F 192.168.1.10
nmap -sV 192.168.1.10
nmap -O 192.168.1.10
nmap -sS 192.168.1.10
nmap -sC -sV 192.168.1.10
nmap -oA scan-results target.com
nmap 192.168.1.1-50
nmap -f 192.168.1.10
