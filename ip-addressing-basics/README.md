# 📡 IP Addressing Basics (Cybrary Lab)

This Readme documents my work on the **IP Addressing Basics** lab completed on Cybrary using GNS3. 

---

## 🧠 What I Learned

- How the **TCP/IP model** works and how it compares to OSI
- Basics of **IP addressing**, including IPv4 structure and subnet masks
- The role of **routers**, **gateways**, and the **default route**
- How **ARP** resolves IP addresses to MAC addresses within a subnet
- How to inspect live network behavior with tools like `ping`, `ifconfig`, `ip a`, `netstat -r`, and Wireshark

---

## 🖥️ Lab Tools

- **GNS3**: Used to simulate a full network topology with routers, switches, and Linux hosts
- **Linux CLI**: Ran commands to view and troubleshoot configurations
- **Wireshark**: Captured live ARP traffic to understand how local device discovery works

---

## 🧪 Key Lab Activities

| Task                      | Tools Used             | Key Takeaway |
|---------------------------|------------------------|--------------|
| Analyzed IP/Subnet setup  | `ifconfig`, `ip a`     | Understood how networks are segmented |
| Verified routes/gateways  | `netstat -r`           | Saw default gateway logic in action |
| Tested connectivity       | `ping`                 | Verified reachability between networks |
| Inspected ARP cache       | `arp -a`               | Learned that ARP is only for local subnet |
| Captured ARP traffic      | Wireshark              | Saw how MAC/IP resolution works behind the scenes |

---
