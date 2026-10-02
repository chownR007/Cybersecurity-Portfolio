# Phishing Investigation — Final Report

**Project:** Phishing Email Investigation  
**Environment:** Controlled Cybersecurity Training Lab  
**Analyst:** Portfolio Lab  
**Date:** October 1, 2026  
**Status:** Completed

---

## 1. Executive Summary

A simulated phishing email was investigated after an employee reported receiving an unexpected Microsoft account-security notification.

The message used urgency and a threat of account suspension to encourage the recipient to verify their account through a provided URL.

Analysis identified a lookalike domain, suspicious sender address, and suspicious verification URL.

Based on the evidence available within this controlled training scenario, the message was determined to be a simulated phishing attempt.

---

## 2. Incident Classification

**Incident Type:** Phishing

**Attack Objective:** Potential credential theft

**Severity:** Medium

**Confidence:** High within the simulated environment

**Affected User:** Simulated employee

---

## 3. Initial Detection

The simulated employee received an email containing the subject:

> URGENT: Your Microsoft Account Will Be Suspended

The message instructed the recipient to verify their account immediately.

The email used urgency and fear of account suspension to encourage immediate action.

---

## 4. Evidence Reviewed

The following evidence was analyzed:

- Simulated phishing email
- Sender address
- Sender domain
- Suspicious URL
- URL structure
- Social-engineering characteristics
- Investigation timeline

---

## 5. Indicators of Compromise

### Suspicious Email Address

`security-alert@micr0soft-security.example`

### Suspicious Domain

`micr0soft-security.example`

### Suspicious URL

`http://micr0soft-security.example/verify`

### Domain Impersonation

The domain uses `micr0soft` instead of `microsoft`.

The number `0` is used in place of the letter `o`.

---

## 6. Social Engineering Techniques

The message used several techniques commonly associated with phishing:

### Urgency

The recipient was told that action was required within 24 hours.

### Fear

The email threatened account suspension.

### Impersonation

The sender attempted to appear associated with Microsoft.

### Call to Action

The recipient was instructed to verify the account through a provided link.

---

## 7. Investigation Methodology

The investigation followed a structured process:

```text
Detection
   ↓
Initial Review
   ↓
Sender Analysis
   ↓
Domain Analysis
   ↓
URL Analysis
   ↓
IOC Identification
   ↓
Timeline Creation
   ↓
Incident Assessment
   ↓
Response Recommendation

8. Findings

The investigation identified multiple suspicious characteristics.

The sender domain did not match Microsoft’s legitimate domain.

The domain used a lookalike spelling designed to resemble Microsoft’s name.

The email used urgent language and an account-suspension threat.

The message directed the recipient to a suspicious verification URL.

Together, these characteristics are consistent with a phishing attempt in this simulated environment.



9. Recommended Response

If this were a real organizational incident, recommended actions would include:

Do not click the suspicious URL.
Do not provide credentials.
Preserve the original email and headers.
Report the email to the security team.
Investigate whether the recipient interacted with the URL.
Review authentication logs for suspicious activity.
Block confirmed malicious domains and URLs where appropriate.
Reset credentials if compromise is confirmed or suspected.
Review other mailboxes for similar messages.
Document the incident and response actions.


10. MITRE ATT&CK Mapping

Potential techniques represented by this scenario include:

T1566.002 — Phishing: Spearphishing Link

The simulated email contains a link intended to encourage the recipient to interact with an external resource.

T1583.001 — Acquire Infrastructure: Domains

Lookalike domains can be used by threat actors as part of phishing infrastructure.

MITRE ATT&CK mappings in this training project are used for educational purposes. Actual technique classification would depend on additional evidence.



11. Lessons Learned

This investigation demonstrated the importance of:

Examining sender information.
Identifying lookalike domains.
Analyzing suspicious URLs without directly visiting them.
Recognizing social-engineering techniques.
Documenting indicators of compromise.
Building an incident timeline.
Following a structured investigation process.


12. Analyst Conclusion

The simulated email demonstrated multiple characteristics associated with phishing, including brand impersonation, urgency, account-suspension threats, and a suspicious verification URL.

The evidence collected during this controlled exercise supports classifying the message as a simulated phishing attempt.

No real user, credential, organization, or malicious infrastructure was involved.



13. Skills Demonstrated

This project demonstrates practical experience with:

Phishing analysis
IOC identification
Domain analysis
URL analysis
Social-engineering identification
Incident documentation
Timeline creation
Basic incident response
MITRE ATT&CK mapping
Security reporting


14. Tools & Resources

The investigation methodology can be extended using:

VirusTotal
URLScan
WHOIS/RDAP
CyberChef
Wireshark
SIEM platforms
MITRE ATT&CK


15. Project Files

README.md — Project overview
investigation.md — Investigation methodology
iocs.md — Indicators of compromise
url-analysis.md — URL investigation
timeline.md — Incident timeline
evidence/phishing-email.txt — Simulated evidence
final-report.md — Final investigation report


Ethics & Safety

This project was created for cybersecurity education and professional development.

All investigation activity was performed using fictional evidence in a controlled environment.

No unauthorized systems, accounts, networks, or individuals were targeted.
