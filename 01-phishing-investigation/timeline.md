# Phishing Incident Timeline

> This timeline represents a fictional cybersecurity training scenario.

## Incident Timeline

| Time | Event | Analyst Observation |
|---|---|---|
| 09:14 AM | Phishing email received | Employee receives an email claiming to be from Microsoft |
| 09:15 AM | Email reviewed | Message contains urgent account-security language |
| 09:16 AM | Sender examined | Sender uses a suspicious lookalike domain |
| 09:17 AM | URL identified | Email contains a suspicious account-verification URL |
| 09:18 AM | Domain analyzed | Domain uses `micr0soft` instead of `microsoft` |
| 09:20 AM | IOC documented | Sender, domain, and URL added to IOC list |
| 09:25 AM | Initial assessment completed | Message classified as suspicious phishing activity |
| 09:30 AM | Recommended response documented | User advised not to interact with the message |

---

## Investigation Timeline

### 09:14 AM — Initial Detection

The employee received an unexpected email claiming that their Microsoft account would be suspended.

### 09:15 AM — Initial Review

The email was reviewed for common phishing characteristics.

The analyst identified:

- Urgent language
- Account suspension threat
- Request for immediate verification
- Suspicious sender

### 09:16 AM — Sender Investigation

The sender address was examined.

The domain appeared to imitate Microsoft using a lookalike spelling.

### 09:17 AM — URL Identification

The email contained the following URL:

`http://micr0soft-security.example/verify`

The URL was documented without directly visiting the destination.

### 09:18 AM — Domain Investigation

The domain was examined as text.

The spelling `micr0soft` uses the number `0` in place of the letter `o`.

### 09:20 AM — IOC Documentation

The following potential indicators were documented:

- Sender email address
- Suspicious domain
- Suspicious URL

### 09:25 AM — Initial Assessment

Based on the available evidence, the message was assessed as suspicious phishing activity within this training scenario.

### 09:30 AM — Response Recommendation

The recommended response was to avoid interacting with the email and preserve the message for security investigation.

---

## Timeline Summary

The investigation followed this sequence:

```text
Email Received
      ↓
Initial Review
      ↓
Sender Analysis
      ↓
URL Identification
      ↓
Domain Analysis
      ↓
IOC Documentation
      ↓
Assessment
      ↓
Response Recommendation
