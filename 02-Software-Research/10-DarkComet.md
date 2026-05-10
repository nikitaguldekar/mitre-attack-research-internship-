# DarkComet Malware Analysis

## 1. Name & Type

- Name: DarkComet
- Type: Remote Access Trojan (RAT)

---

## 2. Description

DarkComet is a Remote Access Trojan (RAT) designed to provide attackers with remote administration, surveillance, credential theft, and system control capabilities.

Although originally promoted as a remote administration tool, DarkComet has been widely abused in malicious cyber operations, espionage campaigns, and unauthorized remote access activities.

---

## 3. Threat Actor Association

Used by:
- Cybercriminal groups
- Espionage operators
- Various malware campaigns

---

## 4. Supported Platforms

- Windows

---

## 5. MITRE ATT&CK Techniques Used

| Technique ID | Technique Name |
|---|---|
| T1059 | Command and Scripting Interpreter |
| T1547 | Boot or Logon Autostart Execution |
| T1113 | Screen Capture |
| T1056 | Input Capture |
| T1071 | Application Layer Protocol |

---

## 6. Execution Method

- Malicious executable delivery
- Phishing attachments
- Script execution
- Social engineering delivery

---

## 7. Persistence Techniques

- Registry Run Keys
- Startup folder persistence
- Service installation
- Scheduled Tasks

---

## 8. Privilege Escalation

DarkComet may support:
- Administrative privilege abuse
- Process manipulation
- Token-related abuse

---

## 9. Defense Evasion

- Obfuscated payloads
- Encrypted communication
- Hidden process activity
- Persistence hiding techniques

---

## 10. Credential Access

DarkComet can facilitate:
- Keylogging
- Credential theft
- Password harvesting
- Input capture

---

## 11. Discovery Techniques

- System information discovery
- User account discovery
- File system enumeration
- Process monitoring

---

## 12. Lateral Movement

DarkComet itself is not primarily focused on lateral movement, but attackers may combine it with:
- SMB movement
- Remote administrative tools
- Credential reuse attacks

---

## 13. Command & Control

DarkComet establishes remote communication channels with attacker-controlled infrastructure for command execution and monitoring.

---

## 14. Exfiltration

The malware may transfer:
- Captured credentials
- Screenshots
- Sensitive files
- System information

to attacker-controlled infrastructure.

---

## 15. Impact Analysis

DarkComet infections can result in:
- Remote attacker access
- Surveillance activity
- Credential compromise
- Privacy violations
- Data theft

---

## 16. Indicators of Compromise (IOCs)

- Suspicious outbound communication
- Registry persistence artifacts
- Unusual screen capture activity
- Keylogging-related behavior

---

## 17. Detection & Mitigation

### Detection

- Monitor unusual outbound traffic
- Detect keylogging behavior
- Monitor persistence mechanisms
- Analyze suspicious RAT activity

### Mitigation

- Deploy endpoint security solutions
- Restrict unauthorized software execution
- Enable application allowlisting
- Conduct phishing awareness training

---

## 18. Conclusion

DarkComet remains a well-known Remote Access Trojan capable of supporting surveillance, credential theft, and remote attacker operations. Organizations should implement strong endpoint monitoring, ATT&CK-based detection strategies, and user awareness programs to reduce exposure to RAT-related threats.
