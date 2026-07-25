# NovaCore Threat Intelligence Capstone Project – Phase 1

## Overview
This repository contains the full Phase 1 deliverables for the **NovaCore Threat Intelligence Capstone Project**, including business profiling, threat landscape analysis, attacker perspective, regional threat context, intelligence requirements, collection planning, and a complete Threat Intelligence (TI) matrix.

NovaCore is a high‑volume financial technology (fintech) platform operating across digital payments, wallets, customer identity, onboarding, and cross‑border financial transactions. Due to its operational footprint, NovaCore is a high‑value target for financially motivated cybercriminals, fraud rings, and advanced persistent threat (APT) groups.

---

## Repository Structure
<img width="917" height="406" alt="image" src="https://github.com/user-attachments/assets/21bbc0ac-30b7-4459-8e8a-87d08002eee7" />


---

## Phase 1 Deliverables

### 1. NovaCore Threat Profile  
**File:** `docs/Novacore-Threat-Profile.md`

This document outlines NovaCore’s core business operations and cyber‑exposed assets, including:

- Digital Payments & FX  
- Digital Wallets  
- Customer Accounts  
- Financial Transactions  
- Business Onboarding (KYB)  
- Customer Identity (KYC)

It also describes NovaCore’s attack surfaces and operational risks across identity, wallets, payments, and transaction systems.

---

### 2. Regional Threat Context (North America)  
**File:** `docs/Regional-Threat-Context.md`

This analysis covers the North American fintech threat landscape, including:

- High‑value asset targeting  
- Double‑extortion ransomware  
- Credential theft & Adversary‑in‑the‑Middle (AitM) phishing  
- Initial Access Broker (IAB) ecosystems  

Key threat actor categories:

- Scattered Spider  
- Akira & Play ransomware groups  
- Storm‑0569 / Storm‑1674 phishing collectives  
- Lazarus Group (DPRK)

---

### 3. Attacker Perspective  
**File:** `docs/Threat_intel_attacker_perspective.md`

This document provides an attacker‑centric view of NovaCore’s environment, identifying:

- High‑value assets (wallets, customer data, payment systems, admin portals)  
- Motivations for targeting each asset  
- Core threats such as phishing, credential theft, malware, ransomware, data theft, payment fraud, and BEC  
- MITRE ATT&CK mappings for each threat  

It explains how adversaries think, prioritize targets, and exploit weaknesses in fintech ecosystems.

---

### 4. Intelligence Requirements (PIRs)  
**File:** `docs/Intelligence-Requirements.md`

Priority Intelligence Requirements define what NovaCore must learn to proactively defend its assets:

1. Fintech‑targeting threat actors  
2. North American threat actor footprint  
3. Phishing & AitM credential harvesting  
4. Ransomware groups using double‑extortion  
5. Historical attacks on payment processors  
6. Defensive prioritization for NovaCore  

The document also includes:

- A tactical collection matrix  
- Data source mapping  
- Collection operations timeline  

---

### 5. References  
**File:** `research/references.md`

This file compiles authoritative sources used throughout the project, including:

- CISA  
- FBI  
- Microsoft Threat Intelligence  
- CrowdStrike Global Threat Intelligence  
- MITRE ATT&CK  
- FS‑ISAC  

---

## Purpose of This Repository
This repository serves as the foundation for NovaCore’s Threat Intelligence program. It is intended for:

- Security analysts  
- Threat intelligence researchers  
- Fintech cybersecurity teams  
- Academic or professional TI capstone evaluation  

Future phases may expand into:

- Threat actor profiling  
- Detection engineering  
- TI automation pipelines  
- Risk scoring and prioritization  
- Defensive strategy development  

---

## Author
**Palence Konissi**  
Threat Intelligence Analyst  
Edmonton, Alberta, Canada  

---

## License
This project is licensed under the MIT License.
