# Basic principles of information security

This document explains the core principles of information security in plain language so that non‑security staff can understand **what we are trying to protect** and **how the technical controls in this guide fit together**.

The goal is not to turn readers into experts, but to give them a clear mental model they can use in daily decisions.

---

## 1. The CIA triad: confidentiality, integrity and availability

Information security is often summarized by three core principles, known as the **CIA triad**:

- **Confidentiality** – keeping information private and accessible only to people who are allowed to see it.  
- **Integrity** – keeping information accurate, complete and not secretly changed.  
- **Availability** – making sure information and systems are accessible when authorized people need them.

You can think of them as:

- **Privacy** (confidentiality)  
- **Correctness** (integrity)  
- **Uptime and access** (availability)

Most security decisions are about balancing these three ideas.

---

## 2. Confidentiality (keeping information private)

**Confidentiality** means only the right people can access sensitive information.

Examples of information that often requires confidentiality:

- Customer data (names, contact details, IDs, purchase history)  
- Financial data (bank accounts, payment information, payroll)  
- Employee data (HR files, performance reviews, health information)  
- Business plans (pricing, contracts, designs, strategy)

Loss of confidentiality can lead to:

- Privacy breaches and regulatory issues.  
- Fraud or identity theft.  
- Loss of customer trust and reputational damage.

Typical controls that protect confidentiality:

- Strong passwords and multi‑factor authentication.  
- Access control and least privilege.  
- Encryption (for data stored and data in transit).  
- Physical security (locked rooms, cabinets, secure disposal).  
- Vendor and third‑party risk management.

---

## 3. Integrity (keeping information accurate and trustworthy)

**Integrity** means information remains correct, complete and unchanged except by authorized actions.

If integrity is lost:

- Financial records may be wrong.  
- Orders, inventory or production plans may be inaccurate.  
- Audit trails and logs may no longer be reliable.

Examples:

- An attacker modifies an invoice to change the destination bank account.  
- A misconfiguration or bug corrupts important database records.  
- A user accidentally overwrites an important file with outdated information.

Controls that support integrity include:

- Access control and change approval processes.  
- Logging and monitoring of important changes.  
- Backups and versioning so data can be restored.  
- Input validation and basic data quality checks.  
- Separation of duties for critical activities (for example, payment approvals).

---

## 4. Availability (keeping systems and data usable)

**Availability** means systems and data are accessible to authorized users when needed.

Loss of availability can come from:

- Ransomware encrypting your files.  
- Hardware failures or power outages.  
- Network or internet connectivity problems.  
- Human error (accidentally deleting key resources).

Availability is especially important for:

- Customer‑facing systems (websites, e‑commerce, portals).  
- Internal systems used to run daily operations (ERP, CRM, email, collaboration tools).  
- Communications channels needed during incidents.

Controls that support availability:

- Reliable backups and tested restore procedures.  
- Patching and secure configuration to reduce the chance of outages.  
- Redundancy for critical components where appropriate.  
- Monitoring and alerting for failures and performance issues.  
- Business continuity and disaster recovery planning.

---

## 5. Other useful principles: least privilege and defense in depth

In addition to the CIA triad, two practical principles help guide day‑to‑day decisions:

### 5.1 Least privilege

**Least privilege** means giving people and systems only the access they need to do their jobs, and no more.

Benefits:

- Reduces the impact if an account is compromised.  
- Limits accidental damage.  
- Makes it easier to explain and justify access to auditors and customers.

You already see least privilege in controls such as:

- Unique user accounts, not shared logins.  
- Role‑based access control (RBAC) and account management.  
- Segmentation between networks and environments.

### 5.2 Defense in depth

**Defense in depth** means using multiple layers of controls so that if one fails, others still provide protection.

Examples:

- Even if a phishing email passes the spam filter, strong passwords and MFA can still protect the account.  
- Even if malware gets onto a device, endpoint protection, secure configuration and limited privileges can reduce impact.  
- Even if a system is compromised, backups and recovery plans can restore operations.

This repository is structured with this in mind: no single control is “magic”; value comes from **several simple controls working together**.

---

## 6. How these principles connect to the rest of the guide

You can use these principles as a lens for the other documents in this repository:

- **Confidentiality**
  - Passwords and MFA, access control basics, Wi‑Fi and VPN, vendor and third‑party risk, physical security, data protection and encryption.

- **Integrity**
  - Patching and updates, device hardening and configuration, logging and monitoring, change management, backups and versioning.

- **Availability**
  - Backups and recovery, patching and secure configuration, endpoint protection, network and power resilience, incident response and business continuity.

When you design or review any control, you can ask:

1. Does this help protect **confidentiality**, **integrity** or **availability** (or more than one)?  
2. Are we applying **least privilege** and **defense in depth** where it makes sense for our size and risk?

This simple mental model makes it easier for non‑security analysts and managers to understand **why** each control exists and how it supports the bigger picture of protecting the business.
