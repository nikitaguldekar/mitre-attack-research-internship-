# QuasarRAT Malware Analysis

## 1. Name & Type

- Name: QuasarRAT
- Type: Remote Access Trojan (RAT)

---

## 2. Description

QuasarRAT is an open-source Remote Access Trojan (RAT) used by threat actors to establish persistent remote access, execute commands, monitor victims, steal credentials, and manage compromised systems remotely.

The malware is commonly used in phishing campaigns, malware delivery operations, and unauthorized remote administration attacks.

---

## 3. Threat Actor Association

Used by:
- Cybercriminal groups
- Malware operators
- Phishing-based attack campaigns

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
- Remote payload delivery

---

## 7. Persistence Techniques

- Registry Run Keys
- Scheduled Tasks
- Startup folder persistence
- Service installation

---

## 8. Privilege Escalation

QuasarRAT may support:
- Administrative privilege abuse
- Token manipulation
- Process injection techniques

---

## 9. Defense Evasion

- Obfuscated payloads
- Hidden process activity
- Encrypted communications
- In-memory execution

---

## 10. Credential Access

QuasarRAT can facilitate:
- Keylogging
- Credential theft
- Password harvesting
- Clipboard monitoring

---

## 11. Discovery Techniques

- System information discovery
- User account discovery
- File system enumeration
- Process monitoring

---

## 12. Lateral Movement

Threat actors may combine QuasarRAT with:
- SMB movement
- Remote administration tools
- Credential reuse techniques

---

## 13. Command & Control

QuasarRAT establishes encrypted communication channels with attacker-controlled infrastructure to support remote administration and surveillance.

---

## 14. Exfiltration

The malware may transfer:
- Credentials
- Screenshots
- Clipboard data
- Sensitive files

to attacker-controlled systems.

---

## 15. Impact Analysis

QuasarRAT infections can result in:
- Persistent attacker access
- Credential compromise
- Surveillance activity
- Data theft
- Enterprise compromise

---

## 16. Indicators of Compromise (IOCs)

- Suspicious outbound communication
- Registry persistence artifacts
- Keylogging-related behavior
- Unusual RAT process activity

---

## 17. Detection & Mitigation

### Detection

- Monitor suspicious outbound traffic
- Detect unauthorized persistence mechanisms
- Analyze abnormal process activity
- Monitor keylogging-related behavior

### Mitigation

- Deploy endpoint protection solutions
- Restrict unauthorized executable execution
- Enable phishing protection controls
- Conduct user awareness training

---

## 18. Conclusion

QuasarRAT remains a widely abused Remote Access Trojan capable of supporting surveillance, credential theft, and persistent attacker access. Organizations should implement ATT&CK-based monitoring, endpoint security controls, and persistence detection strategies to reduce exposure to QuasarRAT-related threats.
 
