# Indicators of Compromise (IOCs)

## Investigation: Simulated Microsoft Phishing Email

> **Important:** All indicators in this project are fictional and created specifically for cybersecurity training.

---

## 1. Suspicious Domain

**Domain:**

`micr0soft-security.example`

### Why is it suspicious?

The domain attempts to resemble Microsoft's name by replacing the letter `o` with the number `0`.

This is consistent with a common phishing technique known as **typosquatting or lookalike-domain impersonation**.

The `.example` top-level domain is intentionally used for this training exercise and is not a real malicious domain.

---

## 2. Suspicious URL

**URL:**

`http://micr0soft-security.example/verify`

### Why is it suspicious?

The URL:

- Uses a lookalike domain.
- Uses HTTP rather than HTTPS.
- Contains a `/verify` path designed to encourage the recipient to take immediate action.
- Is presented in an urgent account-security message.

---

## 3. Suspicious Sender

**Sender:**

`security-alert@micr0soft-security.example`

### Why is it suspicious?

The sender domain does not match the legitimate Microsoft domain.

The domain also uses the character substitution:

`micr0soft`

instead of:

`microsoft`

---

## 4. Social Engineering Indicators

The email uses several social-engineering techniques:

- Urgency
- Fear of account suspension
- Immediate-action language
- Request to verify an account
- Impersonation of a trusted organization

---

## 5. IOC Summary

| Type | Indicator | Reason |
|---|---|---|
| Domain | `micr0soft-security.example` | Lookalike domain |
| URL | `http://micr0soft-security.example/verify` | Suspicious verification link |
| Email | `security-alert@micr0soft-security.example` | Impersonation |
| Technique | Urgency | Social engineering |
| Technique | Account suspension threat | Social engineering |

---

## 6. Analyst Assessment

The indicators identified in this simulated email are consistent with a phishing attempt designed to impersonate a trusted organization and encourage the recipient to interact with a suspicious verification link.

Further investigation would normally include analysis of the complete email headers, URL reputation, domain information, and any associated infrastructure.

---

## 7. Training Note

This is a fictional cybersecurity laboratory exercise.

No real malicious infrastructure or victim information is involved.
