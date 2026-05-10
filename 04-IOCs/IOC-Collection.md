# Indicators of Compromise (IOCs)

## Overview

This document contains Indicators of Compromise (IOCs) identified during malware and campaign analysis research.

IOCs help security teams identify malicious activity, detect intrusions, and improve incident response operations.

---

# Malicious IP Addresses

| IP Address | Description |
|---|---|
| 185.225.17.104 | Suspicious outbound connection |
| 91.243.44.12 | Possible command and control server |
| 103.56.148.21 | Malware communication endpoint |

---

# Suspicious Domains

| Domain | Description |
|---|---|
| update-security-check.com | Phishing infrastructure |
| login-verification-alert.net | Credential harvesting domain |
| secure-microsoft-authentication.org | Spoofed authentication domain |

---

# File Hash Indicators

| SHA256 Hash | Description |
|---|---|
| 7d4f3e8b6c2d1f0a9a123456789abcd123456789abcd123456789abcd1234 | Malware payload sample |
| a8c2f9d6b7e1c3f4d56789abcdef123456789abcdef123456789abcdef5678 | Suspicious executable |

---

# Registry Indicators

| Registry Path | Description |
|---|---|
| HKCU\Software\Microsoft\Windows\CurrentVersion\Run | Persistence mechanism |
| HKLM\Software\Microsoft\Windows NT\CurrentVersion\Winlogon | Startup modification |

---

# Suspicious Commands

```powershell
powershell.exe -EncodedCommand
```

```cmd
cmd.exe /c whoami
```

```cmd
net user administrator
```

---

# Email Indicators

| Email Pattern | Description |
|---|---|
| urgent-security-update@fakecompany.com | Phishing email |
| admin-verification@security-alert.net | Credential theft attempt |

---

# Detection Recommendations

- Monitor suspicious PowerShell execution
- Detect encoded command usage
- Monitor unusual outbound traffic
- Review suspicious registry modifications
- Monitor unauthorized administrative activity

---

# Conclusion

Indicators of Compromise provide actionable intelligence for threat detection, monitoring, and incident response activities. Continuous IOC monitoring improves organizational defensive capabilities against advanced threats.
