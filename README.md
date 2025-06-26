# CyberSecurityinternship-task-3
# 🛡️ Cybersecurity Internship – Task 3 

## 📌 Task Title:
**Basic Vulnerability Scan of a Personal Computer**

---

## 🧠 Objective:
To perform a basic vulnerability assessment on a personal computer using open-source tools like OpenVAS or Nessus Essentials. The goal was to identify existing system vulnerabilities and understand their severity levels based on CVSS.

---

## 🛠️ Tools Used:
- [Nessus Essentials](https://www.tenable.com/products/nessus/nessus-essentials) (Free version)
- OR [OpenVAS](https://www.greenbone.net/en/community-edition/)
- Web browser (for GUI-based dashboard access)
- Localhost as the scan target (`127.0.0.1` or your local IP)

---

## 🧪 Experiment Steps:

### 🧩 Step 1: Tool Setup
- Installed **Nessus Essentials** on the local machine (Linux/Windows)
- Registered with an activation code (free via Tenable)
- Set up the Nessus web interface at `https://localhost:8834`

---

### 🧩 Step 2: Scan Configuration
- Created a new scan with:
  - **Scan type**: Advanced Scan
  - **Target**: Localhost IP or `127.0.0.1`
  - **Scan Settings**: Default for full port and service checks
- Started the scan and allowed 30-45 minutes for completion.

---

### 🧩 Step 3: Review of Scan Report
Once the scan completed, the Nessus dashboard generated a detailed report with:

- Vulnerability severity levels (Critical, High, Medium, Low, Info)
- CVEs (Common Vulnerabilities & Exposures)
- Suggested solutions or patches

---

## 🔍 Top Vulnerabilities Identified:

| Vulnerability Name                  | CVSS Score | Severity  | Description                                      | Suggested Fix                     |
|------------------------------------|------------|-----------|--------------------------------------------------|-----------------------------------|
| Outdated OpenSSH Server            | 9.8        | Critical  | Allows remote code execution via crafted packet | Update OpenSSH to latest version |
| SSL/TLS Weak Cipher Suites Enabled | 7.5        | High      | Server supports outdated cryptographic ciphers   | Disable weak ciphers in configs  |
| SMB Signing Not Required           | 6.1        | Medium    | May allow MITM attacks                          | Enforce SMB signing              |

📌 *Report export and screenshots included in the repo.*

---


## 🔒 Security Insights:

- **CVSS (Common Vulnerability Scoring System)** was used to assess severity.
- Prioritization was based on potential impact and exploitability.
- Identified outdated packages and weak configurations on local services.

---

## ✅ Conclusion:

The scan exposed multiple vulnerabilities including outdated software and weak encryption support. Fixing these issues by updating software and disabling insecure protocols significantly improves the system's security posture. This task provided practical knowledge of using vulnerability scanners, understanding CVSS scores, and interpreting security risks.

---

## 🧠 Concepts Learned:

- Vulnerability Scanning vs Penetration Testing
- Using Nessus or OpenVAS for assessment
- Understanding CVSS scores and severity ratings
- Importance of regular scanning and patching
- Identifying false positives vs actual threats

---

## 🙋‍♂️ Author:

**Name:** Spandan Jana
**Role:** Cybersecurity Intern 
**Task Date:** 26th June 2025
