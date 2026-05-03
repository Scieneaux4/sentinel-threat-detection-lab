
# Microsoft Sentinel Threat Detection Lab

## 📌 Overview
In this project, I built a SIEM lab using Microsoft Sentinel in Azure to simulate and detect real-world attack activity. The lab focuses on monitoring authentication events, identifying brute-force login attempts, and investigating suspicious behavior through log analysis.

---

## 🎯 Objectives
- Ingest and analyze security logs from a Windows virtual machine
- Simulate brute-force login attempts
- Create detection rules within Microsoft Sentinel
- Investigate alerts and identify indicators of compromise (IOCs)

---

## 🧱 Environment Setup
- Microsoft Azure
- Microsoft Sentinel (SIEM)
- Windows Virtual Machine
- Log Analytics Workspace

The virtual machine was configured to generate authentication logs, which were then ingested into Sentinel for monitoring and analysis.

---

## 🚨 Attack Simulation
To simulate real-world attack activity:
- Multiple failed login attempts were generated against the VM
- Successful login attempts were also performed to compare patterns
- Authentication logs were collected and forwarded to Sentinel

This created a dataset representing brute-force attack behavior.

---

## 📊 Log Analysis & Investigation
Using Microsoft Sentinel and Log Analytics:

- Queried authentication logs to identify failed login attempts
- Compared Event ID **4625 (failed login)** and **4624 (successful login)**
- Identified patterns of repeated login attempts from the same source
- Investigated timestamps and login frequency to detect anomalies

---

## ⚠️ Detection & Alerting
- Created analytics rules in Microsoft Sentinel to detect suspicious login activity
- Configured alerts based on repeated failed login attempts
- Triggered alerts and validated detection accuracy

---

## 🔍 Findings
- Repeated failed login attempts can indicate brute-force attacks
- Successful logins following multiple failures may indicate compromised credentials
- Log analysis is critical for identifying early signs of attack activity

---

## 🧠 Skills Demonstrated
- SIEM (Microsoft Sentinel)
- Log Analysis
- Threat Detection
- Incident Investigation
- Understanding of authentication-based attacks

---

## 📸 Screenshots & Walkthrough

### 🔹 Authentication Logs in Sentinel
(Insert screenshot here)

### 🔹 Failed Login Attempts (Event ID 4625)
(Insert screenshot here)

### 🔹 Successful Login Events (Event ID 4624)
(Insert screenshot here)

### 🔹 Detection Rule / Alert Trigger
(Insert screenshot here)

---

## ✅ Conclusion
This lab demonstrates how a SOC analyst can use Microsoft Sentinel to monitor systems, detect suspicious login behavior, and investigate potential security incidents using real log data.
