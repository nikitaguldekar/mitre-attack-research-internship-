# Mimikatz Analysis

## 1. Name & Type

- Name: Mimikatz
- Type: Credential Dumping and Post-Exploitation Tool

---

## 2. Description

Mimikatz is a widely used post-exploitation tool designed to extract plaintext passwords, Kerberos tickets, NTLM hashes, and authentication credentials from Windows systems.

It is frequently abused by threat actors during credential access and privilege escalation operations.

---

## 3. Threat Actor Association

Used by:
- APT29
- FIN6
- Wizard Spider
- Various ransomware operators

---

## 4. Supported Platforms

- Windows

---

## 5. MITRE ATT&CK Techniques Used

| Technique ID | Technique Name |
|---|---|
| T1003 | OS Credential Dumping |
| T1550 | Use Alternate Authentication Material |
| T1558 | Steal or Forge Kerberos Tickets |
| T1078 | Valid Accounts |

---

## 6. Execution Method

- Command-line execution
- PowerShell execution
- In-memory execution
- Script-based delivery

---

## 7. Persistence Techniques

Mimikatz itself is not primarily designed for persistence, but threat actors often combine it with:
- Scheduled Tasks
- Registry Run Keys
- Startup folder abuse

---

## 8. Privilege Escalation

Mimikatz can assist privilege escalation through:
- Token impersonation
- Credential theft
- Administrative account compromise

---

## 9. Defense Evasion

- In-memory execution
- Obfuscated PowerShell commands
- Antivirus evasion techniques
- Reflective loading

---

## 10. Credential Access

Mimikatz specializes in:
- LSASS memory dumping
- Kerberos ticket extraction
- Password retrieval
- NTLM hash extraction

---

## 11. Discovery Techniques

- User account discovery
- Privilege enumeration
- Domain trust discovery
- System information gathering

---

## 12. Lateral Movement

Stolen credentials may be used for:
- Remote Desktop Protocol (RDP)
- PsExec execution
- SMB authentication
- Pass-the-Hash attacks

---

## 13. Command & Control

Mimikatz is often deployed through:
- Cobalt Strike beacons
- PowerShell frameworks
- Remote shells
- Malware loaders

---

## 14. Exfiltration

Extracted credentials and tickets may be transferred to external attacker-controlled infrastructure.

---

## 15. Impact Analysis

Mimikatz can lead to:
- Full domain compromise
- Credential theft
- Administrative account takeover
- Lateral movement across enterprise networks

---

## 16. Indicators of Compromise (IOCs)

- Suspicious LSASS access
- Unusual PowerShell activity
- Encoded command execution
- Unauthorized credential dumping attempts

---

## 17. Detection & Mitigation

### Detection

- Monitor LSASS memory access
- Detect suspicious PowerShell execution
- Monitor credential dumping behavior
- Detect abnormal authentication activity

### Mitigation

- Enable Credential Guard
- Restrict administrative privileges
- Use Endpoint Detection & Response (EDR)
- Enable multi-factor authentication (MFA)

---

## 18. Conclusion

Mimikatz remains one of the most dangerous credential theft tools used in modern cyber attacks. Effective monitoring, credential protection mechanisms, and ATT&CK-based detection strategies are essential for reducing organizational exposure to credential dumping attacks.
