# Complete repository structure

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026  
**Documentation status:** Completed

[Portfolio home](../README.md)

This tree lists the repository files at this presentation update. Future file additions require updating it.

```text
SOC-Investigations/
├── docs/
│   ├── documentation-history.md
│   ├── previous-index.md
│   └── REPOSITORY-STRUCTURE.md
├── LetsDefend/
│   ├── malicious-file-analysis/
│   │   ├── SOC137-Malicious-File-or-Script-Download-Attempt/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── hybrid-analysis-report.png
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal-report.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC138-Detected-Suspicious-Xls-File/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── hybrid-analysis-report.png
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal-report.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   └── README.md
│   ├── malware-analysis/
│   │   ├── SOC104-event-36-Malware-Detected/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── hybrid-analysis.png
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC104-event-84-Malware-Detected/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── hybrid-analysis.png
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC109-Emotet-Malware-Detected/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── hybrid-analysis.png
│   │   │   │   ├── siem-alert.png
│   │   │   │   ├── virustotal1.png
│   │   │   │   └── virustotal2.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC119-Proxy-Malicious-Executable-File-Detected/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC145-Ransomware-Detected/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── hybrid-analysis.png
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   └── README.md
│   ├── phishing-email-analysis/
│   │   ├── SOC114-Malicious-Attachment-Detected-Phishing-Alert/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── email.png
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal-report.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC120-Phishing-Mail-Detected-Internal-to-Internal/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── email.png
│   │   │   │   └── siem-alert.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC140-Phishing-Mail-Detected-Suspicious-Task-Scheduler/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── anyrun.jpeg
│   │   │   │   ├── email.jpeg
│   │   │   │   ├── hybrid-analysis.jpeg
│   │   │   │   └── siem-alert.jpeg
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC141-Phishing-URL-Detected/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal-report.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC282-Phishing-Alert-Deceptive-Mail-Detected/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── anyrun-report.png
│   │   │   │   ├── email.png
│   │   │   │   └── siem-alert.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   └── README.md
│   ├── web-attack-analysis/
│   │   ├── SOC170-Passwd-Found-in-Requested-URL-Possible-LFI-Attack/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── SOC342-CVE-2025-53770-SharePoint-ToolShell-Auth-Bypass-and-RCE/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── virustotal.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   └── README.md
│   └── README.md
├── TryHackMe/
│   ├── phishing-email-analysis/
│   │   ├── 8814-Email-Containing-Suspicious-External-Link/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── siem-alert.png
│   │   │   │   ├── trydetectthis-report.png
│   │   │   │   └── trydetectthis-report2.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── 8815-Email-Containing-Suspicious-External-Link/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── siem-alert.png
│   │   │   │   ├── splunk-log.png
│   │   │   │   └── trydetectthis-report.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── 8816-Access-to-Blacklisted-External-URL-Blocked-by-Firewall/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── trydetectthis.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── 8817-Email-Containing-Suspicious-External-Link/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   ├── siem-alert.png
│   │   │   │   └── trydetectthis-report.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   ├── 8818-Email-Containing-Suspicious-External-Link/
│   │   │   ├── reports/
│   │   │   │   └── investigation.md
│   │   │   ├── screenshots/
│   │   │   │   └── siem-alert.png
│   │   │   ├── analyst-note.md
│   │   │   ├── evidence-index.md
│   │   │   └── README.md
│   │   └── README.md
│   └── README.md
├── ACTION-REQUIRED.md
├── EVIDENCE-STATUS.md
└── README.md
```
