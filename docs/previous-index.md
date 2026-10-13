# Previous repository index

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026
**Documentation status:** Completed

This preserves the earlier landing page before the platform-and-case organization update. Its original claims are retained as historical text and were not independently re-validated by this publication.

[Portfolio home](../README.md)

## Archived landing-page text

### SOC-Investigations
SOC-Investigations
### 🛡️ SOC Investigation & Incident Response Portfolio

A collection of documented security incident investigations, artifact analyses, and threat hunting playbooks mapped to the **MITRE ATT&CK** framework.

---

#### 📋 Investigation Index

| Case ID | Incident Type | Primary Tools Used | MITRE Tactic / Technique | Status |
| :--- | :--- | :--- | :--- | :--- |
| **INC-2026-01** | Data Exfiltration via USB | Microsoft Defender, KQL, ShimCache | Exfiltration (TA0010) / T1052 | ✅ Documented |
| **INC-2026-02** | Credential Harvesting Phishing | Microsoft Sentinel, VirusTotal, Avanan | Initial Access (TA0001) / T1566 | ✅ Documented |
| **INC-2026-03** | Suspicious PowerShell Execution | CrowdStrike Falcon, Event Viewer | Execution (TA0002) / T1059.001 | ✅ Documented |

---

#### 🔍 Sample Investigation Workflow: Data Exfiltration Analysis

##### 1. Alert Triage & Context
* **Source:** Endpoint Detection and Response (EDR) telemetry.
* **Indicator:** Unusual volume of file read operations targeting sensitive design directories followed by rapid USB mass storage attachment.

##### 2. Forensic Artifact Extraction
* **ShimCache & Amcache:** Analyzed execution paths to prove target binaries were executed locally despite user claims.
* **USBSTOR Registry Keys:** Extracted device serial numbers, first/last connection timestamps, and friendly names to establish proof of data theft.

##### 3. Containment & Remediation
* Isolated the affected endpoint via EDR.
* Revoked active user sessions in Microsoft Entra ID and forced credential resets.

