# Red Team Cyber Security — Assignment 1: Foundations, Reconnaissance & Reporting

**Intern:** Azeez Umar Opeyemi (`ITCSR-B02-1269`)  
**Organization:** ITSimplera Solutions — Second Internship Batch (Batch 02 — 2026)  
**Domain:** Cyber Security (Red Teaming)  

---

## Overview
This repository contains my submission and supporting lab evidence for **Assignment 1 (Foundations, Reconnaissance and Reporting)** under the ITSimplera Solutions Red Team Cyber Security Internship.

All active scanning and service enumeration tasks were executed strictly inside an isolated VMware Workstation lab network (`192.168.145.0/24`) between an authorized Kali Linux attacker VM (`192.168.145.128`) and an intentionally vulnerable Metasploitable 2 target (`192.168.145.132`).

---

## Key Components Covered
* **Section A — Red Team Theory & Governance:**
  * Operational distinctions between Red, Blue, and Purple Teams, plus Vulnerability Assessments vs. Penetration Tests vs. Red Team Engagements.
  * Attack lifecycle modeling using the **Lockheed Martin Cyber Kill Chain** and **MITRE ATT&CK** (`T1595`, `T1566.001`, `T1071.001`).
  * Rules of Engagement (ROE), authorization boundaries, and cybercrime legal compliance (Nigeria's Cybercrimes Act 2015 / 2024 Amendment & Pakistan's PECA 2016).
* **Section B — Lab Reconnaissance, Enumeration & Reporting:**
  * **Passive OSINT (`example.com`):** Domain registration, DNS records, and ASN/IP footprinting using `whois`, `nslookup`, `dig`, and `theHarvester` (`urlscan`).
  * **Active Reconnaissance (`192.168.145.132`):** Host discovery (`nmap -sn`), service/version detection (`nmap -sV`), and default NSE scripting (`nmap -sC`).
  * **Service Enumeration:** Web vulnerability scanning with `nikto` (port `80/tcp`) and SMB/NetBIOS null-session & RID cycling enumeration with `enum4linux` (ports `139/445/tcp`).
  * **Vulnerability Analysis & Mini Pentest Report:** Severity-rated findings (`vsftpd 2.3.4` backdoor `CVE-2011-2523`, `Samba 3.0.20` RCE `CVE-2007-2447`, and port `1524` root bindshell) mapped to MITRE ATT&CK and Blue Team detection controls.
* **Section C — Real-World Case Study:**
  * Adversary kill chain analysis, ATT&CK mapping, and defensive lessons from the **2020 SolarWinds Orion (SUNBURST)** supply chain compromise.

---

## Repository Structure
```text
├── RedTeam_Assignment1_AzeezUmarOpeyemi.pdf   # Full formatted assignment & mini pentest report
├── evidence/                                 # Timestamped lab terminal & network screenshots
└── README.md                                 # Project summary and documentation

