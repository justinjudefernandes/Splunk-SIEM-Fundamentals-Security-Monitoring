# Splunk SIEM Fundamentals & Security Monitoring

## 🎯 Objective:
To develop foundational Splunk SIEM skills by deploying a Splunk environment, onboarding multiple security log sources, performing SPL-based investigations, creating dashboards and alerts, and implementing security monitoring use cases commonly performed by SOC analysts.

## 📊 Project Overview:
This project focused on building a fully functional Splunk lab environment to understand core SIEM operations. Activities included installing and configuring Splunk, onboarding multiple log sources, forwarding Windows event logs, performing SPL-based investigations, creating dashboards and alerts, enriching data with lookups, and developing security monitoring use cases. The project simulated real-world SOC analyst tasks and security investigations using Windows, Sysmon, Defender, PowerShell, Zeek, and Suricata logs.

## 🖥️ Lab Setup:
<img width="400" height="600" alt="Splunk Lab Setup" src="https://github.com/user-attachments/assets/1599b9c1-e506-4d92-9613-ff3fb76eab19" />

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
### 1. Splunk Deployment & Configuration
- Installed Splunk Enterprise on Ubuntu.
- Configured Splunk services and web interface.
- Enabled automatic startup and validated functionality.
- Configured UTC time settings.

📌 Screenshots as below:

<img width="600" height="200" alt="image" src="https://github.com/user-attachments/assets/4dfcb9c3-d32a-43e5-91c8-0fadf14ca520" />


### 2. Index Creation
- Learned Splunk indexing concepts.
- Created a dedicated security monitoring index named mydfir-soc.

### 3. Data Onboarding & Forwarder Configuration
- Installed Splunk Universal Forwarder on Windows.
- Configured receiving port 9997.
- Modified inputs.conf to collect Windows Security and Application logs.
- Forwarded logs to the Splunk indexer and validated ingestion.

### 4. Custom Log Ingestion
- Uploaded and onboarded custom datasets including:
  - Application Logs
  - Security Logs
  - Sysmon Logs
  - PowerShell Logs
  - Microsoft Defender Logs
  - Zeek Logs
  - Suricata Logs
  - System Logs
- Configured sourcetypes, timestamps, hosts, and indexes.

### 5. Parsing & Field Extraction
- Learned index-time and search-time parsing.
- Performed field extraction using Regular Expressions (REX).
- Extracted user and source IP fields from authentication logs.
- Validated extracted fields across datasets.

### 6. SPL Query Development
- Applied Splunk search best practices.
- Developed optimized SPL queries using:
  - fields
  - table
  - where
  - sort
  - dedup
  - stats
  - timechart
  - eval
  - fillnull
  - coalesce
- Compared query performance using Job Inspector.

### 7. Data Analysis & Transformations
- Used transforming commands to generate statistics and trends.
- Performed event aggregation and time-based analysis.
- Created summaries using stats and timechart commands.

### 8. Lookup Table Enrichment
- Created a VIP user lookup table.
- Uploaded and integrated lookup data into searches.
- Enriched security events with user role information.

### 9. Security Dashboard Creation
- Designed a Linux Activity dashboard.
- Implemented panels for:
  - Top User Failed Logins
  - Failed Logins by Hour
  - Successful Logins
- Visualized authentication activity for security monitoring.

### 10. Alert Engineering
- Developed a Brute Force Detection alert.
- Configured scheduled execution every minute.
- Tested alert triggering and validated alert management workflows.

### 11. Scheduled Reporting
- Created a Weekly Failed Logins report.
- Scheduled automated report generation for SOC review.

### 12. Splunk App Integration
- Installed and validated:
  - Splunk Add-on for Microsoft Windows
  - Splunk Add-on for Sysmon
- Enhanced field extraction and log normalization capabilities.



## 🚨 Investigation Report:


