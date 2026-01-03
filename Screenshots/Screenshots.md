## Screenshots & Evidence
### Active Log Forwarding
![Forwarder Active](screenshots/forwarder-active.png)

This screenshot confirms that the Splunk Universal Forwarder on the Windows system is actively connected to the Splunk receiver on the Ubuntu SIEM server, ensuring continuous and reliable log forwarding.

---

### Log Ingestion Verification
![Logs Ingested](screenshots/logs-ingested.png)

Splunk search results showing successful ingestion of events into the default index, validating end-to-end log collection from connected endpoints.

---

### Windows Failed Login Detection
![Windows Failed Login](screenshots/windows-failed-login.png)

This search identifies Windows authentication failures (Event ID 4625), demonstrating the SIEM’s ability to detect suspicious login activity commonly associated with brute-force attacks.

---

### Splunk Receiving Port Configuration
![Receiving Port](screenshots/splunk-receiving-port.png)

Splunk Enterprise configured to receive forwarded logs on TCP port 9997, enabling secure ingestion of log data from Universal Forwarders.

---

### Triggered Security Alerts
![Triggered Alerts](screenshots/triggered-alerts.png)

The Triggered Alerts view confirms that both Windows failed login detection and SSH brute-force detection alerts successfully fired after simulated attack activity.

---

### SOC Authentication Monitoring Dashboard
![SOC Dashboard](screenshots/soc-dashboard.png)

A custom SOC dashboard visualizing authentication activity, failed login attempts, and detected brute-force behavior to support security monitoring and basic incident triage.

---

*All IP addresses, hostnames, and credentials shown in this repository belong to an isolated lab environment.*
