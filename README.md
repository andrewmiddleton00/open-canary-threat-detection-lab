# open-canary-threat-detection-lab
A personal SOC lab project using OpenCanary honeypot, Python log analysis, and Streamlit dashboards.
# OpenCanary Threat Detection Lab

This project simulates a SOC workflow using OpenCanary to detect attacker behavior, collect logs, and build a Python dashboard for analysis. It's a personal lab project designed to improve my hands-on detection, investigation, and automation skills as a future SOC Analyst.

---

## 🔧 Lab Environment

- **Honeypot:** Ubuntu 24.04 VM with OpenCanary installed
- **Analyst Workstation:** Kali Linux VM
- **Virtualization:** Oracle VirtualBox with Host-only Adapter + Static IPs
- **Log Transport:** Shared folder (manual transfer after troubleshooting)

---

## 📌 Objectives

- Deploy OpenCanary to emulate services like SSH, HTTP, FTP
- Simulate attacker activity (Nmap scans, curl requests)
- Collect and analyze `access.log` from honeypot
- Build a Streamlit dashboard for log visualization
- Create an incident response playbook

---

## 🧠 Key Skills Practiced

- Log analysis & parsing (Python + Pandas)
- Data visualization (Streamlit, Matplotlib)
- Threat detection (port scans, web probes)
- Troubleshooting VM networking issues
- Building IR playbooks

---

## 🧪 Project Artifacts

### 📋 [Playbook: Port Scan Investigation](playbooks/port-scan-investigation.md)

### 📸 Screenshots  
![Streamlit Dashboard](screenshots/streamlit_dashboard.png)  
![Canary Logs](screenshots/canary_log_sample.png)

---

## 🚀 Next Steps

- Add automatic alerting for high-severity events
- Integrate basic threat intel lookups (VirusTotal, AbuseIPDB)
- Expand dashboard with timestamp filtering and attacker summaries

---

## 🧑‍💻 Author

Andrew – Aspiring SOC Analyst | Cloud Security Engineer-in-Training  
🔗 GitHub: [yourusername]  
📘 LinkedIn: www.linkedin.com/in/andrew-middleton-8b00a3327

# Incident Response Playbook: Port Scan Detected on Honeypot

**Date:** July 18, 2025  
**Source:** OpenCanary (Ubuntu VM)  
**Log File:** `access.log`

3. Monitored `access.log` for new events
4. Transferred log to Kali using VirtualBox shared folder
5. Parsed log using Python and visualized with Streamlit

---

## 🔬 Analysis Observations

- Detected multiple connections in rapid succession
- SSH and HTTP ports hit within milliseconds
- Activity matched typical scanning behavior

---

## 🛡️ Response Actions

- Logged source IP for tracking
- Created Streamlit dashboard to monitor additional hits
- No real system compromise – environment was simulated

---

## 📊 Outcome

- Successfully detected and visualized port scan
- Demonstrated how a SOC analyst can detect early-stage recon



---

## 🧭 Summary

A simulated attacker from `192.168.56.102` performed a horizontal port scan using Nmap. The honeypot captured interaction attempts on SSH, FTP, and HTTP.

---

## 🔍 Detection Steps

1. Deployed OpenCanary with common services emulated
2. Ran Nmap scan from Kali VM:

3. Monitored `access.log` for new events
4. Transferred log to Kali using VirtualBox shared folder
5. Parsed log using Python and visualized with Streamlit

---

## 🔬 Analysis Observations

- Detected multiple connections in rapid succession
- SSH and HTTP ports hit within milliseconds
- Activity matched typical scanning behavior

---

## 🛡️ Response Actions

- Logged source IP for tracking
- Created Streamlit dashboard to monitor additional hits
- No real system compromise – environment was simulated

---

## 📊 Outcome

- Successfully detected and visualized port scan
- Demonstrated how a SOC analyst can detect early-stage recon

