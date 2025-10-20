# 🔐 Wazuh SIEM Lab — Real-Time Detection & Response

This project is my personal **Wazuh-based SIEM lab**, built to practice **detection engineering**, **incident response**, and **log analysis** in a hands-on environment.  
It’s part of my continuous journey to deepen my cybersecurity skills while preparing for certifications like **CompTIA Security+** and **OSCP**.

---

## 🚀 Project Overview
The lab demonstrates how real-world security events (like brute-force attacks or malware execution) can be **detected**, **analyzed**, and **responded to automatically** using Wazuh.  

I will keep improving this project week by week — documenting each step and adding new detections, configurations, and integrations.

---

## 🧠 Learning Goals
- Understand **SIEM architecture** and **log ingestion pipelines**  
- Write and test **custom Wazuh rules & decoders**  
- Practice **detection engineering** and **active response automation**  
- Document every improvement for others to follow

---

## 🧩 Lab Components

| Role | OS | Description |
|------|----|--------------|
| 🧱 **Wazuh Manager** | Linux | Core SIEM platform for log collection, rules, and response |
| 💻 **Windows 10 Agent** | Windows 10 | Monitored endpoint generating logs (RDP, Defender, Sysmon) |
| ⚔️ **Attacker VM** | Kali Linux | Used to simulate attacks (RDP brute force, malware tests) |

---

## 🧰 Current Capabilities
✅ Detects RDP brute-force attempts (Rule ID `60204`)  
✅ Detects simulated malware events (EICAR test file)  
✅ Triggers Active Response (IP auto-block via `firewalldrop`)  
✅ Collects logs from Windows Defender and Event Viewer  

---

## ⚙️ Quickstart (Scaffold in Progress)
> These steps will become fully runnable once the Docker setup is added (Day 2 in my roadmap).

1. **Start the stack** (after `docker-compose.yml` is added):
   ```bash
   docker compose pull
   docker compose up -d
   docker compose ps
