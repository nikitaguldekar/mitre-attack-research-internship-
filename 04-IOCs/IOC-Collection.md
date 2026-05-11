# Indicators of Compromise (IOC) Collection Analysis

## 1. Overview

Indicators of Compromise (IOCs) are forensic artifacts and observable security events that help identify malicious activity within systems and networks.

This section documents common IOCs associated with the researched malware families, adversary behaviors, and MITRE ATT&CK techniques identified during the internship project.

---

# 2. Types of IOCs

The following IOC categories were analyzed:

- Malicious IP addresses
- Suspicious domains
- Malware file hashes
- Registry persistence artifacts
- Suspicious process activity
- Command & Control traffic
- Phishing artifacts
- Malicious executable behavior

---

# 3. Network-Based IOCs

| IOC Type | Description |
|---|---|
| Suspicious IP Addresses | Communication with attacker infrastructure |
| Malicious Domains | Fake or attacker-controlled domains |
| Encrypted C2 Traffic | Abnormal outbound encrypted traffic |
| Unusual Ports | Suspicious remote communication channels |
| Beaconing Activity | Periodic communication with C2 servers |

---

# 4. Host-Based IOCs

| IOC Type | Description |
|---|---|
| Registry Run Keys | Persistence mechanisms |
| Suspicious Processes | Malware-related process execution |
| DLL Injection | Process injection artifacts |
| Startup Folder Changes | Persistence activity |
| Scheduled Tasks | Unauthorized scheduled execution |

---

# 5. File-Based IOCs

| IOC Type | Description |
|---|---|
| Executable Files | Malicious .exe payloads |
| DLL Files | Malicious DLL side-loading artifacts |
| Script Files | PowerShell or malicious scripts |
| Dropped Payloads | Malware delivery artifacts |
| Modified System Files | Unauthorized file modification |

---

# 6. Malware IOC Examples

| Malware | Common IOC Indicators |
|---|---|
| Cobalt Strike | Beacon traffic, injected processes |
| Mimikatz | LSASS access attempts |
| PoisonIvy | Registry persistence artifacts |
| NjRAT | Keylogging-related behavior |
| QuasarRAT | Suspicious outbound communication |
| Remcos | Screen capture activity |
| PlugX | DLL side-loading behavior |
| DarkComet | Remote administration traffic |

---

# 7. ATT&CK-Aligned IOC Mapping

| ATT&CK Technique | IOC Evidence |
|---|---|
| T1059 | Suspicious script execution |
| T1547 | Registry persistence artifacts |
| T1055 | Process injection behavior |
| T1071 | Encrypted outbound communication |
| T1113 | Unauthorized screen capture activity |
| T1056 | Keylogging behavior |

---

# 8. IOC Collection Methodology

The IOC collection process included:

1. Malware behavior analysis
2. ATT&CK technique mapping
3. Threat intelligence research
4. Security log analysis
5. Process behavior monitoring
6. Network traffic inspection
7. Persistence mechanism analysis

---

# 9. Detection Recommendations

Organizations should monitor:

- Suspicious outbound connections
- Persistence mechanism creation
- Process injection activity
- Unauthorized PowerShell execution
- Remote administration behavior
- Registry modifications
- Credential dumping attempts
- RAT-related communication patterns

---

# 10. Security Mitigation Strategies

To reduce IOC-related threats:

- Deploy Endpoint Detection & Response (EDR)
- Enable centralized logging
- Monitor ATT&CK-mapped techniques
- Restrict administrative privileges
- Conduct regular IOC threat hunting
- Use threat intelligence feeds
- Implement phishing protection controls

---

# 11. Conclusion

IOC analysis plays a critical role in threat detection, malware investigation, and incident response operations. Identifying malicious indicators helps security teams detect attacker activity, improve monitoring capabilities, and strengthen organizational cybersecurity defenses.
