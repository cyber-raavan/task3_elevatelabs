# Task 3: Vulnerability Scan Report

This repository contains the documentation and findings for **Task 3: Perform a Basic Vulnerability Scan on Your PC**.

## Overview
The task involved:
1. Installing and using a vulnerability scanner (OpenVAS, Nessus, or equivalent).  
   - I used **ManageEngine Vulnerability Manager Plus** for its free and user-friendly interface.  
2. Scanning my personal PC (Windows 11 - *Phoenix*).  
3. Reviewing and classifying vulnerabilities into **Critical, High, and Medium** severity.  
4. Researching remediation and mitigation steps for critical vulnerabilities.

## Key Findings
- Multiple applications such as **VMware Workstation, Google Chrome, VLC Media Player, WinRAR, 7-Zip, Adobe Photoshop, CURL, and MS Visual C++** had vulnerabilities.  
- Vulnerabilities included **Remote Code Execution (RCE), Guest-to-Host Escapes, Memory Corruption, and Privilege Escalation flaws**.  
- Several vulnerabilities had **patches available**, while legacy/unsupported software like older Photoshop versions remained vulnerable.

## Critical Vulnerabilities Researched
1. **VLC Media Player** (CVE-2023-47359, CVE-2023-47360) – Remote code execution via malicious video files.  
2. **VMware Workstation** (CVE-2025-22224, CVE-2025-41225–41228) – Guest-to-host escape vulnerabilities.  
3. **Google Chrome** (CVE-2025-10890, CVE-2025-10892) – Zero-day browser exploits.  
4. **WinVerifyTrust** (CVE-2013-3900) – Signature validation bypass.  
5. **WinRAR / 7-Zip** – Archive parsing flaws leading to code execution.  

## Mitigation Recommendations
- **Update vulnerable applications** (WinRAR 7.13, 7-Zip 25.01, VLC 3.0.21, Chrome 140.0.7339.208, VMware Workstation 17.6.4, etc.).  
- **Apply registry fixes/workarounds** where patches are unavailable (e.g., WinVerifyTrust).  
- **Upgrade unsupported software** (e.g., Adobe Photoshop CC 21.x → Latest Creative Cloud release).  
- **Enforce stricter policies** like AppLocker, EDR monitoring, and application inventory for long-term resilience.  

## Repository Contents
- `README.md` (this file)  
- `task3report.pdf` – Full detailed report with vulnerability tables, research, and remediation steps.  
- `ScannedVulnerabilities.csv` scan result file in .csv format. (For Raw DATA)
-  `ScannedVulnerabilities.pdf` scan result file in .pdf format. (For Readable DATA)

## Author
**Kush Thaker**  
📧 kthaker442@gmail.com  

---
👉 For full details and screenshots, please see the [task3report.pdf](./Task3Report.pdf).
