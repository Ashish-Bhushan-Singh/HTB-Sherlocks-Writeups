# HTB Sherlocks – Blue Team Investigation Writeups

A collection of hands-on **Hack The Box Sherlocks** investigations documenting practical experience in Security Operations Center (SOC) analysis, Digital Forensics and Incident Response (DFIR), threat hunting, network forensics, and security monitoring.

This repository serves as my personal Blue Team learning journey and cybersecurity portfolio, progressing from beginner-level investigations to advanced incident response and threat hunting.

---

## 🎯 Objectives

- Develop practical SOC Analyst skills (L1 → L2 → L3).
- Investigate suspicious network and endpoint activity.
- Analyze Windows Event Logs, Sysmon, Linux authentication logs, and system artifacts.
- Perform network traffic analysis using Wireshark.
- Understand attack techniques and adversary behavior.
- Identify and document Indicators of Compromise (IOCs).
- Reconstruct incident timelines using forensic evidence.
- Practice incident response and threat hunting methodologies.
- Develop detection opportunities using SIEM queries and security tools.
- Build professional investigation reports supported by evidence.

---

## 📚 Investigation Roadmap

The repository is organized by investigation difficulty.

| Level | Difficulty | Learning Focus |
|---|---|---|
| 01 | Easy | SOC fundamentals and basic investigation |
| 02 | Medium | Network forensics and endpoint analysis |
| 03 | Hard | Advanced DFIR and threat hunting |
| 04 | Insane | Complex incident investigations |

*Difficulty classifications will be verified against the individual HTB Sherlock before starting each investigation.*

### Level 01 – Easy

| Sherlock | Primary Skills | Status |
|---|---|---|
| Brutus | Linux authentication logs, SSH investigation | ⬜ Not Started |
| Unit42 | Sysmon and Windows event analysis | ⬜ Not Started |
| BFT | Windows file-system forensics | ⬜ Not Started |
| Campfire-1 | Kerberoasting and Windows logs | ⬜ Not Started |

### Level 02 – Medium

| Sherlock | Primary Skills | Status |
|---|---|---|
| Meerkat | Suricata and network investigation | ⬜ Not Started |
| Noted | Windows artifacts and forensics | ⬜ Not Started |
| Knock Knock | PCAP and network forensics | ⬜ Not Started |
| Logjammer | Log analysis and incident investigation | ⬜ Not Started |
| Safecracker | Malware analysis | ⬜ Not Started |
| Constellation | Digital forensics and incident response | ⬜ Not Started |
| Hunter | Threat hunting | ⬜ Not Started |
| Noxious | LLMNR poisoning and NTLM analysis | ⬜ Not Started |
| Reaper | SMB, Windows logs and network forensics | ⬜ Not Started |

### Level 03 – Hard

| Sherlock | Primary Skills | Status |
|---|---|---|
| Subatomic | Malware analysis and Discord hijacking | ⬜ Not Started |
| Nubilum-1 | AWS CloudTrail and cloud forensics | ⬜ Not Started |
| Crown Jewel-1 | Active Directory forensics | ⬜ Not Started |
| Crown Jewel-2 | Active Directory investigation | ⬜ Not Started |
| SmartyPants | Windows event logs and RDP investigation | ⬜ Not Started |
| Campfire-2 | Kerberos and authentication attacks | ⬜ Not Started |
| MangoBleed | Linux forensics and MongoDB logs | ⬜ Not Started |

### Level 04 – Advanced Investigations

| Sherlock | Primary Skills | Status |
|---|---|---|
| APTNightmare | Advanced persistent threat investigation | ⬜ Not Started |
| APTNightmare2 | Advanced incident investigation | ⬜ Not Started |
| OpTinselTrace | Threat intelligence and APT investigation | ⬜ Not Started |
| UFO-1 | APT44 and ICS security | ⬜ Not Started |
| Dream Job-1 | Lazarus Group and threat intelligence | ⬜ Not Started |

*This is a learning roadmap, not a complete or currently verified HTB catalogue. Sherlock availability and difficulty may change.*

---

## 🔬 Investigation Methodology

Every completed Sherlock will follow a consistent investigation methodology.

1. **Scenario Overview** – Understand the incident and investigation requirements.
2. **Initial Triage** – Identify relevant evidence sources and suspicious activity.
3. **Evidence Collection** – Identify logs, artifacts, timestamps, and relevant files.
4. **Investigation** – Analyze the evidence using appropriate security tools.
5. **Timeline Reconstruction** – Establish the chronological sequence of events.
6. **Findings** – Document confirmed findings and supporting evidence.
7. **IOC Identification** – Extract relevant IP addresses, domains, hashes, and other indicators.
8. **MITRE ATT&CK Mapping** – Map observed attacker behavior to relevant techniques.
9. **Detection Opportunities** – Identify monitoring and detection improvements.
10. **Lessons Learned** – Document knowledge gained and areas for improvement.

---

## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| Network Analysis | Wireshark, TShark, Zeek |
| Network Security Monitoring | Suricata |
| Windows Investigation | Event Viewer, Sysmon |
| SIEM | Splunk, Elastic / Kibana |
| Linux Investigation | Linux CLI, grep, journalctl |
| Digital Forensics | Autopsy, Volatility, KAPE |
| Windows Forensics | Eric Zimmerman's Tools |
| Data Analysis | CyberChef |
| Threat Intelligence | MITRE ATT&CK |

Tools will be selected according to the evidence and requirements of each investigation.

---

## 📁 Repository Structure

```text
HTB-Sherlocks-Writeups/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── 01-Easy/
│   ├── Brutus/
│   ├── Unit42/
│   ├── BFT/
│   └── Campfire-1/
│
├── 02-Medium/
│   ├── Meerkat/
│   ├── Reaper/
│   └── Noxious/
│
├── 03-Hard/
│   ├── APTNightmare/
│   └── Subatomic/
│
├── 04-Insane/
│
├── Templates/
│   └── WRITEUP-TEMPLATE.md
│
└── Resources/
    ├── Tools.md
    ├── Useful-Commands.md
    ├── SIEM-Queries.md
    ├── Windows-Event-IDs.md
    └── Investigation-Checklist.md
```

Each completed Sherlock will have its own investigation documentation and supporting screenshots where appropriate.

---

## 📊 Skills Development

Throughout this project, I aim to develop practical experience in:

- Security alert triage and investigation.
- Network traffic analysis.
- Windows and Linux log analysis.
- Endpoint detection and investigation.
- Digital forensics and incident response.
- Threat intelligence and IOC analysis.
- Attack timeline reconstruction.
- SIEM queries and detection engineering.
- MITRE ATT&CK framework.
- Professional incident reporting.

---

## 📖 Resources

Additional learning materials and investigation references will be maintained here.

| Resource | Description |
|---|---|
| [Investigation Template](Templates/WRITEUP-TEMPLATE.md) | Standard investigation report structure |
| [Tools](Resources/Tools.md) | Security tools and their purposes |
| [Useful Commands](Resources/Useful-Commands.md) | Frequently used investigation commands |
| [SIEM Queries](Resources/SIEM-Queries.md) | SPL, KQL and Elastic queries |
| [Windows Event IDs](Resources/Windows-Event-IDs.md) | Important Windows security events |
| [Investigation Checklist](Resources/Investigation-Checklist.md) | Repeatable investigation workflow |

---

## ⚠️ Disclaimer

This repository is maintained for educational and professional development purposes.

- Investigations are conducted within authorized Hack The Box environments.
- Original Sherlock challenge archives and proprietary challenge files are not redistributed.
- Real malware samples and sensitive personal information are not uploaded.
- Solutions, flags, hints, and spoilers for active Sherlocks are not publicly disclosed.
- Writeups are published in accordance with applicable Hack The Box publication guidelines.
- All findings are documented using supporting evidence rather than unsupported assumptions.

---

## 🚀 Project Goal

My ultimate goal is to develop the practical knowledge and investigation methodology required to work as a **Security Operations Center (SOC) Analyst**, progressing from L1 to L3 capabilities.

Rather than simply documenting challenge answers, I aim to explain:

- What happened?
- How did it happen?
- Which evidence supports the findings?
- How can the activity be detected?
- What should a SOC analyst investigate next?

**Evidence-driven investigations. Clear methodology. Continuous learning.**
