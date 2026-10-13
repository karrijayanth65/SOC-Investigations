# SOC170 - Passwd Found in Requested URL - Possible LFI Attack

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026 (Asia/Calcutta)  
**Platform:** LetsDefend  
**Category:** web-attack-analysis  
**Case ID:** SOC170  
**Documentation status:** Completed
**Lab execution verification:** Not recorded

[Platform index](../../README.md) · [Category index](../README.md) · [Portfolio home](../../../README.md)

## Screenshot preview

[View all screenshots in the report](reports/investigation.md#screenshot-evidence) · [Open this image at full resolution](https://raw.githubusercontent.com/karrijayanth65/SOC-Investigations/refs/heads/main/LetsDefend/web-attack-analysis/SOC170-Passwd-Found-in-Requested-URL-Possible-LFI-Attack/screenshots/siem-alert.png)

![SIEM alert preview](screenshots/siem-alert.png)

*Existing SIEM alert image: `siem-alert.png`. Open the full-resolution image and click it to enlarge small text. Image treatment and provenance are recorded in the [evidence index](evidence-index.md).*

## Case overview

### Overview

This investigation relates to a web application security alert triggered by a request attempting to access the `/etc/passwd` file through a Local File Inclusion (LFI) technique.

### Alert Details

* Event ID: 120
* Rule: SOC170 - Passwd Found in Requested URL - Possible LFI Attack
* Event Time: March 01, 2022, 10:10 AM
* Hostname: WebServer1006
* Destination IP: 172.16.17.13
* Source IP: 106.55.45.162
* HTTP Method: GET
* Device Action: Allowed

### Requested URL

https://172.16.17.13/?file=../../../../etc/passwd

### Summary

An external source IP attempted to access the Linux password file (`/etc/passwd`) using directory traversal sequences in the URL. The target server is a Windows-based system, making the requested file path invalid. The server responded with HTTP status code 500 and a response size of 0 bytes, indicating the attack attempt was unsuccessful.

### Investigation Outcome

* Classification: True Positive
* Attack Type: Local File Inclusion (LFI) Attempt
* Impact: No evidence of successful file disclosure
* Status: Failed Attack Attempt

### Conclusion

The alert correctly identified a malicious attempt to exploit a potential LFI vulnerability. The request failed because the targeted file does not exist on the Windows server, resulting in an internal server error.

## Documents and evidence

- [Detailed investigation](reports/investigation.md)
- [Analyst note](analyst-note.md)
- [Evidence index and missing information](evidence-index.md)
- [Screenshots folder](screenshots/)

## Evidence status

2 existing screenshots are linked from the report. Personal execution date, original logs for that execution, and independent validation are **Not recorded**. Preserve the original event timestamps in the narrative. Account-name personalization does not establish who performed the lab.
