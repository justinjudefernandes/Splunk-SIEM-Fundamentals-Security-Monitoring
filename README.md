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

<img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/4dfcb9c3-d32a-43e5-91c8-0fadf14ca520" />
<img width="975" height="580" alt="image" src="https://github.com/user-attachments/assets/f87d5eac-6d8e-4209-b7a9-9671f0d3a85e" />
<img width="975" height="170" alt="image" src="https://github.com/user-attachments/assets/64ebb021-a3a6-4d89-89eb-844231e98f42" />
<img width="975" height="571" alt="image" src="https://github.com/user-attachments/assets/57f7cb2a-95f6-4f89-b09a-185526935de4" />
<img width="975" height="636" alt="image" src="https://github.com/user-attachments/assets/cdbbeee7-938c-45b0-992d-7feaa76b1712" />
<img width="975" height="459" alt="image" src="https://github.com/user-attachments/assets/6c43ae0d-39d7-4313-9817-f0091f956d38" />
<img width="975" height="766" alt="image" src="https://github.com/user-attachments/assets/d8cdff30-75c5-4dd9-b957-065f53ca33e3" />
<img width="975" height="569" alt="image" src="https://github.com/user-attachments/assets/fc88bedb-0837-41be-bf00-7346c99b292d" />
<img width="975" height="102" alt="image" src="https://github.com/user-attachments/assets/f85aa0c1-c22a-4307-92fd-a7935fdce507" />
<img width="975" height="497" alt="image" src="https://github.com/user-attachments/assets/b0cefceb-de5d-4a13-8866-1a45da0a82d9" />
<img width="975" height="447" alt="image" src="https://github.com/user-attachments/assets/5f33fb08-93c3-4433-831f-44482c78378a" />
<img width="975" height="782" alt="image" src="https://github.com/user-attachments/assets/134e2dc2-37fd-4602-a09f-24d3f0ba32e3" />




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


