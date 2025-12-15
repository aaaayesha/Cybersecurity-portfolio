# Cybersecurity Incident Report

## Section 1: Identify the type of attack that may have caused this network interruption

One potential explanation for the website’s connection timeout error message is a
denial-of-service (DoS) attack. The logs show that the web server stops responding
after being overloaded with TCP SYN packet requests. This behavior is consistent
with a DoS attack known as a TCP SYN flood.

## Section 2: Explain how the attack is causing the website to malfunction

When website visitors attempt to establish a connection with the web server, a
three-way handshake occurs using the TCP protocol. The handshake consists of
three steps:

1. A SYN packet is sent from the source to the destination requesting a connection.
2. The destination replies with a SYN-ACK packet and reserves system resources
   for the connection.
3. A final ACK packet is sent from the source to the destination acknowledging
   the connection.

In a SYN flood attack, a malicious actor sends a large number of SYN packets
without completing the handshake process. This creates numerous half-open
connections and exhausts the server’s available resources.

As a result, the web server becomes unable to process legitimate connection
requests. Visitors experience connection timeout errors, and the website becomes
unavailable.
