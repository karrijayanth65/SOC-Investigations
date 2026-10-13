# SOC141 - Phishing URL Detected

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026 (Asia/Calcutta)  
**Platform:** LetsDefend  
**Category:** phishing-email-analysis  
**Case ID:** SOC141  
**Documentation status:** Completed
**Lab execution verification:** Not recorded

[Platform index](../../README.md) · [Category index](../README.md) · [Portfolio home](../../../README.md)

## Screenshot preview

[View all screenshots in the report](reports/investigation.md#screenshot-evidence) · [Open this image at full resolution](https://raw.githubusercontent.com/karrijayanth65/SOC-Investigations/refs/heads/main/LetsDefend/phishing-email-analysis/SOC141-Phishing-URL-Detected/screenshots/siem-alert.png)

![SIEM alert preview](screenshots/siem-alert.png)

*Existing SIEM alert image: `siem-alert.png`. Open the full-resolution image and click it to enlarge small text. Image treatment and provenance are recorded in the [evidence index](evidence-index.md).*

## Case overview

### 📌 Overview
This case involves a phishing URL detection alert triggered by outbound traffic from an internal endpoint attempting to access a known malicious domain.

The activity was identified and validated as a **True Positive**, requiring containment and escalation for further investigation.

---

### 🚨 Alert Details

- **Event ID:** 86  
- **Event Time:** Mar 22, 2021, 09:23 PM  
- **Rule Name:** SOC141 - Phishing URL Detected  
- **Severity Level:** Security Analyst  

---

### 🌐 Network Information

- **Source IP:** 172.16.17.49  
- **Hostname:** EmilyComp  
- **User:** ellie  

- **Destination IP:** 91.189.114.8  
- **Domain:** mogagrocol.ru  

- **Request URL:**  
  http://mogagrocol.ru/wp-content/plugins/akismet/fv/index.php?email=ellie@letsdefend.io  

---

### 🧪 Detection Summary

- The URL was confirmed **malicious via VirusTotal**.
- Initial connection was **allowed**, but subsequent requests were **blocked by the firewall**.
- The endpoint showed signs of **compromise**.

---

### ⚠️ Impact

- Potential credential exposure (email parameter observed).
- Possible malware delivery or command-and-control communication.
- Endpoint integrity compromised.

---

### ✅ Actions Taken

- Endpoint **contained** from the network.
- Malicious domain identified and blocked.
- Incident **escalated to L2 / Incident Response team**.

---

### 🔄 Next Steps

- Perform **EDR analysis** on the endpoint.
- Conduct **full malware scan**.
- Reset user credentials.
- Review firewall and proxy logs for additional activity.

---

### 🏁 Conclusion

This alert is confirmed as a **True Positive** phishing attempt with endpoint compromise. Immediate containment was successful, and further investigation is required to assess full impact.

---

## Documents and evidence

- [Detailed investigation](reports/investigation.md)
- [Analyst note](analyst-note.md)
- [Evidence index and missing information](evidence-index.md)
- [Screenshots folder](screenshots/)

## Evidence status

2 existing screenshots are linked from the report. Personal execution date, original logs for that execution, and independent validation are **Not recorded**. Preserve the original event timestamps in the narrative. Account-name personalization does not establish who performed the lab.
