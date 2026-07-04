
## About This Repository

This repo is my personal study log and portfolio piece from working through LetsDefend's SOC Analyst curriculum. It's organized into two parts:

- **`MD Files/`** — Concept write-ups covering core SOC theory (SIEM, malware analysis, threat intel, phishing, etc.)
- **`Labs/`** — Real incident walkthroughs: alert triage, investigation, evidence gathering, and closing the case, based on simulated SOC alerts.

Each write-up follows the mindset of an actual analyst on shift: receive the alert → investigate logs/endpoints/files → determine true/false positive → escalate or close → document findings.

---

## Folder Structure

```
SOC/
├── Assets/           # Screenshots and visual aids used across write-ups
├── MD Files/         # Concept notes, one per lecture/topic
├── Labs/             # Individual incident walkthroughs (numbered by event ID)
├── LICENSE           # MIT License
└── README.md         # You are here
```

---

## MD Files — Core Concepts

| # | Topic |
|---|-------|
| 1 | [SOC Fundamentals](<./MD Files/1 - SOC Fundamentals.md>) |
| 2 | [Cyber Kill Chain](<./MD Files/2 - Cyber Kill Chain.md>) |
| 3 | [MITRE ATT&CK Framework](<./MD Files/3 - MITRE ATT&CK Framework.md>) |
| 4 | [Introduction to Phishing](<./MD Files/4 - Introduction to Phishing.md>) |
| 5 | [Detecting Web Attacks](<./MD Files/5 - Detecting Web Attacks.md>) |
| 6 | [Detecting Web Attacks - 2](<./MD Files/6 - Detecting Web Attacks - 2.md>) |
| 7 | [How to Investigate a SIEM Alert](<./MD Files/7 - How to Investigate a SIEM Alert.md>) |
| 8 | [Malware Analysis Fundamentals](<./MD Files/8 - Malware Analysis Fundamentals.md>) |
| 9 | [Dynamic Malware Analysis](<./MD Files/9 - Dynamic Malware Analysis.md>) |
| 10 | [Malicious Document Analysis](<./MD Files/10 - Malicious Document Analysis.md>) |
| 11 | [Security Solutions](<./MD Files/11 - Security Solutions.md>) |
| 12 | [Network Log Analysis](<./MD Files/12 - Network Log Analysis.md>) |
| 13 | [SIEM 101](<./MD Files/13 - SIEM 101.md>) |
| 14 | [Incident Management 101](<./MD Files/14 - Incident Management 101.md>) |
| 15 | [Splunk](<./MD Files/15 - Splunk.md>) |
| 16 | [Cyber Threat Intelligence](<./MD Files/16 - Cyber Threat Intelligence.md>) |
| 17 | [VirusTotal for SOC Analysts](<./MD Files/17 - VirusTotal for SOC Analysts.md>) |
| 18 | [IT Security Basis for Corporates](<./MD Files/18 - IT Security Basis for Corporates.md>) |
| 19 | [Detecting Brute Force Attacks](<./MD Files/19 - Detecting Brute Force Attacks.md>) |
| 20 | [Building a Malware Analysis Lab](<./MD Files/20 - Building a Malware Analysis Lab.md>) |

---

## Labs - Incident Walkthroughs

Each lab documents a real alert investigated inside the LetsDefend platform, following the full analyst workflow (alert review → log/endpoint analysis → verdict → containment/closure).

| # | Lab | Alert Rule | Category |
|---|-----|-----------|----------|
| 1 | [SOC282 - Phishing Alert](<./Labs/SOC282 - Phishing Alert.md>) | SOC282 | Phishing |
| 2 | [28 - SOC105 - Requested T.I. URL Address](<./Labs/28 - SOC105 - Requested T.I. URL address.md>) | SOC105 | Threat Intel / URL |
| 3 | [36 - SOC104 - Malware Detected](<./Labs/36 - SOC104 - Malware Detected.md>) | SOC104 | Malware |
| 4 | [83 - SOC119 - Proxy - Malicious Executable File Detected](<./Labs/83 - SOC119 - Proxy - Malicious Executable File Detected.md>) | SOC119 | Proxy / Web |
| 5 | [85 - SOC109 - Emotet Malware Detected](<./Labs/85 - SOC109 - Emotet Malware Detected.md>) | SOC109 | Malware (Emotet) |
| 6 | [84 - SOC104 - Malware Detected](<./Labs/84 - SOC104 - Malware Detected.md>) | SOC104 | Malware |
| 7 | [92 - SOC145 - Ransomware Detected](<./Labs/LetsDefend SOC Walkthrough - 92 - SOC145 - Ransomware Detected.md>) | SOC145 | Ransomware |
| 8 | [20 - SOC105 - Requested T.I. URL Address](<./Labs/20 - SOC105 - Requested T.I. URL address.md>) | SOC105 | Threat Intel / URL |
| 9 | [14 - SOC104 - Malware Detected](<./Labs/14 - SOC104 - Malware Detected.md>) | SOC104 | Malware |
| 10 | [75 - SOC105 - Requested T.I. URL Address](<./Labs/75 - SOC105 - Requested T.I. URL address.md>) | SOC105 | Threat Intel / URL |
| 11 | [76 - SOC137 - Malicious File Script Download Attempt](<./Labs/76 - SOC137 - Malicious File Script Download Attempt.md>) | SOC137 | Malicious Download |
| 12 | [320 - SOC342 - CVE-2025-53770 SharePoint ToolShell Auth Bypass & RCE](<./Labs/320 - SOC342 - CVE-2025-53770 SharePoint ToolShell Auth Bypass and RCE.md>) | SOC342 | Exploit / CVE |


---

## Investigation Methodology

Every lab write-up follows a consistent analyst workflow so the process is easy to follow and repeat:

1. **Alert Triage** - Review the alert details (source/destination, rule triggered, severity).
2. **Evidence Collection** - Pull relevant logs, endpoint data, file hashes, or network traffic.
3. **Analysis** - Check indicators against VirusTotal / threat intel sources, sandbox suspicious files, review process trees or proxy logs.
4. **Verdict** - Classify as True Positive or False Positive with supporting evidence.
5. **Response & Containment** - Recommend or apply containment (isolate host, block IOC, disable account, etc.).
6. **Documentation** - Record findings, timeline, and lessons learned for future reference.

---

## Tools & Concepts Covered

- **SIEM** platforms & alert investigation
- **EDR** tools (SentinelOne, CrowdStrike, Carbon Black, Palo Alto, FireEye HX)
- **VirusTotal** for hash/URL/file reputation checks
- **Sandboxing** for dynamic malware analysis
- **MITRE ATT&CK** framework mapping
- **Cyber Kill Chain** analysis
- Phishing & malicious document analysis
- Network/proxy log analysis
- Splunk querying basics
- Cyber Threat Intelligence (CTI) fundamentals
- Incident classification & escalation procedures

---
