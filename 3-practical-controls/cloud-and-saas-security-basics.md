# Cloud and SaaS security basics

Many small and medium businesses now rely primarily on cloud and Software-as-a-Service (SaaS) platforms for email (like O365), file sharing, collaboration, CRM, HR, finance and more.

These services reduce the need to run your own servers, but **do not eliminate your security responsibilities**. You still need to configure them securely, manage access and monitor activity.

This document covers practical cloud and SaaS security basics for non‑specialists.

---

## 1. Shared responsibility (plain language)

Cloud and SaaS providers typically operate under a **shared responsibility** model:

- The **provider** is responsible for:
  - The security of the underlying infrastructure (data centres, hardware, core software).  
  - Many technical protections (for example, physical security, network segmentation, some default controls).

- **You** are responsible for:
  - How accounts, identities and permissions are managed.  
  - Which security features you enable or disable (for example, MFA, logging, data retention).  
  - What data you store and how you classify it.  
  - Which third‑party apps and integrations you approve.

In short: the provider secures **the platform**, you must secure **how your organization uses it**.

---

## 2. Inventory and identify your cloud services

First, understand which cloud and SaaS services your business uses:

- Core platforms:
  - Email and collaboration (for example, Microsoft 365, Google Workspace).  
  - File storage and sharing (for example, OneDrive, SharePoint, Google Drive, Box, Dropbox).  
  - CRM, ERP, HR, accounting, ticketing and other line‑of‑business SaaS.

- Supporting tools:
  - Identity and access management, password managers.  
  - Security and backup services.  
  - Vendor portals, payment systems and e‑commerce platforms.

Add these to your **asset inventory** with information such as:

- Data stored (customer, financial, HR, operational).  
- Criticality to operations.  
- Who owns the business relationship and configuration.

This inventory is the basis for prioritizing where to apply the controls in this document.

---

## 3. Identity, access and MFA in the cloud

Identity is usually the **first and most important layer** in cloud and SaaS security:

- **Strong authentication**
  - Enforce **MFA** for all users on core platforms (email, collaboration, key SaaS).  
  - Require stronger MFA (for example, authenticator apps or hardware keys) for admins and high‑risk roles.

- **Single sign-on (SSO)** (if available)
  - Where possible, integrate SaaS applications with a central identity provider (for example, Microsoft Entra ID / Azure AD, Google Identity).  
  - This allows you to enforce consistent policies (MFA, conditional access, password rules) and simplifies offboarding.

- **Role-based access**
  - Use built‑in roles and groups instead of granting individual permissions ad hoc.  
  - Apply **least privilege**: only give users access to the apps and data they need.

- **Account lifecycle (joiner–mover–leaver)**
  - When people join: assign them to the correct groups/roles.  
  - When roles change: remove old access as well as adding new.  
  - When people leave: disable or remove their accounts from central identity and key SaaS promptly.

---

## 4. Secure configuration of core SaaS platforms

Most cloud platforms include security settings that are **off by default** or need to be tuned. Key areas:

- **Security defaults / baseline policies**
  - Many providers (for example, Microsoft 365, Google Workspace) offer default security configurations.  
  - Review and enable appropriate defaults (for example, blocking legacy authentication, enforcing MFA, safe links/attachments).

- **Data sharing and external access**
  - Restrict public file sharing or linking, especially for folders that contain sensitive or internal data.  
  - Prefer sharing with specific people or groups instead of “anyone with the link”.  
  - For collaboration tools (Teams, SharePoint, Google Drive), define:
    - When external guests are allowed.  
    - How guest access is approved and reviewed.

- **Device and session controls**
  - If your platform supports it, configure:
    - Session timeouts and reauthentication requirements.  
    - Conditional access (for example, blocking logins from risky locations or unmanaged devices).  
    - Basic mobile device management for corporate phones and tablets.

- **Application and API access**
  - Review and control third‑party apps and integrations that access your cloud data via APIs or OAuth.  
  - Remove or disable apps that are not needed or not trusted.

Document key settings and decisions so you can review and update them later.

---

## 5. Backups and data retention for cloud services

Cloud does not automatically mean “no need for backups”. You still need to consider:

- **Native retention and recovery**
  - Understand what your SaaS provider offers:
    - Version history for files.  
    - Recycle bins and time‑limited restore.  
    - Built‑in backup or archive options.

- **Third‑party backups (if needed)**
  - For critical data (for example, email, SharePoint/Drive, CRM), consider:
    - Independent backup solutions that can restore data beyond standard retention.  
    - Especially important if accidental deletion, insider misuse or ransomware in sync’d folders is a concern.

- **Retention policies**
  - Define how long different types of data must be kept for:
    - Business needs.  
    - Legal or regulatory requirements.  
  - Configure retention policies in the SaaS platforms where supported.

Make sure cloud data is included in your overall **backup and data protection strategy**, not treated separately.

---

## 6. Logging, monitoring and alerts in the cloud

Most major SaaS platforms provide **audit logs** and **security alerts** – but they may not be enabled or retained by default:

- **Enable audit logs**
  - Turn on and retain logs for:
    - Sign‑ins and failed logins.  
    - Admin and configuration changes.  
    - File access and sharing changes (for sensitive repositories).

- **Security alerts**
  - Configure built‑in alerting for:
    - Suspicious logins (unusual locations, impossible travel).  
    - Mass download or deletion events.  
    - Changes to admin roles and configurations.

- **Centralize or at least consolidate**
  - Where feasible, send important cloud logs to:
    - A central logging platform, or  
    - Your managed service provider’s monitoring system.

- **Define who reviews alerts**
  - Assign responsibility (for example, IT lead or MSP) to review and act on security alerts from key SaaS services.

This directly supports your **logging and monitoring** and **incident response** controls.

---

## 7. Vendor risk and contracts for SaaS

Your SaaS providers are **critical vendors**. Apply the vendor and third‑party risk basics here:

- **Before choosing a provider**
  - Check:
    - Where data is stored (region/country).  
    - Which certifications or audits they hold (for example, SOC 2, ISO 27001).  
    - Their documentation on security, privacy and incident response.

- **In contracts**
  - Where possible, include:
    - Clauses about protecting your data and using it only for agreed purposes.  
    - Obligations to notify you promptly of security incidents.  
    - How data will be returned or deleted when you leave the service.

- **Ongoing**
  - Monitor for:
    - Major incidents or breaches reported in the news.  
    - Significant changes to terms of service or privacy policies.

Include SaaS providers in your **vendor inventory** and review them periodically based on risk.

---

## 8. User training for cloud and SaaS

Cloud and SaaS change **how** people work (for example, easier file sharing, remote access). Training should reflect that:

Key messages:

- Only store **business data** in approved cloud services, not in unapproved personal accounts.  
- Be careful with **sharing settings** (“anyone with the link” vs. specific people).  
- Log out of shared or public devices and do not save passwords in browsers on such devices.  
- Report unusual behavior (unexpected MFA prompts, login alerts, unknown devices) immediately.

Link this training to your `security-awareness-and-training.md` plan.

---

## 9. Minimal checklist for cloud and SaaS security basics

Use this checklist to assess your current state:

- [ ] We maintain an inventory of our main cloud and SaaS services, with owners and data stored.  
- [ ] MFA is enabled for all users on core platforms (email, collaboration, key SaaS) where technically possible.  
- [ ] Admin and privileged roles are limited and protected with strong MFA.  
- [ ] Basic secure configuration is applied (for example, restricted external sharing, blocked legacy auth, safe defaults).  
- [ ] Cloud data is covered by our backup and data retention strategy.  
- [ ] Audit logging is enabled and security alerts are reviewed by a designated person or provider.  
- [ ] SaaS providers are included in our vendor risk process, with basic due diligence and contractual expectations.  
- [ ] Staff receive training on safe use of cloud services and how to handle sharing and remote access.

Unchecked boxes highlight priorities for your next 3–12 months of cloud and SaaS security improvements.
