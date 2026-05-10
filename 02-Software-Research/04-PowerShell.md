# PowerShell Attack Analysis

## 1. Name & Type

- Name: PowerShell
- Type: Command-Line Shell and Scripting Environment

---

## 2. Description

PowerShell is a legitimate Microsoft scripting and automation framework widely used for system administration and task automation.

Threat actors frequently abuse PowerShell for malicious execution, persistence, credential access, lateral movement, and command & control operations due to its powerful scripting capabilities and deep integration with Windows systems.

---

## 3. Threat Actor Association

Abused by:
- APT29
- FIN7
- Wizard Spider
- Multiple ransomware groups

---

## 4. Supported Platforms

- Windows
- Linux
- macOS

---

## 5. MITRE ATT&CK Techniques Used

| Technique ID | Technique Name |
|---|---|
| T1059 | Command and Scripting Interpreter |
| T1086 | PowerShell |
| T1027 | Obfuscated Files or Information |
| T1105 | Ingress Tool Transfer |
| T1055 | Process Injection |

---

## 6. Execution Method

- PowerShell console execution
- Script execution
- Encoded commands
- Remote PowerShell sessions

---

## 7. Persistence Techniques

- Scheduled Tasks
- Registry Run Keys
- Startup scripts
- WMI event subscriptions

---

## 8. Privilege Escalation

PowerShell may assist attackers through:
- Administrative script execution
- Token manipulation
- UAC bypass techniques

---

## 9. Defense Evasion

- Encoded PowerShell commands
- Obfuscated scripts
- Fileless malware execution
- In-memory execution

---

## 10. Credential Access

PowerShell can facilitate:
- Credential dumping
- Password harvesting
- LSASS memory access
- Token theft

---

## 11. Discovery Techniques

- System information discovery
- User account discovery
- Network scanning
- Process enumeration

---

## 12. Lateral Movement

PowerShell supports:
- Remote administration
- WMI execution
- SMB-based movement
- Remote command execution

---

## 13. Command & Control

Threat actors may use PowerShell scripts to establish encrypted communication channels with remote attacker-controlled infrastructure.

---

## 14. Exfiltration

PowerShell scripts may compress, encrypt, and transfer sensitive data to external servers.

---

## 15. Impact Analysis

Malicious PowerShell activity can result in:
- Remote code execution
- Credential compromise
- Enterprise-wide compromise
- Persistent attacker access

---

## 16. Indicators of Compromise (IOCs)

- Encoded PowerShell commands
- Suspicious script execution
- Abnormal parent-child process relationships
- PowerShell network connections

---

## 17. Detection & Mitigation

### Detection

- Enable PowerShell logging
- Monitor Event ID 4104
- Detect encoded command execution
- Analyze suspicious script activity

### Mitigation

- Restrict unnecessary PowerShell usage
- Enable constrained language mode
- Deploy EDR solutions
- Implement application control policies

---

## 18. Conclusion

PowerShell remains one of the most frequently abused legitimate tools in modern cyber attacks. Effective monitoring, script analysis, and ATT&CK-based detection strategies are essential for identifying malicious PowerShell activity within enterprise environments.
