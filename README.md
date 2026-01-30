# Wireshark DNS Investigation Lab

## Overview
This project demonstrates a SOC-style DNS traffic investigation using Wireshark.  
I analyzed a malware-related PCAP dataset from Malware-Traffic-Analysis.net to identify abnormal DNS query behavior and validate suspicious-looking activity.

---

## Skills Demonstrated
- DNS traffic filtering and analysis
- Long DNS query detection (tunneling indicators)
- Host-to-resolver conversation analysis
- Noise reduction and domain validation
- Incident-style documentation and reporting

---

## Key Findings
- Workstation IP: **10.1.17.215**
- DNS Resolver IP: **10.1.17.2**
- Total DNS packets observed: **~39,427**
- Long DNS queries detected: **46**
- Long queries confirmed as legitimate Active Directory lookups (not tunneling)

---

## Filters Used

### Baseline DNS Filter
```wireshark
dns

