# Logging and monitoring basics

Logging and monitoring give you visibility into what is happening in your systems and network.  
Without logs, it is very hard to detect attacks, investigate incidents or prove what did and did not happen.

This document explains, in practical terms, what small and medium businesses should log, how to monitor it at a basic level, and how this supports detection and response.

---

## 1. What logging and monitoring are (plain language)

- **Logging**  
  - Systems, applications and devices record events (for example, logins, configuration changes, errors) into log files or log streams.

- **Monitoring**  
  - People and tools **look at those logs** to:
    - Spot suspicious activity.  
    - Detect failures or misconfigurations.  
    - Support incident response and troubleshooting.

In small and medium businesses, logging and monitoring do not need to be highly complex, but they must be **purposeful**: you should know why you are collecting logs and what you intend to do with them.

---

## 2. Why logging and monitoring matter for SMBs

Good logging and monitoring help you to:

- Detect suspicious logins, unusual access patterns or repeated failed login attempts.  
- See when important settings or permissions change.  
- Investigate incidents (for example, “Which account was used?”, “From where?”, “What was accessed?”).  
- Demonstrate due diligence to customers, partners or regulators when something goes wrong.

National guidance emphasizes that logging and monitoring are essential to **identify indicators of compromise (IoCs)** and to minimize the impact of incidents.

---

## 3. What to log (priorities for SMBs)

You cannot log everything in detail on day one. Start with **high‑value events** from key systems.

Recommended priorities:

1. **Identity and access events**
   - Successful and failed logins (including admin and remote access).  
   - Account lockouts and password resets.  
   - Changes to roles, groups and privileges.

2. **Email and collaboration**
   - Security alerts from email security and spam/phishing filters.  
   - Suspicious or blocked messages and attachments (summary level is often enough).

3. **Endpoint protection**
   - Antivirus / endpoint protection detections (malware blocked, quarantined, allowed).  
   - Ransomware or exploit prevention alerts.

4. **Servers and critical applications**
   - Admin actions (for example, configuration changes, new user creation).  
   - Application errors or unexpected restarts.  
   - Access to sensitive data or critical transactions, where supported.

5. **Network and remote access**
   - VPN connections (who connected, from where, when).  
   - Firewall blocks and significant policy changes.

If you use cloud services (for example, Microsoft 365, Google Workspace, major SaaS):

- Enable and retain **audit logs** for sign‑ins, admin activities and configuration changes, following provider guidance.

---

## 4. Centralizing logs (at the right scale)

Scattered logs on individual devices are difficult to use. Where possible:

- **Centralize important logs** into:
  - A simple log management tool or SIEM (security information and event management) platform.  
  - A cloud‑based logging service.  
  - A solution provided by your managed service provider.

Benefits of centralization:

- Single place to search and review security‑relevant events.  
- Easier correlation across systems (for example, same user across VPN, email and endpoints).  
- Consistent retention policies and better protection of log integrity.

For very small environments, you may start with:

- Keeping logs enabled on key systems.  
- Exporting or forwarding only critical alerts to a central dashboard or to your IT/security provider.

---

## 5. Retention and protection of logs

Logs themselves can contain sensitive information (for example, usernames, IP addresses, possibly personal data). They also become important evidence if there is an incident.

Basic expectations:

- **Retention**
  - Keep security‑relevant logs long enough to support:
    - Detection of slow‑moving or long‑running attacks.  
    - Investigation and legal or regulatory needs.  
  - Many organizations aim for at least **several months** of searchable logs, with longer‑term archive where feasible (for example, 6–12 months).

- **Integrity and confidentiality**
  - Protect logs from tampering and unauthorized deletion.  
  - Restrict access to logs to authorized personnel (for example, IT, security, or your managed provider).  
  - Secure log storage (encrypted and access‑controlled).

Document your basic retention and access rules in a short internal note or policy.

---

## 6. Basic monitoring practice for SMBs

Monitoring does not always mean having a full‑time security operations center. For small and medium businesses, a **pragmatic approach** is:

- **Define what you will look for**
  - Unusual login activity (for example, logins from unexpected locations or times).  
  - Repeated failed login attempts and account lockouts.  
  - Malware detections and blocked connections.  
  - Changes to admin roles or critical configuration.

- **Set up alerts where possible**
  - Configure your email, VPN, endpoint protection and cloud platforms to send alerts for high‑severity events.  
  - Route alerts to a monitored mailbox, ticketing system or your managed security provider.

- **Schedule regular reviews**
  - Even with alerts, plan simple periodic reviews (for example, weekly or monthly) of summary reports:
    - Top security events.  
    - New admin accounts created.  
    - Unusual spikes in failed logins or blocked traffic.

- **Integrate with incident response**
  - Ensure your incident response procedure references where logs are located and how to retrieve them quickly when needed.

If you use a managed security service (SOC/MDR), clarify which logs they monitor, what alerts they receive and how they will contact you if they detect something.

---

## 7. Starting small and improving over time

You do not need an enterprise‑grade logging program from day one. A realistic path for SMBs is:

1. **Enable logging on key systems**
   - Turn on and verify logging for identity, email, endpoint protection, VPN and critical applications.

2. **Centralize or at least consolidate**
   - Forward high‑value security events to:
     - A simple central system you control, or  
     - Your managed service provider’s platform.

3. **Define basic alerts and review routines**
   - Configure alerts for high‑severity events.  
   - Establish weekly or monthly log review tasks.

4. **Adjust based on incidents and findings**
   - After an incident or near‑miss, review which logs were useful and which were missing.  
   - Update your logging scope, alerting and retention accordingly.

5. **Mature with your environment**
   - As you adopt more cloud services or complex systems, expand logging and monitoring to cover them.  
   - Align with frameworks (for example, NIST CSF Detect Function) and national guidance over time.

---

## 8. Minimal checklist for logging and monitoring

Use this checklist as a quick status check:

- [ ] Logging is enabled on key systems (identity, email, VPN, endpoint protection, servers and critical applications).  
- [ ] We collect and keep security‑relevant logs for an appropriate period (for example, several months).  
- [ ] Access to logs is restricted and logs are protected from tampering or unauthorized deletion.  
- [ ] We receive alerts for high‑severity events (for example, suspicious logins, malware detections, major configuration changes).  
- [ ] We regularly review summary reports or dashboards for unusual patterns.  
- [ ] Logs are used during incident investigations and our procedures reference where to find them.  
- [ ] If we use a managed security provider, we know which logs they monitor and how they will notify us of incidents.

Unchecked boxes indicate areas where you can gradually improve visibility and detection over the next 30–90 days.
