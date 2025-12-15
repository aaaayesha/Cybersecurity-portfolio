# TCP SYN Flood Denial-of-Service Attack Analysis

## Project Overview
This project documents the analysis of a network interruption caused by a denial-of-service (DoS) attack targeting a web server. Packet-level evidence was analyzed to identify a TCP SYN flood attack and explain its impact on website availability.

## Scenario
An automated monitoring alert indicated abnormal behavior on a company web server. Employees attempting to access the website experienced connection timeout errors. Network traffic analysis revealed an unusually high volume of TCP SYN requests originating from a single unfamiliar IP address.

## Tools Used
- Wireshark
- TCP/IP protocol analysis
- Network traffic inspection

## Attack Identified
**TCP SYN Flood (Denial-of-Service Attack)**

## Key Findings
- Excessive TCP SYN packets targeting port 443
- Incomplete TCP three-way handshakes
- Server resources exhausted by half-open connections
- Legitimate users experienced connection timeouts and service disruption

## Impact
The attack overwhelmed the web server, preventing it from responding to legitimate traffic and causing website downtime.

## Skills Demonstrated
- Network attack identification
- TCP traffic analysis
- Denial-of-service attack analysis
- Incident documentation and reporting

## Disclaimer
This project is based on a simulated incident scenario and is intended for educational and portfolio demonstration purposes.
