# BloodHound Analysis

## 1. Name & Type

- Name: BloodHound
- Type: Active Directory Enumeration and Attack Path Analysis Tool

---

## 2. Description

BloodHound is an Active Directory (AD) reconnaissance and analysis tool designed to identify attack paths, privilege escalation opportunities, and trust relationships within enterprise environments.

Threat actors frequently abuse BloodHound to map enterprise networks and identify high-value attack paths for lateral movement and domain compromise.

---

## 3. Threat Actor Association

Used by:
- APT groups
- Ransomware operators
- Red-team operators
- Enterprise attackers

---

## 4. Supported Platforms

- Windows
- Linux

---

## 5. MITRE ATT&CK Techniques Used

| Technique ID | Technique Name |
|---|---|
| T1087 | Account Discovery |
| T1018 | Remote System Discovery |
| T1482 | Domain Trust Discovery |
| T1069 | Permission Groups Discovery |
| T1082 | System Information Discovery |

---

## 6. Execution Method

- Active Directory enumeration
- LDAP queries
- PowerShell collection scripts
- SharpHound data collection

---

## 7. Persistence Techniques

BloodHound itself is not primarily designed for persistence, but attackers may use collected information to establish:
- Administrative persistence
- Service-based persistence
- Privileged account access

---

## 8. Privilege Escalation

BloodHound helps identify:
- Privileged group memberships
- Misconfigured permissions
- Kerberos delegation abuse
- Escalation attack paths

---

## 9. Defense Evasion

- Use of legitimate administrative protocols
- Internal reconnaissance activity
- LDAP-based enumeration

---

## 10. Credential Access

BloodHound supports analysis of:
- Privileged account exposure
- Administrative session discovery
- Credential attack opportunities

---

## 11. Discovery Techniques

BloodHound specializes in:
- Domain enumeration
- Trust relationship mapping
- User and group discovery
- Session enumeration

---

## 12. Lateral Movement

Attackers may use BloodHound findings to perform:
- SMB-based movement
- Remote administration
- Administrative account abuse
- Domain-wide compromise

---

## 13. Command & Control

BloodHound itself is not a command & control framework, but it is frequently deployed through post-exploitation frameworks such as Empire and Cobalt Strike.

---

## 14. Exfiltration

Collected Active Directory data may be transferred to attacker-controlled systems for offline attack path analysis.

---

## 15. Impact Analysis

BloodHound abuse can result in:
- Full Active Directory compromise
- Privilege escalation
- Enterprise-wide lateral movement
- Administrative account exposure

---

## 16. Indicators of Compromise (IOCs)

- Excessive LDAP queries
- SharpHound execution artifacts
- Abnormal Active Directory enumeration
- Unusual administrative discovery activity

---

## 17. Detection & Mitigation

### Detection

- Monitor LDAP query activity
- Detect SharpHound execution
- Monitor abnormal enumeration behavior
- Analyze suspicious PowerShell activity

### Mitigation

- Restrict unnecessary administrative privileges
- Harden Active Directory permissions
- Implement tiered administration
- Monitor privileged account usage

---

## 18. Conclusion

BloodHound remains one of the most powerful tools for Active Directory attack path analysis. Organizations should monitor enumeration activity, secure privileged accounts, and implement ATT&CK-based defensive strategies to reduce exposure to enterprise compromise.
