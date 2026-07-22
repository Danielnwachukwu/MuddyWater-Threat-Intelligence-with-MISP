# 🛡️ MuddyWater Threat Intelligence Investigation with MISP

![Threat Intelligence](https://img.shields.io/badge/Threat%20Intelligence-MISP-blue)
![Docker](https://img.shields.io/badge/Docker-Deployed-2496ED?logo=docker&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-SOC%20Analyst-success)
![License](https://img.shields.io/badge/License-MIT-green)

---

## Threat Intelligence Investigation using MISP to Profile the MuddyWater Advanced Persistent Threat (APT)

This project demonstrates how the **Malware Information Sharing Platform (MISP)** can be deployed using Docker to investigate a real-world Advanced Persistent Threat (APT). The investigation focuses on the **MuddyWater** threat group, leveraging community threat intelligence feeds to identify Indicators of Compromise (IOCs), correlate threat actor infrastructure, analyze adversary behavior, and map observed techniques to the **MITRE ATT&CK Framework**.

The project was conducted as a practical Threat Intelligence investigation for **SecureOps Cybersecurity Inc.**, simulating how a Security Operations Center (SOC) or Threat Intelligence Team would collect, enrich, and analyze intelligence to support proactive cyber defense.

---

## 📌 Business Challenge

SecureOps Cybersecurity Inc. supports organizations operating in government, finance, healthcare, and critical infrastructure sectors across Europe. The organization faces an increasingly sophisticated threat landscape driven by Advanced Persistent Threat (APT) groups targeting strategic assets through phishing campaigns, malware deployment, and infrastructure compromise.

One of the most prominent threat actors affecting SecureOps' clients is **MuddyWater**, an Iranian state-sponsored APT known for conducting espionage operations against government agencies, telecommunications providers, defense organizations, and critical infrastructure.

The growing volume of Indicators of Compromise (IOCs) collected from multiple intelligence sources created several operational challenges:

- Difficulty correlating threat intelligence from multiple community feeds.
- Delayed identification of malicious infrastructure.
- Limited visibility into adversary tactics, techniques, and procedures (TTPs).
- Slow production of actionable intelligence for incident responders and SOC analysts.

To address these challenges, SecureOps deployed the **Malware Information Sharing Platform (MISP)** to centralize threat intelligence, correlate Indicators of Compromise (IOCs), enrich threat data, and profile the MuddyWater threat actor using community intelligence feeds and MITRE ATT&CK mappings.

This project demonstrates how threat intelligence platforms can improve an organization's ability to identify, investigate, and respond to nation-state cyber threats through structured intelligence analysis.

## 🎯 Project Objectives

The primary objective of this project was to deploy the Malware Information Sharing Platform (MISP) and use it to investigate the **MuddyWater Advanced Persistent Threat (APT)** by collecting, analyzing, and correlating threat intelligence from community feeds.

### Specific Objectives

- Deploy the MISP platform using Docker in a controlled laboratory environment.
- Configure and enable default threat intelligence feeds within MISP.
- Collect Indicators of Compromise (IOCs) associated with the MuddyWater threat actor.
- Analyze malicious infrastructure, including IP addresses, URLs, domains, and file hashes.
- Profile the MuddyWater threat actor by identifying known aliases, motivations, targeted sectors, and notable campaigns.
- Correlate collected threat intelligence with MITRE ATT&CK techniques and adversary behaviors.
- Develop a structured threat intelligence report containing technical findings, IOC datasets, threat actor profiling, and recommended mitigation strategies.
- Demonstrate how Threat Intelligence Platforms (TIPs) enhance Security Operations Center (SOC) investigations and support proactive cyber defense.

### Expected Outcomes

Upon completion of the investigation, the project provides:

- A deployed and operational MISP instance.
- A structured repository of threat intelligence artifacts.
- A comprehensive IOC dataset exported from MISP.
- A detailed profile of the MuddyWater threat actor.
- MITRE ATT&CK mappings of observed adversary techniques.
- Actionable intelligence to support threat detection, incident response, and security monitoring.

- ## 🏗️ Threat Intelligence Investigation Workflow

The investigation followed a structured Threat Intelligence lifecycle, beginning with the deployment of the Malware Information Sharing Platform (MISP) and culminating in actionable threat intelligence reporting.

The workflow demonstrates how Indicators of Compromise (IOCs) were collected, correlated, enriched, and analyzed to build a comprehensive profile of the MuddyWater Advanced Persistent Threat (APT).

### Investigation Workflow

<p align="center">
  <img src="Screenshots/Threat_Intelligence_Investigation_Workflow.png" alt="Threat Intelligence Investigation Workflow" width="900"/>
</p>

### Workflow Description

1. **Deploy MISP using Docker**
   - Deploy the MISP Threat Intelligence Platform in a controlled laboratory environment using Docker containers.

2. **Configure Threat Intelligence Feeds**
   - Load the default MISP feed metadata.
   - Enable the first three community feeds.
   - Cache and import threat intelligence events.

3. **Threat Intelligence Collection**
   - Retrieve Indicators of Compromise (IOCs) from community threat intelligence sources.
   - Collect IP addresses, URLs, domains, file hashes, malware references, and related artifacts.

4. **Threat Actor Profiling**
   - Investigate the MuddyWater threat actor.
   - Identify aliases, motivations, targeted industries, campaigns, and associated infrastructure.

5. **Threat Correlation**
   - Correlate collected intelligence using MISP relationships.
   - Analyze links between malware, infrastructure, attack patterns, and adversary activity.

6. **MITRE ATT&CK Mapping**
   - Map observed behaviors to MITRE ATT&CK techniques.
   - Identify adversary tactics, techniques, and procedures (TTPs).

7. **IOC Export**
   - Export Indicators of Compromise (IOCs) as a CSV dataset for documentation, intelligence sharing, and future analysis.

8. **Threat Intelligence Reporting**
   - Produce a comprehensive threat intelligence report summarizing technical findings, IOC analysis, threat actor profiling, MITRE ATT&CK mappings, and mitigation recommendations.

---

## 🛠️ Technology Stack

| Technology | Purpose | Role in Project |
|------------|---------|-----------------|
| **MISP (Malware Information Sharing Platform)** | Threat Intelligence Platform | Collected, analyzed, correlated, and managed Indicators of Compromise (IOCs) and threat actor intelligence. |
| **Docker** | Containerization | Deployed and managed the MISP environment using Docker containers for consistent and reproducible deployment. |
| **Docker Compose** | Container Orchestration | Managed the MISP multi-container architecture, including supporting services such as the database and web application. |
| **Kali Linux** | Investigation Environment | Served as the primary operating system for deploying MISP and conducting threat intelligence investigations. |
| **Git** | Version Control | Managed project files and maintained version history throughout the investigation. |
| **GitHub** | Project Repository | Hosted the complete project documentation, screenshots, IOC dataset, and final investigation report. |
| **MITRE ATT&CK Framework** | Threat Modeling | Mapped MuddyWater adversary behaviors and Techniques, Tactics, and Procedures (TTPs) to industry-recognized ATT&CK techniques. |
| **Community Threat Intelligence Feeds** | Threat Intelligence Source | Supplied real-world threat intelligence events, Indicators of Compromise (IOCs), and threat actor information through MISP. |

### Core Skills Demonstrated

- Threat Intelligence Analysis
- Threat Actor Profiling
- IOC Collection and Correlation
- MITRE ATT&CK Mapping
- Threat Intelligence Feed Management
- Docker Deployment
- Threat Hunting
- Technical Documentation
- Cyber Threat Analysis
- Security Operations Center (SOC) Investigation

- ## 📂 Repository Structure

The repository is organized to separate project documentation, extracted threat intelligence artifacts, supporting resources, and implementation evidence.

```text
MuddyWater-Threat-Intelligence-with-MISP/
│
├── README.md
├── LICENSE
│
├── IOC_Data/
│   └── MuddyWater_IOCs.csv
│
├── Reports/
│   └── MuddyWater_Threat_Intelligence_Investigation_Report.pdf
│
├── Resources/
│   └── references.md
│
└── Screenshots/
    ├── 01_Project_Directory_Creation.png
    ├── 02_MISP_Docker_Repository_Cloned.png
    ├── 03_MISP_Docker_Project_Structure.png
    ├── 04_MISP_Core_Service_Started.png
    ├── 05_MISP_Docker_Stack_Healthy.png
    ├── 06_MISP_Login.png
    ├── 07_MISP_Default_Feed_Metadata_Loaded.png
    ├── 08_MISP_Default_Feeds_Enabled.png
    ├── 09_MISP_Threat_Intelligence_Events_Imported.png
    ├── 10_MuddyWater_Event_Overview.png
    ├── 11_Microsoft_Mango_Sandstorm_Profile.png
    ├── 12_MuddyWater_IOCs.png
    ├── 13_MuddyWater_Threat_Actor_Profile.png
    ├── 14_MuddyWater_Associated_Events.png
    ├── 15_MITRE_ATTACK_Mapping.png
    ├── 16_MuddyWater_Aliases.png
    ├── 17_MuddyWater_Threat_Relationship_Graph.png
    └── Threat_Intelligence_Investigation_Workflow.png
```

### Folder Description

| Folder | Description |
|----------|-------------|
| **IOC_Data/** | Contains the extracted Indicators of Compromise (IOCs) exported from MISP in CSV format. |
| **Reports/** | Contains the complete Threat Intelligence Investigation Report documenting the methodology, findings, IOC analysis, MITRE ATT&CK mappings, and recommendations. |
| **Resources/** | Contains supporting references and documentation used throughout the investigation. |
| **Screenshots/** | Contains implementation evidence documenting the deployment of MISP, threat intelligence feed configuration, IOC extraction, threat actor profiling, MITRE ATT&CK mapping, and relationship analysis. |

---

