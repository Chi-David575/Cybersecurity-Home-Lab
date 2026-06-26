# Cybersecurity-Home-Lab
A Windows-hosted cybersecurity lab environment utilizing Graylog for centralized log aggregation, threat detection, and real-time security monitoring.

# Cybersecurity Home Lab: Centralized Log Analysis
A Windows-based home lab environment designed for centralized log management and threat detection using Graylog and Wazuh.

## 🚀 Project Overview
This project focuses on building a functional Security Operations Center (SOC) pipeline to monitor and detect malicious activity. By integrating Wazuh for endpoint telemetry and Graylog for log aggregation, this lab simulates real-world threat detection workflows.

## 🛠️ Tech Stack
* **Host OS:** Windows
* **Security Tools:** Graylog
* **Infrastructure:** Docker (for service containerization)
* **Log Sources:** Windows Event Logs, Sysmon

## 🏗️ Architecture
[ Windows Host ] 
      |
      | (Generates Logs: Event Logs)
      v
[ Log Forwarder / Sidecar ] 
      |
      | (Transmits Data)
      v
[ Graylog Server (Docker) ]
      |
      | (Processes, Indexes & Stores)
      v
[ Graylog Web Interface ]
      |
      | (Visualizes & Alerts)
      v
[ Security Analyst ]

## 🔍 Key Features
* **Log Aggregation:** Centralized collection of logs from local Windows endpoints.
* **Threat Detection:** Configured rules to detect brute-force authentication attempts.
* **Incident Monitoring:** Created dashboards in Graylog to visualize security events and failed login patterns.

## 📈 Lessons Learned
* **Troubleshooting:** Overcame terminal errors during Docker container initialization by adjusting resource allocation.
* **Optimization:** Fine-tuned log streaming to ensure only relevant security data is indexed, reducing storage overhead.
* **Defender Mindset:** Learned to distinguish between benign system noise and actionable security alerts.

## 📸 Lab Evidence
[Insert screenshots of your Graylog Dashboard or Wazuh alert logs here]
