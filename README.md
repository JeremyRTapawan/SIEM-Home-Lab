# SIEM Home Lab/SSH Detections & Alerts

## Overview
This project simulates a **Security Operations Center (SOC)** environment using a Security Information and Event Management (SIEM) platform to centralize logs, detect suspicious activity, and perform basic incident triage. The lab mirrors real-world SOC workflows used by enterprise security teams.

---

## Tools & Technologies
- **SIEM Platform:** Splunk Enterprise
- **Operating Systems:** Linux (Ubuntu), Windows
- **Virtualization:** Oracle VirtualBox
- **Log Sources:**
  - Linux authentication logs (`/var/log/auth.log`)
  - Windows Event Logs

---

## Design Decisions
- Deployed the SIEM on a **dedicated Linux server** to replicate enterprise SOC architecture
- Used **both Linux and Windows endpoints** to demonstrate cross-platform log ingestion
- Centralized logs to enable **correlation and detection** across multiple hosts
- Focused on **authentication-related events** as a common SOC detection use case

---

## Lab Architecture
The lab consists of a centralized SIEM server collecting logs from multiple endpoints within an isolated internal network.
![SIEM](https://github.com/user-attachments/assets/6fb58430-d766-4e15-b569-7e560887208c)


---

## Methodology
- Deployed Linux and Windows virtual machines on an internal network
- Installed and configured the SIEM platform on a Linux server
- Configured log forwarding from endpoints to the SIEM
- Generated normal authentication activity to establish a baseline
- Simulated suspicious behavior (failed login attempts)
- Created alerts to detect abnormal authentication patterns
- Reviewed alerts to perform basic incident triage

---

##  Key Use Cases
- Detection of repeated authentication failures
- Identification of potential brute-force login attempts
- Monitoring of user authentication activity across hosts
- Comparison of baseline versus anomalous behavior

---

## Analysis & Alerting
Custom SIEM searches and alerts were created to identify suspicious authentication activity. Dashboards were used to visualize login trends, failed attempts, and event timelines to support SOC-style analysis.

---

## Limitations
- Detection logic was limited to **authentication-based events**
- Alerts were tuned for a lab environment and not production scale
- No automated response actions were implemented

---

## Skills Demonstrated
- SIEM deployment and configuration
- Log ingestion and normalization
- Alert creation and tuning
- Basic SOC incident triage
- Security monitoring and analysis
- Enterprise security tooling familiarity

---

## Notes
This project was conducted in a **controlled lab environment** for educational purposes. All systems used private IP addressing and simulated activity only.
All systems operate within a **private LAN environment** using non-routable IP addressing.

