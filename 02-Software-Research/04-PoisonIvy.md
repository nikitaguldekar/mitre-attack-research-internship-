# PoisonIvy Malware Analysis

## 1. Name & Type

- Name: PoisonIvy
- Type: Remote Access Trojan (RAT)

---

## 2. Description

PoisonIvy is a Remote Access Trojan (RAT) used by threat actors to establish persistent remote access to compromised systems. The malware supports command execution, surveillance, credential theft, data exfiltration, and attacker-controlled operations.

PoisonIvy has historically been associated with espionage campaigns and targeted intrusions against enterprise and government environments.

---

## 3. Threat Actor Association

Used by:
- APT1
- APT groups
- Espionage-focused threat actors

---

## 4. Supported Platforms

- Windows

---

## 5. MITRE ATT&CK Techniques Used

| Technique ID | Technique Name |
|---|---|
| T1059 | Command and Scripting Interpreter |
| T1547 | Boot or Logon Autostart Execution |
| T1071 | Application Layer Protocol |
| T1105 | Ingress Tool Transfer |
| T1056 | Input Capture |

---

## 6. Execution Method

- Malicious executable delivery
- Phishing attachments
- DLL execution
- Script-based delivery

---

## 7. Persistence Techniques

- Registry Run Keys
- Service installation
- Scheduled Tasks
- Startup folder persistence

---

## 8. Privilege Escalation

PoisonIvy may support:
- Administrative privilege abuse
- Token manipulation
- Process injection techniques

---

## 9. Defense Evasion

- Obfuscated payloads
- Encrypted communication
- Hidden process activity
- DLL side-loading

---

## 10. Credential Access

PoisonIvy can facilitate:
- Keylogging
- Credential theft
- Password harvesting
- Input capture

---

## 11. Discovery Techniques

- System information discovery
- User account discovery
- Process enumeration
- File system discovery

---

## 12. Lateral Movement

Threat actors may combine PoisonIvy with:
- SMB movement
- Remote administrative tools
- Credential reuse techniques

---

## 13. Command & Control

PoisonIvy establishes remote communication channels with attacker-controlled infrastructure for command execution and remote surveillance.

---

## 14. Exfiltration

The malware may exfiltrate:
- Credentials
- Screenshots
- Sensitive documents
- System information

to attacker-controlled systems.

---

## 15. Impact Analysis

PoisonIvy infections can result in:
- Persistent remote access
- Espionage operations
- Credential compromise
- Data theft
- Enterprise compromise

---

## 16. Indicators of Compromise (IOCs)

- Suspicious outbound traffic
- Registry persistence artifacts
- Keylogging-related behavior
- Abnormal RAT activity

---

## 17. Detection & Mitigation

### Detection

- Monitor suspicious outbound communication
- Detect persistence mechanism creation
- Analyze RAT-related process activity
- Monitor keylogging behavior

### Mitigation

- Deploy endpoint protection solutions
- Restrict unauthorized executable execution
- Conduct phishing awareness training
- Enable centralized logging

---

## 18. Conclusion

PoisonIvy remains a historically significant Remote Access Trojan used in espionage and enterprise compromise operations. Organizations should implement ATT&CK-based monitoring, strong endpoint security, and persistence detection strategies to reduce exposure to PoisonIvy-related threats.
