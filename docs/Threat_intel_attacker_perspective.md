# Threat Intelligence Profile: Attacker Perspective & Threat Matrix

## 1. Think Like an Attacker
If a cybercriminal were targeting a fintech platform like NovaCore, they would systematically exploit assets that yield the highest financial payout, the most valuable data, or the deepest operational control. 

### High-Value Asset Target Matrix

| Asset | Why Attack It? |
| :--- | :--- |
| **Customer Database** | Accesses personal information (PII/KYC) for identity theft, blackmail, or resale on the dark web. |
| **Wallets** | Direct access to stored digital value, allowing instant, irreversible drain of liquid monetary assets. |
| **Payment System** | Facilitates automated financial fraud, transaction rerouting, or unauthorized duplicate payouts. |
| **Employee Accounts** | Grants initial access to the internal corporate network via phishing or session hijacking. |
| **Cloud Storage** | Offers bulk data theft of sensitive files, source code, and cryptographic configuration keys. |
| **Admin Portal** | Achieves full privilege escalation to modify global platform rules, balances, and security policies. |

---

## 2. Threat Identification
The following threats directly target the assets identified above, mapping out the precise mechanisms an adversary would deploy against the platform.

### Core Threat Matrix

| Threat | Why Relevant |
| :--- | :--- |
| **Phishing** | Manipulates employees or customers to steal credentials or session tokens via deceptive communications. |
| **Credential Theft** | Allows adversaries to access accounts cleanly without triggering standard brute-force alarms. |
| **Malware** | Infiltrates internal devices to achieve initial compromise, keylogging, or persistent network access. |
| **Ransomware** | Encrypts critical transaction systems and ledgers to completely halt operations and extort funds. |
| **Data Theft** | Enables attackers to exfiltrate and sell customer data, leading to severe regulatory fines and brand damage. |
| **Payment Fraud** | Exploits system logic or flaws to route unauthorized transactions for direct financial gain. |
| **Business Email Compromise** | Spoofs executive or partner emails to authorize fraudulent wire transfers and fake invoices. |

---

## 3. MITRE ATT&CK Matrix Mapping
The core threats identified above map directly to specific **MITRE ATT&CK Enterprise tactics and techniques**, establishing a standardized baseline for detection and defense.

| Threat | MITRE ATT&CK Tactic | Technique ID | Technique Name |
| :--- | :--- | :--- | :--- |
| **Phishing** | Initial Access | **T1566** | Phishing |
| **Credential Theft** | Credential Access | **T1003** | OS Credential Dumping |
| | Credential Access | **T1539** | Steal Web Session Information |
| **Malware** | Execution | **T1204** | User Execution |
| | Persistence | **T1547** | Boot or Logon Autostart Execution |
| **Ransomware** | Impact | **T1486** | Data Encrypted for Impact |
| **Data Theft** | Exfiltration | **T1020** | Automated Exfiltration |
| | Exfiltration | **T1567** | Exfiltration Over Web Service |
| **Payment Fraud** | Impact | **T1496** | Resource Hijacking |
| | Impact | **T1565** | Data Manipulation |
| **Business Email Compromise** | Initial Access | **T1566.002** | Phishing: Spearphishing Link / Attachment |
| | Resource Development | **T1585** | Establish Accounts |

---

## 4. Regional Threat Context (North America)

Operating a fintech platform in North America introduces immediate exposure to highly sophisticated, well-funded cybercriminal ecosystems. According to threat intelligence data from [CISA](https://www.cisa.gov/), [Microsoft Threat Intelligence](https://www.microsoft.com/en-us/security/security-insider/threat-landscape), and [CrowdStrike](https://www.crowdstrike.com/en-us/global-threat-report/), the regional threat vectors targeting banking, cryptocurrency, and financial operations are categorized into three distinct adversary archetypes:

### 1. Cybercriminal & APT Groups Targeting Banks
* **Lazarus Group (DPRK):** State-sponsored threat group notorious for high-profile financial heists, SWIFT banking compromises, and targeting crypto-adjacent fintech infrastructure to evade sanctions.
* **Scattered Spider (UNC3944):** A highly active cybercriminal collective utilizing aggressive social engineering, SMS phishing, and SIM-swapping to compromise financial institution identities and initial access brokers.

### 2. Ransomware Ecosystems Attacking Financial Firms
* **Qilin:** A highly active Ransomware-as-a-Service (RaaS) network aggressively hitting financial hubs via third-party service provider supply-chain exploits.
* **Akira & Play:** Prominent threat actors executing double-extortion campaigns against Western financial data pools, combining silent data exfiltration (PII/KYC ledgers) with operational lockouts.

### 3. Phishing & Social Engineering Collectives
* **Storm-0569 / Storm-1674:** Threat networks tracked by Microsoft deploying highly personalized Adversary-in-the-Middle (AitM) phishing templates to bypass financial multi-factor authentication (MFA).
* **AI-Driven Synthetic Fraud Rings:** Unaligned threat groups weaponizing generative AI and voice cloning to target digital onboarding systems and bypass automated eKYC/liveness checks.
