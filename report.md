# Wireshark DNS Investigation Lab (Fake Software Download Case)

## Overview
This project demonstrates a SOC-style DNS traffic investigation using Wireshark.  
I analyzed a malware-related PCAP dataset from Malware-Traffic-Analysis.net to practice identifying abnormal DNS behavior and validating suspicious-looking queries.

---

## Key Findings
- Workstation IP: **10.1.17.215**
- DNS Server IP: **10.1.17.2**
- Total DNS packets observed: **~39,427**
- Long DNS query packets detected: **46**
- Long queries were confirmed as legitimate Active Directory service lookups (not DNS tunneling)

---

## Investigation Steps Performed

### Baseline DNS Filter
```wireshark
dns
