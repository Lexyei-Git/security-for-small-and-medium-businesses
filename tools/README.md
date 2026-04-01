# Security Tools for SMB

Practical open source security tools for small and medium businesses. Each tool includes SMB-focused guidance and links to official documentation.

## Available Tools

| Tool | Purpose | Key Use Case |
|------|---------|-------------|
| **[OpenVAS](openvas/)** | Vulnerability scanning | Network/server vuln assessment |
| **[OSSEC](ossec/)** | Host Intrusion Detection | Log monitoring + file integrity |
| **[Nmap](nmap/)** | Network discovery | Asset inventory + service mapping |
| **[ClamAV](clamav/)** | Antivirus engine | Malware scanning + mail gateway |

## Quick Start

1. **Choose your priority**: Start with **Nmap** (network visibility) + **ClamAV** (malware protection)
2. **Follow each tool's guide**: `overview.md` → `official-links.md` → `deployment-and-operations.md` → `smb-usage-guide.md`
3. **Test first**: Use pilot scope before production deployment
4. **Automate**: Set up scheduled scans/updates

## Tool Selection Guide
Network visibility → Nmap
Server vuln scan → OpenVAS
Endpoint HIDS → OSSEC
Malware detection → ClamAV

## Structure

Each tool folder contains:
- `overview.md` - What it does + SMB value
- `official-links.md` - Vendor documentation  
- `deployment-and-operations.md` - Install + basic ops
- `smb-usage-guide.md` - SMB workflows + cautions

## Next Steps

Add these tools to your maturity roadmap:
Week 1: Nmap + ClamAV (immediate value)
Week 4: OSSEC (endpoint visibility)
Month 2: OpenVAS (vuln management)

**Focus**: Start small → validate → automate → expand

**Focus**: Start small → validate → automate → expand
