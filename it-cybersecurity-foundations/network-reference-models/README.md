##  Summary

In this lab I explored how data is transmitted across networks using the OSI and TCP/IP models. I used Wireshark to inspect real captured packets and trace how each layer of data is encapsulated and decapsulated in practice.

---

##  Key Concepts Learned

 Structure and purpose of the OSI (7-layer) and TCP/IP (4-layer) models  
 How encapsulation adds headers/trailers at each layer  
 How Wireshark displays each protocol layer from Physical to Application  
 How to analyze key protocols and data fields in a real packet capture

---

##  Protocols & Layers Analyzed

| OSI Layer | Example Protocols | What I Saw in Wireshark |
|-----------|--------------------|--------------------------|
| 7 - Application | HTTP | Request/Response content |
| 4 - Transport | TCP | Source/destination ports, sequence numbers |
| 3 - Network | IPv4 | Source/destination IPs |
| 2 - Data Link | IEEE 802.11 | MAC addresses, Beacon frames |
| 1 - Physical | Radiotap | Channel, frequency, signal strength |

---

##  Lab Outcome

- Used **display filters** (`tcp`) to isolate meaningful packets  
- Traced a full **HTTP request and response** across all layers  
- Located the flag `{CLAB-Practicum}` inside an HTTP response  
- Learned to differentiate between broadcast beacons (Layer 1-2 only) and actual traffic (Layer 3-7)

---
