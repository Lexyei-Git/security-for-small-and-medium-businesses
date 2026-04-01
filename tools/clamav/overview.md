# ClamAV Overview

ClamAV is an open source antivirus engine for detecting trojans, viruses, malware & other malicious threats.

Key components:
- **clamscan**: Command-line scanner for on-demand scans
- **freshclam**: Virus signature updater
- **clamd**: Multi-threaded daemon for real-time scanning
- **clamdscan**: Client for clamd (faster than clamscan)

For SMB, ClamAV provides essential malware protection for:
- File servers and shared directories
- Email gateways (with milter integration)
- Web uploads and downloads
- Scheduled system scans
- On-access scanning (Linux)

Cross-platform (Linux, Windows, macOS) with no licensing costs.
