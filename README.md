# 🔐 Wazuh SIEM Lab - Real-Time Detection & Response

A complete local SIEM lab built using Wazuh to simulate real-time detection of brute-force attacks and malware execution, along with automated blocking.

---

## 💻 Lab Setup

| Role          | OS            | Description         |
|---------------|---------------|---------------------|
| Wazuh Manager | Parrot OS     | SIEM platform       |
| Target Agent  | Windows 10    | Monitored endpoint  |
| Attacker VM   | Kali Linux    | Runs simulated attacks |

---

## ✅ Features

- 🔍 RDP brute-force detection (Rule ID 60204)
- 🦠 Malware detection with EICAR (Rule IDs 62123, 62124)
- 🛡️ Active Response: IP auto-block via `firewalldrop`
- 📊 Real-time log ingestion from Windows Defender

---

## 📄 Documentation

See [`Wazuh_SIEM_Project_Final.docx`](./Wazuh_SIEM_Project_Final.docx) for full step-by-step implementation and screenshots.

---

## 📸 Screenshots

### Agent status in Wazuh
![Agent status](./Agent%20status%20in%20Wazuh%20dashboard.png)

### Wazuh dashboard login
![Dashboard login](./Wazuh%20dashboard%20login%20page.png)

### Wazuh manager service
![Manager service](./Wazuh%20manager%20service%20status%20(systemctl%20output).png)

### Nmap RDP scan
![Nmap scan](./Nmap%20scan%20result%20showing%203389_tcp%20open.png)

### Failed login detection
![Failed logins](./Wazuh%20Security%20Events%20panel%20with%20failed%20login%20alerts.png)

### Malware detection (EICAR)
![EICAR detected](./Wazuh%20alert%20showing%20malware%20detection%20(EICAR).png)

### Rule ID 60204 triggered
![Active response](./Rule%20ID%2060204%20triggered%20with%20description%20Multiple%20Windows%20logon%20failures.png)

---

## 🔜 Next Steps

- Add Sysmon for deeper process visibility  
- Enable email alerts  
- Deploy in a cloud-hosted SOC lab (AWS/Azure)

---

👋 Connect with me on [LinkedIn](https://www.linkedin.com/in/raj-konkar-b70b512a0/)
