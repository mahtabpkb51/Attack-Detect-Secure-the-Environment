# MAJOR PROJECT – Attack, Detect & Secure the Environment

---

## 1. Overview

In this major project, students will act as both **Red Team (Attackers)** and **Blue Team (Defenders)**.

Students will:

- Attack the infrastructure deployed in the Minor Project  
- Generate real-world security events  
- Analyze logs using SIEM  
- Identify misconfigurations  
- Apply full system hardening  
- Validate that logs after hardening are significantly different  

**Minor Project Reference:** Minor Project 2

---

## 2. Objective

To simulate cyber-attacks on a cloud-based enterprise environment, detect malicious activity using SIEM logs, identify root causes, fix vulnerabilities, and harden the system following industry security standards.

---

## 3. Tasks to be Completed

---

### Phase 1 – Red Team Attack Simulation

**Team Size:** 3 Students  
**Roles:**

- Attacker  
- Defender  
- Documenter  

#### Attack Scenarios

- SSH Brute Force Attack on VM1 & VM2  
- Privilege Escalation Attempts  
- Web Attacks on Apache/Nginx (VM2):
  - Directory Traversal  
  - SQL Injection (on simple forms)  
  - File Enumeration  
- Enumeration of FreeIPA  
- Scanning for Open Ports / Services  

#### Tools Allowed

- Nmap  
- Hydra  
- Nikto  
- Gobuster  
- Default Linux tools  

#### Goal

Generate logs that clearly show attack activities in the SIEM.

---

### Phase 2 – Blue Team (Investigation + Hardening)

---

#### 1. Analyze SIEM Logs

Students must:

- Identify attacker IP addresses  
- Review:
  - Syslog  
  - auth.log  
  - audit.log  
- Examine Wazuh alerts  
- Document Indicators of Compromise (IOC)

---

#### 2. Find Misconfigurations

Examples include:

- Open ports  
- Weak SSH configuration  
- Weak passwords  
- World-readable directories  
- Missing firewall rules  
- No password policies  

---

#### 3. Apply Security Hardening

> **Note:** This section is moved from the Minor Project and now belongs to the Major Project.

##### System Logging Enhancements

- Install Sysmon for Linux  
- Configure custom Auditd rules  
- Enable verbose Apache/Nginx logging  

##### Network & Access Controls

- Configure UFW / Iptables  
- Harden SSH:
  - Key-based authentication  
  - Disable root login  
  - Change SSH port  
  - Enable rate limiting  

##### Firewall & NSG Hardening

- Restrict DMZ → Internal traffic  
- Allow SSH only from SIEM VM  

##### Server Hardening

- Disable unnecessary services  
- Enforce strong password policies  
- Apply least privilege permissions  
- Secure FreeIPA  
- Harden Apache/Nginx  

---

#### 4. Re-Attack After Hardening

Students must repeat the same attacks and demonstrate:

- Reduced attack surface  
- Different SIEM logs  
- Improved detection and alerting  

---

## 4. Deliverables

### 1. Attack Report

- Attack steps  
- Tools used  
- Screenshots  
- Logs generated:
  - Screenshots of logs **before hardening**
  - Screenshots of logs **after hardening**
- SIEM alerts  

### 2. Investigation Report

- Findings  
- IOC documentation  
- Attack patterns  

### 3. Hardening Report

- Security measures implemented  
- Reason for implementation  
- Before/after log comparison  

### 4. Final Security Posture Report

- Complete security overview  
- Screenshots with **Student Name visible in Azure**

---

## 5. Expected Learning Outcomes

Students will gain:

- Hands-on Red Team attack experience  
- SOC-level SIEM log analysis skills  
- Linux system hardening knowledge  
- Incident response capabilities  
- Understanding of before/after security states  
- Ability to design and implement a complete defensive security architecture  

---
