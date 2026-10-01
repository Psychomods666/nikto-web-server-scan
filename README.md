
<div align="center">

# 🔎 Nikto Web Server Security Assessment

### Web Server Scanning & Security Testing with Kali Linux

![Nikto](https://img.shields.io/badge/Nikto-2.6.1-blue?style=for-the-badge)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-Security%20Testing-black?style=for-the-badge)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Learning-red?style=for-the-badge)
![Web Security](https://img.shields.io/badge/Web%20Security-Assessment-orange?style=for-the-badge)

</div>

---

## 🧭 Overview

This project demonstrates the use of **Nikto** for basic web server security assessment in a Kali Linux environment.

Nikto is an open-source web server scanner that checks for potentially interesting files, outdated server components, insecure configurations, and other commonly known issues.

The project documents the complete learning workflow:

```text
Installation
    ↓
Version Verification
    ↓
Command & Options
    ↓
Authorized Web Server Scan
    ↓
Result Analysis

> ⚠️ Ethical Use: Perform security testing only against systems you own or have explicit authorization to assess.




---

🎯 Objectives

Install Nikto on Kali Linux

Verify the Nikto installation

Learn essential Nikto options

Understand web server scanning

Perform a basic authorized scan

Read and interpret scan output

Understand the limitations of automated scanners

Practice documenting security testing results



---

🛠️ Tools & Technologies

Tool	Purpose

🐉 Kali Linux	Security testing environment
🔎 Nikto	Web server scanner
💻 Terminal	Command-line interface
🌐 HTTP/HTTPS	Web protocols



---

🧪 Practical Walkthrough

01 — Installation

Command

sudo apt update
sudo apt install -y nikto

What it does

Installs Nikto and its required packages on Kali Linux.

📸 Terminal Evidence

Screenshot of Nikto installation showing the package installation process in Kali Linux terminal.


---

02 — Verify Installation

After installation, verify the installed version.

Command

nikto -Version

Example Output

Nikto 2.6.1 (LW 2.5)

📸 Terminal Evidence

Screenshot of Nikto version 2.6.1 displayed in the Kali Linux terminal.


---

03 — Explore Nikto Options

Command

nikto -h

This displays the available command-line options.

Common Options

Option	Description

-h	Specify host / display help
-Version	Display Nikto version
-url	Specify target URL
-p	Specify port
-ssl	Force SSL mode
-output	Save scan results



---

04 — Basic Authorized Scan

For a system that you own or have explicit permission to test:

HTTP

nikto -h http://TARGET

HTTPS

nikto -h https://TARGET

Replace TARGET with your authorized lab server.


---

📸 Scan Evidence

The following screenshot shows example Nikto scan output, including target information and server response details.

Screenshot of Nikto displaying target and web server scan information in Kali Linux terminal.


---

📊 Understanding the Output

Nikto may display information such as:

Target IP
Target Hostname
Target Port
Platform
Web Server
HTTP Response Information
Multiple IP Addresses
CGI Information
Potentially Interesting Findings

Example

+ Target IP:        ...
+ Target Hostname:  ...
+ Target Port:      80
+ Platform:         Unknown
+ Server:           ...

> Important: A scanner finding does not automatically mean that a confirmed vulnerability exists. Findings should be manually verified.




---

🔬 Key Learning

What Nikto Can Help Identify

Potentially outdated server components

Interesting files and directories

Common web-server issues

HTTP configuration information

Potentially insecure configurations


What Nikto Does NOT Replace

Automated Scan
      ↓
Potential Finding
      ↓
Manual Verification
      ↓
Security Analysis
      ↓
Final Finding

Automated tools are useful for discovery, but security professionals still need to validate and understand the results.


---

🧠 What I Learned

Through this practical, I learned how to:

Install Nikto on Kali Linux

Verify the installation

Use Nikto's help menu

Understand common scanning options

Perform basic authorized web-server assessment

Read scanner output

Document security-testing evidence

Distinguish scanner findings from confirmed vulnerabilities



---

🛡️ Scope & Authorization

Activity	Environment	Authorization

Nikto Installation	Local Kali Linux	Own system
Command Testing	Local environment	Own system
Web Server Assessment	Authorized lab/test target	Explicit permission required


> 🔐 Only scan systems that you own or have explicit permission to test.




---

📁 Project Structure

nikto-web-server-scan/
│
├── README.md
│
├── 1000521170.jpg
├── 1000521171.jpg
└── 1000521172.jpg


---

<details>
<summary>📸 View All Screenshots</summary>Installation

Nikto installation screenshot.

Version & Help

Nikto version and command help screenshot.

Scan Output

Nikto web server scan output screenshot.

</details>
---

⚠️ Responsible Use

This repository is intended for educational cybersecurity learning and authorized security testing.

Nikto should only be used against:

Your own websites

Your own servers

Local test environments

CTF/lab environments

Systems where you have explicit written authorization


Unauthorized scanning can violate laws, organizational policies, or terms of service.


---

👨‍💻 Author

<div align="center">PsychoMods

Cybersecurity • Security Research • Technology

⭐ Learning by building and documenting.

</div>
