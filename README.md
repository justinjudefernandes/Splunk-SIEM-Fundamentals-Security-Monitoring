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

#### 📌 Screenshots as below: (from left to right)

<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/a4669d4f-d615-49f7-a980-16fb698c0ea8" />
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/f87d5eac-6d8e-4209-b7a9-9671f0d3a85e" />
<img width="500" height="200" alt="image" src="https://github.com/user-attachments/assets/64ebb021-a3a6-4d89-89eb-844231e98f42" />
<img width="500" height="200" alt="image" src="https://github.com/user-attachments/assets/6c43ae0d-39d7-4313-9817-f0091f956d38" />
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/d8cdff30-75c5-4dd9-b957-065f53ca33e3" />
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/fc88bedb-0837-41be-bf00-7346c99b292d" />
<img width="500" height="150" alt="image" src="https://github.com/user-attachments/assets/f85aa0c1-c22a-4307-92fd-a7935fdce507" />
<img width="500" height="150" alt="image" src="https://github.com/user-attachments/assets/b0cefceb-de5d-4a13-8866-1a45da0a82d9" />
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/5f33fb08-93c3-4433-831f-44482c78378a" />
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/134e2dc2-37fd-4602-a09f-24d3f0ba32e3" />

### 2. Index Creation
- Learned Splunk indexing concepts.
- Created a dedicated security monitoring index named mydfir-soc.

#### 📌 Screenshots as below:

<img width="975" height="375" alt="image" src="https://github.com/user-attachments/assets/a0133714-40bb-4c22-a870-b584552fed42" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/cad7b9e9-e10b-4d67-9b70-eb61fa835e41" />
<img width="975" height="312" alt="image" src="https://github.com/user-attachments/assets/2af70c31-fcdc-466f-a737-64ad5b1d5ded" />



### 3. Data Onboarding & Forwarder Configuration
- Installed Splunk Universal Forwarder on Windows.
- Configured receiving port 9997.
- Modified inputs.conf to collect Windows Security and Application logs.
- Forwarded logs to the Splunk indexer and validated ingestion.

#### 📌 Screenshots as below: (from left to right)

<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/97ee05da-b038-4a77-a335-5a05d1de97a0" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/a9ac7a6c-204f-4f9c-860f-fd173e8beddb" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/a6ef9a52-b1ff-4b89-a979-b6427720947b" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/4cdec103-7bd5-485c-8910-12191b79acde" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/9e430eee-f05a-4a24-98d5-d693857e1d88" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/3679759f-af1a-48f8-8fb9-7486a4e3a1f5" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/d940ac1c-489a-430c-b050-8d4ab0983fe5" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/eac26bf4-1c41-4b70-aa0a-57c47f504182" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/d627204c-7c01-4e8e-bc0c-6136958a93e9" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/42edd5fb-a56f-420a-ae55-8b4025418de1" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/233618ef-708a-414e-9d5e-babf7dd7456c" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/ec1a2581-73df-4c3c-b907-d323aebf260c" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/a663125a-46aa-4414-aac7-dd9be4eebd75" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/2e68db1a-deef-4ae0-889e-008f544d3302" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/d53c58e1-4971-4661-8078-5d3685d6f119" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/8c759f53-580a-42d7-b3a5-2a9e52e24265" />

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


