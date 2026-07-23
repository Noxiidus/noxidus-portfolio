<div align="center">

# Katona Balázs — `Noxidus`

**Penetration Tester @ KryloneEsport**

Red team offensive testing and blue team digital forensics — Hungary 🇭🇺

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ankara.herho@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Noxiidus)
[![Credly](https://img.shields.io/badge/Credly-FF6B00?style=for-the-badge&logo=credly&logoColor=white)](https://www.credly.com/users/noxidus)

</div>

---

## Professional Summary

I work both sides of offensive and defensive security. On the red team side I focus on
reconnaissance, web application testing, credential attacks and post-exploitation. On the blue team
side I investigate the aftermath — log forensics, packet analysis, malware triage and threat
intelligence.

The two disciplines reinforce each other constantly. Running a vhost fuzzing campaign teaches me
exactly what it looks like in a web server log. Reconstructing an intrusion from a PCAP teaches me
which of my own techniques would have been caught, and which would have slipped past. I keep both
skill sets deliberately, and I document everything — an undocumented finding is a finding that
helps nobody.

This repository is a detailed portfolio. For the short version, see
[my GitHub profile](https://github.com/Noxiidus).

---

## Table of Contents

- [Areas of Expertise](#areas-of-expertise)
- [Technical Skills](#technical-skills)
- [Featured Work — Digital Forensics](#featured-work--digital-forensics)
- [Security Tooling](#security-tooling)
- [Web Development](#web-development)
- [Certifications](#certifications)
- [How I Work](#how-i-work)
- [Contact](#contact)

---

## Areas of Expertise

### ⚔️ Offensive Security (Red Team)

| Area | Detail |
|---|---|
| **Reconnaissance** | Subdomain and virtual-host discovery, content discovery, service fingerprinting, OSINT collection |
| **Web application testing** | Authentication flaws, access control issues, input validation, session handling |
| **Credential attacks** | Password spraying, brute-force methodology, default-credential auditing |
| **Privilege escalation** | Linux SUID/capability abuse, misconfiguration exploitation, role and permission abuse |
| **Post-exploitation** | Persistence mechanisms, lateral movement, cloud API abuse, data staging |
| **Reporting** | Reproducible findings with clear impact statements and remediation guidance |

### 🛡️ Defensive Security (Blue Team)

| Area | Detail |
|---|---|
| **Host forensics** | Linux authentication logs, `wtmp`/`utmp` binary session artifacts, timeline reconstruction |
| **Network forensics** | PCAP analysis, attack-chain reconstruction, exfiltration identification, C2 detection |
| **Malware analysis** | Static ELF triage — symbol recovery, disassembly, string extraction, C2 configuration extraction |
| **Threat intelligence** | Multi-source correlation, actor profiling, IOC extraction, MITRE ATT&CK mapping |
| **Detection engineering** | Translating attacker behaviour into practical detection logic |

---

## Technical Skills

**Offensive tooling**

![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6633?style=for-the-badge&logo=burpsuite&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-4682B4?style=for-the-badge&logo=gnometerminal&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=for-the-badge&logo=metasploit&logoColor=white)
![ffuf](https://img.shields.io/badge/ffuf-2E8B57?style=for-the-badge&logo=gnometerminal&logoColor=white)

**Forensics & analysis**

![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-C81D25?style=for-the-badge&logo=mitre&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Capstone](https://img.shields.io/badge/Capstone-5C2D91?style=for-the-badge&logo=gnometerminal&logoColor=white)

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**Web & data**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**Platforms & tools**

![Hack The Box](https://img.shields.io/badge/Hack_The_Box-9FEF00?style=for-the-badge&logo=hackthebox&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Unity](https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white)

---

## Featured Work — Digital Forensics

Full writeups live in **[htb-sherlock-writeups](https://github.com/Noxiidus/htb-sherlock-writeups)**.
These are condensed case summaries of retired Hack The Box Sherlocks.

### Case Study — SSH Brute-Force Intrusion (*Brutus*)

**Artifacts:** Linux `auth.log`, binary `wtmp`
**Focus:** Host forensics, timeline reconstruction

An AWS-hosted Confluence server was compromised through an SSH brute-force attack. The investigation
reconstructed the full intrusion timeline from two artifacts.

The analytically interesting part was separating the *automated* credential hit from the attacker's
*interactive* session. The brute-force tool validated the `root` password and disconnected within
the same second, opening and closing a session immediately. The real hands-on-keyboard login came
64 seconds later as a separate session — and only correlating `auth.log` against the binary `wtmp`
records made that distinction provable.

`wtmp` was parsed directly by walking its 384-byte record structure rather than relying on the
bundled helper script, which formats timestamps in local time and silently produces wrong answers
on a non-UTC host.

**Findings:** attacker IP, compromised account, backdoor account creation with `sudo` group
membership, shadow-file access, and retrieval of an open-source Linux persistence toolkit.
**Mapped to:** T1110 (Brute Force), T1136.001 (Create Account: Local Account), T1548.003 (Sudo and
Sudo Caching)

---

### Case Study — OpenStack Cloud Compromise (*Vantage*)

**Artifacts:** Two PCAPs — public web server and OpenStack controller
**Focus:** Network forensics, cloud attack-chain reconstruction

A full intrusion reconstructed packet by packet, from initial reconnaissance through credential
theft, data exfiltration and persistence.

The attacker fuzzed **3,579 virtual hosts** to find a single unadvertised dashboard. Isolating that
one hit required correlating every HTTP response back to its request — and the obvious approach of
matching on `tcp.stream` produces false positives, because HTTP keep-alive places many requests on
one stream. Matching on `http.request_in` gave exact pairing and reduced 3,579 candidates to one:
the only host returning a 302 redirect instead of the uniform 200 baseline.

From there the chain was: credential brute-force against the dashboard, theft of the OpenStack
`openrc` API credentials file, and a pivot to direct API abuse. That pivot is visible as a clean
User-Agent transition from a browser string to `openstacksdk/keystoneauth1` — a highly practical
detection signal for stolen-credential abuse in cloud environments.

The attacker then enumerated the Keystone service catalog, discovered the Swift object store,
listed its containers and exfiltrated PII. Because Swift was served over plaintext HTTP, the stolen
records were fully recoverable from the capture. Persistence was a backdoor cloud account granted
the `admin` role.

**Findings:** full timeline to the second, exfiltrated data quantified, backdoor account and
credentials recovered.
**Mapped to:** T1595 (Active Scanning), T1110 (Brute Force), T1552.001 (Credentials In Files),
T1530 (Data from Cloud Storage), T1136.003 (Create Account: Cloud Account)

---

### Case Study — APT Threat Profiling (*FortySeven-1*)

**Artifacts:** Three public vendor reports
**Focus:** Threat intelligence, multi-source correlation

An intelligence-fusion exercise profiling **Mysterious Elephant (APT-K-47)**, a South Asian actor
using Hajj-themed phishing lures to steal WhatsApp data from government and diplomatic targets.

The work involved correlating a Kaspersky report against two Knownsec 404 analyses to build a
unified picture: custom backdoor internals and its DLL-hijacking deployment, an attribution pivot
linking the actor to Bitter through shared tooling, the four-version evolution of the group's
primary implant (including its C2 migration from TCP to HTTPS), sandbox-evasion and hidden-desktop
techniques in their loader, and their WhatsApp exfiltration toolset.

**Output:** actor profile, toolset inventory, IOC extraction, CVE attribution, full ATT&CK mapping.

---

### Static Malware Analysis — io_uring C2 Implant

**Artifact:** 31 KB stripped-symbol-free ELF64 binary
**Focus:** Static reverse engineering

Analysis of a Linux C2 agent built specifically to evade EDR. Every I/O operation — network and
filesystem alike — is routed through the kernel's `io_uring` interface rather than conventional
syscalls, so tooling that hooks syscalls or eBPF tracepoints never observes the activity.

The binary was analysed **entirely statically** — never executed. ELF structure and symbols were
recovered with `pyelftools`, the command dispatcher and network setup disassembled with `capstone`
to extract the hardcoded C2 endpoint, reconnection interval and full command set.

Its most notable capability is an anti-EDR routine that disables kernel ftrace, deletes pinned BPF
objects, and terminates any process whose memory map references a BPF map — a direct attack on
eBPF-based security agents.

**Mapped to:** T1562.001 (Impair Defenses), T1070.004 (Indicator Removal: File Deletion),
T1106 (Native API)

---

## Security Tooling

### [Simple Port Scanner](https://github.com/Noxiidus/Simple-Port-Scanner) · `Python`
A TCP port scanner written from scratch to understand socket programming, connection handling and
service enumeration at a level that using `nmap` alone does not teach.

### [Password Strength Checker](https://github.com/Noxiidus/Password-Strength-Checker) · `Python`
Evaluates passwords against common weakness patterns. Building it was a practical demonstration of
why entropy and length outperform arbitrary complexity rules — and why composition requirements
often push users toward predictable substitutions.

---

## Web Development

Web development is where I started, and it remains directly useful — understanding how applications
are actually built makes it far easier to find where they break.

### [Crypto Price Tracker](https://github.com/Noxiidus/crypto-price-tracker) · `JavaScript`
Live cryptocurrency price tracking against a public API, covering asynchronous requests, error
handling and dynamic DOM rendering.

### [Weather App](https://github.com/Noxiidus/weather-app) · `HTML · CSS · JavaScript`
Fully responsive, mobile-friendly weather client built around third-party API consumption and
responsive layout techniques.

---

## Certifications

[![Verify on Credly](https://img.shields.io/badge/Verify_all_badges_on_Credly-FF6B00?style=for-the-badge&logo=credly&logoColor=white)](https://www.credly.com/users/noxidus)

### Security

| Certification | Issuer | Issued |
|---|---|---|
| **Google Cloud Cybersecurity Certificate** | Google Cloud | Jul 2026 |

Covers security principles in cloud environments — identity and access management, network
security controls, threat detection and incident response, and compliance frameworks.

### AI & Data

| Certification | Issuer | Issued |
|---|---|---|
| **Google AI Professional Certificate** | Google Career Certificates | Jul 2026 |
| **Google AI Essentials** | Google Career Certificates | Jul 2026 |

<details>
<summary><b>Component badges</b> — Google AI Professional Certificate</summary>

<br>

| Badge | Issued |
|---|---|
| AI Fundamentals | Jul 2026 |
| AI for App Building | Jul 2026 |
| AI for Brainstorming and Planning | Jul 2026 |
| AI for Content Creation | Jul 2026 |
| AI for Data Analysis | Jul 2026 |
| AI for Research and Insights | Jul 2026 |
| AI for Writing and Communicating | Jul 2026 |

</details>

### Web Development

| Certification | Issuer |
|---|---|
| **Responsive Web Design** | freeCodeCamp |

![Responsive Web Design Certification](https://github.com/user-attachments/assets/a1ceaf6a-011e-4357-8a20-5c2bf6803404)

---

## How I Work

**Evidence over assumption.** Every claim in my writeups traces back to a specific artifact — a log
line, a frame number, a byte offset. If I cannot point at it, I do not assert it.

**Document the wrong turns.** My writeups include the approaches that failed, because the reasoning
that rules something out is often more instructive than the answer itself.

**Verify the method, not just the result.** A correct answer reached by a flawed method will fail
the next time. When an approach produces a suspicious result, I check the approach before I check
the data.

**Analyse safely.** Malware is examined statically in controlled environments. Nothing is executed
to find out what it does.

---

## Contact

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ankara.herho@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Noxiidus)

Open to discussing offensive security, forensics, and CTFs.

---

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=noxiidus&show_icons=true&theme=radical)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=noxiidus&layout=compact&theme=radical)

<sub>All security work shown here was performed in authorized lab environments and CTF platforms.</sub>

</div>
