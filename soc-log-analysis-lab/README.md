# 🛡️ SOC Analyst Log Analysis Lab

## 📌 Objective
This project simulates a Tier 1 SOC analyst investigating suspicious authentication activity using SIEM tools. The objective was to detect brute-force behavior, analyze indicators of compromise, and document response recommendations.

## 🧰 Tools Used
- Splunk Enterprise (Free)
- Windows Security Event Logs (CSV)
- GitHub

## 🔍 Investigation Overview
- Ingested authentication logs into Splunk
- Filtered failed login attempts (Event ID 4625)
- Identified repeated failures from a single external IP
- Correlated events across multiple user accounts
- Visualized activity using SOC dashboards

## 🚨 Key Findings
- Multiple failed login attempts from IP address **203.0.113.45**
- Targeted privileged and disabled accounts (admin, guest, root)
- Activity pattern consistent with brute-force authentication attacks

## 📊 Dashboards
A SOC-style dashboard was created to monitor authentication failures, source IP activity, and attack timelines.

## 🛠️ Recommendations
- Block malicious IP addresses at firewall
- Enforce account lockout thresholds
- Enable Multi-Factor Authentication (MFA)
- Improve alerting for authentication anomalies

## 📁 Repository Structure
```
soc-log-analysis-lab/
├── README.md
├── logs/
├── screenshots/
└── report/
```

## 🧠 What I Learned
- How SOC analysts use SIEM tools for threat detection
- How to identify brute-force attacks using log correlation
- How to document security incidents professionally
