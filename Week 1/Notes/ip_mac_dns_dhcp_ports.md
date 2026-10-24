# IP, MAC, DNS, DHCP and Ports

## Definitions
- **IP (Internet Protocol)**: Numeric label (IPv4/IPv6) used to identify devices on a network.
- **MAC (Media Access Control) address**: Hardware address burned into NIC, used at Layer 2.
- **DNS (Domain Name System)**: Resolves human‑readable domain names to IP addresses.
- **DHCP (Dynamic Host Configuration Protocol)**: Automatically assigns IP, subnet mask, gateway, DNS to hosts.
- **Port**: Logical endpoint for a network service (0‑65535).

## Common Ports

| Port | Service | Typical Risk |
|------|---------|--------------|
| 21   | FTP (File Transfer) | Clear‑text credentials, data exfiltration |
| 22   | SSH (Secure Shell) | Brute‑force login, lateral movement if compromised |
| 23   | Telnet (unencrypted) | Plaintext traffic, easy credential theft |
| 25   | SMTP (Mail) | Spam relay, email spoofing |
| 53   | DNS (Domain) | DNS poisoning, amplification DDoS |
| 80   | HTTP (Web) | Web‑app attacks (XSS, SQLi) |
| 110  | POP3 (Mail) | Credential theft, clear‑text emails |
| 143  | IMAP (Mail) | Credential theft, mailbox enumeration |
| 443  | HTTPS (Secure Web) | SSL/TLS misconfig, certificate spoofing |
| 445  | SMB (Windows file sharing) | Ransomware spread, EternalBlue exploit |
| 3306 | MySQL database | SQL injection, unauthorized DB access |
| 3389 | RDP (Remote Desktop) | Brute‑force, ransomware via remote access |
