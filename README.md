# Vulnerablity-Assement-Using-Nessus-and-metasploit-And-Metasploitable

# Vulnerability Assessment Report

## Candidate: Sai Deepak  
**Position Applied**: Cybersecurity Intern / Analyst  
**Assessment Focus**: Network Vulnerability Identification and Risk Mitigation

---

## 🔍 Target Overview
- **IP Address Assessed**: 192.168.240.129  
- **Tools Used**:  
  - **Nmap** – For service discovery, OS fingerprinting, and open port scanning.  
  - **Nessus** – For detecting known vulnerabilities, CVEs, and configuration issues.

---

## 🎯 Objective
The primary objective of this assessment was to identify vulnerabilities in a target host through service enumeration and vulnerability scanning. This process simulates an ethical approach to understanding risks and improving security posture.

---

## ⚙️ Tools and Methodology

### 🔧 Nmap Command Executed:
```bash
nmap -sV -O -Pn 192.168.240.129
```
- `-sV`: Service and version detection  
- `-O`: OS detection  
- `-Pn`: Skip host discovery (assume target is online)

### 🔎 Nessus Scan:
Nessus was used to perform vulnerability analysis after identifying open services. This scan focused on discovering high-severity and critical vulnerabilities present in the system.

---

## 📋 Key Findings

### 1. UnrealIRCd Backdoor (Critical)
- **CVSS**: 10.0
- **Impact**: Remote code execution due to backdoored version.
- **Resolution**: Upgrade to a clean release from a verified source.

### 2. Samba Badlock Vulnerability (High)
- **CVSS**: 7.5
- **Impact**: Possible man-in-the-middle attacks and privilege escalation.
- **Resolution**: Patch the system and update Samba to a secure version.

### 3. SMB Misconfigurations (High-Medium)
- **Impact**: Risk of lateral movement and unauthorized access.
- **Resolution**: Apply latest patches, disable older SMB versions, and limit access.

---

## 🛠️ Remediation Summary

| Vulnerability         | Suggested Action                                           |
|------------------------|------------------------------------------------------------|
| UnrealIRCd Backdoor    | Replace with secure version from verified distribution     |
| Samba Badlock          | Apply patches, upgrade Samba                              |
| SMB Vulnerabilities    | Reconfigure service, restrict access, keep it updated      |

---

## 📌 Notes
- This assessment was conducted in a safe lab environment using a controlled virtual machine.
- The findings demonstrate understanding of real-world vulnerabilities and how to mitigate them responsibly.
- The tools and steps used reflect hands-on skills that can translate to live environments.

---

## 🧑‍💻 About Me
I’m a cybersecurity student with practical experience in vulnerability assessment, networking, and security tools. I am passionate about identifying threats and securing systems in both enterprise and research environments.

