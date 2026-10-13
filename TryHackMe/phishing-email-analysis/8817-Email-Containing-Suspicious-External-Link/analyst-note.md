# Analyst note — 8817

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026 (Asia/Calcutta)  
**Platform:** TryHackMe  
**Category:** phishing-email-analysis  
**Case ID:** 8817  
**Documentation status:** Completed
**Lab execution verification:** Not recorded

[Case overview](README.md) · [Detailed investigation](reports/investigation.md) · [Evidence index](evidence-index.md)

## Existing case note

Investigated alert ID 8817 related to a suspicious Microsoft account security email.

Reviewed the URL `https://m1crosoftsupport.co/login` in Splunk and observed the connection action was allowed. Further analysis in TryDetectThis confirmed the URL as malicious.

The email used a typosquatted Microsoft domain and social engineering tactics to lure the user into credential theft.

Recommended actions:
- Rotate affected user credentials
- Block malicious sender domain
- Block associated malicious IP address

Verdict: True Positive.

## Verification status

Independent re-check against personal raw logs: **Not recorded**. This documentation update adds navigation and evidence organization; it does not establish that Jayanth K performed the response actions described above.
