# DNS and ICMP Network Traffic Incident Analysis

## Project Overview
This project documents the investigation of a network connectivity incident where users were unable to access a website due to DNS resolution failure. A network protocol analyzer (tcpdump) was used to examine DNS and ICMP traffic and identify the root cause.

## Scenario
Users reported receiving a “destination port unreachable” error when attempting to access `www.yummyrecipesforme.com`. Initial testing confirmed the issue, prompting packet capture and analysis.

## Tools Used
- tcpdump
- DNS protocol analysis
- ICMP error analysis
- TCP/IP model

## Key Findings
- DNS queries were sent via UDP to port 53.
- The DNS server returned ICMP messages stating “udp port 53 unreachable.”
- DNS resolution failed, preventing website access.

## Suspected Root Cause
The DNS service on the destination server was unavailable or UDP port 53 was blocked by a firewall or access control rule.

## Skills Demonstrated
- Network traffic analysis
- DNS troubleshooting
- ICMP interpretation
- Incident documentation
- Technical reporting

## Evidence

This project includes representative tcpdump log output demonstrating
DNS queries sent to UDP port 53 and corresponding ICMP error messages
indicating that the port was unreachable.

## Disclaimer
This project is based on a simulated incident scenario and is intended for educational and portfolio demonstration purposes.
