# HTTP Analysis Using Wireshark (Text Traffic)

## Course Information

- **Course:** SBT-DF203 - Basic Computer Skills for Digital Forensics
- **Lab Title:** HTTP Analysis Using Wireshark - Text Traffic
- **Student:** Ibrahim Diseh Garba
- **Student ID:** 2025/FWSD/11521
- **Instructor:** Aminu Idris, AMCPN (CCNA, CompTIA Security+, CEH, OSCP, CISSP, CISM)
- **Date Submitted:** 8 September 2026

---

## Overview

This repository contains the documentation, packet captures, screenshots, and forensic analysis performed for **Lab 1: HTTP Analysis Using Wireshark (Text Traffic)**.

The objective of this exercise was to capture and analyze plaintext HTTP communication between a client and a locally hosted Apache web server using Wireshark and Tshark. The lab demonstrates fundamental networking and digital forensic concepts including:

- TCP Three-Way Handshake
- HTTP Request/Response Analysis
- Packet Reconstruction
- Network Protocol Encapsulation
- Connection Termination Analysis
- Evidence Preservation
- SHA-256 Integrity Verification

---

## Lab Objectives

- Create and host a local webpage using Apache2.
- Capture HTTP traffic on the loopback interface.
- Analyze the TCP three-way handshake.
- Identify HTTP requests and responses.
- Reconstruct communications using TCP Streams.
- Examine protocol encapsulation across network layers.
- Verify evidence integrity using SHA-256 hashes.
- Document forensic findings and observations.

---

## Environment Information

| Component | Description |
|-----------|-------------|
| Operating System | Kali Linux 2026.1 |
| Web Server | Apache2 |
| Traffic Analysis Tool | Wireshark / Tshark |
| Network Interface | Loopback (lo) |
| Protocol Analyzed | HTTP |
| Target URL | http://127.0.0.1/basic.html |

---

## Repository Structure

```text
SBT-DF203-Lab1/
├── evidence/
│   └── basic.pcapng
├── working/
│   └── basic_working.pcapng
├── exported/
├── reports/
│   ├── capture_hashes.txt
│   ├── curl_verbose.txt
│   ├── handshake.tsv
│   ├── http_requests.tsv
│   ├── http_responses.tsv
│   ├── connection_close.tsv
│   └── follow_stream.txt
├── screenshots/
│   ├── screenshot_01_folder_structure.png
│   ├── screenshot_02_apache_status.png
│   ├── screenshot_03_port80_listener.png
│   ├── screenshot_04_webpage_browser.png
│   ├── screenshot_05_curl_verbose.png
│   ├── screenshot_06_capture_running.png
│   ├── screenshot_07_hashes.png
│   ├── screenshot_08_handshake.png
│   ├── screenshot_09_syn_details.png
│   ├── screenshot_10_http_request.png
│   ├── screenshot_11_http_response.png
│   ├── screenshot_12_follow_stream.png
│   ├── screenshot_13_encapsulation.png
│   └── screenshot_14_connection_close.png
└── scripts/
    └── analysis_commands.sh
