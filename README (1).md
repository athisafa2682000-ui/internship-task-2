# 📧 Phishing Email Analysis – Task 2

This project focuses on analyzing suspicious email headers and content to detect phishing attempts using **MXToolbox** and manual inspection techniques. The analysis demonstrates how email authentication failures (SPF, DKIM, and DMARC) can be used to identify spoofed or fraudulent emails.

---

## 🧾 Project Overview

Phishing is a common cyberattack where attackers impersonate trusted organizations to steal personal information.  
This task involved analyzing email headers and verifying their authenticity using MXToolbox tools.

Two sample phishing cases were analyzed:

1. **Microsoft Phishing Email**
2. **Jain University Online MCA Degree Phishing Email**

---

## 🧠 Analysis Steps

1. **Collect the Email Header**  
   Export or copy the full email header from the suspicious message.

2. **Use MXToolbox SuperTool**  
   - Open [MXToolbox Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)  
   - Paste the header and run analysis.

3. **Check Authentication Results**
   - **SPF (Sender Policy Framework)** – validates the sending server.
   - **DKIM (DomainKeys Identified Mail)** – verifies email content integrity.
   - **DMARC (Domain-based Message Authentication)** – checks alignment of SPF and DKIM.

4. **Interpret Results**
   - If DMARC or DKIM fails, the email is likely spoofed.
   - Check domain mismatches and suspicious relay information.

5. **Verify Visual and Content Clues**
   - Unusual sender addresses.
   - Grammar or formatting errors.
   - Links/buttons directing to unknown or unofficial sites.

6. **Generate Reports**
   - Document each analysis in a **PDF report**.

---

## 📄 Reports Included

| Report Name | Description |
|--------------|-------------|
| **Microsoft_Phishing_Analysis.pdf** | Analysis of a phishing email pretending to be from Microsoft. |
| **Jain_University_Phishing_Analysis.pdf** | Analysis of a fake university email promoting a false MCA program. |

---

## ⚠️ Findings Summary

| Indicator | Microsoft Email | Jain University Email |
|------------|-----------------|------------------------|
| DMARC | ❌ Failed | ❌ Failed |
| SPF | ✅ Passed but misaligned | ✅ Passed but misaligned |
| DKIM | ❌ Failed | ❌ Failed |
| Verdict | **Phishing Attempt** | **Phishing Attempt** |

---

## 🧩 Tools Used
- **MXToolbox SuperTool**
- **Email Header Analyzer**
- **Python (ReportLab)** – to generate PDF reports
- **Manual content inspection**

---

## 🛡️ Recommendations
- Never click links or download attachments from suspicious emails.
- Verify sender addresses directly from official websites.
- Report phishing emails through your email provider.
- Use strong spam filters and enable DMARC protection.

---

## 📚 Author
**Atheeka Bi Safa**  
Cybersecurity Project – Task 2  
Email Phishing Detection and Analysis using MXToolbox

---

## 📎 License
This project is created for educational and research purposes only.
