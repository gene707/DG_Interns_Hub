# VM Networking Modes

| Mode | Description | When to Use | Why Vulnerable Labs Must Not Use Bridged |
|------|-------------|-------------|----------------------------------------|
| **NAT** | VM gets private IP; host does network address translation for outbound traffic. | Quick internet access for a single VM. | Bridged would expose the lab directly to the external network, allowing attackers to reach vulnerable services.
| **NAT Network** | Multiple VMs share a virtual network with NAT to the host. | Lab environments where VMs need to talk to each other and the internet. | Still isolates from the physical LAN, preventing accidental exposure.
| **Host‑only** | VMs can only communicate with the host and each other; no external internet. | Isolated testing, offline labs. | Guarantees no external reachability, keeping vulnerable services safe.
| **Bridged** | VM appears as a separate device on the physical LAN, getting its own IP from the router. | Situations needing full LAN visibility (e.g., testing network services in real environment). | Exposes vulnerable services to the corporate/ home network, risking compromise of other devices.

> [!WARNING] Never use **Bridged** for labs that contain intentionally vulnerable services; they could be discovered and exploited by anyone on the same network.
