## Screenshots & Evidence
### Active Log Forwarding
![activeforwarding](https://github.com/user-attachments/assets/d0fc914f-5674-4a01-bc7a-78d444f4fc47)

This screenshot confirms that the Splunk Universal Forwarder on the Windows system is actively connected to the Splunk receiver on the Ubuntu SIEM server, ensuring continuous and reliable log forwarding.

---

### Log Ingestion Verification
![logs-ingested](https://github.com/user-attachments/assets/8e0f9f57-4c89-42d2-859b-bf7deb591e97)

Splunk search results showing successful ingestion of events into the default index, validating end-to-end log collection from connected endpoints.

---

### Windows Failed Login Detection
![failedlogin](https://github.com/user-attachments/assets/b0ca8874-680f-4c7a-afac-8c17415b6381)

This search identifies Windows authentication failures (Event ID 4625), demonstrating the SIEM’s ability to detect suspicious login activity commonly associated with brute-force attacks.

---

### Splunk Receiving Port Configuration
![ReceivingPort](https://github.com/user-attachments/assets/e56cb0fb-ed56-4f85-8eae-369521e93153)

Splunk Enterprise configured to receive forwarded logs on TCP port 9997, enabling secure ingestion of log data from Universal Forwarders.

---

### Triggered Security Alerts
![tiggeralerts](https://github.com/user-attachments/assets/9d033536-181c-4c5b-8541-c774f0e133b3)

The Triggered Alerts view confirms that both Windows failed login detection and SSH brute-force detection alerts successfully fired after simulated attack activity.

---

### SOC Authentication Monitoring Dashboard
![dashboard](https://github.com/user-attachments/assets/2fa9d210-a463-41f0-8d59-0fbc53641921)

A custom SOC dashboard visualizing authentication activity, failed login attempts, and detected brute-force behavior to support security monitoring and basic incident triage.

---

*All IP addresses, hostnames, and credentials shown in this repository belong to an isolated lab environment.*
