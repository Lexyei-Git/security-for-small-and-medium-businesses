# Privacy and data protection overview

This document explains, in plain language, how **information security** relates to **privacy and data protection laws** such as GDPR (EU/EEA), LGPD (Brazil) and PIPEDA/Canadian privacy laws.

It is not legal advice. The goal is to help non‑security staff understand the big picture and know when to seek specialist or legal support.

---

## 1. Security vs. privacy: how they relate

- **Information security** focuses on protecting the **confidentiality, integrity and availability** of information and systems.  
- **Privacy and data protection** focus on **how personal data is collected, used, shared and retained**, and on individuals’ rights over their data.

You can think of it this way:

- Security is about **“can someone break in or cause damage?”**  
- Privacy is about **“are we allowed to collect and use this personal data, and are we doing it fairly and transparently?”**

Good security is **necessary** for privacy compliance, but not **sufficient**:

- You can have strong security and still break privacy rules if you collect data you do not need, keep it too long, or use it for purposes you never explained.  
- You cannot have good privacy without basic security: laws expect you to protect personal data with appropriate technical and organizational measures.

---

## 2. What is “personal data” or “personal information”?

Most data protection laws define **personal data / personal information** broadly:

- Any information relating to an **identified or identifiable person**, such as:
  - Name, email address, phone number, identification numbers.  
  - Online identifiers (for example, IP address, cookies, device IDs) when they can be linked to a person.  
  - Location data, photos, recordings, customer IDs.

Many laws also define **sensitive** or **special category** data, such as:

- Health information, racial or ethnic origin, religious beliefs, political opinions.  
- Financial data, biometric data, sexual life or orientation, union membership.

Handling personal data almost always brings **privacy obligations**, even for small businesses.

---

## 3. Examples of key laws that may affect SMBs

Depending on where you operate and whose data you handle, different laws may apply:

- **GDPR (European Union / EEA)**  
  - Applies when you offer goods or services to people in the EU/EEA or monitor their behavior, regardless of where your business is based.  
  - No exemption just because you are a small business.

- **LGPD (Brazil)**  
  - Applies to processing of personal data in Brazil or about individuals located in Brazil, including by foreign organizations offering goods or services there.

- **PIPEDA and provincial privacy laws (Canada)**  
  - PIPEDA applies to many private‑sector organizations in Canada that collect, use or disclose personal information in the course of commercial activities.  
  - Some provinces (for example, Quebec’s Law 25) have additional or “substantially similar” laws.

Other countries and regions have their own frameworks. If your business is online, you may be subject to multiple regimes at once.

For this guide, the important point is: **if you handle customer or employee personal data, you likely have legal privacy obligations**, even as a small business.

---

## 4. Common privacy principles (simplified)

Although the details differ, many privacy laws share similar **core principles**:

- **Lawfulness, fairness and transparency**
  - You must have a legal basis for processing personal data (for example, contract, legal obligation, legitimate interests, consent).  
  - You must be open and honest about what you do with the data (clear privacy notices).

- **Purpose limitation**
  - Collect data for **specific, explicit and legitimate purposes**.  
  - Do not use it later for unrelated purposes without a proper legal basis or new consent.

- **Data minimization / necessity**
  - Collect only the data you **actually need** for the stated purposes.  
  - Avoid “just in case” data hoarding.

- **Accuracy / data quality**
  - Keep personal data **accurate and up to date** where necessary.

- **Storage limitation**
  - Do not keep personal data longer than needed for the purpose, legal or contractual requirements.

- **Security and prevention**
  - Protect personal data with **appropriate technical and organizational measures** against unauthorized access, alteration, loss or destruction.

- **Accountability**
  - Be able to **demonstrate** that you follow these principles (for example, policies, records, training, DPIAs where required).

These principles should guide both your **security controls** and your **business processes** involving personal data.

---

## 5. How security in this guide supports privacy compliance

The controls and processes in this repository are not a full privacy compliance program, but they strongly support it:

- **Asset inventory and risk assessment**
  - Help you understand where personal data lives, who uses it and what risks exist.

- **Access control, passwords and MFA, least privilege**
  - Reduce the chance that unauthorized people access personal data.

- **Backups and data recovery**
  - Help you meet obligations to keep data available and recoverable after incidents.

- **Logging, monitoring and incident response**
  - Support breach detection, investigation and notification processes.

- **Vendor and third‑party risk management**
  - Align with requirements to ensure processors and service providers protect data properly (for example, Data Processing Agreements under GDPR).

- **Security awareness and training**
  - Reinforce staff responsibilities in handling personal data and reporting potential breaches.

Privacy laws generally **expect** this kind of security hygiene as a baseline.

---

## 6. Typical additional privacy tasks beyond security

To comply with laws like GDPR, LGPD or PIPEDA, you usually need to do **more than security**:

Examples (high‑level, not exhaustive):

- **Maintain a record of processing activities** (what personal data you process, why, where it is stored, who you share it with).  
- **Create and publish a clear privacy notice/policy** explaining:
  - What data you collect and why.  
  - Legal bases (for example, consent, contract).  
  - How long you keep data.  
  - Rights that individuals have and how they can exercise them.

- **Manage individual rights requests**, such as:
  - Access to their data.  
  - Correction of inaccurate data.  
  - Deletion, where appropriate.  
  - Objection to certain processing.

- **Sign Data Processing Agreements (DPAs)** with vendors that handle personal data on your behalf.

- **Appoint a Privacy Officer / DPO or contact point**, where required by law, and document privacy governance.

- **Define and follow a process for privacy breaches**, including notifying regulators and affected individuals where required and within deadlines.

This guide focuses on **security‑related foundations**. For specific legal obligations, you should consult your legal advisor or privacy specialist.

---

## 7. When to ask for help

As a small or medium business, you do not need to solve everything alone, but you must know when to ask for help.

Situations where you should consider consulting **legal or privacy experts** in addition to using this guide:

- You handle **large volumes of personal data** or sensitive categories (for example, health, financial, children’s data).  
- You operate in or serve customers in multiple jurisdictions (for example, EU, Brazil, Canada, US) and are unsure which laws apply.  
- You are planning a **new product, app or data‑driven service** that collects or analyzes personal data.  
- You suffered or suspect a **data breach** involving personal data and need to know your notification obligations.  
- You receive complex data subject requests (for example, broad access or deletion requests) and are unsure how to respond.

Security improvements from this repository will **reduce your risk** and support compliance, but they do not replace tailored legal advice.

---

## 8. Minimal checklist: privacy awareness for non‑specialists

This is a basic checklist (not a legal compliance checklist) for managers and non‑security staff:

- [ ] We know which systems and processes handle **personal data** (customers, employees, others).  
- [ ] We have at least one **public privacy notice/policy** explaining, in simple language, what we do with personal data.  
- [ ] We apply the principles of **data minimization**, **purpose limitation** and **storage limitation** when designing processes.  
- [ ] We have **security controls** in place to protect personal data (MFA, access control, backups, logging, vendor management, incident response).  
- [ ] We know **who** is responsible for privacy and who to contact for questions (internal or external).  
- [ ] We have a basic process for dealing with **data breaches** involving personal data (even if it is part of our general incident response).

If several boxes are unchecked, treat this as a sign that you should:

- Use the rest of this security guide to strengthen your foundation, and  
- Engage legal or privacy expertise to design a fuller privacy compliance approach for your organization.
