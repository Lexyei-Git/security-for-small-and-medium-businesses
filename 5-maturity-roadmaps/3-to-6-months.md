# 3–6 month security roadmap

This roadmap describes what a small or medium business can realistically achieve in the **3–6 month** period after completing the initial 30‑day quick‑win plan.

It focuses on consolidating basic controls, formalizing simple processes, and starting to build ongoing habits around security.

You should adapt this roadmap based on your own risk assessment and priorities.

---

## 1. Assumed starting point

This roadmap assumes that you have already done most of the following (as covered in `2-where-to-start/first-30-days.md` and the practical controls):

- Identified key assets and critical systems with a **simple asset inventory**.  
- Completed a **basic risk assessment** and identified high‑priority risks.  
- Enabled **MFA** on email and key business systems where possible.  
- Turned on or verified **automatic updates** for endpoints and common software.  
- Set up **at least one reliable backup** for critical data and tested a basic restore.  
- Implemented **basic email and phishing awareness**.  
- Deployed or confirmed **antivirus/endpoint protection** on business devices.

If some of these are not yet complete, treat them as early tasks in the 3–6 month window before moving to new items.

---

## 2. High-level goals for months 3–6

Between months 3 and 6, the focus should be on:

1. Making the initial controls more **consistent and repeatable**.  
2. Closing obvious gaps (especially around access control, configuration and vendors).  
3. Introducing light‑weight **governance**: simple policies, roles and review cadences.  
4. Improving **detection and response readiness**, not just prevention.

---

## 3. Month 3–4: standardize and finish the basics

### 3.1 Solidify asset and software inventories

- Complete and refine your **asset inventory**:
  - Ensure all critical devices, systems and data sets are listed.  
  - Add owners and criticality (critical/important/nice‑to‑have).

- Start a basic **software inventory**:
  - At least list key applications and services in use (local and cloud).  
  - Note versions for critical on‑premises software where feasible.

Deliverables:

- Updated `simple-asset-inventory.md` used as a living reference.  
- A short list of “must‑know” systems with owners.

### 3.2 Harden endpoints and configurations

Use `device-hardening-and-configuration.md` and `patching-and-updates.md` to:

- Apply a **baseline configuration** to laptops and desktops:
  - Screen lock, disk encryption, host firewall, limited local admin.  
  - Removal of unnecessary software.

- Confirm a **monthly patching cycle** for:
  - Endpoints (automatic updates where practical).  
  - Key servers and infrastructure (with simple test/approval steps).

Deliverables:

- Documented baseline for endpoints.  
- Simple monthly patching schedule (who does what, when).

### 3.3 Roll out and formalize core policies

Using the `policies/` folder and `starter-policies-and-templates.md`:

- Finalize and approve:
  - Acceptable use policy.  
  - Passwords and MFA policy.  
  - Backup and data protection policy.  
  - Email, internet and phishing policy.  
  - Incident reporting policy.

- Ensure:
  - Policies are approved by management.  
  - Published in an accessible location.  
  - Communicated to staff with basic acknowledgment.

Deliverables:

- Approved policy set, with documented approval date and owner.  
- Evidence that staff have been informed (for example, email or HR record).

---

## 4. Month 4–5: strengthen access, logging and vendor oversight

### 4.1 Improve access control and account hygiene

Using `access-control-basics.md` and `passwords-and-mfa.md`:

- Review **admin and privileged accounts**:
  - Limit who has admin rights on systems and cloud platforms.  
  - Ensure separate admin and normal user accounts for IT staff.

- Implement or refine a **joiner–mover–leaver process**:
  - New staff: accounts created and access granted based on roles.  
  - Role changes: remove access that is no longer needed.  
  - Departures: accounts disabled promptly, access removed across systems.

- Reduce or formalize **shared accounts**:
  - Replace where possible with named accounts + proper roles.  
  - Where not possible, strictly control and monitor shared credentials.

Deliverables:

- Short documented JML checklist or process.  
- Reduced number of privileged and shared accounts.

### 4.2 Establish basic logging and monitoring

Using `logging-and-monitoring-basics.md`:

- Confirm that logging is **enabled** on:
  - Identity platforms (sign‑ins, admin actions).  
  - Email and endpoint protection (security alerts).  
  - VPN and remote access (connections, failures).  
  - Critical applications and servers (where possible).

- Start **centralizing or at least consolidating** logs:
  - Even a simple, low‑cost log management solution or MSP‑provided portal is helpful.  
  - At a minimum, ensure security alerts are sent to a monitored mailbox or ticket system.

- Define a **basic review cadence**:
  - High‑severity alerts: as they happen.  
  - Summary reports: monthly or quarterly review.

Deliverables:

- Documented list of log sources and where they go.  
- Defined responsibilities for reviewing alerts and reports.

### 4.3 Formalize vendor and third‑party risk basics

Using `vendor-and-third-party-risk-basics.md` and `vendor-and-third-party-security-policy.md`:

- Complete or refine your **vendor inventory**:
  - Identify which vendors hold data or have access to systems.  
  - Classify them as high/medium/low risk.

- For **high‑risk vendors**:
  - Perform basic security due diligence (short questionnaire or checklist).  
  - Ensure contracts include at least minimal expectations for data protection and incident notification, where feasible.

Deliverables:

- Vendor inventory with risk classification.  
- Recorded basic due diligence for top high‑risk vendors.

---

## 5. Month 5–6: improve response, awareness and planning

### 5.1 Create a simple incident response playbook

Even a short, structured playbook dramatically improves response to incidents.

Using `incident-reporting-policy.md` (and later `incident-response-basics.md` when available):

- Define:
  - Who leads incident response (role, not just a name).  
  - A simple **incident severity scale** (for example, low/medium/high).  
  - Standard steps for common scenarios (for example, phishing, lost device, ransomware).

- Document:
  - Contact details (internal and external).  
  - Where logs and evidence are stored.  
  - When and how to escalate to management, legal, insurers or regulators.

- Run at least one **tabletop exercise**:
  - Walk through a realistic scenario with key people (for example, ransomware or business email compromise).  
  - Note gaps and update the playbook.

Deliverables:

- Short incident response playbook (2–5 pages).  
- Notes from at least one tabletop exercise.

### 5.2 Strengthen security awareness and training

Security awareness should start in the first 30 days and grow in the 3–6 month window.

Actions:

- Create a **simple annual training plan**:
  - For example: short quarterly topics (phishing, passwords/MFA, physical security, incident reporting).

- Include security topics in:
  - Onboarding for new staff.  
  - Regular team meetings or internal newsletters.

- If feasible, adopt:
  - A basic phishing simulation or awareness tool, or  
  - At least share real anonymized examples of phishing attempts the organization received.

Deliverables:

- Short written awareness plan (topics, frequency, responsibilities).  
- Evidence of at least one training or awareness activity in this period.

### 5.3 Begin a longer-term roadmap (6–12 months)

In the 3–6 month window, you will also start planning for the **6–12 month** horizon.

Examples of next‑stage items:

- Expanding logging and monitoring to more systems.  
- Formalizing business continuity and disaster recovery planning.  
- Increasing coverage of CIS Controls IG1 based on the mapping in `cis-controls-for-beginners.md`.  
- Considering additional controls (for example, application security, more advanced network monitoring) where risk justifies it.

Deliverables:

- Draft list of target improvements for months 6–12.  
- Linkage to NIST CSF and CIS Controls where useful for explaining the roadmap to management.

---

## 6. High-level checklist for months 3–6

Use this checklist to confirm you are on track:

- [ ] Asset and software inventories are complete enough to cover all critical systems and data.  
- [ ] Endpoint configuration and patching follow a basic, documented standard.  
- [ ] Core security policies are adapted, approved and communicated to staff.  
- [ ] Admin and privileged access is limited and managed through a joiner–mover–leaver process.  
- [ ] Logging is enabled on key systems and there is a plan for reviewing alerts and reports.  
- [ ] High‑risk vendors are identified and basic due diligence has been performed.  
- [ ] A simple incident response playbook exists and has been exercised at least once.  
- [ ] A basic security awareness plan is in place and at least one activity has been delivered.  
- [ ] A draft list of 6–12 month improvement goals has been created.

If many boxes are still unchecked, treat this roadmap as a **menu**, not a rigid schedule. Pick the items that best address your highest‑priority risks and available capacity, then iterate.
