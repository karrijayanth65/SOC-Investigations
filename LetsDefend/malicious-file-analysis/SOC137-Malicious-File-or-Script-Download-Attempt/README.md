# SOC137 - Malicious File/Script Download Attempt

**Documentation author:** Jayanth K  
**Documentation updated:** 13 October 2026 (Asia/Calcutta)  
**Platform:** LetsDefend  
**Category:** malicious-file-analysis  
**Case ID:** SOC137  
**Documentation status:** Completed
**Lab execution verification:** Not recorded

[Platform index](../../README.md) · [Category index](../README.md) · [Portfolio home](../../../README.md)

## Case overview

### 📌 Alert Overview
- **Event ID:** 76  
- **Event Time:** Mar 14, 2021, 07:15 PM  
- **Rule Name:** SOC137 - Malicious File/Script Download Attempt  
- **Severity Level:** Security Analyst  

### 🖥️ Affected System
- **Source IP:** 172.16.17.37  
- **Hostname:** NicolasPRD  

### 📁 File Details
- **File Name:** INVOICE PACKAGE LINK TO DOWNLOAD.docm  
- **File Hash (MD5):** f2d0c66b801244c059f636d08a474079  
- **File Size:** 16.66 KB  
- **Action Taken:** Blocked  

### 🔗 Sample File
- Password-protected sample (password: `infected`):  
  https://files-ld.s3.us-east-2.amazonaws.com/f2d0c66b801244c059f636d08a474079.zip  

### ⚠️ Threat Summary
The detected file is a malicious macro-enabled document (.docm) commonly used to deliver malware via phishing campaigns. The file was successfully blocked before execution.

### 🧾 Final Verdict
✅ **True Positive**  
The file is confirmed malicious and associated with trojan activity.

### 🔐 Recommendations
- Keep macro execution disabled by default.
- Educate users about phishing attachments.
- Ensure endpoint protection signatures are updated.
- Monitor for similar file hashes or filenames.

## Documents and evidence

- [Detailed investigation](reports/investigation.md)
- [Analyst note](analyst-note.md)
- [Evidence index and missing information](evidence-index.md)
- [Screenshots folder](screenshots/)

## Evidence status

3 existing screenshots are linked from the report. Personal execution date, original logs for that execution, and independent validation are **Not recorded**. Preserve the original event timestamps in the narrative. Account-name personalization does not establish who performed the lab.
