# Intelligence Requirements

This document outlines the core intelligence requirements (IRs) needed to proactively defend NovaCore's operational assets against active financial cybercrime ecosystems.

## Core Priority Intelligence Requirements (PIRs)

1. **Fintech Targeting:** Which financially motivated threat actors actively target fintech companies, digital wallets, and decentralized payment rails?
2. **Geographic Footprint:** Which threat actors are most active in North America, and what are their preferred network access times or geographic origins?
3. **Initial Access Vectors:** Which specific threat groups primarily use advanced phishing campaigns, AitM infrastructure, or social engineering to harvest credentials?
4. **Ransomware Deployment:** Which ransomware groups consistently deploy double-extortion tactics against financial institutions and core banking ledgers?
5. **Historical Precedent:** Which groups have previously targeted payment processors or digital wallet providers, and what post-compromise behaviors did they exhibit?
6. **Defensive Prioritization:** What defensive measures and technical controls should NovaCore prioritize to most effectively reduce operational risk and protect customer identities?

---

Threat Intelligence Collection Plan

This collection plan maps the priority intelligence requirements (PIRs) to specific data sources, collection methods, and functional tools to ensure NovaCore continuously gathers actionable threat data.

## 1. Tactical Collection Plan Matrix

| Intelligence Requirement (IR) | Primary Data Sources | Collection Method / Tools | Processing Action |
| :--- | :--- | :--- | :--- |
| **PIR 1 & 5: Fintech & Wallet Targeting** | Financial Sector ISACs, Dark Web forums, commercial threat feeds. | Automated ingestion of FS-ISAC alerts; monitoring underground asset marketplaces (e.g., Tor, Telegram). | Extract indicators of compromise (IoCs) related to payment API exploitation. |
| **PIR 2: North American Footprint** | CISA Alerts, FBI Flash reports, CrowdStrike/Mandiant global reports. | RSS feeds, threat intelligence platform (TIP) synchronization, API tracking. | Map observed group infrastructure to geographic geofencing policies. |
| **PIR 3: Phishing & Access Vectors** | Internal email gateway logs, commercial phishing threat feeds. | Demisto/Cortex XSOAR automation, analyzing active AitM kits via URLScan.io. | Update email gateway blacklists and security awareness training models. |
| **PIR 4: Ransomware Deployment** | Ransomware data leak sites, threat researcher blogs, CISA StopRansomware. | Automated web scraping of active leak sites (onion sites), tracking group infrastructure. | Feed known ransomware file hashes and C2 IPs into the EDR/SIEM environment. |
| **PIR 6: Defensive Prioritization** | MITRE ATT&CK/D3FEND frameworks, internal gap analysis audits. | Cross-referencing active threat actor TTPs against current defensive postures. | Generate a prioritized engineering ticket queue for infrastructure hardening. |

---

## 2. Collection Operations Timeline
* **Daily (Automated):** Pull IoCs from commercial feeds, open-source intelligence (OSINT), and security vendor APIs directly into the SIEM.
* **Weekly (Operational):** Review newly disclosed ransomware leak listings and CISA/FBI advisories targeting North American financial infrastructure.
* **Monthly (Strategic):** Evaluate the overall collection efficiency against the PIRs to tune automated alerting and eliminate duplicate intelligence noise.
