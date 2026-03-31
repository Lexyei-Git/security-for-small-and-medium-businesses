# Access control basics

Access control is about making sure that only the right people, using the right accounts, can access the right systems and data – and only to the extent they need for their work.

For small and medium businesses, good access control does not need to be complex. It is mainly about clear roles, unique accounts, limited privileges and proper removal of access when people leave or change roles.

---

## 1. Key ideas in simple terms

There are a few core ideas that matter most:

- **Least privilege**
  - Each person should have only the access required to perform their job, and nothing more.

- **Unique user accounts**
  - Everyone should have their own account; shared generic accounts should be rare and tightly controlled.

- **Account lifecycle**
  - Access should be granted when someone joins, adjusted when roles change and removed when they leave (the “joiner–mover–leaver” lifecycle).

- **Stronger control for admin access**
  - Administrator or privileged accounts need extra protection and should not be used for everyday activities like email or web browsing.

These concepts apply to on‑premises systems, cloud services and third‑party platforms.

---

## 2. Least privilege (just enough access)

The **principle of least privilege** means giving each user, vendor or application only the permissions they need to do their work – nothing more.

In practice for SMBs:

- Default access should be **minimal**. New users start with only what their role requires.  
- Extra access should be **approved and time‑bound** where possible (for example, temporary elevated access for a project or an incident).  
- Access should be **reviewed periodically** to remove permissions that are no longer needed.

Benefits:

- Limits the impact if an account is compromised (attackers cannot automatically reach everything).  
- Reduces the chance of accidental damage or exposure by well‑intentioned staff.  
- Helps with compliance and customer trust by restricting who can see sensitive data.

---

## 3. Unique accounts and reducing shared logins

Unique user accounts create accountability: you can see who did what, and revoke access for specific individuals when needed.

Basic expectations:

- Each employee, contractor or vendor with access to your systems should have their **own** login.  
- Avoid generic shared accounts such as “admin”, “finance”, “sales” or “reception”, except where absolutely necessary.  
- If a shared account is unavoidable (for example, a shared kiosk), protect it with:
  - Strong credentials and MFA where possible.  
  - Restricted scope (limited systems and data).  
  - Clear rules about who may use it and when.

Where software supports it, use **named accounts with roles** instead of sharing passwords.

---

## 4. Joiner–mover–leaver (JML) lifecycle

The **joiner–mover–leaver (JML) process** is a simple way to think about access throughout a person’s time with the organization:

- **Joiner** – a new person joins (employee, contractor, vendor).
  - Create accounts.  
  - Assign access based on their role (for example, “Sales”, “Finance”, “Support”).  
  - Ensure they receive guidance on acceptable use and security expectations.

- **Mover** – the person changes role, team or responsibilities.
  - Add access needed for the new role.  
  - Remove access that is no longer needed from the old role (to avoid privilege accumulation).

- **Leaver** – the person leaves the organization or no longer needs access.
  - Disable or delete accounts promptly.  
  - Revoke access from cloud services, VPN, email, line‑of‑business apps.  
  - Recover or wipe company devices where applicable.

For small and medium businesses, you can track JML with:

- A simple checklist linked to HR processes (for example, when HR creates or closes a record).  
- A shared list or ticketing system where account changes are requested and recorded.

---

## 5. Admin and privileged accounts

Privileged accounts (for example, system administrators, domain admins, cloud tenant admins) are high‑value targets for attackers.

Good practices:

- **Minimize the number of admins**
  - Only grant admin rights to people who truly need them.  

- **Separate admin and normal accounts**
  - Administrators should have:
    - One normal account for email and everyday tasks.  
    - One or more admin accounts used only for administrative activities.  
  - Do not use admin accounts for browsing the web or reading email.

- **Protect admins more strongly**
  - Enforce multi‑factor authentication (MFA) on all privileged accounts.  
  - Use strong, unique passwords stored in a secure password manager.  
  - Consider additional monitoring or logging for privileged actions.

- **Review admin access regularly**
  - Periodically review who has admin rights and whether they still need them.  
  - Remove or reduce privileges for roles that changed or are no longer relevant.

---

## 6. Role‑based access (RBAC) in simple terms

**Role‑based access control (RBAC)** means defining roles (for example, “Sales”, “Finance”, “HR”, “IT Support”) and assigning permissions to roles instead of individual people one by one.

For small and medium businesses, you can implement a light version of RBAC by:

- Defining a short list of roles and what they should access.  
- Mapping new staff to one or more roles.  
- Using built‑in role features in your main systems (for example, Microsoft 365 roles, application roles, folder permissions by group).

Benefits:

- Easier onboarding – new staff get the right access by being assigned to a role.  
- Easier audits – you can explain who should have access to what and why.  
- Less “access drift” over time, as changes are made through role adjustments.

---

## 7. Third‑party and vendor access

Vendors and partners often need access to your systems or data to provide services. This access must also follow good access control practices.

Consider:

- **Scope**
  - Limit vendor access to the specific systems and data required for their work.  
  - Avoid giving broad admin rights unless absolutely necessary.

- **Duration**
  - Where possible, make vendor access **time‑bound** (for example, access active only during a project or support window).  
  - Remove access when the contract ends or the work is complete.

- **Account management**
  - Prefer named accounts for vendor staff, not a single shared vendor account.  
  - Enforce MFA and strong passwords for vendor access.

- **Monitoring and review**
  - Periodically review vendor accounts and adjust or remove them as needed.

---

## 8. Documentation and visibility

Even a small amount of documentation greatly improves access control.

At minimum, maintain:

- A simple **access control policy** or standard:
  - Unique accounts, least privilege, MFA for admins, JML handling, and vendor access rules.  

- A **list of key systems and who has what level of access**:
  - For example, a table with system name, owner, admin users, and main roles.

- A **record of approvals** for unusual or elevated access:
  - Especially for privileged roles or exceptions to normal policy.

This makes it easier to respond to incidents, answer questions from customers or auditors, and plan improvements.

---

## 9. Minimal checklist for access control

Use this checklist as a quick status check:

- [ ] We follow the principle of least privilege (users have only the access they need).  
- [ ] Each user has a unique account; shared accounts are rare and controlled.  
- [ ] We have a basic joiner–mover–leaver process for creating, changing and removing access.  
- [ ] Administrator and privileged accounts are limited in number and protected with MFA.  
- [ ] Admin accounts are used only for administrative tasks, not for email or web browsing.  
- [ ] We have defined basic roles (for example, Sales, Finance, HR, IT) and use them to guide access.  
- [ ] Vendor and third‑party access is limited, time‑bound and reviewed periodically.  
- [ ] We maintain simple documentation of who has access to key systems and at what level.

Unchecked boxes indicate areas where you can strengthen your access control over the next 30–90 days.
