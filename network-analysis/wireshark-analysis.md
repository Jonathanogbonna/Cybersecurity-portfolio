# Wireshark Network Traffic Analysis

## Objective

To analyse captured network traffic and identify suspicious or potentially malicious activity.

---

## Tools Used

* Wireshark

---

## Methodology

* Captured network traffic using Wireshark
* Applied filters to isolate relevant protocols (DNS, HTTP, TCP)
* Analysed packet details including source and destination IP addresses
* Reviewed traffic patterns and communication behaviour

---

## Analysis & Findings

During the analysis, DNS traffic was isolated using Wireshark display filters. The capture revealed multiple DNS queries and responses to external domains, including services associated with Microsoft and cloud infrastructure providers.

Key observations include:

- Frequent DNS queries to external domains such as Microsoft-related services, indicating normal system background activity.
- Presence of multicast DNS (mDNS) traffic, commonly used for local network service discovery.
- Encrypted traffic protocols such as TLS and QUIC observed in the broader capture, indicating secure communications.
- TCP reset (RST) packets detected, suggesting normal connection termination behaviour rather than malicious activity.

No clear indicators of compromise were identified; however, the analysis demonstrates how unusual patterns or unknown domains could be flagged for further investigation in a real-world SOC environment.

---

## Conclusion

This project demonstrates how packet-level analysis can be used to identify potential security threats. Monitoring and analysing network traffic is a key skill in Security Operations Centre (SOC) environments.

---

## Skills Developed

* Network traffic analysis
* Packet inspection
* Threat identification
* Use of Wireshark for monitoring
## Evidence

### Packet Capture Overview
![Overview](../screenshots/wireshark-overview.png)

### DNS Traffic Analysis
![DNS Filter](../screenshots/wireshark-dns-filter.png)
