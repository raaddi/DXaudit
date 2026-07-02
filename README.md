# DXaudit

DXaudit is a local Windows application for defensive workstation auditing. It checks system configuration, baseline security, backup posture, performance, stability, and data loss risks.

This public repository contains product materials and a compiled executable only. The application source code is not published.

## Download

The application executable is available here:

```text
download/DXaudit.exe
```

Run it by double-clicking the file. For a more complete audit, run it as administrator.

## What It Checks

- Windows system information, hardware, RAM, CPU, and disks.
- Microsoft Defender, firewall, Windows Update, BitLocker, UAC, RDP, and SMBv1.
- Local administrators, user accounts, startup entries, and installed software.
- Basic performance, free disk space, processes, event log, and printers.
- Backup indicators, cloud sync, restore points, and data loss risk.
- Remote access tools and basic local network configuration.
- Optionally, public domain records: MX, SPF, DMARC, HTTPS, SSL certificate, and HTTP security headers.

## What It Does Not Do

- It does not collect passwords, tokens, cookies, or browser history.
- It does not read document contents, emails, photos, or private files.
- It does not run exploits, password cracking, or offensive security tests.
- It does not scan other hosts on the network.
- It does not upload reports to the internet in the MVP version.
- It does not automatically repair system settings.

## Reports

After an audit, the application creates a local report package:

- `client_report.html` - client-readable report,
- `technical_report.html` - detailed technical report,
- `audit.json` - report data in JSON format,
- `README_DLA_KLIENTA.txt` - short guide for reading the report,
- `offer_draft.md` - draft scope of recommended follow-up work.

## Privacy

DXaudit runs locally. The MVP version does not upload reports to the internet. Privacy mode masks hostname, username, domain, IP addresses, local paths, and serial numbers in generated reports.

Details: [docs/PRIVACY.md](docs/PRIVACY.md)

## Status

Current public version: `0.1.0 MVP`

This is an early product release. Audit results should be treated as a technical diagnostic aid, not as a guarantee of complete security.
