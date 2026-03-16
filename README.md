# Network Traffic Monitoring & Protocol Analysis

## Project Overview
This project focused on using **Wireshark** to capture, analyze, and interpret real-time network traffic. The goal was to understand protocol behavior, identify traffic patterns (TCP, TLS, DNS), and verify security best practices within a network environment.

---

## Technical Skills Demonstrated
* **Packet Capture:** Utilized Wireshark and TCPdump to monitor live network interfaces.
* **Protocol Analysis:** Inspected the **TCP 3-Way Handshake** and validated encrypted **TLS** sessions.
* **Traffic Identification:** Analyzed DNS queries and response times to troubleshoot name resolution.
* **Security Hardening:** Correlated packet-level data with security events like firewall blocks and connection resets.

---

## Analysis Workflow

### 1. Protocol Identification
Captured and filtered various traffic types to understand application communication:
* **TCP:** Observed reliable data transmission and session management.
* **TLS:** Verified encrypted web browsing sessions to ensure data privacy.
* **DNS:** Monitored domain name resolution requests from the local machine to external servers.

![Wireshark Traffic Capture](images/traffic_capture.png)

### 2. Connection Analysis (TCP Handshake)
Documented the standard 3-way handshake process:
1. **SYN:** Client request to synchronize.
2. **SYN-ACK:** Server acknowledgment of the request.
3. **ACK:** Final connection establishment.

### 3. Security Reflection & Best Practices
Based on the traffic analysis, I documented the necessity for:
* **Intrusion Detection Systems (IDS/IPS):** To automate the detection of malicious patterns identified during manual analysis.
* **Network Segmentation:** Using VLANs and ACLs to minimize the attack surface.
* **Encryption:** Ensuring all sensitive traffic is wrapped in TLS to prevent man-in-the-middle (MITM) attacks.

---

## Tools Used
* **Wireshark:** Deep packet inspection and protocol analysis.
* **Linux (Ubuntu):** Host environment for traffic generation.
* **Docker:** Used to simulate service-based traffic.
