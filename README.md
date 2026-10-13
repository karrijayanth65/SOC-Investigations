# SOC Investigations

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026 (Asia/Calcutta)  
**Status:** Starter portfolio documentation; personal lab execution evidence pending

SOC case documentation organized around platforms, analysis categories, case reports, and evidence. This workspace contains 19 case narratives and 50 existing screenshots. A document count is not a claim of personally completed labs.

## Platforms

| Platform | Case documents | Index |
|---|---|---|
| LetsDefend | 14 | [Complete case index](LetsDefend/README.md) |
| TryHackMe | 5 | [Complete case index](TryHackMe/README.md) |

## How to review a case

1. Open its README for the case overview and navigation.
2. Read `analyst-note.md` for the existing case note.
3. Open `reports/investigation.md` for the narrative and captioned images.
4. Review `evidence-index.md` for image hashes and missing proof-of-work fields.

## Evidence status

Original logs for Jayanth K's execution, capture provenance, and actual execution dates are **Not recorded** in this workspace. Existing narrative conclusions have not been independently verified here. The documentation update date is separate from retained event timestamps. See [the evidence requirements](EVIDENCE-STATUS.md).

## Actual repository structure

```text
SOC-Investigations/
  README.md
  EVIDENCE-STATUS.md
  LetsDefend/
    README.md
    malicious-file-analysis/
      README.md
      SOC137-Malicious-File-or-Script-Download-Attempt/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          hybrid-analysis-report.png
          siem-alert.png
          virustotal-report.png
      SOC138-Detected-Suspicious-Xls-File/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          hybrid-analysis-report.png
          siem-alert.png
          virustotal-report.png
    malware-analysis/
      README.md
      SOC104-event-36-Malware-Detected/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          hybrid-analysis.png
          siem-alert.png
          virustotal.png
      SOC104-event-84-Malware-Detected/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          hybrid-analysis.png
          siem-alert.png
          virustotal.png
      SOC109-Emotet-Malware-Detected/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          hybrid-analysis.png
          siem-alert.png
          virustotal1.png
          virustotal2.png
      SOC119-Proxy-Malicious-Executable-File-Detected/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          siem-alert.png
          virustotal.png
      SOC145-Ransomware-Detected/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          hybrid-analysis.png
          siem-alert.png
          virustotal.png
    phishing-email-analysis/
      README.md
      SOC114-Malicious-Attachment-Detected-Phishing-Alert/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          email.png
          siem-alert.png
          virustotal-report.png
      SOC120-Phishing-Mail-Detected-Internal-to-Internal/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          email.png
          siem-alert.png
      SOC140-Phishing-Mail-Detected-Suspicious-Task-Scheduler/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          anyrun.jpeg
          email.jpeg
          hybrid-analysis.jpeg
          siem-alert.jpeg
      SOC141-Phishing-URL-Detected/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          siem-alert.png
          virustotal-report.png
      SOC282-Phishing-Alert-Deceptive-Mail-Detected/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          anyrun-report.png
          email.png
          siem-alert.png
    web-attack-analysis/
      README.md
      SOC170-Passwd-Found-in-Requested-URL-Possible-LFI-Attack/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          siem-alert.png
          virustotal.png
      SOC342-CVE-2025-53770-SharePoint-ToolShell-Auth-Bypass-and-RCE/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          siem-alert.png
          virustotal.png
  TryHackMe/
    README.md
    phishing-email-analysis/
      README.md
      8814-Email-Containing-Suspicious-External-Link/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          trydetectthis-report.png
          trydetectthis-report2.png
          siem-alert.png
      8815-Email-Containing-Suspicious-External-Link/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          siem-alert.png
          splunk-log.png
          trydetectthis-report.png
      8816-Access-to-Blacklisted-External-URL-Blocked-by-Firewall/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          siem-alert.png
          trydetectthis.png
      8817-Email-Containing-Suspicious-External-Link/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          siem-alert.png
          trydetectthis-report.png
      8818-Email-Containing-Suspicious-External-Link/
        README.md
        analyst-note.md
        evidence-index.md
        reports/
          investigation.md
        screenshots/
          siem-alert.png
```

## Documentation conventions

[Documentation history](docs/documentation-history.md) · [Previous repository index](docs/previous-index.md)

- Platform names retain their official casing; category folders use lowercase kebab-case.
- Case folder names preserve unique case IDs, including both SOC104 event IDs.
- All detailed reports use `reports/investigation.md`.
- Screenshot filenames are lowercase and keep their actual PNG or JPEG format.
- All indexes and images use relative links.
- Unsupported fields are marked Not recorded.
