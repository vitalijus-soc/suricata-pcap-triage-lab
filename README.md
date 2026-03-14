# Suricata IDS + PCAP Triage Lab

## Overview

This lab demonstrates how Suricata IDS can detect suspicious network activity and how packet captures (PCAP) can be analyzed during incident investigation.

The goal of this project is to simulate the workflow of a SOC analyst investigating network alerts.

---

## Lab Environment

- Ubuntu Server
- Suricata IDS
- Wireshark
- PCAP traffic analysis

Suricata was configured to monitor network traffic and generate alerts based on suspicious activity detected in the PCAP file.

---

## Scenario

A packet capture containing suspicious network activity was analyzed.

Suricata processed the PCAP file and generated alerts indicating potentially malicious behavior.

The traffic was then inspected using Wireshark to understand the nature of the communication.

---

## Suricata Alert

Suricata detected suspicious traffic patterns in the PCAP file.

![Suricata Alert](screenshots/suricata_alert.png)

The alert indicates that the IDS detected activity matching known detection rules.

---

## Packet Analysis (Wireshark)

The PCAP file was opened in Wireshark to investigate the network communication.

![Wireshark Analysis](screenshots/wireshark_analysis.png)

Key observations:

- Suspicious HTTP requests
- External IP communication
- Unusual traffic patterns

---

## Suricata Logs (EVE JSON)

Suricata generated logs in EVE JSON format containing detailed event information.

![Suricata Logs](screenshots/eve_json_log.png)

These logs provide valuable telemetry for SOC analysts.

---

## Detection Value

This lab demonstrates how Suricata can be used for:

- Network intrusion detection
- Traffic inspection
- Alert generation
- Incident investigation

---

## Skills Demonstrated

- Network traffic analysis
- Suricata IDS configuration
- PCAP investigation
- SOC alert triage

---

## MITRE ATT&CK Mapping

Possible related techniques:

- T1046 – Network Service Discovery
- T1071 – Application Layer Protocol
- T1049 – System Network Connections Discovery

---

## Conclusion

This project demonstrates how network telemetry can be analyzed using Suricata IDS and Wireshark during a security investigation.

It reflects a typical SOC workflow involving detection, investigation, and traffic analysis.
