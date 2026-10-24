# OSI vs TCP/IP Model Comparison

| OSI Layer | TCP/IP Layer | Typical Protocols | Example Attack |
|-----------|--------------|-------------------|----------------|
| **7 Application** | Application | HTTP, FTP, SMTP, DNS | **SQL Injection** on a web app |
| **6 Presentation** | — (functions in Application) | TLS/SSL, JPEG, MPEG | **Man‑in‑the‑Middle (TLS downgrade)** |
| **5 Session** | — (functions in Application) | NetBIOS, RPC | **Session hijacking** |
| **4 Transport** | Transport | TCP, UDP | **TCP SYN Flood** |
| **3 Network** | Internet | IP, ICMP, IGMP | **IP spoofing / ICMP flood** |
| **2 Data Link** | Network Access | Ethernet, ARP, PPP | **ARP poisoning** |
| **1 Physical** | Network Access | Ethernet cabling, Wi‑Fi | **Cable tap / wireless jamming** |

> [!NOTE] The OSI model is conceptual; TCP/IP collapses several layers (Presentation & Session) into the Application layer.
