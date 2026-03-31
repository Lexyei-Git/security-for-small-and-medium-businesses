# Passwords and multi-factor authentication (MFA)

Strong passwords and multi-factor authentication (MFA) are two of the most effective and affordable ways for small and medium businesses to reduce account compromise risk.

This document explains, in practical terms, how to set expectations for passwords, when and how to use MFA, and what non‑security staff should actually do.

---

## 1. Why passwords and MFA matter

Most attacks against small and medium businesses still involve stolen or guessed passwords.  
Attackers use phishing emails, password reuse from other breaches, or automated guessing to get into accounts.

Key points:

- A **strong, unique password or passphrase** makes it harder for attackers to guess or brute‑force an account.
- **MFA** adds an extra layer: even if the password is stolen, the attacker still needs a second factor (for example, code from an app or hardware key).
- For important accounts (email, admin accounts, finance, HR, remote access), MFA is now widely considered **mandatory**, not optional.

---

## 2. Basic terminology

- **Password** – a secret string you type to log in.  
- **Passphrase** – a longer secret made of several words, often easier to remember and stronger than a short complex password (for example, “quiet-river-orange-window”). 
- **Multi-factor authentication (MFA)** – logging in with **two or more different factors**:
  - Something you know (password or PIN)
  - Something you have (phone with authenticator app, hardware token)
  - Something you are (biometrics such as fingerprint or face)

Some services call it **two-factor authentication (2FA)** or **two-step verification**. Treat these as part of the same family: more than just a password.

---

## 3. Password / passphrase requirements for SMBs

You do not need complicated, hard‑to‑remember rules. Modern guidance focuses on **length and uniqueness**, not weird character combinations.

A reasonable, business‑friendly standard:

- **Length**
  - For normal business accounts: minimum **12 characters**.  
  - Prefer passphrases with **at least 4 words and 15+ characters** where possible.

- **Content**
  - Encourage passphrases or passwords that mix words, numbers and symbols **in a way that is easy for the user but hard to guess**.  
  - Examples of good patterns:
    - Several unrelated words joined by dashes or spaces.
    - Adding numbers or symbols in the middle or between words, not just at the end.

- **Uniqueness**
  - Never reuse passwords across different systems, especially not between work accounts and personal accounts.  
  - Do not reuse the same password for email, banking, cloud apps, VPN, or admin access.

- **Avoid obvious choices**
  - Do not use personal details that are easy to find (names, birthdays, company name, sports team) or common passwords (for example, “Password123!”, “Summer2025!”).

If your organization can screen passwords against known breach lists (via a password manager or identity platform), that is even better.

---

## 4. Using a password manager

For teams with many systems, using a **business‑grade password manager** is often the simplest way to manage password complexity and uniqueness.

Benefits:

- Stores passwords in an encrypted vault so users do not need to remember each one.  
- Generates strong, random passwords for each account.  
- Supports secure sharing when multiple people need access to the same credential.  
- Often integrates with MFA and provides admin controls and reporting.

High‑level expectations:

- Each user has their own vault and master credential (protected by MFA).  
- Shared passwords are shared through the manager, **not** by email, chat or spreadsheets.  
- Administrators can revoke access when people leave the company.

---

## 5. Where to require MFA

For a small or medium business, a good default is:

> Turn on MFA **everywhere it is available**, starting with the most sensitive and critical accounts.

Priority order:

1. **Email and identity platform**
   - Company email accounts (for example, Microsoft 365, Google Workspace).  
   - Identity providers or single sign‑on (SSO) platforms.

2. **Administrator and privileged accounts**
   - System administrators, cloud admins, domain admins, IT support accounts.  
   - Any account that can create users, change security settings or access many systems.

3. **Financial and highly sensitive systems**
   - Online banking and payment systems.  
   - Accounting/ERP, payroll, HR, and systems containing sensitive personal or financial data.

4. **Remote access**
   - VPN, remote desktop gateways, remote management tools.

5. **Other business‑critical cloud services**
   - Project management tools, CRM, ticketing systems and any SaaS platform that would significantly impact operations if compromised.

If a service does not offer MFA, consider whether you can replace it with one that does.

---

## 6. Types of MFA factors (practical view)

Common options:

- **Authenticator apps** (recommended default)
  - Apps like Microsoft Authenticator, Google Authenticator, Authy.  
  - Generate one‑time codes that refresh every 30 seconds.  
  - More secure than SMS, generally easy to deploy.

- **Push notifications**
  - The service sends a prompt to an app on your phone asking you to approve or deny the login.  
  - Very convenient, but you must train users **not to approve unexpected prompts**.

- **SMS or phone calls**
  - One‑time codes sent by text message or voice call.  
  - Better than password‑only, but easier to intercept or abuse than app‑based codes. 
  - Acceptable as a starting point if no better option is available, but plan to move toward stronger methods.

- **Hardware security keys**
  - Physical keys (for example, FIDO2/U2F keys like YubiKey).  
  - Very strong security, recommended for administrators and high‑risk users.

Choose a mix that fits:

- Authenticator apps for most employees.  
- Hardware keys for admins and very sensitive roles.  
- SMS as a temporary option when no better factor is available.

---

## 7. Simple user guidance (what to tell staff)

Users do not need to understand the full technical details. You can provide something like:

- Use **a long, unique passphrase** for your main work account.  
- Do **not reuse** your work password on any personal website or service.  
- Enable MFA on your work account and on personal accounts that matter (email, banking, cloud storage, social media).  
- Never approve an MFA push notification you did not initiate. If you see unexpected prompts, report them immediately.  
- Do not share passwords with colleagues. If you must share access, use approved tools (such as a password manager or group account managed by IT).

---

## 8. Administrative practices and policies

From an administrative perspective, consider defining:

- **Password and MFA policy**
  - Minimum length, passphrase recommendation, when MFA is required, and approved MFA methods.  
  - Clear statement that password reuse is not allowed between major systems.

- **Onboarding**
  - New users receive:
    - Instructions on creating a strong passphrase.  
    - Immediate activation of MFA on their primary account.  
    - Access to the password manager (if used) with a short how‑to guide.

- **Offboarding**
  - When someone leaves:
    - Disable or remove their accounts.  
    - Revoke access in the password manager and shared vaults.  
    - Rotate shared secrets that they might have known.

- **Monitoring and review**
  - Periodic review of admin and privileged accounts.  
  - Ensure MFA is still enabled and functioning.  
  - Check for accounts that no longer need elevated access.

---

## 9. Minimal checklist for passwords and MFA

Use this checklist as a quick status check:

- [ ] We have a documented expectation for password/passphrase length and uniqueness.  
- [ ] Users are encouraged to use long passphrases instead of short complex passwords.  
- [ ] We strongly discourage password reuse, especially between work and personal accounts.  
- [ ] We use a business‑grade password manager (or have a clear plan to introduce one).  
- [ ] MFA is enabled for:
  - [ ] Email and identity/SSO  
  - [ ] Administrator and privileged accounts  
  - [ ] Financial and highly sensitive systems  
  - [ ] Remote access (VPN, remote desktop)  

- [ ] We use stronger MFA methods (authenticator apps or hardware keys) where possible.  
- [ ] Staff receive simple, written guidance on passwords and MFA during onboarding.  
- [ ] We have a basic process to remove access and update shared credentials when staff leave.

If several boxes are unchecked, use this list to prioritize improvements over the next 30–90 days.
