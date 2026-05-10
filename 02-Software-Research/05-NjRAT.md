# PsExec Analysis

## 1. Name & Type

- Name: PsExec
- Type: Remote Administration and Execution Tool

---

## 2. Description

PsExec is a legitimate Microsoft Sysinternals tool used for remote command execution and administrative management across Windows systems.

Threat actors frequently abuse PsExec for lateral movement, remote execution, privilege escalation, and enterprise-wide compromise operations.

---

## 3. Threat Actor Association

Used by:
- APT29
- FIN7
- Wizard Spider
- Multiple ransomware groups

---

## 4. Supported Platforms

- Windows

---

## 5. MITRE ATT&CK Techniques Used

| Technique ID | Technique Name |
|---|---|
| T1021 | Remote Services |
| T1569 | System Services |
| T1570 | Lateral Tool Transfer |
| T1078 | Valid Accounts |

---

## 6. Execution Method

- Remote command execution
- SMB-based execution
- Administrative share abuse
- Service-based execution

---

## 7. Persistence Techniques

PsExec itself is not primarily a persistence tool, but attackers may combine it with:
- Scheduled Tasks
- Service creation
- Registry modifications

---

## 8. Privilege Escalation

PsExec may assist attackers through:
- Administrative account abuse
- Service-level execution
- Elevated remote sessions

---

## 9. Defense Evasion

- Use of legitimate administrative tools
- Remote execution through trusted protocols
- Minimal malware footprint

---

## 10. Credential Access

PsExec often relies on:
- Stolen credentials
- Administrative passwords
- Pass-the-Hash techniques

---

## 11. Discovery Techniques

- Network share discovery
- Remote system enumeration
- Administrative account identification

---

## 12. Lateral Movement

PsExec is commonly used for:
- Remote execution across enterprise systems
- SMB-based lateral movement
- Remote service deployment

---

## 13. Command & Control

Threat actors may deploy PsExec through:
- Cobalt Strike
- Empire frameworks
- Remote command shells

---

## 14. Exfiltration

PsExec itself is not primarily designed for exfiltration, but it may support remote data access and attacker-controlled operations.

---

## 15. Impact Analysis

Abuse of PsExec can result in:
- Enterprise-wide lateral movement
- Remote attacker execution
- Administrative compromise
- Rapid ransomware deployment

---

## 16. Indicators of Compromise (IOCs)

- Suspicious service creation
- Unusual SMB traffic
- Remote command execution
- Administrative share access

---

## 17. Detection & Mitigation

### Detection

- Monitor remote service creation
- Detect unusual SMB activity
- Analyze remote administrative execution
- Monitor PsExec-related process creation

### Mitigation

- Restrict administrative privileges
- Limit SMB access
- Enable network segmentation
- Monitor remote execution tools

---

## 18. Conclusion

PsExec remains a commonly abused administrative tool in enterprise cyber attacks. Organizations should monitor remote administrative activity, detect lateral movement behavior, and implement ATT&CK-based detection strategies to reduce exposure to PsExec-related abuse.
