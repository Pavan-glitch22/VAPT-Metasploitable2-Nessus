#  VAPT Report — Metasploitable 2 (Nessus Essentials)

##  Introduction

In this project, I performed a Vulnerability Assessment and Penetration Testing (VAPT) on Metasploitable 2, which is an intentionally vulnerable Linux machine used for practicing cybersecurity.

The main goal of this project was to understand how real-world vulnerability scanning works and how security issues are identified in a system. I used Nessus Essentials for scanning and performed the entire setup in a virtual lab environment to ensure safe testing.

This project helped me understand how attackers can find weaknesses in systems and how those issues can be fixed.

---

##  Objective

- To perform vulnerability assessment on a vulnerable system  
- To identify security issues using Nessus  
- To understand the severity of vulnerabilities using CVSS  
- To analyze how these vulnerabilities can be exploited  
- To suggest possible fixes for the identified issues  
- To gain hands-on experience in cybersecurity tools  

---

##  Project Overview

This project is based on scanning Metasploitable 2 using Nessus Essentials.

- Scan Type: Basic Network Scan  
- Total Vulnerabilities Found: 68  
- Scan Duration: 14 minutes  
- Environment: VirtualBox Lab  

The scan detected multiple vulnerabilities including critical, high, and medium-level issues.

---

##  Tools Used

- Nessus Essentials (for vulnerability scanning)  
- Kali Linux (attacker machine)  
- Nmap (for scanning and checking open ports)  
- VirtualBox (for creating lab environment)  
- Metasploitable 2 (target machine)  

---

##  Lab Setup

I created a virtual lab using VirtualBox.

- Host Machine: Windows 11  
- Attacker Machine: Kali Linux  
- Target Machine: Metasploitable 2  
- Network Type: NAT Network  

Both machines were connected to the same network so they could communicate with each other. The environment was isolated, so no real systems were affected.

---

##  Methodology

### 1. Reconnaissance
First, I identified the IP address of the target machine and checked connectivity.

### 2. Scanning
Then I ran a Nessus Basic Network Scan on the target IP. The scan took around 14 minutes.
### Screenshots


### 3. Analysis
After the scan, I analyzed the vulnerabilities based on severity and CVSS score.

### 4. Reporting
Finally, I documented all the findings along with their impact and possible solutions.

---

##  Key Findings

The scan found a total of 68 vulnerabilities.

### Critical Issues:
- End-of-Life Operating System (Ubuntu 8.04)  
- VNC using default password  
- Bind shell backdoor on port 1524  
- Ghostcat vulnerability (CVE-2020-1938)  
- SSL vulnerabilities (SSLv2/SSLv3 enabled)  

### High Severity:
- rlogin service (insecure communication)  
- Samba vulnerability (Badlock)  
- NFS shares accessible without authentication  

These vulnerabilities can allow attackers to gain access to the system, steal data, or even get full control.

---

##  Possible Attacks

Based on the vulnerabilities, the following attacks are possible:

- Getting root access using bind shell  
- Accessing system using VNC with weak password  
- Reading sensitive files using Ghostcat exploit  
- Performing MITM attacks using weak SSL  
- Accessing shared files via NFS  

---

##  Remediation

Some of the solutions for these issues are:

- Upgrade the operating system  
- Change default passwords  
- Disable unused services  
- Use secure protocols like SSH instead of rlogin  
- Disable SSLv2 and SSLv3  
- Apply regular security updates  

---

##  Report

The detailed VAPT report is included in this repository.

---

##  What I Learned

- How vulnerability scanning works  
- How to use Nessus for real-world scenarios  
- Importance of patching and updates  
- How small misconfigurations can lead to serious issues  
- Basics of penetration testing workflow  

---

##  Disclaimer

This project was done in a controlled lab environment using intentionally vulnerable machines.  
It is only for educational purposes.

---

##  Author

Pavan N 
CEH Candidate | Learning Cybersecurity
