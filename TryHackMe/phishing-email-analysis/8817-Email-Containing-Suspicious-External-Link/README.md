# Inbound Email Containing Suspicious External Link - Investigation

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026 (Asia/Calcutta)  
**Platform:** TryHackMe  
**Category:** phishing-email-analysis  
**Case ID:** 8817  
**Documentation status:** Completed
**Lab execution verification:** Not recorded

[Platform index](../../README.md) · [Category index](../README.md) · [Portfolio home](../../../README.md)

## Case overview

### Alert Information

- **Alert ID:** 8817
- **Alert Name:** Inbound Email Containing Suspicious External Link
- **Severity:** Medium
- **Category:** Phishing
- **Date:** May 11, 2026

### Objective

Investigate the inbound email containing a suspicious Microsoft account security notification and determine whether the email is malicious.

### Investigation Summary

The investigation included:
- Reviewing the embedded URL activity in Splunk
- Verifying URL reputation using TryDetectThis
- Identifying phishing indicators within the email
- Assessing potential impact to the user account

### Key Findings

- The embedded URL was allowed through security controls.
- The URL `https://m1crosoftsupport.co/login` was identified as malicious in TryDetectThis.
- The sender domain `m1crosoftsupport.co` impersonates Microsoft using typosquatting.
- The email used fear-based social engineering tactics related to account compromise.
- User credential exposure risk exists if the link was accessed.

### Recommended Actions

- Force password reset / credential rotation for the affected user.
- Block the malicious sender domain.
- Block the associated malicious IP address.
- Monitor for suspicious login attempts related to the user account.

### Final Verdict

**True Positive**

The email is a confirmed phishing attempt impersonating Microsoft account security notifications.

## Documents and evidence

- [Detailed investigation](reports/investigation.md)
- [Analyst note](analyst-note.md)
- [Evidence index and missing information](evidence-index.md)
- [Screenshots folder](screenshots/)

## Evidence status

2 existing screenshots are linked from the report. Personal execution date, original logs for that execution, and independent validation are **Not recorded**. Preserve the original event timestamps in the narrative. Account-name personalization does not establish who performed the lab.
