# Wireshark Network Traffic Analysis

This project explores basic packet capture and traffic analysis using Wireshark. As part of my cybersecurity learning journey, I captured and inspected HTTP/S traffic from common websites to identify key protocols, packet flows, and security headers.

## Tools Used
- Wireshark (macOS version)
- Browser (Safari/Chrome)

## Capture Details
I captured 11 seconds of live traffic while visiting:
- [https://owasp.org](https://owasp.org)
- [https://yahoo.com](https://yahoo.com)

The `.pcapng` file was saved and uploaded for analysis. It contains both HTTP and HTTPS traffic, DNS queries, and TLS handshake data.

> Capture file size was kept small for GitHub upload compatibility.

## Skills Practiced
- Identifying DNS queries and IP resolutions
- Observing TCP 3-way handshakes
- Analyzing TLS handshake details (e.g. SNI, cipher suites)
- Filtering traffic using Wireshark display filters:
  - `http`, `tls`, `ip.addr == 104.16.133.229`, etc.

## What I Learned
- HTTPS encrypts payloads, but you can still observe metadata
- OWASP implements strong TLS security
- TLS handshake shows which server was contacted and which cipher suites were negotiated
- DNS lookups can reveal all domains contacted by a user, even on secure sites

## Next Steps
- Analyze packet flags and TCP stream behavior
- Capture malicious or suspicious traffic (via test labs)
- Create custom Wireshark filters to identify threat indicators

---

Feel free to fork or recreate this project to improve your own network analysis skills.
