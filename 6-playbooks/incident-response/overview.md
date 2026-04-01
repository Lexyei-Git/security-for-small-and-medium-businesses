# Incident Response Overview

Structured process to handle security alerts and incidents. Designed for SMB teams without 24/7 SOC.

## When to trigger

Run this playbook when:
- OSSEC/ClamAV alerts arrive
- Unusual network activity (Nmap)
- User reports suspicious activity
- OpenVAS finds critical vulnerabilities
- Backup/server failures

## Team roles

- **Incident Commander**: Makes decisions, approves actions
- **Technical Lead**: Investigates technical details  
- **Communications**: Notifies stakeholders
- **Documentation**: Records actions/decisions

## Expected outcomes

- Contain incident impact
- Restore normal operations
- Document lessons learned
- Prevent recurrence

**Duration**: 30min → 4hrs (most SMB incidents)
