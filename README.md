Nikto Web Server Scanning – Basic Security Testing

Nikto Platform Purpose

📌 Overview

This project documents a basic Nikto web server security assessment performed using Kali Linux.

Nikto is an open-source web server scanner that checks web servers for potentially interesting files, outdated components, insecure configurations, and other commonly known issues.

> ⚠️ Legal & Ethical Notice: Only scan websites, servers, or applications that you own or have explicit permission to test. The screenshots are provided as a learning demonstration.




---

🛠️ Tool Used

Tool: Nikto

Version: 2.6.1

Operating System: Kali Linux

Interface: Terminal



---

🚀 Installation

Nikto can be installed on Kali Linux using:

sudo apt update
sudo apt install -y nikto

Check the installed version:

nikto -Version

Example:

Nikto 2.6.1 (LW 2.5)


---

📖 Help & Options

To view Nikto's available options:

nikto -h

Some commonly used options:

Option	Purpose

-h	Display help / specify host
-Version	Display Nikto version
-url	Specify target URL/host
-p	Specify port
-ssl	Force SSL mode
-output	Save scan results to a file



---

🔍 Basic Scan

For an authorized lab target, a basic scan can be started with:

nikto -h http://TARGET

For HTTPS:

nikto -h https://TARGET

Replace TARGET with a host that you are authorized to assess.


---

🧪 Scan Result Example

During the demonstration, Nikto displayed information such as:

Target IP address

Target hostname

Target port

Web server/platform information

Multiple IP addresses

HTTP response information

CGI directory test status


Example:

- Nikto v2.6.1

+ Target IP:        ...
+ Target Hostname:  ...
+ Target Port:      80
+ Platform:         Unknown
+ Server:           ...

Important

A Nikto result is not automatically proof of a vulnerability. Findings should be manually verified and interpreted in the context of the target environment.


---

📸 Screenshots

1. Nikto Installation

Nikto Installation

2. Nikto Version & Help

Nikto Help

3. Example Scan Output

Nikto Scan


---

🎯 Learning Objectives

This exercise demonstrates:

1. Installing Nikto on Kali Linux.


2. Checking the installed Nikto version.


3. Understanding Nikto command-line options.


4. Performing a basic web-server assessment in an authorized environment.


5. Reading and interpreting scanner output.


6. Understanding that automated scanner findings require manual verification.




---

🧠 What is Nikto?

Nikto is a web server scanner designed to identify potentially interesting or insecure web-server configurations and files.

It can help security professionals during the reconnaissance and vulnerability-assessment stages of an authorized security assessment.


---

📂 Project Structure

nikto-web-server-scan/
├── README.md
├── 1000521170.jpg
├── 1000521171.jpg
└── 1000521172.jpg


---

⚠️ Responsible Use

Use Nikto only for:

Your own websites

Local test servers

CTF/lab environments

Systems where you have written authorization


Unauthorized scanning may violate laws, terms of service, or organizational policies.


---

👨‍💻 Author

PsychoMods

Cybersecurity learning & security research projects.
