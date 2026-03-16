
## Job 02 - ID 02

## Introduction

Like the job 01, a host has been compromised, we need to find the compromised assets, user, ips, domains...

## Examination

### Evidence

.pcap network dump showing multiple suspect communication towards a suspicious address.

### Tools used (./tools.md for a more in-depth tool explanation)

Wireshark, Shodan.io

## Conclusion

### IOC

172.17.0.99 is infected with a Stealer malware and contacts a C2 periodically

#### Domains reached:

46.254.34.201

### Possible remediation ?

Monitoring network traffic, firewall rules, file integrity monitoring, network isolation of the computer and full reset.
