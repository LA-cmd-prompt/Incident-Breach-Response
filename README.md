# Incident-Breach-Response
Incident &amp; Breach Response
# Breach Response Playbook – HealthTrack App

##  Purpose
This playbook outlines how HealthTrack will respond to a **personal data breach** in compliance with **PIPEDA** and global best practices.  

A data breach may involve unauthorized access, disclosure, loss, or misuse of personal information (e.g., email addresses, health logs, location data).

---

##  Guiding Principles
- **Timeliness:** Respond quickly — PIPEDA requires notification "as soon as feasible."  
- **Transparency:** Communicate openly with affected individuals and regulators.  
- **Accountability:** Assign clear roles and responsibilities.  
- **Mitigation:** Contain, assess, and prevent recurrence.  

---

##  Step-by-Step Response Process

### 1. Detection & Reporting
- All staff trained to **report suspicious activity immediately**.  
- Centralized reporting channel: `privacy@healthtrack.ca`.  
- Log the incident in the **Breach Register**.  

---

### 2. Initial Containment
- IT team isolates affected systems.  
- Disable compromised accounts/access.  
- Stop further unauthorized use or disclosure.  

---

### 3. Assessment & Risk Evaluation
- **What happened?** (e.g., phishing attack, lost device, ransomware).  
- **What data is involved?** (sensitive health logs vs. email only).  
- **Who is affected?** (one user, a group, or entire customer base).  
- **Likelihood of harm?** (identity theft, embarrassment, financial loss).  

 Tool: Use **Risk Matrix** (included in repo) to classify breach as **Low / Medium / High severity**.  

---

### 4. [Notification Obligations](https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/incidence_3.jpeg)
#### Under PIPEDA:
- Report breach to the **Office of the Privacy Commissioner of Canada (OPC)** if it poses a “real risk of significant harm.”  
- Notify **affected individuals** directly (email, in-app notification).  
- Notify **third parties** who can help mitigate harm (e.g., banks, law enforcement).  
- Maintain **records of all breaches** for at least 24 months, even if not reported.  

 Global Note:  
- GDPR: notify supervisory authority within **72 hours**.  
- U.S. State Laws: notification timelines vary (often 30–60 days).  

---

### 5. Communication Templates
- **User Notification Email Example:**  

  > Subject: Important Notice – Security Incident  
  >  
  > Dear [User],  
  >  
  > We are writing to inform you of a recent incident that may have involved your personal data (steps, calorie logs, email).  
  >  
  > What happened: [Plain-language description]  
  >  
  > What we are doing: [Containment & mitigation steps]  
  >  
  > What you can do: [Change password, enable 2FA, monitor accounts]  
  >  
  > We take your privacy seriously and will provide updates.  
  >  
  > – The HealthTrack Privacy Team  

---

### 6. Post-Incident Remediation
- Conduct **root cause analysis** (e.g., patch vulnerabilities, improve training).  
- Update security controls (multi-factor authentication, encryption upgrades).  
- Review and update **incident response plan**.  
- Conduct **tabletop exercise** within 3 months.  

---

##  Roles & Responsibilities
- **Privacy Officer:** Leads investigation, decides if reportable under PIPEDA (RROSH)
- **IT Security Team:** Containment, forensic analysis, system hardening.  
- **Communications Team:** Drafts and sends notifications.  
- **Legal/Compliance:** Reviews obligations across jurisdictions.  
- **Executive Sponsor:** Approves public disclosures.  

---

##  Supporting Deliverables
 
- **`risk-scoring matrix.xlsx`** → [Risk scoring scoring template](https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/breach-risk-matrix.xlsx) 

A practical, visual guide to evaluating **data breach severity** and identifying when notification is required under **Canadian (PIPEDA)** and **EU (GDPR)** law.

This README replaces an interactive calculator with a clean, human-readable visual layout that still demonstrates your ability to **score risk**, **document incidents**, and **recommend actions**.

---

## Risk Scoring Framework

| **Category** | **Factor** | **Weight / Score Impact** |
|---------------|-------------|----------------------------|
| **Data Type Affected** | Financial, Health, Biometric | +25 each |
|  | Credentials, Children’s Data | +20 each |
|  | Employment Data | +15 |
|  | Location Data | +10 |
|  | Basic Contact Info | +5 |
| **Volume of Records** | Low (&lt;100) | +5 |
|  | Medium (100–1,000) | +10 |
|  | High (1,000–100,000) | +20 |
|  | Massive (&gt;100,000) | +30 |
| **Sensitivity of Data** | Low | +5 |
|  | Medium | +10 |
|  | High | +15 |
| **Controls / Context** | No encryption | +15 |
|  | Third-party processor involved | +10 |
|  | Public exposure (online leak) | +20 |

---

##  Score Calculation

**Formula:**
Total Risk Score = Σ(Data Type Scores) + Volume + Sensitivity + Control Factors

**Example:**
- Financial + Health + Medium Volume + High Sensitivity + No Encryption  
= 25 + 25 + 10 + 15 + 15 = **90**

🟩 **Minimal** (0–19) | 🟦 **Low** (20–39) | 🟨 **Medium** (40–59) | 🟧 **High** (60–79) | 🟥 **Critical** (80–100)

---

## Risk Level Legend

| **Risk Level** | **Score Range** | **Color** | **Meaning** | **Action Guidance** |
|----------------|----------------|------------|--------------|----------------------|
| 🟩 Minimal | 0–19 | Green | Insignificant privacy impact | Internal record only |
| 🟦 Low | 20–39 | Blue | Limited scope / contained | Document, no external notification |
| 🟨 Medium | 40–59 | Yellow | Possible individual impact | Review mitigation, consider follow-up |
| 🟧 High | 60–79 | Orange | Significant exposure | Notify Privacy Officer & assess for regulator notice |
| 🟥 Critical | 80–100 | Red | Severe or widespread harm | Mandatory regulator + individual notification |

---

## Notification Guidance

### 🇨🇦 Canada (PIPEDA)

| **Risk Level** | **Regulatory Action** |
|----------------|-----------------------|
| Minimal / Low | Record internally; assess risk of significant harm |
| Medium | Consider notification if harm cannot be fully mitigated |
| High / Critical | **Mandatory:** Notify Privacy Commissioner of Canada & affected individuals “as soon as feasible” |

### 🇪🇺 European Union (GDPR)

| **Risk Level** | **Regulatory Action** |
|----------------|-----------------------|
| Minimal / Low | Record in internal breach register |
| Medium | Notify supervisory authority **within 72 hours** (if personal data compromised) |
| High / Critical | Notify both **authority** and **data subjects**; regulatory inquiry may follow |

---

## Example: Sample Assessment

| **Factor** | **Selection** | **Score** |
|-------------|----------------|-----------|
| Data Types | Health + Credentials | 45 |
| Volume | Medium | 10 |
| Sensitivity | High | 15 |
| Encryption | No | 15 |
| Third Party | Yes | 10 |
| Public Exposure | No | 0 |
| **Total** |  | **95 / 100 (Critical)** |

> **Result:** 🟥 **Critical Severity**  
> - **Notify OPC and affected individuals immediately**  
> - **Document containment measures and mitigation steps**  
> - **Review breach response policy for procedural updates**

---

##  Visual Summary

| Likelihood → / Impact ↓ | 1 (Low) | 2 | 3 | 4 | 5 (Severe) |
|--------------------------|----------|---|---|---|--------------|
| **5 (Severe)** | 🟥 Critical | 🟥 Critical | 🟥 High | 🟧 High | 🟨 Medium |
| **4 (Major)** | 🟥 High | 🟧 High | 🟧 Medium | 🟨 Medium | 🟦 Low |
| **3 (Moderate)** | 🟧 Medium | 🟨 Medium | 🟨 Medium | 🟦 Low | 🟩 Minimal |
| **2 (Minor)** | 🟦 Low | 🟩 Minimal | 🟩 Minimal | 🟩 Minimal | 🟩 Minimal |
| **1 (Negligible)** | 🟩 Minimal | 🟩 Minimal | 🟩 Minimal | 🟩 Minimal | 🟩 Minimal |

---

## Related Files in This Repository

---

## ✉️ Example Notification Structure - **`user-notification`** → Pre-drafted communication

| **Section** | **Description** | **Sample Snippet** |
|--------------|-----------------|--------------------|
| **1. Introduction** | Explain the context and purpose of the message | “We are writing to inform you of a recent incident involving your personal information.” |
| **2. What Happened** | Brief, factual summary of the breach | “On October 22, 2025, an email containing client contact details was inadvertently sent to an unauthorized recipient.” |
| **3. Information Involved** | Identify affected data types | “The information included your name and email address. No financial or health information was exposed.” |
| **4. Steps Taken** | Describe remediation & containment | “We immediately recalled the email, secured the system, and initiated a privacy investigation.” |
| **5. Recommended Actions** | Guide the user on next steps | “We recommend you remain vigilant for suspicious emails and avoid sharing personal details with unknown senders.” |
| **6. Contact Details** | Provide a direct contact channel | “If you have questions, please contact privacy@company.ca.” |
| **7. Regulatory Statement (if applicable)** | Demonstrate compliance | “This notification is provided in accordance with the Personal Information Protection and Electronic Documents Act (PIPEDA).” |

---

##  Best Practices for Privacy-Compliant Communication

 **Be Transparent:** Provide accurate facts — avoid speculation.  
 **Be Prompt:** Notify “as soon as feasible” under PIPEDA.  
 **Be Reassuring:** Outline mitigation steps to build trust.  
 **Be Consistent:** Align public statements, user notices, and regulator reports.  
 **Be Accessible:** Use plain language; avoid legal jargon.  

 # 📨 User Notification Template  
**Version:** 1.0  
**Prepared by:** [Your Name], Privacy Compliance Professional  
**Jurisdiction(s):** Canada (PIPEDA) | EU (GDPR)  
**Last Updated:** October 2025  

---

## 📋 Purpose

This document provides **pre-drafted notification messages** to be sent to affected individuals following a confirmed privacy incident or data breach.  
It ensures compliance with:
- 🇨🇦 **Personal Information Protection and Electronic Documents Act (PIPEDA)**
- 🇪🇺 **General Data Protection Regulation (GDPR)**, Articles 33–34

Each template follows the **“plain-language principle”** — making sure the message is **understandable, transparent, and actionable**.

---

## 🧾 Template 1: Standard User Notification (PIPEDA-Compliant)

**Subject:** Notice of Privacy Incident – [Organization Name]  

**Body:**

Dear [First Name],

We are writing to inform you of a recent privacy incident involving your personal information.

### What Happened
On [Date], we identified an incident where [brief factual summary – e.g., “an email containing client contact details was inadvertently sent to an unintended recipient”].  
The issue was detected on [Detection Date] and contained on [Containment Date].

### What Information Was Involved
Based on our investigation, the information involved includes:
- [e.g., Full name, business email address, and contact phone number]  
No financial, health, or password data were affected.

### What We Are Doing
We immediately:
- Contained the incident and secured our systems  
- Conducted an internal privacy investigation  
- Implemented additional safeguards to prevent reoccurrence

### What You Can Do
At this time, we recommend:
- Remaining alert to any suspicious emails or communications  
- Avoiding the sharing of personal information with unverified sources

### Our Commitment
We take privacy very seriously and are committed to maintaining the trust you place in us.  
If you have any questions or would like more information, please contact our Privacy Office:

📧 **privacy@company.ca**  
📞 **1-800-XXX-XXXX**

Sincerely,  
**[Name]**  
Privacy Officer  
[Organization Name]  

---

## Template 2: High-Risk / Regulatory Notification (PIPEDA + GDPR Aligned)

**Subject:** Important: Data Breach Notification – Immediate Action Recommended  

**Body:**

Dear [First Name],

We are contacting you to inform you of a data breach that may involve your personal information.  
Transparency and accountability are key parts of our privacy commitments.

### What Happened
On [Date], unauthorized access was detected in our [system/platform].  
The breach was contained on [Containment Date], and an investigation is underway.

### What Information Was Involved
The affected information may include:
- [Data categories, e.g., “financial account details, transaction history, and government-issued ID numbers”]

### What We Have Done
We have:
- Contained the breach and disabled the affected system  
- Informed the **Office of the Privacy Commissioner of Canada (OPC)**  
- Notified relevant **EU supervisory authorities** (if applicable)  
- Implemented multi-factor authentication and encryption across all accounts  

### What You Should Do
To protect your information:
- Change your account passwords immediately  
- Monitor your accounts for unusual activity  
- Consider placing fraud alerts with major credit bureaus  
- Contact us directly if you notice any suspicious activity  

### Contact Information
📧 **privacy@company.ca**  
📞 **1-800-XXX-XXXX**  
🌐 [Privacy Incident FAQ Page – optional]

### Regulatory Note
This notice is provided in accordance with:
- **PIPEDA** – Notification to individuals under s.10.1(6)  
- **GDPR** – Articles 33 & 34, requiring timely notice to data subjects and supervisory authorities  

We regret any inconvenience this incident may cause and appreciate your understanding as we work to enhance our privacy safeguards.

Sincerely,  
**[Name]**  
Chief Privacy Officer  
[Organization Name]  

---

## Internal Use Only – Privacy Team Notes

| **Field** | **Entry** |
|------------|------------|
| Incident ID | [e.g., INC-2025-002] |
| Risk Score (from breach matrix) | [e.g., 85 – Critical] |
| Date Notified | [YYYY-MM-DD] |
| Notification Type | [Standard / High-Risk / Regulator] |
| Prepared By | [Your Name] |
| Approved By | [Manager / CPO] |
| Review Date | [YYYY-MM-DD] |

---
---

**Incident response process visual:**
 
- **`flow-diagram.png`** →.  
<figure style="text-align:center">
  <img src="https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/step%201.jpeg" width="800" 
    <figure style="text-align:center">
  <img src="https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/step%202.jpeg" width="800" 
    <figure style="text-align:center">
  <img src="https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/step%203.jpeg" width="800" 
    <figure style="text-align:center">
  <img src="https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/step%204.jpeg" width="800" 
    <figure style="text-align:center">
  <img src="https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/step%205.jpeg" width="800" 
    <figure style="text-align:center">
  <img src="https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/step%206.jpeg" width="800" 
   <figure style="text-align:center">
  <img src="https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/step%207.jpeg" width="800" 
   <figure style="text-align:center">
  <img src="https://github.com/LA-cmd-prompt/images-.gitkeep/blob/main/step%208.jpeg" width="800" 
---

##  Key Takeaways
- A breach is not just an IT problem — it’s a **privacy + compliance issue**.  
- Clear **roles, documentation, and communication** prevent chaos.  
- Meeting **PIPEDA requirements** builds trust with users and regulators.  

---

⚡ Built as part of the HealthTrack Privacy Portfolio by [LA-cmd-prompt](https://github.com/LA-cmd-prompt).
### Facilitated by: [Lola]  
**Privacy Compliance Professional**  
_Specializing in Privacy Incident Response & Data Subject Communication_  

