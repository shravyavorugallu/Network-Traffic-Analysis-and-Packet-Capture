# Network-Traffic-Analysis-and-Packet-Capture Project

## Overview
This project focuses on network traffic analysis and packet capture using various tools, including **Wireshark** and **tcpdump**. The goal is to provide hands-on experience in network packet analysis, filtering, and traffic examination, crucial for network administrators, cybersecurity analysts, and system administrators. The project covers multiple labs with different tasks that aim to build a deep understanding of network traffic, DNS requests, HTTP content, packet capture, and filtering techniques.

## Table of Contents
1. [Lab 1: Wireshark and Network Traffic Analysis](#lab-1-wireshark-and-network-traffic-analysis)
2. [Lab 2: Packet Capture Analysis](#lab-2-packet-capture-analysis)
3. [Lab 3: Tcpdump](#lab-3-tcpdump)
4. [Lab 4: Wireshark Display Filters](#lab-4-wireshark-display-filters)
5. [Lab 5: BPF Syntax](#lab-5-bpf-syntax)
6. [Tools and Technologies Used](#tools-and-technologies-used)
7. [Conclusion](#conclusion)

## Lab 1: Wireshark and Network Traffic Analysis
In this lab, the focus was on understanding **Wireshark**, a powerful network traffic analysis tool. The lab included tasks such as:
- Setting up Wireshark
- Filtering network traffic by SMTP, ICMP, and HTTP protocols
- Analyzing packet details like IP addresses, timestamps, and protocol types

Key findings from the lab:
- **Resolved vs Unresolved Ports**: Resolved ports display service names, while unresolved ports show only the port numbers.
- **Wireshark Filters**: Filters like `tcp.port eq 25 or icmp` help isolate specific traffic types.

## Lab 2: Packet Capture Analysis
This lab involved analyzing a packet capture file to extract key information from network traffic. Tasks included:
- **DNS Request Analysis**: Identifying server names and IP addresses from DNS requests.
- **Browser User Agent Analysis**: Extracting user agent strings from HTTP requests.
- **Web Server Analysis**: Identifying web server engines.
- **Content and Query Analysis**: Extracting content from HTTP responses and analyzing search queries.

Key findings:
- DNS requests map domain names to IP addresses.
- HTTP traffic can reveal user search intentions and web server details.

## Lab 3: Tcpdump
This lab provided an in-depth look at **tcpdump**, a command-line packet analysis tool. Tasks included:
- **Reading and Writing PCAP Files**: Using `-w` to write packets to a file.
- **Listing Available Interfaces**: Using `-D` to list network interfaces.
- **Filtering Packets**: Filtering packets by IP address, port, and protocol.

Key findings:
- Tcpdump is a powerful tool for filtering and capturing network traffic.
- Writing captured packets to files and verifying them using MD5 sums is essential for network forensics.

## Lab 4: Wireshark Display Filters
In this lab, we explored advanced filtering techniques in Wireshark:
- **Filtering SMTP Traffic**: Using filters to search for specific content like "Subject: ".
- **Filtering UDP Packets**: Isolating traffic based on source ports.
- **Using Slice Expressions**: Filtering specific sections of a packet for detailed analysis.

Key findings:
- Wireshark filters are essential for isolating specific traffic patterns, especially in large capture files.
- Complex filtering using slice expressions helps pinpoint exact data in packets.

## Lab 5: BPF Syntax
The focus of this lab was on **Berkeley Packet Filter (BPF)** syntax, a powerful tool for capturing and filtering network traffic:
- **Understanding BPF**: BPF allows for efficient filtering of network traffic at the capture level.
- **Creating Complex Filters**: Using BPF expressions to isolate traffic based on IP addresses, ports, and specific packet contents.

Key findings:
- BPF is an efficient and low-level filtering method used in tools like tcpdump and Wireshark.
- BPF expressions are composed of primitives and operators that allow for precise filtering.

## Tools and Technologies Used
- **Wireshark**: A GUI-based network protocol analyzer.
- **tcpdump**: A command-line packet analyzer.
- **BPF (Berkeley Packet Filter)**: A low-level filtering tool for network traffic.
- **PCAP Files**: Packet capture files used for analysis.

## Conclusion
This project provided hands-on experience with network traffic analysis and packet capture tools. By working with Wireshark, tcpdump, and BPF, we gained valuable skills in:
- Analyzing and filtering network traffic
- Extracting key information from DNS, HTTP, and SMTP packets
- Understanding low-level packet filtering using BPF

These skills are essential for anyone working in network security, system administration, or cybersecurity analysis. The ability to analyze and interpret network traffic is crucial for identifying anomalies, troubleshooting network issues, and enhancing overall network security.

---
