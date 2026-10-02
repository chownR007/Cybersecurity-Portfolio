# Network Traffic Analysis Findings

**Project:** Network Traffic Analysis — Wireshark  
**Environment:** Controlled Cybersecurity Training Lab  
**Analyst:** Portfolio Lab  
**Status:** In Progress

---

## Finding 1 — SMTP Traffic Identified

### Observation

Wireshark analysis identified SMTP traffic within the provided packet capture.

The SMTP traffic represents email communication between network hosts.

### Evidence

The following evidence was collected:

- SMTP packet traffic
- Source and destination information
- SMTP protocol details
- Email communication observed within the TCP stream

### Analysis

SMTP is commonly used for sending email between mail systems.

The captured traffic provides useful information for a security analyst, including communication endpoints and email-related activity.

Analyzing SMTP traffic can help identify suspicious email activity, unauthorized communication, or potential indicators of compromise.

### Security Relevance

Email traffic can be valuable during a security investigation because phishing, malware delivery, credential theft, and other attacks may involve email communication.

### Evidence Files

- `smtp-analysis.png`
- `email-traffic-analysis.png`
- `tcp-stream-analysis.png`

### Analyst Assessment

The observed SMTP traffic is documented as part of the network traffic investigation.

Additional analysis is required before determining whether any activity is malicious or represents an indicator of compromise.

---

## Next Investigation Step

Continue analyzing:


- Source and destination hosts
- DNS activity
- Network protocols
- TCP conversations
- Potential indicators of compromise
## Finding 2 — Network Endpoints Identified

### Observation

Wireshark's IPv4 Endpoints statistics were used to identify hosts communicating within the packet capture.

The endpoint information provides visibility into the systems involved in the captured network activity.

### Evidence

The following information was reviewed:

- IPv4 source addresses
- IPv4 destination addresses
- Packet counts
- Byte counts
- Transmitted packets
- Received packets

### Analysis

Endpoint statistics help a security analyst establish which hosts participated in network communication and determine which systems generated or received the most traffic.

This information can be used as a starting point for further investigation.

### Security Relevance

Identifying communicating hosts is an important step in network investigations because suspicious connections, unusual traffic volumes, or unexpected communication with external systems may provide additional indicators for investigation.

### Evidence File

- `ipv4-endpoints.png`

### Analyst Assessment

The IPv4 endpoint information has been documented for further analysis.

No malicious activity is concluded from endpoint statistics alone. Additional protocol and traffic analysis is required.
