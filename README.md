# 🌐 Network Monitoring & Packet Analysis

## 📌 Overview
This project demonstrates network traffic analysis using Wireshark and basic Linux networking tools. It focuses on understanding how DNS, HTTP, and TCP protocols work and identifying potential security risks in network communication.

---

## 🛠️ Tools Used
- Wireshark  
- Kali Linux  
- Linux Commands (netstat, ifconfig)  

---

## 🔍 DNS Packet Analysis

### Observations
- Captured DNS queries while accessing websites  
- DNS requests were sent from the local system to DNS servers  
- Domain names (e.g., google.com) were resolved into IP addresses  

### Analysis
DNS (Domain Name System) is responsible for translating domain names into IP addresses, enabling communication between clients and servers.

### ⚠️ Security Insight
- DNS traffic is unencrypted  
- Can reveal browsing activity  
- Vulnerable to DNS spoofing attacks  

---

## 🌍 HTTP Packet Analysis

### Observations
- Captured HTTP GET requests  
- Host field shows requested website  
- Data transmitted in plain text  

### Analysis
HTTP protocol does not encrypt data, making it possible to view transmitted information directly from captured packets.

### ⚠️ Security Insight
- Sensitive data can be exposed  
- Vulnerable to Man-in-the-Middle (MITM) attacks  
- Highlights need for HTTPS  

---

## 🔗 TCP Packet Analysis

### Observations
- Identified TCP 3-way handshake:
  - SYN (connection initiation)  
  - SYN-ACK (server response)  
  - ACK (connection established)  

### Analysis
TCP ensures reliable communication by establishing a connection before data transfer.

### ⚠️ Security Insight
- Can be targeted by SYN flood attacks  
- Useful in detecting abnormal traffic patterns  

---

## 🖥️ Linux Network Analysis

### Commands Used
```bash
netstat -tuln
ifconfig
