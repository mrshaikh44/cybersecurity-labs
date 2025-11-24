# Wireshark / Tshark Lab

This section covers packet capturing, filtering, and analyzing network traffic using **Wireshark** (GUI) and **Tshark** (CLI). Useful for understanding protocols, debugging traffic, and performing basic forensic analysis.

---

## 🎥 Capture Live Packets (Tshark)
```bash
tshark -i eth0
tshark -i eth0 -w capture.pcap
tshark -r capture.pcap -Y "http"
http.request
ip.addr == 192.168.1.10
http
dns
ftp
tcp
udp
icmp
ip.src == 192.168.1.5
ip.dst == 192.168.1.10
http.request.method == "GET"
tcp.flags.syn == 1 and tcp.flags.ack == 0
