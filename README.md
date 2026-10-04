# SOC-Threat-Detection-Suricata-Splunk
End-to-End SOC Detection Pipeline using Suricata NIDS &amp; Splunk SIEM.
# Network Intrusion Detection & SIEM Alerting System (Suricata + Splunk)

![Domain](https://img.shields.io/badge/Domain-SOC%20%7C%20SIEM%20%7C%20Threat%20Detection-blue)
![Tools](https://img.shields.io/badge/Tools-Suricata%20%7C%20Splunk%20%7C%20Kali%20Linux-orange)

## 📌 Project Overview
This project demonstrates an end-to-end **Security Operations Center (SOC) Detection Pipeline**. It involves setting up **Suricata NIDS** to monitor network traffic, writing custom intrusion detection rules for SSH threat patterns, forwarding logs to **Splunk SIEM** for indexing, simulating SSH attack vectors using **Kali Linux** against an **Ubuntu target**, and configuring real-time SIEM alerting.

---

## 🏗️ Architecture & Lab Setup
- **Attacker Machine:** Kali Linux (Attack Simulation)
- **Target Machine:** Ubuntu Server
- **Network NIDS:** Suricata (Custom Rule Engine)
- **SIEM Platform:** Splunk Enterprise (Log Analysis & Alerting)

---

## 🛠️ Implementation Steps

### 1. Suricata Custom Rule Creation
Created custom IDS signature rules in Suricata to detect suspicious SSH connection attempts and payload patterns targeting the Ubuntu server.

### 2. Splunk Data Ingestion & Indexing
- Configured Splunk Universal Forwarder / Log Ingestion to process Suricata `eve.json` and alert logs.
- Created a dedicated **Splunk Index** for network threat analysis.

### 3. Threat Simulation & Attack Execution
- Performed SSH brute-force and connection attempts from Kali Linux targeting the Ubuntu machine.
- Verified traffic interception and signature triggers in Suricata logs.

### 4. Splunk SIEM Detection & Real-time Alerting
- Queried Splunk logs using **SPL (Search Processing Language)** to correlate SSH alert events.
- Configured custom **Splunk Real-time Alerts** to notify upon detecting malicious SSH activity threshold breaches.

---

## 📊 Key Takeaways & SOC Skills Learned
- Writing and testing custom **NIDS rules** in Suricata.
- Log aggregation, ingestion, and index management in **Splunk Enterprise**.
- Analyzing real-time threat telemetry and building actionable **SIEM Alerting Rules**.
- Hands-on threat simulation using Kali Linux against Linux endpoints.

---

## 👤 Author
**Ishan Mittal**  
*Aspiring Cybersecurity Analyst & SOC Engineer*  
- **LinkedIn:** [www.linkedin.com/in/ishan-mittal-215005mi10]
- **GitHub:** https://github.com/Ishan-mittal105
