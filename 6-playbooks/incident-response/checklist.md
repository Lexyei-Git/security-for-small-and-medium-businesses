# Incident Response Checklist

**Document everything**: Start timer, log all actions/decisions.

## PHASE 1: Assess (0-15 min)

**Triage alert**:
- [ ] Source: OSSEC/Nmap/ClamAV/user report
- [ ] Severity: Critical/High/Medium/Low
- [ ] Affected systems:
- [ ] Business impact:

**Initial containment** (if active attack):
- [ ] Disconnect affected system from network
- [ ] Block source IP (if external)
- [ ] Kill suspicious processes


## PHASE 2: Investigate (15-60 min)

**Collect evidence**:
- [ ] Screenshots of alerts/dashboard
- [ ] nmap -sV affected-ip
- [ ] OSSEC agent logs: /var/ossec/logs/alerts/
- [ ] clamscan -r /tmp /home
- [ ] ps aux | grep suspicious
- [ ] netstat -tlnp or ss -tlnp1

**Determine scope**:
- [ ] Affected: 1 server / Multiple / Unknown
- [ ] Lateral movement: Yes/No evidence
- [ ] Data exfiltration: Yes/No evidence


## PHASE 3: Resolve (60-120 min)

**Remediate root cause**:
- [ ] Kill malware/process
- [ ] Patch vulnerability (OpenVAS finding)
- [ ] Restore clean files from backup
- [ ] Reset compromised credentials
- [ ] Block attack vectors (firewall)

**Validate fix**:
- [ ] Re-scan with ClamAV/Nmap
- [ ] Verify services normal
- [ ] Test business functions


## PHASE 4: Document & Prevent (120+ min)

**Lessons learned**:
- [ ] Root cause:
- [ ] Detection source:
- [ ] Time to respond: minutes
- [ ] Prevention: _


**Notify** (if required):
- [ ] Internal stakeholders
- [ ] Customers (if data breach)
- [ ] Insurance/regulators (if threshold met)


**Close incident**: All systems normal + prevention in place.

---

**Escalation**: If ransomware/unknown malware/large breach → External experts/legal counsel.
