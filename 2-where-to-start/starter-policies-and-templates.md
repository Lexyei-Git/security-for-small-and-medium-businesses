# Starter policies and templates

This document provides **simple starter policy text** you can adapt for your organization.  
The goal is to give non‑security staff and managers clear, minimal rules that support the controls in this guide, without legal or technical jargon.

You should review and adapt these templates with your leadership and, where appropriate, legal counsel.

---

## 1. How to use these starter policies

- Treat them as **starting points**, not final legal documents.
- Replace placeholders like `[Company Name]` and `[Role/Owner]` with your details.  
- Keep policies **short and focused**, especially for small and medium businesses.  
- Publish them where staff can easily find them (intranet, shared drive, HR system).  
- Make sure onboarding includes a quick walkthrough of the key expectations.

---

## 2. Acceptable use – short policy

You can save this as `policies/acceptable-use-policy.md` or similar.

### 2.1 Purpose and scope

> This policy defines how employees and other authorized users may use `[Company Name]` devices, systems, networks and data.  
> It exists to protect the organization, our customers and our partners from misuse, data loss and security incidents.

**Applies to:** All employees, contractors, interns and other users with access to `[Company Name]` systems or data.

### 2.2 Core rules (plain language)

- Company devices and accounts are provided **for business use first**. Limited personal use is acceptable if it:
  - Does not interfere with work.  
  - Does not violate any law or company policy.  

- Users **must not**:
  - Install software or browser extensions without approval from `[IT / Security / System Owner]`.  
  - Disable or tamper with security settings (antivirus, firewall, updates, MFA).  
  - Use company systems for illegal activities or harassment.  
  - Store company data on personal cloud services or devices without approval.

- Users **must**:
  - Use strong, unique passwords or passphrases and enable MFA where required.  
  - Lock their screens when leaving devices unattended.  
  - Report lost or stolen devices and suspected security incidents immediately to `[Contact/Team]`.

---

## 3. Passwords and MFA – short policy

This complements `3-practical-controls/passwords-and-mfa.md`.

### 3.1 Purpose

> To ensure passwords and multi‑factor authentication (MFA) are used in a way that reduces the risk of account compromise.

### 3.2 Requirements

- Passwords for company accounts must:
  - Be at least **12 characters** long.  
  - Preferably be **passphrases** (several words) rather than short complex strings.  
  - Be **unique** and not reused on personal services (for example, social media, personal email).

- Users must not:
  - Share passwords with colleagues or third parties.  
  - Store passwords in plain text (for example, in documents, email, sticky notes).

- `[Company Name]` will:
  - Provide or approve a **password manager** for storing and sharing passwords securely where needed.  
  - Require **MFA** on email, remote access and other key systems whenever technically possible.  
  - Periodically review admin and privileged accounts.

- Users must:
  - Not approve unexpected MFA prompts. If in doubt, deny and report to `[Contact/Team]`.  

---

## 4. Backup and data protection – short policy

This supports `3-practical-controls/backups.md`.

### 4.1 Purpose

> To ensure critical data can be recovered after incidents and to define basic expectations for data protection.

### 4.2 Requirements

- `[Company Name]` will:
  - Identify critical systems and data that must be backed up.  
  - Run **regular backups** of those systems and data (at least daily or as defined by `[Owner]`).  
  - Store at least one backup copy **separate** from the main systems (for example, off‑site or in the cloud).  
  - Encrypt backups and restrict access to authorized personnel only.  
  - Test restores periodically to verify that backups work.

- Users must:
  - Save important work in approved locations (for example, company file shares or cloud storage), not only on local desktop folders.  
  - Not create their own unofficial backup copies in unapproved locations (for example, personal cloud accounts, unencrypted USB drives).

---

## 5. Email, internet and phishing – short policy

This complements `email-and-phishing.md` and `wifi-and-vpn.md`.[web:25][web:21]

### 5.1 Purpose

> To reduce the risk of phishing, malware and data leakage via email and internet use.

### 5.2 Requirements

- Users must:
  - Be cautious with unexpected emails, links and attachments.  
  - Not click on links or open attachments in suspicious messages.  
  - Verify unusual requests for payments or sensitive information using a trusted channel (for example, phone number on file).  
  - Report suspected phishing emails to `[Contact/Team]` using the agreed method (for example, forward to a specific address, use “Report phishing” button).

- Internet use on company devices must:
  - Be primarily for business purposes.  
  - Avoid visiting clearly inappropriate or high‑risk sites (for example, illegal content, untrusted download sites).  
  - Follow any additional content filtering or blocking in place.

- `[Company Name]` will:
  - Implement email and web protections (for example, spam filters, safe browsing, DNS filtering).  
  - Mark external messages clearly where supported by the email platform.

---

## 6. Incident reporting – short policy

A minimal incident reporting policy aligned with your controls.[web:21][web:236]

### 6.1 Purpose

> To ensure that potential security incidents are reported quickly so that `[Company Name]` can respond, limit damage and learn from them.

### 6.2 What to report

Users must promptly report:

- Suspected phishing emails they have clicked or responded to.  
- Lost or stolen company devices.  
- Suspicious logins or account activity (for example, unexpected password reset emails).  
- Systems that behave unusually (for example, frequent crashes, unknown software, pop‑ups).  
- Any situation where they believe data may have been seen or accessed by unauthorized people.

### 6.3 How to report

- Primary contact: `[security@company.com / IT helpdesk / Named role]`.  
- Backup contact: `[Manager / External provider contact]`.  

Reports should include:

- What was observed.  
- When it happened.  
- Which systems or accounts are involved.  
- Any actions already taken (for example, disconnected from Wi‑Fi).

The priority is **early reporting**, not perfect detail. Staff will not be punished for reporting honest mistakes.

---

## 7. Vendor and third‑party – short policy

This complements `vendor-and-third-party-risk-basics.md`.[web:188][web:192][web:198]

### 7.1 Purpose

> To ensure that third‑party services and vendors with access to `[Company Name]` systems or data are selected and managed with basic security in mind.

### 7.2 Requirements

- Staff must **not** engage new vendors that will:
  - Store or process customer, employee or sensitive business data, or  
  - Have remote or admin access to `[Company Name]` systems,

without approval from `[Owner/Team]`.

- For higher‑risk vendors, `[Owner/Team]` will:
  - Ask basic security questions (about MFA, data protection, incident response, certifications).  
  - Ensure contracts include appropriate data protection and incident notification clauses, where feasible.

- A simple record of approved vendors and their access must be maintained.

---

## 8. Minimal checklist for starter policies

Use this checklist to track implementation:

- [ ] We have an **acceptable use** policy published and explained to staff.  
- [ ] We have a **passwords and MFA** policy aligned with our technical controls.  
- [ ] We have a **backup and data protection** policy that defines expectations and responsibilities.  
- [ ] We have an **email, internet and phishing** policy that sets clear rules for staff behavior.  
- [ ] We have an **incident reporting** policy that tells staff what to report and how.  
- [ ] We have a basic **vendor and third‑party** policy for approving and tracking higher‑risk suppliers.  
- [ ] These policies are accessible to staff and included in onboarding.

You can later split these sections into separate policy documents if your organization grows or regulatory needs increase.
