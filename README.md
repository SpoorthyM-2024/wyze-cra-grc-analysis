# Wyze Labs — EU Cyber Resilience Act GRC Gap Analysis

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Framework: NIST CSF 2.0](https://img.shields.io/badge/Framework-NIST%20CSF%202.0-green.svg)
![Regulation: EU CRA](https://img.shields.io/badge/Regulation-EU%20CRA%202024-red.svg)

## Overview

This repository contains an independent graduate-level GRC (Governance, Risk, and 
Compliance) research project assessing the cybersecurity compliance posture of 
**Wyze Labs Inc.** against the **EU Cyber Resilience Act (CRA)**, which becomes 
fully enforceable on December 11, 2027.

The analysis evaluates all 21 mandatory requirements outlined in CRA Annex I across 
product security and vulnerability handling categories, using NIST CSF 2.0 as the 
primary comparison framework and CISA Secure by Design as supplementary guidance.

---

## Key Findings

| Metric | Result |
|---|---|
| Total CRA requirements assessed | 21 |
| HIGH risk gaps identified | 12 |
| MEDIUM risk gaps identified | 6 |
| LOW risk / Compliant | 3 |
| Real incidents used as evidence | 4 (2019–2024) |
| Report length | 20 pages |

### Top 3 Critical Findings
- **No SBOM** — Wyze has no published Software Bill of Materials for any product, 
  creating critical supply chain visibility gaps (CRA-P2-01)
- **3-year patch delay** — Wyze was notified of critical vulnerabilities in 2019 
  but did not patch or disclose them for 3 years (CRA-P2-02)
- **Data sold to advertisers** — Wyze's privacy policy explicitly states personal 
  data is shared with third-party advertisers, directly violating CRA's data 
  minimisation requirement (CRA-P1-07)

---

## Repository Contents

| File | Description |
|---|---|
| `wyze_cra_gap_analysis_report.docx` | Full 20-page GRC report |
| `risk_register.md` | Complete 21-row risk register in markdown |
| `README.md` | This file |

---

## Methodology

### Frameworks Used
- **EU Cyber Resilience Act (CRA)** — Regulation (EU) 2024/2847, Annex I
- **NIST Cybersecurity Framework 2.0** — Primary comparison benchmark
- **CISA Secure by Design** — Supplementary guidance (Oct 2023)

### Assessment Approach
1. All 21 CRA Annex I requirements extracted and catalogued
2. Each requirement mapped to NIST CSF 2.0 subcategory codes
3. Gap assessed (Y / Partial / N) using publicly available Wyze evidence
4. Risk scored using Likelihood × Impact matrix (H/M/L)
5. Remediation actions defined per requirement
6. Owner and timeline assigned per industry GRC practice

### Evidence Sources
All findings are based exclusively on publicly available information:
- Wyze Security Transparency Reports (2022, 2023, 2024)
- Wyze Privacy Policy (wyze.com/policies/privacy-policy)
- Bitdefender CVE disclosure report (March 2022)
- NIST NVD CVE records (CVE-2023-6322, CVE-2023-6323, CVE-2023-6324)
- Mozilla Foundation Privacy Not Included assessment
- Twingate breach analysis
- TechRadar and SafeWise security reporting

---

## Risk Register Summary

| Req ID | Requirement | Gap | Risk | Timeline |
|---|---|---|---|---|
| CRA-P1-01 | No known vulnerabilities at release | Y | HIGH | Immediate |
| CRA-P1-02 | Secure by default configuration | Y | HIGH | Immediate |
| CRA-P1-03 | Automatic security updates | Partial | HIGH | Immediate |
| CRA-P1-04 | Access control and authentication | Partial | HIGH | Short-term |
| CRA-P1-05 | Data encryption at rest and transit | Partial | HIGH | Short-term |
| CRA-P1-06 | Data integrity verification | Y | HIGH | Short-term |
| CRA-P1-07 | Data minimisation | Y | HIGH | Short-term |
| CRA-P1-08 | DoS resilience and availability | Partial | MEDIUM | Medium-term |
| CRA-P1-09 | Minimise impact on other devices | N | LOW | No action |
| CRA-P1-10 | Attack surface reduction | Partial | HIGH | Short-term |
| CRA-P1-11 | Exploitation mitigation techniques | Y | HIGH | Short-term |
| CRA-P1-12 | Security logging (free) | Y | MEDIUM | Medium-term |
| CRA-P1-13 | User data deletion feature | Y | MEDIUM | Medium-term |
| CRA-P2-01 | SBOM for all products | Y | HIGH | Short-term |
| CRA-P2-02 | Timely vulnerability remediation | Y | HIGH | Immediate |
| CRA-P2-03 | Regular security testing | Y | HIGH | Short-term |
| CRA-P2-04 | Public vulnerability disclosure | Partial | MEDIUM | Medium-term |
| CRA-P2-05 | Coordinated disclosure policy | Partial | MEDIUM | Medium-term |
| CRA-P2-06 | Vulnerability reporting contact | Partial | LOW | Long-term |
| CRA-P2-07 | Secure update distribution | Y | HIGH | Short-term |
| CRA-P2-08 | Free security updates | Y | MEDIUM | Medium-term |

---

## Regulatory Context

| Item | Detail |
|---|---|
| Regulation | EU Cyber Resilience Act — Regulation (EU) 2024/2847 |
| Entered into force | December 10, 2024 |
| Fully enforceable | December 11, 2027 |
| Scope | All products with digital elements sold in the EU |
| Maximum penalty | EUR 15M or 2.5% of global annual turnover |
| SBOM requirement | CRA Annex I, Part II, §1 |
| Incident reporting | 24 hours to ENISA for actively exploited vulnerabilities |

---

## Tools Used

| Tool | Purpose | Cost |
|---|---|---|
| Google Sheets | Risk register creation | Free |
| Google Docs | Report writing | Free |
| Zotero | Citation management | Free |
| draw.io | Compliance diagrams | Free |
| NIST CSF 2.0 Reference Tool | Framework mapping | Free |

---

## Academic Context

This project was completed as part of a graduate cybersecurity program in the 
United States. It demonstrates applied GRC methodology including regulatory 
analysis, gap assessment, risk scoring, and remediation planning — all grounded 
in real-world public evidence.

**Target roles:** GRC Analyst, Compliance Analyst, Risk Analyst, 
Security Analyst, DevSecOps Engineer

---

## Disclaimer

This report is an independent academic analysis based entirely on publicly 
available information. It is not affiliated with, endorsed by, or 
commissioned by Wyze Labs Inc. All findings are based on publicly 
available security disclosures, CVE records, and published documentation.

---

## References

1. European Union. (2024). Regulation (EU) 2024/2847 — Cyber Resilience Act. https://eur-lex.europa.eu
2. NIST. (2024). Cybersecurity Framework 2.0. https://doi.org/10.6028/NIST.CSWP.29
3. CISA et al. (2023). Shifting the Balance of Cybersecurity Risk: Secure by Design. https://www.cisa.gov
4. Wyze Labs. (2022). Response to 3-29-22 Security Report. https://www.wyze.com
5. Bitdefender. (2022). Multiple Vulnerabilities in Wyze Cam. https://www.bitdefender.com
6. Mozilla Foundation. (2023). Wyze Cams — Privacy Not Included. https://foundation.mozilla.org