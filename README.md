# Task 5: Capture and Analyze Network Traffic Using Wireshark

## Objective
Capture live network packets and identify basic protocols and traffic types.

## Tool Used
- Wireshark (https://www.wireshark.org/)

---

## Steps Followed

### 1. Install Wireshark
Wireshark was downloaded and installed from the official website. It is an open-source network protocol analyzer used for network troubleshooting and analysis.

### 2. Start Packet Capture
- Wireshark was launched.
- The active network interface (e.g., Ethernet or Wi-Fi) was selected.
- Packet capture was started using the "Start Capturing Packets" button.

### 3. Generate Network Traffic
- A website (www.google.com) was opened in the browser to generate traffic.
- This action triggered protocols such as HTTP, TCP, DNS, and ARP.

### 4. Stop Packet Capture
- The capture was stopped after approximately 1 minute using the red "Stop" button in Wireshark.

### 5. Filter Packets by Protocol
The following display filters were applied in Wireshark to analyze specific types of traffic:
- `http` for HTTP traffic
- `tcp` for TCP communications
- `dns` for DNS queries and responses
- `arp` for ARP requests and replies

### 6. Protocols Identified

#### a. HTTP (Hypertext Transfer Protocol)
- Used for web browsing.
- Example: GET request to `www.google.com`.
- Includes headers like Host, User-Agent, and Accept.

#### b. TCP (Transmission Control Protocol)
- Handles data transport and connection management.
- Example: SYN, ACK, and FIN packets were captured during handshake and termination.

#### c. DNS (Domain Name System)
- Resolves domain names to IP addresses.
- Example: Query and response for `www.google.com`.

#### d. ARP (Address Resolution Protocol)
- Resolves IP addresses to MAC addresses on the local network.
- Example: ARP request like "Who has 192.168.0.103? Tell 192.168.0.1".

### 7. Export the Capture
- The captured traffic was saved as a `.pcap` file via:
  - File > Save As
  - File name: `Captured_Packets.pcap`

---

## Summary of Findings

| Protocol | Function          | Example Packet Details                  |
|----------|-------------------|-----------------------------------------|
| HTTP     | Web traffic       | GET request to www.google.com           |
| TCP      | Data transport    | SYN, ACK, FIN packets                   |
| DNS      | Name resolution   | Query for www.google.com                |
| ARP      | MAC resolution    | Who has 192.168.0.103? Tell 192.168.0.1 |

---

## Deliverables
- `.pcap` file: `Captured_Packets.pcap`
- Screenshots: Attached in the GitHub repository
- Report: See `Task 5.pdf` for detailed documentation
