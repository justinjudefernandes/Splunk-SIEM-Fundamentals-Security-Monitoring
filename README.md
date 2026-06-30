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

<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/a4669d4f-d615-49f7-a980-16fb698c0ea8" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/f87d5eac-6d8e-4209-b7a9-9671f0d3a85e" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/64ebb021-a3a6-4d89-89eb-844231e98f42" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/b0900db8-812b-4be8-97a2-2a5a3c233509" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/76ccdd89-61c9-489d-894d-6419dd4027ba" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/6c43ae0d-39d7-4313-9817-f0091f956d38" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/d8cdff30-75c5-4dd9-b957-065f53ca33e3" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/fc88bedb-0837-41be-bf00-7346c99b292d" />
<img width="330" height="150" alt="image" src="https://github.com/user-attachments/assets/f85aa0c1-c22a-4307-92fd-a7935fdce507" />
<img width="330" height="150" alt="image" src="https://github.com/user-attachments/assets/b0cefceb-de5d-4a13-8866-1a45da0a82d9" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/5f33fb08-93c3-4433-831f-44482c78378a" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/134e2dc2-37fd-4602-a09f-24d3f0ba32e3" />

### 2. Index Creation
- Learned Splunk indexing concepts.
- Created a dedicated security monitoring index named mydfir-soc.

#### 📌 Screenshots as below: (from left to right)

<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/a0133714-40bb-4c22-a870-b584552fed42" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/cad7b9e9-e10b-4d67-9b70-eb61fa835e41" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/2af70c31-fcdc-466f-a737-64ad5b1d5ded" />



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

#### 📌 Screenshots as below: (from left to right)

<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/3b076fd3-e751-4b5a-a1e4-214d48f84657" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/bc6c2de0-a04b-4a93-96ae-c00c30d896d8" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/4e6814a1-69f7-4c56-b0a2-45596820aa8e" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/681e69b6-99d4-49df-82bf-cb7afd7bb43d" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/0fe96931-e46d-424d-a44b-4f125c6c5e62" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/35d0c29a-4607-4af2-9dde-4a2c3c4cd2ec" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/9f6a6b93-044d-4e82-9fff-1898e167b1e4" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/93e15e54-03a3-4718-ab99-c14aafd411fd" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/a76e696c-069e-4cde-a6ee-eed7dcf78957" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/fce943c3-9dfe-4f86-b9ea-eee0b5441514" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/8e1aa8e4-068a-4b30-a016-04aa5ca62100" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/ecf478f5-452f-48f7-b7dc-dbf353fbfc14" />

### 5. Parsing & Field Extraction
- Learned index-time and search-time parsing.
- Performed field extraction using Regular Expressions (REX).
- Extracted user and source IP fields from authentication logs.
- Validated extracted fields across datasets.

#### 📌 Screenshots as below: (from left to right)

<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/d14217e8-1852-44f3-bd6f-be560cf46349" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/2041613c-37a6-49d8-b30b-5735ce68f724" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/e963a153-ee0f-41a8-9584-d9d622938b4b" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/c1ef93e2-08af-4767-be0d-8e8121d76464" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/908ddcd1-adb0-46bf-b9e1-38059e6abf9d" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/e93bcba6-b26c-4c2e-81de-df8189e1cb58" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/2309bb77-0c06-496e-b882-5d366dc15729" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/bff6d81b-aeb8-4208-ad54-c06707f9056f" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/083f109e-c1b5-4319-aa34-e9bd1c701c56" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/3ab96df9-11cc-41f4-8677-dde72d83a1c6" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/e7699e44-3136-4bd1-8fcc-59ae97842c5b" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/84f9c987-d1ed-4acf-b06a-242e1eb74dfe" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/66ec83d7-f5fa-4c45-bf82-eb5d6ae4e526" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/2033e6d2-744b-490e-9782-669da26e0524" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/85ac3c02-6cc6-46c4-b3f0-0b362c0ebcc4" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/8a2dfbd7-d821-463d-8509-2bd84827999b" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/851d8465-1296-46d8-a449-515f4a281440" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/04bf9727-a33e-4523-b92e-7d81b645ea23" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/a270c29c-e6ad-4271-a5a0-979d9d4cc915" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/90ce4495-976d-430c-bdfe-2d7e54e15af0" />



### 6. SPL Query Development
- Compared query performance using Job Inspector.
- Learned that field names are sensitive while field values are not.
- Reviewed the different search modes in Splunk:
  - fast - showcases only a few interesting fields.
  - smart - showcases a lot more interesting fields.
- The main difference between smart and verbose modes is that when using transformation commands:
  - smart - only displays statistics and visualizations, no events are displayed
  - verbose - only displays events, statistics and visualizations
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


