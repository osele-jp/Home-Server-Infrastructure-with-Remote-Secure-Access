# 🖥️ Home Server Infrastructure with Secure Remote Access

This project showcases my practical experience with **networking**, **system administration**, and **secure service deployment**.  
It documents how I designed, configured, and currently maintain a **TrueNAS SCALE home server** for file storage, remote access, and media streaming.  

Through this project, I applied key concepts from my computer science coursework, strengthened my understanding of **TCP/IP networking**, and gained hands-on experience with **VPNs**, **firewall configuration**, and **secure remote management** — all important areas for a network engineering role.

---

## 🌐 Project Overview

I set up a **TrueNAS SCALE server** as a home lab to host files, backups, and media.  
The system is accessible both locally and remotely through a **Tailscale VPN**, allowing me to connect securely from any device via **SMB** or **SSH**.

For media streaming, I deployed **Plex Media Server** inside a **Kubernetes container** (using TrueNAS SCALE’s built-in K3s).  
This provides container isolation, easy maintenance, and consistent performance.

To improve accessibility and fault tolerance, I also set up a **Caddy reverse proxy** on a cloud relay server connected through Tailscale, enabling secure traffic forwarding and TLS encryption.

---

## ⚙️ Technologies Used

| Category | Tools / Protocols |
|-----------|------------------|
| Server OS | TrueNAS SCALE |
| Remote Access | Tailscale (WireGuard-based VPN) |
| File Sharing | SMB, SSH, NFS |
| Media Streaming | Plex Media Server (Kubernetes container) |
| Container Platform | K3s (TrueNAS SCALE Kubernetes) |
| Cloud Relay | Caddy reverse proxy |
| Storage | ZFS filesystem, snapshots, datasets |
| Programming | Python (for automation and scripting tasks) |
| Networking Protocols | TCP/IP, UDP, RDP |
| Security | Encrypted VPN tunnels, access control, and firewall configuration |

---

## 🧩 Network Overview

