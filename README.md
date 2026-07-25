#  Executive Case Study: Incident Post-Mortem & Strategic Cybersecurity Transformation

> **Project Type:** Cybersecurity Master's Academic Case Study (Immune Technology Institute)  
> **Role:** Virtual CISO (vCISO) / Senior Security Consultant  
> **Author:** Jhonny Valdivieso  
> **Target Client:** Terra Renewables (Fictional Enterprise)  
> **Date:** November 17, 2025  

---

##  Executive Summary

This repository contains a comprehensive post-mortem analysis and strategic remediation roadmap following a series of simulated, escalating cyber-attacks against **Terra Renewables**. 

The goal of this case study is to bridge the gap between technical incident forensics and C-level risk governance demonstrating how unaddressed hygiene issues (such as credential exposure via social media) can evolve into multi-million euro financial fraud and persistent internal threats.

---

##  Table of Contents
1. [Executive Narrative: The Anatomy of the Breach](#1-executive-narrative-the-anatomy-of-the-breach)
2. [Systematic Vulnerability Assessment](#2-systematic-vulnerability-assessment)
3. [Multi-Dimensional Impact Analysis](#3-multi-dimensional-impact-analysis)
4. [Strategic Security Remediation](#4-strategic-security-remediation)
5. [Cybersecurity Leadership Dashboard (KPIs)](#5-cybersecurity-leadership-dashboard-kpis)
6. [Crisis Communication & Awareness Framework](#6-crisis-communication--awareness-framework)
7. [Conclusion & Takeaways](#7-conclusion--takeaways)

---

## 1. Executive Narrative: The Anatomy of the Breach

The security crisis at Terra Renewables was not a sudden event, but a two-year failure of oversight resulting in a persistent threat actor exploiting an unaddressed culture of vulnerability.

### The Pool Pass Incident (Dwell-Time Origin)
* **Date & Time:** July 25th, 18:30
* **Scope:** Screens across all 20 global branches were compromised to display a message promising free pool passes using the code `#PoolPass`.
* **Root Cause:** A subcontracted IT technician posted a photo on LinkedIn from a beach. In the background, his laptop screen exposed a remote access portal alongside a physical sticky note containing his plain-text credentials.
* **Initial Management Action:** The firm simply replaced the technician without revoking existing tokens, enforcing MFA, or segmenting the network.

### Escalation: CEO Fraud & Data Exfiltration
* **Dwell Time:** 2 years of silent persistence.
* **Exfiltration:** Forensic analysis confirmed customer data (January) and employee data (March) exfiltration routed to `cr4ck.100@irnini.com`.
* **The Climax:** A €3,500,000 CEO fraud attack. A treasury employee received a spoofed email requesting an urgent transfer for "new windmills" and initiated the transaction without out-of-band validation.
* **Forensic Evidence:** Both the initial "Pool Pass" incident and the phishing attack originated from the exact same IP address: `79.3.190.255`.

> ** vCISO Strategic Perspective:**  
> The "Pool Pass" incident was treated as a harmless prank, but it was in fact a successful penetration test by an adversary. Granting an attacker a two-year dwell time due to lack of MFA and network segmentation proves that an attacker who finds an open door will wait, observe, and strike when the financial stakes are highest.

---

## 2. Systematic Vulnerability Assessment

| Category | Vulnerability | Strategic Impact |
| :--- | :--- | :--- |
| **People** | Social Media & Digital Hygiene | Staff awareness regarding digital footprints was non-existent; a single photo compromised the entire global perimeter. |
| **Technology** | Absence of Multi-Factor Authentication (MFA) | Remote access relied solely on static passwords. Single factor access to corporate systems is equivalent to leaving the front door unlocked. |
| **Technology** | Lack of Network Segregation | Absence of internal micro-segmentation allowed lateral movement from a single endpoint to global display systems across 20 locations. |
| **Process** | Restricted Monitoring Windows | "Office-hours-only" monitoring (08:00–17:00) left a daily 15-hour window of opportunity for unmonitored threat actor activity. |
| **Process** | Weak Third-Party Risk Management (TPRM) | Subcontracted staff received high-level access without sufficient security vetting or technical guardrails. |
| **Process** | Inadequate Financial Controls | Absence of dual-authorization or voice verification protocols for high-value transfers enabled successful CEO fraud execution. |

> ** vCISO Strategic Perspective:**  
> Adversaries do not adhere to standard business hours; they actively target "dark hours" knowing SIEM systems are unmonitored. Furthermore, modern perimeters are defined by employee digital behavior, not just corporate firewalls.

---

## 3. Multi-Dimensional Impact Analysis

*  **Economic Impact:** Although the €3.5M transfer was eventually recovered, unplanned expenditure was incurred. Terra was forced to honor the attacker's "pool passes" to manage internal morale and de-escalate tensions.
*  **Reputational Impact:** With 20 branches serving ~400 clients daily (8,000 daily exposures), the exfiltration of customer data created severe long-term liability, risk of regulatory fines, and loss of institutional trust.
*  **Human & Operational Impact:** Terminating technical staff resulted in a loss of institutional knowledge. The subsequent recruitment and retraining overhead far exceeded the immediate initial costs of the breach.

---

## 4. Strategic Security Remediation

Terra Renewables must transition from a "policy-only" stance to strict technical enforcement.

1. **Mandatory Technical MFA (Preventive):** Enforce MFA across all remote, cloud, and privileged access accounts.
2. **Network Micro-segmentation (Preventive):** Restructure global architecture so compromised endpoints cannot reach critical operational networks or display infrastructure.
3. **Dual-Authorization & Segregation of Duties (Process):** Mandate that transfers above a defined monetary threshold require secondary digital sign-off and verbal confirmation via secondary channels.
4. **24/7 Managed SOC / SIEM Deployment (Detective):** Shift from manual monitoring to continuous 24/7 detection and real-time incident handling.

---

## 5. Cybersecurity Leadership Dashboard (KPIs)

| Metric | Description | Green (Target) | Amber (Warning) | Red (Critical) |
| :--- | :--- | :---: | :---: | :---: |
| **MFA Coverage** | % of remote/privileged accounts with active MFA | `100%` | `95–99%` | `<95%` |
| **MTTC** | Mean Time to Containment for active threats | `<60m` | `61–120m` | `>120m` |
| **Dual-Auth Compliance** | % of high-value payments following dual approval | `100%` | `98–99%` | `<98%` |
| **Data Leak Incidents** | Successful vs. Blocked exfiltration attempts | `0` | `1` | `>1` |
| **Training Completion** | % of staff completing social engineering labs | `>95%` | `80–94%` | `<80%` |

---

## 6. Crisis Communication & Awareness Framework

###  External Template: Customer Data Transparency
```text
To: [Customer Name]
Subject: Important Security Update Regarding Your Personal Information

Dear Valued Client,

At Terra Renewables, our mission to protect the environment includes safeguarding our community's data. 
We recently identified a security incident that may have involved some of your personal information. 
We have taken immediate action to secure our systems, including deploying 24/7 SOC monitoring and mandatory multi-factor authentication.

We are offering protective support services to all affected parties. We value your trust and remain committed to full transparency.

Sincerely,  
The Terra Renewables Leadership Team

```

###  Internal Template: The Human Firewall

```text
To: All Staff
Subject: Security Alert – Mandatory Social Media & Payment Protocols

Team,

Recent events demonstrate how a single social media post can expose global infrastructure. 
Effective immediately, the following policies are strictly enforced:

1. Zero Digital Footprint: Never post photos of your workstation, badges, or credentials online.
2. Dual-Authorization: No payment is urgent enough to bypass two-person approval and voice verification.
3. Universal MFA: MFA is now mandatory across all systems. Security is our shared responsibility.

```

---

## 7. Conclusion & Takeaways

The transformation of Terra Renewables from a vulnerable target to a resilient enterprise requires aligning technical controls with executive governance. By introducing continuous 24/7 monitoring, enforcing MFA at the technical level, and fostering a "Human Firewall" security culture, organizations can protect both their operational continuity and strategic reputation.

---

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para obtener más información.

*Disclaimer: This case study was developed for academic and portfolio demonstration purposes as part of the Cybersecurity Master's curriculum at Immune Technology Institute.*
