# 🔎 Nikto Web Server Security Scanning

Basic web server security assessment using **Nikto on Kali Linux**

![Nikto](https://img.shields.io/badge/Tool-Nikto-blue)
![Kali Linux](https://img.shields.io/badge/OS-Kali%20Linux-black)
![Cybersecurity](https://img.shields.io/badge/Skill-Cybersecurity-red)
![Web Security](https://img.shields.io/badge/Skill-Web%20Security-orange)
![Security Testing](https://img.shields.io/badge/Type-Security%20Testing-green)

---

## 📌 Project Overview

This project demonstrates the basic use of **Nikto**, an open-source web server scanner used during security assessments.

The practical covers:

1. Installing Nikto on Kali Linux.
2. Checking the installed Nikto version.
3. Understanding Nikto command-line options.
4. Performing a basic web server scan.
5. Understanding and interpreting scanner output.

Nikto is commonly used during the reconnaissance and vulnerability-assessment stages of an authorized security assessment.

> ⚠️ **Important:** Nikto should only be used against systems that you own or have explicit permission to test.

---

## 🎯 Objectives

- Install Nikto on Kali Linux.
- Verify the Nikto installation.
- Learn basic Nikto commands.
- Understand important command-line options.
- Perform a basic authorized web server scan.
- Identify information returned by the scanner.
- Understand that automated findings require manual verification.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Kali Linux | Security testing environment |
| Nikto | Web server scanner |
| Terminal | Command-line interface |

---

## 🛡️ Scope & Authorization

| Phase | Target | Authorization |
|---|---|---|
| Installation | Local Kali Linux system | Own system |
| Nikto Testing | Authorized lab/test server | Explicit permission |

> ⚠️ **Important:** Security scanning must only be performed against systems you own or have explicit authorization to test.

---

# 🧪 Part 1 — Nikto Installation

## Task 1 — Install Nikto

### Command

```bash
sudo apt update
sudo apt install -y nikto

Explanation

This command updates the package information and installs Nikto on Kali Linux.

Screenshot

Nikto Installation


---

🔍 Part 2 — Verify Nikto Installation

Task 2 — Check Nikto Version

Command

nikto -Version

Example Output

Nikto 2.6.1 (LW 2.5)

Explanation

This command displays the installed Nikto version and confirms that Nikto is available on the system.

Screenshot

Nikto Version


---

📖 Part 3 — Nikto Help & Options

Task 3 — View Nikto Commands

Command

nikto -h

Explanation

The -h option displays Nikto's available command-line options.

Some useful options include:

Option	Description

-h	Display help / specify target
-Version	Display Nikto version
-url	Specify target URL
-p	Specify target port
-ssl	Force SSL mode
-output	Save results to a file



---

🌐 Part 4 — Basic Web Server Scan

Task 4 — Scan an Authorized Target

For an authorized lab or test server:

HTTP

nikto -h http://TARGET

HTTPS

nikto -h https://TARGET

Replace TARGET with the hostname or IP address of a system you are authorized to test.


---

🧪 Example Scan Output

A Nikto scan can provide information such as:

Target IP address

Target hostname

Target port

Web server information

HTTP response information

Multiple IP addresses

CGI directory information

Potentially interesting server configurations


Example

- Nikto v2.6.1

+ Target IP:        ...
+ Target Hostname:  ...
+ Target Port:      80
+ Platform:         Unknown
+ Server:           ...

Screenshot

Nikto Scan Output


---

📊 Part 5 — Understanding the Results

Nikto results should be interpreted carefully.

A scanner finding does not automatically mean that a vulnerability exists.

Security professionals should manually verify findings and consider:

Server configuration

Application behavior

HTTP response codes

Software versions

Whether the finding is relevant to the environment



---

🧠 What I Learned

Through this practical, I learned:

How to install Nikto on Kali Linux.

How to verify the installation.

How to access Nikto's help menu.

How web server scanning works.

How to read basic Nikto output.

Why automated security findings require manual verification.

The importance of authorization during security testing.



---

📂 Project Structure

nikto-web-server-scan/
│
├── README.md
│
├── 1000521170.jpg
├── 1000521171.jpg
└── 1000521172.jpg


---

⚠️ Responsible Use

This project is intended for educational and authorized security testing.

Use Nikto only against:

Your own websites

Your own servers

Local test environments

CTF/lab environments

Systems for which you have explicit permission


Unauthorized security scanning may violate laws, policies, or terms of service.


---

👨‍💻 Author

PsychoMods

Cybersecurity Learning & Security Research


---

⭐ If you found this project useful, consider giving the repository a star.
