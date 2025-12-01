# Network-Traffic-Analysis-Toolkit

# Network Traffic & Vulnerability Analysis Portfolio

A professional cybersecurity portfolio demonstrating practical skills in **Nmap scanning**, **network traffic analysis**, **tcpdump**, **Wireshark**, and **web fuzzing (FFUF)**. This repository is designed to showcase hands-on capability for **penetration testing**, **bug bounty**, and **network security** roles.

---

## Project Description

This project contains structured, real-world examples of analyzing networks, understanding protocols, identifying hosts, capturing packets, and performing reconnaissance similar to early-stage penetration testing.

The goal is to demonstrate:

* Ability to enumerate networks safely
* Ability to analyze packet-level behavior
* Understanding of normal vs suspicious traffic
* Ability to use industry-standard tools (Nmap, tcpdump, Wireshark, FFUF)
* Professional documentation and reporting

---

## Tools Used

* **Nmap** — Host discovery and service enumeration
* **tcpdump** — CLI packet capture and filtering
* **Wireshark** — Deep packet inspection and protocol analysis
* **FFUF** — Web fuzzing and directory enumeration

---

## Nmap Scan

### Command Used

```
nmap -sn 192.168.1.0/24
```

### Reason for Using This Command

The `-sn` (ping scan) option is used to:

* Discover active hosts without port scanning
* Understand the size and structure of the local network
* Safely enumerate devices without being intrusive

### Analysis Result

* Identified active hosts
* Mapped local network topology
* Detected reachable devices for further analysis

### Cybersecurity Relevance

This mirrors real penetration-testing reconnaissance:

* Identifying potential targets
* Understanding attack surfaces
* Detecting unknown or rogue devices

---

## tcpdump Analysis

### Command Used

```
tcpdump -i wlan0 -vvv -w capture.pcap
```

### Reason for Using This Command

* Capture raw packet data on the interface
* Monitor DNS, ARP, and TCP handshake behavior
* Produce a PCAP file for deeper inspection in Wireshark

### Analysis Result

* Identified DNS queries and outbound connections
* Observed TCP handshakes and device communication patterns

### Cybersecurity Relevance

This helps detect:

* Suspicious outbound traffic
* Misconfigured services
* Malware beaconing behavior

---

## Wireshark Analysis

### Process

* Loaded captured PCAP
* Applied filters (e.g., `http`, `tcp.flags.syn==1`, `dns`) to isolate protocol behavior

### Findings

* Clear understanding of network interactions
* Visualization of packets for learning and documentation

### Cybersecurity Relevance

Wireshark is essential for:

* Incident response
* Malware traffic analysis
* Network troubleshooting

---

## FFUF Web Fuzzing

### Command Used

```
ffuf -u https://target.com/FUZZ -w wordlist.txt -mc 200
```

### Reason for Using This Command

* Enumerate hidden directories or files
* Identify potential attack points (admin panels, backups, APIs)

### Analysis Result

* Discovered accessible paths
* Identified resources that may expose sensitive functionality

### Bug Bounty Relevance

Directory fuzzing helps find:

* IDOR endpoints
* Hidden API routes
* Misconfigured web services

---

## Contac

Name: Rifqi Subhan
Email: rifkisubhan89@gmail.com
Phone: +62 821-2381-1711
Location: Indonesia
GitHub: https://github.com/RifqiSubhan

## Conclusion

This repository demonstrates hands-on, practical cybersecurity skills across reconnaissance, packet analysis, and web fuzzing. All examples are created in a safe, controlled environment, suitable for:

* Cybersecurity job applications
* Bug bounty beginner portfolios
* SOC and penetration testing entry-level positions

If you are a recruiter reviewing this portfolio, this repository highlights real technical capabilities, not just theoretical knowledge.
