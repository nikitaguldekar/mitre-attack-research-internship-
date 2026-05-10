# MITRE ATT&CK Technique Mapping

## 1. Overview

This section maps the identified adversary behaviors, malware families, and attack activities observed during the research internship project to the MITRE ATT&CK framework.

The mapping helps identify:
- Adversary tactics
- Attack techniques
- Malware behavior
- Detection opportunities
- Defensive monitoring strategies

---

# 2. ATT&CK Tactic Mapping

| Tactic | Technique ID | Technique Name |
|---|---|---|
| Initial Access | T1566 | Phishing |
| Execution | T1059 | Command and Scripting Interpreter |
| Persistence | T1547 | Boot or Logon Autostart Execution |
| Privilege Escalation | T1055 | Process Injection |
| Defense Evasion | T1027 | Obfuscated Files or Information |
| Credential Access | T1056 | Input Capture |
| Discovery | T1082 | System Information Discovery |
| Lateral Movement | T1021 | Remote Services |
| Collection | T1113 | Screen Capture |
| Command and Control | T1071 | Application Layer Protocol |
| Exfiltration | T1041 | Exfiltration Over C2 Channel |

---

# 3. Software-to-Technique Mapping

| Software | Associated ATT&CK Techniques |
|---|---|
| Cobalt Strike | T1059, T1105, T1071 |
| Mimikatz | T1003, T1056 |
| Empire | T1059, T1547 |
| PoisonIvy | T1056, T1071 |
| NjRAT | T1113, T1056 |
| QuasarRAT | T1113, T1547 |
| Remcos | T1056, T1071 |
| Brute Ratel C4 | T1055, T1071 |
| PlugX | T1547, T1105 |
| DarkComet | T1113, T1056 |

---

# 4. APT29 Campaign ATT&CK Mapping

| ATT&CK Tactic | ATT&CK Technique | Description |
|---|---|---|
| Initial Access | Spearphishing Attachment | Malicious attachments used for access |
| Execution | PowerShell Execution | Malicious command execution |
| Persistence | Registry Run Keys | Persistence mechanisms |
| Credential Access | Credential Dumping | Credential theft activities |
| Discovery | System Information Discovery | Internal environment enumeration |
| Lateral Movement | Remote Services | Internal network traversal |
| Command & Control | Web Protocols | Encrypted attacker communication |
| Exfiltration | Data Transfer | Sensitive information theft |

---

# 5. ATT&CK-Based Detection Opportunities

Security teams can improve detection by monitoring:

- Suspicious PowerShell execution
- Credential dumping behavior
- Registry persistence mechanisms
- Remote service creation
- Process injection activity
- Encrypted outbound communication
- RAT-like behavior patterns
- Suspicious phishing attachments

---

# 6. Defensive Security Recommendations

Organizations should:

- Deploy Endpoint Detection & Response (EDR)
- Enable centralized log monitoring
- Conduct phishing awareness training
- Restrict administrative privileges
- Implement network segmentation
- Monitor ATT&CK-mapped attack patterns
- Use threat intelligence feeds
- Conduct regular security audits

---

# 7. Conclusion

The MITRE ATT&CK framework provides a structured methodology for understanding adversary behavior, attack lifecycle stages, and malware capabilities. Mapping software tools and campaigns to ATT&CK techniques helps improve threat detection, incident response, and defensive cybersecurity operations.
