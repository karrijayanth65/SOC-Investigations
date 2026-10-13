# Inbound Email Containing Suspicious External Link - Investigation

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026 (Asia/Calcutta)  
**Platform:** TryHackMe  
**Category:** phishing-email-analysis  
**Case ID:** 8815  
**Status:** Documentation organized; personal lab execution not verified

[Platform index](../../README.md) · [Category index](../README.md) · [Portfolio home](../../../README.md)

## Case overview

### Alert Information

- **Alert ID:** 8815
- **Alert Name:** Inbound Email Containing Suspicious External Link
- **Severity:** Medium
- **Category:** Phishing
- **Date:** May 11, 2026

### Objective

Investigate the inbound email containing a suspicious external link and determine whether the email is malicious or benign.

### Investigation Summary

The investigation included:
- Reviewing the suspicious URL in Splunk
- Verifying whether the message was blocked
- Analyzing the embedded link using TryDetectThis in AnalystVM
- Identifying phishing indicators within the email

### Key Findings

- The embedded URL used a shortened `bit.ly` link.
- Splunk logs confirmed the message was blocked by security controls.
- TryDetectThis classified the URL as malicious.
- The sender domain `amazon.biz` is suspicious and not associated with the legitimate Amazon domain.
- The email used urgency and delivery failure themes commonly associated with phishing attacks.

### Final Verdict

**True Positive**

The email was confirmed to contain a malicious phishing URL and was successfully blocked by security controls.

## Documents and evidence

- [Detailed investigation](reports/investigation.md)
- [Analyst note](analyst-note.md)
- [Evidence index and missing information](evidence-index.md)
- [Screenshots folder](screenshots/)

## Evidence status

3 existing screenshots are linked from the report. Personal execution date, original logs for that execution, and independent validation are **Not recorded**. Preserve the original event timestamps in the narrative. Account-name personalization does not establish who performed the lab.
