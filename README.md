# 🖥️ Home Server Infrastructure with Secure Remote Access

This project showcases my practical experience with **networking**, **system administration**, and **secure service deployment**.  
It documents how I designed, configured, and currently maintain a **TrueNAS SCALE home server** for file storage, remote access, and media streaming.  

Through this project, I strengthened my understanding of **TCP/IP networking**, and gained hands-on experience with **VPNs**, **firewall configuration**, and **secure remote management**.

---

## 🌐 Project Overview

I set up a **TrueNAS SCALE server** as a home lab to host files, backups, and media.  
The system is accessible both locally and remotely through a **Tailscale VPN**, allowing me to connect securely from any device via **SMB** or **SSH**.

For media streaming, I deployed **Plex Media Server** inside a **Docker container** (using TrueNAS SCALE’s built-im Docker-based system).  
This provides container isolation, easy maintenance, and consistent performance.

To improve accessibility and fault tolerance, I also set up a **Caddy reverse proxy** on a cloud relay server connected through Tailscale, enabling secure traffic forwarding and TLS encryption.

---

## ⚙️ Technologies Used

| Category | Tools / Protocols |
|-----------|------------------|
| Server OS | TrueNAS SCALE |
| Remote Access | Tailscale (WireGuard-based VPN) |
| File Sharing | SMB, SSH, NFS |
| Media Streaming | Plex Media Server (Docker container) |
| Container Platform | Docker (TrueNAS SCALE Built-in) |
| Cloud Relay | Caddy reverse proxy |
| Storage | ZFS filesystem, snapshots, datasets |
| Networking Protocols | TCP/IP |
| Security | Encrypted VPN tunnels, access control, and firewall configuration |

---

## 🧩 Network Overview
Laptop/Phone ──► Tailscale VPN ──►  TrueNAS SCALE Server │ Plex Media Server (Docker)



---

## 🧠 What I Learned

- Configuring **VPN tunnels (Tailscale / WireGuard)** for secure remote access  
- Managing **SMB shares**, **ZFS datasets**, and **user permissions**  
- Running **containerized services** in **Docker**  
- Understanding and troubleshooting **networking protocols (TCP/IP, UDP, RDP, SMB)**  
- Implementing **firewall rules** and **port forwarding** to control access  
- Monitoring system health and network performance  
- Incorporating **security best practices** in every configuration decision  

---

<!--## 🛠️ Project Structure
---
-->

## 🚀 Future Improvements

- Add **Prometheus + Grafana** for advanced monitoring and visualization  
- Configure **automated ZFS replication** to a secondary backup server  
- Experiment with **routing protocols** (BGP and OSPF) in a virtual lab environment  
- Expand automation scripts for regular system health checks using Python  
- Deploy additional self-hosted services through Docker  

---

## 📚 Reflection

This project has been a key part of my growth as a computer science student interested in **network engineering**.  
I’ve gained hands-on experience with **real network protocols**, **VPN connectivity**, and **secure system design**, applying theory directly to a functional home infrastructure.

It also strengthened my ability to balance **technical learning, academics, and personal projects**, showing initiative and persistence; qualities I bring to team projects and future internships.

---

## 🧾 License

This repository is for educational and demonstration purposes only.  
All configuration examples are generalized for privacy and security.

---

### ✉️ Contact

If you’d like to discuss this project, networking concepts, or system setup best practices, feel free to reach out through my GitHub profile.


