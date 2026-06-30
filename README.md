# Splunk SIEM Fundamentals & Security Monitoring

## 🎯 Objective:
To develop foundational Splunk SIEM skills by deploying a Splunk environment, onboarding multiple security log sources, performing SPL-based investigations, creating dashboards and alerts, and implementing security monitoring use cases commonly performed by SOC analysts.

## 📊 Project Overview:
This project focused on building a fully functional Splunk lab environment to understand core SIEM operations. Activities included installing and configuring Splunk, onboarding multiple log sources, forwarding Windows event logs, performing SPL-based investigations, creating dashboards and alerts, enriching data with lookups, and developing security monitoring use cases. The project simulated real-world SOC analyst tasks and security investigations using Windows, Sysmon, Defender, PowerShell, Zeek, and Suricata logs.

## 🖥️ Lab Setup:
- Splunk Enterprise deployed on Ubuntu Linux
- Windows 10 Endpoint
- Splunk Universal Forwarder
- Custom Security Log Datasets
- Security Monitoring Index (mydfir-soc)
- Browser-based Splunk Search & Reporting Interface

### 🧰 Tools Used:
- Splunk Enterprise
- Splunk Universal Forwarder
- Search Processing Language (SPL)
- Ubuntu Linux
- Windows 10
- Sysmon
- Microsoft Defender Logs
- Windows Event Logs
- PowerShell Logs
- Zeek Logs
- Suricata Logs
- CSV Lookup Tables

### 🛡️ Skill Developed:
- Splunk SIEM Administration
- Log Collection & Data Onboarding
- Index Management
- Forwarder Configuration
- SPL Query Development
- Search Optimization
- Field Extraction (REX & EVAL)
- Data Parsing & Normalization
- Security Event Analysis
- Dashboard Development
- Alert Engineering
- Scheduled Reporting
- Lookup Table Enrichment
- Security Monitoring & Threat Hunting Fundamentals

### 📁 Key Deliverables:
- Splunk Enterprise Deployment
- Universal Forwarder Configuration
- Windows Security Log Collection
- Custom Log Onboarding
- SPL Search Library
- Search-Time Field Extractions
- Threat Hunting Queries
- Lookup Table Implementation
- Linux Activity Dashboard
- Brute Force Detection Alert
- Weekly Failed Login Report
- Splunk Add-on Deployment for Windows & Sysmon

## 🔍 Steps Performed:

#### Key Findings:

#### What I Learned:

#### What I Would Do Differently in a Production SOC:



## 🚨 Investigation Report:

#### Phishing Email Investigation:
A phishing email impersonating SharePoint was delivered to an executive mailbox despite multiple authentication failures and a phishing verdict.

#### Query Used:
```KQL
- MailGuard365_Threats_CL     
  | where ThreatVerdict contains "phish" and Direction == "Inbound"
  | where Action contains "Allow" and SPFResult == "Fail" and DKIMResult == "None" and DMARCResult == "Fail"
  | sort by ThreatConfidence
```
<img width="758" height="420" alt="image" src="https://github.com/user-attachments/assets/a788bad8-b715-4eff-b256-0f427dfbb744" />

#### Indicators Identified:
- IP: 185.220.101.55
- Domain: sh4repoint-pkwork[.]xyz
- Recipient: ceo@pkwork.onmicrosoft.com
- Subject: SharePoint: Board meeting documents shared with you
- Attachment: Q4-Board-Meeting-Agenda.docx
- Verdict: Phishing (Confidence: 93)
- Email Authentication: SPF Fail | DKIM None | DMARC Fail
- Delivery Status: Allowed

#### Investigation:
A phishing email was received on 2026‑06‑11 07:17:42 UTC from sharepoint-notify@h4repoint-pkwork[.]xyz, originating from the malicious IP 185.220.101.55 (100% abuse on AbuseIPDB). The message included a typosquatted URL (hxxp[://]sh4repoint-pkwork[.]xyz/download/board-agenda) and a Word attachment (Q4-Board-Meeting-Agenda.docx). Email authentication checks failed (SPF/DMARC failed, DKIM none), yet the email was still delivered despite a phishing threat score of 93. An investigation is ongoing to determine whether the link or attachment was accessed and to assess any potential data exposure.

<img width="501" height="428" alt="image" src="https://github.com/user-attachments/assets/b2b77daa-7009-497a-8ff9-1a268660d5fc" />
<img width="1239" height="647" alt="image" src="https://github.com/user-attachments/assets/92f4a39a-9506-452d-a243-0b2f7fe7a7b9" />

#### Triage (5W1H Analysis):
- WHO: Malicious sender IP 185.220.101.55 (100% abuse on AbuseIPDB).
- WHAT: Phishing email from sharepoint-notify@sh4repoint-pkwork[.]xyz containing a typosquatted URL and the attachment Q4‑Board‑Meeting‑Agenda.docx.
- WHEN: Sent on 2026‑06‑11 07:17:42 UTC and delivered despite failing email security checks.
- WHERE: Targeted ceo@pkwork.onmicrosoft.com with subject “SharePoint: Board meeting documents shared with you.”  
- WHY: Likely aimed at credential theft or delivering malware to compromise the CEO’s system.
- HOW: Email passed through because the security gateway was likely not configured to block or quarantine such threats.

### 🛑 Response Actions:
- Quarantined and removed the phishing email from the environment.
- Initiated an organization-wide search for related sender IP/domain activity.
- Blocked the malicious IP (185.220.101.55) and the typosquatted domain at email gateway level.
- Elevated the incident in Microsoft Sentinel for further SOC tracking and correlation.
- Validated the email security posture and reviewed filtering policy gaps for remediation.

### 💡 Recommendations:
- Enforce strict anti-spoofing controls - SPF, DKIM, DMARC enforcement set to reject wherever necessary.
- Implement automatic quarantine for high-confidence phishing verdicts.
- Enable domain impersonation and lookalike detection policies in Microsoft Defender for Office 365.
- Integrate real-time threat intelligence feeds for automated enrichment and blocking.
- Conduct targeted executive phishing simulations and awareness training.
- Establish automated Sentinel playbooks for phishing triage and response.

### 🧠 Lessons Learned:
- Email authentication failures do not guarantee blocking if policies are misconfigured.
- Threat intelligence validation is critical for confirming malicious infrastructure.
- Sentinel workbooks significantly improve visibility and SOC decision-making speed.
- KQL-driven threat hunting is essential for uncovering hidden or correlated threats.
- Phishing investigations require cross-correlation between email, identity, and endpoint telemetry.
- Effective SOC operations depend on automation, enrichment, and consistent alert tuning.

