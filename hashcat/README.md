# Hashcat Lab

This section covers password cracking basics using **Hashcat**, including commands for dictionary attacks, hash modes, mask attacks, and result extraction. Hashcat is a GPU-based password recovery tool widely used in penetration testing.

---

## 🔐 Check GPU Support
```bash
hashcat -I
hashcat -m 0 -a 0 hashes.txt wordlist.txt
hashcat --show -m 0 hashes.txt
hashcat -h | grep "Hash modes"
hashcat -m 0 -a 3 hashes.txt ?l?l?l?l?l?l
hashcat --restore
