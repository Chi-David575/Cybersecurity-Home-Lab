# Cybersecurity-Home-Lab
A Windows-hosted cybersecurity lab environment utilizing Graylog for centralized log aggregation, threat detection, and real-time security monitoring.

# Cybersecurity Home Lab: Centralized Log Analysis

I built this lab because I wanted to move beyond the theory and understand how security teams actually catch bad actors in the wild. This project is my sandbox for log management and threat detection.

## 🚀 The Mission
My goal with this setup was to create a functional Security Operations Center (SOC) pipeline. By combining the deep visibility of Sysmon with the powerful analysis of Graylog, I’ve built a lab that can actually spot malicious activity rather than just logging random system events.

## 🛠️ My Tech Stack
* **Host:** Windows 10/11
* **Analysis Engine:** Graylog (running in Docker)
* **Endpoint Telemetry:** Sysmon (System Monitor)
* **Data Sources:** Windows Event Logs & Sysmon Events

## 🏗️ Architecture
I wanted to keep the data flow simple but effective:


[ Windows Host (Sysmon + Logs) ] 
      |
      | (Log Forwarding)
      v
[ Graylog Server (Docker) ]
      |
      v
[ Dashboard & Alerting ]
## 🔍 Key Features
* **Log Aggregation:** Centralized collection of logs from local Windows endpoints.
* **Threat Detection:** Configured rules to detect brute-force authentication attempts.
* **Incident Monitoring:** Created dashboards in Graylog to visualize security events and failed login patterns.

  ## 📸 Lab Evidence
Here is a snapshot of my Graylog instance detecting a brute force attack within my environment:

![Brute Force Detection](https://github.com/Chi-David575/Cybersecurity-Home-Lab/blob/main/Screenshot%202026-06-11%20143434.png)

## 📈 Lessons Learned
* **Troubleshooting:** Overcame terminal errors during Docker container initialization by adjusting resource allocation.
* **Optimization:** Fine-tuned log streaming to ensure only relevant security data is indexed, reducing storage overhead.
* **Defender Mindset:** Learned to distinguish between benign system noise and actionable security alerts.

