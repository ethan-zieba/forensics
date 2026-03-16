## Case name and ID

## Introduction

A host has been compromised, we need to find the compromised assets, user, ips, domains...

## Examination

### Evidence

.pcap network dump showing multiple suspect communication towards four public IP addresses.

### Tools used (./tools.md for a more in-depth tool explanation)

Wireshark, Shodan.io

## Conclusion

### IOC

172.16.1.66 is the compromised host's IP, account "ccolier" (Full name: Clark Collier).
The device's MAC address is `00:1e:64:ec:f3:08`, hostname `DESKTOP-SKBR25F`
Sends multiple requests to different public IPs including a STRAT server and a geolocation API (ip-api.com)
#### Domains reached:
githubusercontent.com
STRAT (141.98.10.79)
repo1.maven.org
ip-api.com

### Possible remediation ?

Monitoring network traffic, firewall rules, file integrity monitoring, network isolation of the computer and full reset.
