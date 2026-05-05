TCP Three-Way Handshake Analysis
Description:
This lab demonstrates the fundamental TCP Three-Way Handshake process between a local host (172.20.10.5) and a remote server (142.251.157.119).

SYN: The client initiates the connection with a [SYN] packet to port 443 (HTTPS).

SYN-ACK: The server responds with [SYN, ACK] to acknowledge the request.

ACK: The client completes the handshake with an [ACK] packet.

Analysis: The capture also shows the subsequent TLS 1.3 handshake, including the Client Hello and Change Cipher Spec messages, indicating the establishment of an encrypted session.

2. DNS Query and Response Mapping
Description:
This analysis focuses on the Domain Name System (DNS) protocol, specifically an AAAA (IPv6 address) record request for facebook.com.

Query: The client (172.20.10.5) sends a Standard Query for the AAAA record of facebook.com to the gateway (172.20.10.1).

Response: The DNS server responds with a Standard query response, providing the IPv6 address 2a03:2880:f167:81:face:b00c:0:25de.

Key Detail: The transaction ID 0x526b is used to match the specific request to its corresponding response.

3. HTTP GET Request & Redirection
Description:
This lab captures an unencrypted HTTP/1.1 session, highlighting how browsers request resources from web servers.

Request: The user agent (Firefox on Linux) sends an HTTP GET request for a favicon (/favicon.ico) from the host coolglowingastoundingstars.neverssl.com.

Traffic Flow: The capture shows various HTTP status codes, including 200 OK for successful data retrieval and 301 Moved Permanently, which demonstrates how servers redirect traffic to different URIs.
