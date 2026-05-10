# NjRAT Malware Analysis

## 1. Name & Type

- Name: NjRAT
- Type: Remote Access Trojan (RAT)

---

## 2. Description

NjRAT is a Remote Access Trojan (RAT) used by cybercriminals and threat actors to gain unauthorized remote access to compromised systems. The malware supports surveillance, credential theft, file management, command execution, and remote attacker control.

NjRAT is commonly distributed through phishing campaigns, malicious downloads, and infected attachments.

---

## 3. Threat Actor Association

Used by:
- Cybercriminal groups
- Financially motivated attackers
- Malware distribution campaigns

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
- Drive-by downloads
- Script execution

---

## 7. Persistence Techniques

- Registry Run Keys
- Startup folder persistence
- Service installation
- Scheduled Tasks

---

## 8. Privilege Escalation

NjRAT may support:
- Administrative privilege abuse
- Process manipulation
- Token-related abuse

---

## 9. Defense Evasion

- Obfuscated payloads
- Hidden process activity
- Encrypted communications
- Persistence hiding techniques

---

## 10. Credential Access

NjRAT can facilitate:
- Keylogging
- Password theft
- Credential harvesting
- Input capture

---

## 11. Discovery Techniques

- System information discovery
- User account discovery
- File system enumeration
- Process monitoring

---

## 12. Lateral Movement

Threat actors may combine NjRAT with:
- SMB movement
- Remote administration tools
- Credential reuse attacks

---

## 13. Command & Control

NjRAT establishes communication with attacker-controlled infrastructure to support remote surveillance and command execution.

---

## 14. Exfiltration

The malware may transfer:
- Credentials
- Screenshots
- Sensitive documents
- System information

to attacker-controlled infrastructure.

---

## 15. Impact Analysis

NjRAT infections can result in:
- Persistent remote attacker access
- Credential compromise
- Surveillance activity
- Data theft
- Privacy violations

---

## 16. Indicators of Compromise (IOCs)

- Suspicious outbound communication
- Registry persistence artifacts
- Keylogging behavior
- Unusual RAT-related activity

---

## 17. Detection & Mitigation

### Detection

- Monitor suspicious outbound traffic
- Detect persistence mechanism creation
- Analyze abnormal process behavior
- Monitor keylogging-related activity

### Mitigation

- Deploy endpoint security solutions
- Restrict unauthorized software execution
- Enable phishing protection
- Conduct security awareness training

---

## 18. Conclusion

NjRAT remains a widely used Remote Access Trojan capable of supporting surveillance, credential theft, and remote attacker operations. Organizations should implement ATT&CK-based monitoring, strong endpoint protection, and persistence detection strategies to reduce exposure to NjRAT-related threats.
