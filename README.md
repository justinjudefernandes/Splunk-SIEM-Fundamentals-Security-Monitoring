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
<img width="320" height="200" alt="image" src="https://github.com/user-attachments/assets/cad7b9e9-e10b-4d67-9b70-eb61fa835e41" />
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
  - Fast Mode – Displays a limited set of relevant fields to optimize search performance.
  - Smart Mode – Displays a broader set of relevant fields while balancing performance and detail.
  - Verbose Mode – Displays all available fields and event data, providing the most comprehensive search results.
- The primary difference between Smart and Verbose search modes becomes apparent when using transforming commands:
  - Smart Mode – Displays only the resulting statistics and visualizations; the underlying events are not shown.
  - Verbose Mode – Displays the raw events alongside the resulting statistics and visualizations, providing complete visibility into the search results.
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
- Used these transforming commands to generate statistics and trends.
- Performed event aggregation and time-based analysis.
- Created summaries using stats and timechart commands.

#### 📌 Screenshots as below: (from left to right)

<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/ed514acc-5b73-4e85-ab12-ad993f69758b" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/81bcdfb7-edcb-4923-8003-78744771ae20" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/18e12f22-0dc1-405f-bc00-f9afd84b81d0" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/a41eea78-0b44-4eee-8e0e-961e36c95707" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/e0884463-fb1b-495c-b3fb-0b6b30cb1fc0" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/91fd3b26-3594-4666-ad0e-1552006ee277" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/3708e8c0-fb20-4659-8a1c-408839ac8b3b" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/7df707c2-c51c-4782-b034-05374ff62d1a" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/b3b8478b-b6b1-4416-8136-8eb6a40756d0" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/66677559-8fb7-4dc7-99f2-17db8ff61638" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/bb134b2f-5e6f-4798-aec9-72df8fa31f54" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/1e3623a6-2e5f-49bb-ae43-ae79888469d1" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/aedf24ef-ff19-4998-8982-71ac8a9af4d2" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/e2c43f2e-c5da-4b10-b374-69fee0edb044" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/15c42749-bfd4-4929-966e-6f52d32a87c9" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/ef1509b3-c711-4fe3-992a-47f18c686810" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/152c4f67-744b-484c-8239-c2e073ff1850" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/06d49387-7146-48d3-be76-244822bda68d" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/729ba00f-d042-42f1-8432-221f55c3204e" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/de7dfcc4-036e-4f16-adde-75c1c05cf578" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/ea761b98-0b41-4757-835c-f47bd7b7f3dd" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/b6d97cd0-16e8-408e-82ba-913338eda74d" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/e86ec3bd-88d9-4572-88ae-9fe738bb9cf2" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/bdac85c4-fd73-477c-ae58-95fe8057064d" />

### 7. Lookup Table Enrichment
- Created a VIP user lookup table.
- Uploaded and integrated lookup data into searches.
- Enriched security events with user role information.

#### 📌 Screenshots as below: (from left to right)

<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/e96b1010-112e-46f8-8337-d5afe82942db" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/97a42a5d-7816-40d1-86fd-0e7d99df2bce" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/39ba6d5a-a6cb-403e-8401-82af2890cd36" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/4d4466f0-ef5c-4cee-9f7a-b39be65d95d2" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/c9b5a3ad-3218-442b-aa81-0dd36216396d" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/b86894fc-da90-4577-9f3b-431d7d784a87" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/442ed2aa-6df5-4903-b2b1-b9854508d7d8" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/319ebb3f-603c-4a92-b6fe-721f422ec195" />

### 8. Security Dashboard Creation
- Designed a Linux Activity dashboard.
- Implemented panels for:
  - Top User Failed Logins
  - Failed Logins by Hour
  - Successful Logins
- Visualized authentication activity for security monitoring.

#### 📌 Screenshots as below: (from left to right)

<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/aed58d44-a182-43cc-947e-68d835521029" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/1d4153a3-7ade-4869-bb2f-41c5253b65fe" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/cd7a88da-f421-4077-a464-67460c400421" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/b5b27740-96c5-492a-995b-bec74e3df74b" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/bedafa77-288d-4cc2-b5b1-13947041ed49" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/152b650c-00f8-4a26-97b3-02099dfa50db" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/d7e0d572-abc7-4b22-adc3-b3be9ca564f1" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/a6631258-4780-4644-8968-947ff8189059" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/8cbad0f0-e80d-4f41-8076-8366824763f8" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/259dfe93-ab56-41e0-812d-b71cf5120748" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/3d01b262-b2a0-48c6-bf16-786da2cfcfe4" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/9a79b05e-284b-458e-8e54-ca87f7bca535" />

### 9. Created Actionable Alerts 
- Developed a Brute Force Detection alert.
- Configured scheduled execution every minute.
- Tested alert triggering and validated alert management workflows.

#### 📌 Screenshots as below: (from left to right)

<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/4f27102f-60e1-4ff5-89a7-c9fb4bd50855" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/65cdd571-4f45-4d80-ab8b-a7f05c15854b" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/651df90a-4eb2-4823-a175-6ca6d6a7aeb9" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/5c91bac1-13f8-413f-b6a8-ce01fca7df39" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/5edc1214-fbeb-4e8c-afe0-fafb76fd5916" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/b9f0434a-a5f8-4b65-a658-2d0e5fb51e62" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/b389d0a4-8e30-4af7-a968-80486fcb9632" />
<img width="240" height="200" alt="image" src="https://github.com/user-attachments/assets/fc3c925b-4e5c-4c44-837b-40b6e2437baf" />

### 10. Scheduled Reporting
- Created a Weekly Failed Logins report.
- Scheduled automated report generation for SOC review.

#### 📌 Screenshots as below: (from left to right)

<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/75cf472b-89de-4b77-b7ce-63c81937371b" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/48a63b9d-060b-46da-b967-507b37bf5334" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/a0334c8a-fd55-44ba-945a-c773a31b9b32" />
<img width="500" height="200" alt="image" src="https://github.com/user-attachments/assets/84d6d5f6-17c6-4ba6-8af5-2c1ae2bf5ec3" />
<img width="500" height="200" alt="image" src="https://github.com/user-attachments/assets/d7bc453c-af5d-4a23-ac42-daef02eeb50d" />

### 11. Splunk App Integration
- Installed and validated:
  - Splunk Add-on for Microsoft Windows
  - Splunk Add-on for Sysmon
- Enhanced field extraction and log normalization capabilities.

#### 📌 Screenshots as below: (from left to right)

<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/1693e716-4c8d-4117-8140-5465a275e13a" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/12149b2b-bf45-4f20-8e34-c8724a655f8d" />
<img width="330" height="200" alt="image" src="https://github.com/user-attachments/assets/8128bbe3-be92-4a6d-a558-2e46bcbf6b5a" />
<img width="500" height="200" alt="image" src="https://github.com/user-attachments/assets/50f9b68b-d9d1-4c53-a8c7-fb3d4529a059" />
<img width="500" height="200" alt="image" src="https://github.com/user-attachments/assets/686af70e-4790-4fb2-9679-0825313d3375" />
<img width="500" height="200" alt="image" src="https://github.com/user-attachments/assets/c55cb884-6f89-4a9a-9293-0f601d32fe0d" />
<img width="500" height="200" alt="image" src="https://github.com/user-attachments/assets/c3d1a70f-c262-424a-a738-338c3f0cce1a" />






