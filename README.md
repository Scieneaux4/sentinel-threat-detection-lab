# Microsoft Sentinel Threat Detection Lab
---

In this project, I built a SIEM lab using Microsoft Sentinel in Azure to monitor and analyze authentication activity from a Windows virtual machine. The virtual machine was intentionally exposed to the internet as a honeypot to attract and capture real-world login attempts. The goal of this lab was to simulate real attack behavior and gain hands-on experience working with logs, detecting suspicious activity, and understanding how security events are investigated in a SOC environment.

---

## 📸 Screenshots & Walkthrough

### 1️⃣ Authentication Logs Ingested
![Logs](insert-image-link)

This screenshot shows Windows Security logs successfully ingested into Microsoft Sentinel. These logs include authentication events such as logon attempts, which serve as the foundation for detecting suspicious or potentially malicious activity.

---

### 2️⃣ Failed Login Attempts (Event ID 4625)
![Failed Logins](insert-image-link)

Here, I filtered for failed login attempts (Event ID 4625) to identify repeated authentication failures. A high volume of failed logins within a short period of time can indicate brute-force attack behavior against the system.

---

### 3️⃣ Successful Login Events (Event ID 4624)
![Successful Logins](insert-image-link)

This view shows successful login events (Event ID 4624), which are useful for comparing against failed attempts during an investigation. Looking at both successful and failed logins together helps provide better context around user activity.

---

### 4️⃣ Detection Query
![Query](insert-image-link)

In this step, I used a query in Microsoft Sentinel to filter authentication logs and isolate suspicious login behavior. Writing and refining queries is a key part of identifying patterns and narrowing down potential threats.

---

### 5️⃣ Alert / Detection Rule
![Alert](insert-image-link)

I configured an alert rule in Microsoft Sentinel to trigger when suspicious login activity is detected. This allows for automated detection and helps simulate how alerts would be generated in a real SOC environment.

---

### 6️⃣ Investigation Timeline
![Timeline](insert-image-link)

This timeline view shows authentication activity over time, making it easier to spot unusual patterns such as spikes in failed login attempts or abnormal login behavior.

---

## ✅ Summary

Through this lab, I was able to build a working SIEM environment and gain hands-on experience analyzing authentication logs, detecting brute-force activity, and investigating suspicious behavior. This project reflects the core workflow of a SOC analyst, from monitoring and detection to investigation and analysis.
