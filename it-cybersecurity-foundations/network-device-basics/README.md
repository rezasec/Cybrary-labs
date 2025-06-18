# Network Device Basics 

In this lab, I built and tested a simple network setup using GNS3. It included hosts, switches, a router, and a pfSense firewall. The main goal was to understand how each device works, how routing happens, how DHCP assigns IPs, and how firewalls control traffic.

---

## Lab Objective

- Examine how traffic flows within a LAN and from LAN to WAN
- Configure static routing for a newly segmented subnet
- Verify firewall rule behavior using stateful inspection
- Practice essential diagnostic tools (`ping`, `netstat`, `ifconfig`)

---

## Environment Overview

**Devices included:**
- pfSense Firewall (LAN/WAN interfaces, DHCP)
- Router (dual NICs: 192.168.1.254 and 10.10.10.1)
- Linux hosts (Linux-1, Linux-2, firefox)
- ISP node and simulated Web server
- Two LAN switches

---

## Key Technical Tasks

- Configured DHCP server on pfSense for LAN clients
- Verified address assignments and gateway settings via CLI
- Routed traffic from a new subnet (10.10.10.0/24) through a router to the firewall
- Added static routes and adjusted firewall rules to enable bidirectional traffic
- Tested routing and rule behavior using ping across network segments

---

## Security Context

- Demonstrated how a stateful firewall handles return traffic without explicit inbound rules
- Highlighted the importance of routing awareness in multi-subnet environments
- Simulated real world misconfigurations 
- Practiced proper use of allow rules and default deny strategies

---
