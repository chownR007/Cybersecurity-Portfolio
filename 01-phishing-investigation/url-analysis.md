# URL Analysis

## URL Under Investigation

`http://micr0soft-security.example/verify`

> This URL is fictional and was created specifically for this cybersecurity training exercise.

---

## URL Breakdown

| Component | Value |
|---|---|
| Protocol | HTTP |
| Domain | micr0soft-security.example |
| Path | /verify |

---

## 1. Protocol Analysis

The URL uses:

`HTTP`

rather than:

`HTTPS`

HTTPS provides encryption for traffic between the client and server.

The use of HTTP alone does not prove that a URL is malicious, but it is an additional characteristic worth noting when the URL appears in a suspicious email.

---

## 2. Domain Analysis

The domain is:

`micr0soft-security.example`

The domain appears designed to resemble the legitimate Microsoft brand.

The letter `o` in `Microsoft` has been replaced with the number `0`.

This is a common lookalike-domain technique.

---

## 3. Path Analysis

The URL contains the path:

`/verify`

The path suggests that the recipient is expected to perform an account verification action.

Combined with the urgent language in the email, this increases the need for further investigation.

---

## 4. Threat Intelligence Considerations

In a real SOC investigation, an analyst could investigate the domain and URL using approved security-analysis resources.

Examples include:

- VirusTotal
- URLScan
- WHOIS/RDAP information
- DNS information
- Internal security tools
- SIEM data
- Secure sandboxing platforms

The analyst should avoid directly visiting an unknown suspicious URL from a normal workstation.

---

## 5. Findings

The URL contains several characteristics that warrant investigation:

1. Lookalike domain.
2. Brand impersonation.
3. Account-verification language.
4. HTTP rather than HTTPS.
5. Urgent phishing context.

---

## 6. Analyst Assessment

The URL should be treated as suspicious within this simulated investigation.

Additional technical evidence would normally be collected before determining whether the URL is malicious.

---

## 7. Safety Note

This URL is intentionally fictional and uses the reserved `.example` domain.

It should not be treated as a real malicious website.
