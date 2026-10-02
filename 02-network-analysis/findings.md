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

## Finding 3 — DNS Traffic Not Observed

### Observation

Wireshark was used to search the packet capture for DNS traffic.

The following display filters were tested:

- `dns`
- `dns.qry.name`

The packet capture did not return DNS traffic using these filters.

Wireshark's Protocol Hierarchy was also reviewed, and DNS was not listed among the protocols present in the capture.

### Analysis

The available packet capture does not appear to contain DNS traffic that can be analyzed as part of this investigation.

This limits the ability to investigate domain-resolution activity within this specific dataset.

### Security Relevance

DNS analysis can be useful during security investigations because analysts may use DNS activity to identify suspicious domains, command-and-control infrastructure, or unusual resolution patterns.

Because DNS traffic was not present in this capture, no DNS-based conclusions are being made.

### Analyst Assessment

**Result:** DNS traffic not observed in the provided PCAP.

No malicious activity is inferred from the absence of DNS traffic.

Further investigation will focus on protocols and evidence that are actually present in the capture.

## Finding 4 — HTTP Traffic Not Observed

### Observation

Wireshark was used to search the packet capture for HTTP traffic using the following display filter:

`http`

No packets were returned by the filter.

### Analysis

The provided packet capture does not appear to contain HTTP traffic that can be analyzed during this investigation.

Because HTTP traffic was not observed, there is no HTTP request or response evidence available from this dataset.

### Security Relevance

HTTP analysis can provide useful information during network investigations, including requested resources, HTTP methods, hosts, user-agents, and server responses.

However, conclusions should only be made from traffic actually present in the capture.

### Analyst Assessment

**Result:** HTTP traffic not observed in the provided PCAP.

No malicious activity is inferred from the absence of HTTP traffic.

The investigation will continue using protocols and evidence present in the capture.

## Finding 5 — Protocol Hierarchy

### Observation

Wireshark's Protocol Hierarchy was reviewed to identify the protocols represented in the packet capture.

The following protocols were observed:

- Frame
- Ethernet
- Internet Protocol Version 4 (IPv4)
- Transmission Control Protocol (TCP)
- Simple Mail Transfer Protocol (SMTP)
- Internet Message Format (IMF)

### Analysis

The protocol hierarchy indicates that the capture contains network traffic associated with email communication.

SMTP provides the transport mechanism for sending email, while Internet Message Format contains the structure and content of email messages.

IPv4 and TCP provide the underlying network and transport communication.

### Security Relevance

Email traffic can provide valuable evidence during security investigations.

Analyzing SMTP and email-message traffic can help an analyst investigate:

- Suspicious senders
- Email recipients
- Message subjects
- Email content
- Potential malicious attachments
- Suspicious communication patterns

### Analyst Assessment

The protocol hierarchy confirms that the provided PCAP is primarily focused on email-related network traffic.

Further investigation will focus on the SMTP and Internet Message Format data available in the capture.

## Finding 6 — Email Header Information Identified

### Observation

SMTP traffic was examined to identify email header information within the captured communication.

The investigation reviewed available message metadata, including:

- Sender information
- Recipient information
- Subject
- Date information
- Message-ID

### Analysis

Email headers provide important context during a security investigation.

Header information can help analysts establish:

- Who sent a message
- Who received it
- When the message was sent
- How the message can be uniquely identified
- Which email communication should be examined further

### Security Relevance

Email header analysis is commonly used during phishing and email-security investigations.

Analysts can compare sender information, domains, timestamps, and message identifiers against other available evidence.

### Evidence

- `email-headers.png`

### Analyst Assessment

Email header information was successfully identified from the SMTP traffic and documented as part of the investigation.

Further analysis should correlate the header information with the SMTP conversation and other available packet evidence.

## Finding 7 — SMTP Sender and Recipient Information

### Observation

SMTP request traffic was examined to identify the email envelope information.

A `MAIL FROM` command was identified in the packet capture.

A `RCPT TO` command was also reviewed to identify the intended recipient.

### Analysis

SMTP envelope information provides useful evidence about the communication between mail systems.

The `MAIL FROM` command identifies the envelope sender, while `RCPT TO` identifies the intended recipient.

This information can be correlated with email headers and other network evidence during an investigation.

### Security Relevance

SMTP sender and recipient information can help analysts:

- Trace email communication
- Identify unexpected senders
- Identify intended recipients
- Correlate messages with security alerts
- Build an incident timeline

### Evidence

- `smtp-sender.png`

### Privacy Note

Email addresses from the training capture were treated as investigation data and were not reproduced in this public portfolio documentation.

### Analyst Assessment

SMTP envelope information was successfully identified and documented.

The sender and recipient information should be correlated with the available email-header and message-content evidence before drawing additional conclusions.
