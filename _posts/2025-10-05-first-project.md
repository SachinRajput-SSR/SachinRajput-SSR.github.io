---
title: "Building My First Port Scanner: A Beginner's Journey into Cybersecurity"
date: 2025-10-05
last_modified_at: 2025-10-05
categories:
  - Projects
  - Python
  - Cybersecurity
tags:
  - port-scanner
  - python
  - networking
  - ethical-hacking
  - CEH
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/blog-header.jpg
excerpt: "Learn how I built my first cybersecurity project: a multi-threaded Python port scanner. Discover the concepts, challenges, and lessons learned."
---

<style>
  .blog-highlight {
    background: linear-gradient(135deg, rgba(102, 126, 234, 0.2) 0%, rgba(124, 58, 237, 0.2) 100%);
    padding: 20px;
    border-radius: 8px;
    border-left: 4px solid #4ade80;
    margin: 20px 0;
  }

  .blog-code {
    background: #0f172a;
    border: 1px solid #334155;
    border-radius: 8px;
    padding: 15px;
    overflow-x: auto;
  }
</style>

## Introduction

As part of my cybersecurity learning journey, I recently completed my first hands-on project: a **Python-based port scanner**. This project taught me fundamental networking concepts, socket programming, and reconnaissance techniques aligned with the **CEH v13 curriculum**. In this blog post, I'll share my experience, the concepts I learned, and the challenges I faced.

---

## 🎯 What is a Port Scanner?

A port scanner is a cybersecurity tool that probes network hosts to identify open ports and running services. It's one of the first steps in **reconnaissance** during penetration testing.

### Why Port Scanning Matters

1. **Reconnaissance:** Identify active services on target networks
2. **Vulnerability Assessment:** Discover potential attack surfaces
3. **Network Mapping:** Understand network architecture
4. **CEH Foundation:** Core concept in ethical hacking curriculum

---

## 🏗️ Project Overview

### What I Built

I created two versions of a port scanner:

1. **Basic Scanner** - Simple, single-threaded implementation for learning
2. **Advanced Scanner** - Multi-threaded with banner grabbing and CLI

### Key Features

✅ Multi-threaded port scanning for performance  
✅ Banner grabbing to identify services  
✅ Customizable port ranges  
✅ Results export to file  
✅ Command-line interface with argument parsing  

---

## 📚 Concepts Learned

### 1. Networking Fundamentals

<div class="blog-highlight">
<strong>TCP/IP Basics:</strong> Learned how TCP three-way handshake works and how connection attempts reveal port status.
</div>

- **TCP Ports:** 0-1023 (well-known), 1024-49151 (registered), 49152-65535 (dynamic)
- **Common Services:** HTTP (80), HTTPS (443), SSH (22), FTP (21), DNS (53)
- **Connection Status:** Open, Closed, Filtered

### 2. Python Socket Programming

<div class="blog-highlight">
<strong>Socket Library:</strong> Python's socket library provides low-level networking interfaces.
</div>

``` python

import socket

#Create a socket object
sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)

#Set timeout
sock.settimeout(1)

#Attempt connection
result = sock.connect_ex(('target_ip', port))
sock.close()

#Check result
if result == 0:
  print(f"Port {port}: Open")

```
### 3. Threading & Concurrency

<div class="blog-highlight">
<strong>Multi-threading:</strong> Scanning 65,535 ports sequentially takes too long. Threading enables scanning multiple ports simultaneously.
</div>

```python
import threading

def scan_port(target, port):
  # Scanning logic here
  pass

# Create threads for concurrent scanning
threads = []
for port in range(1, 1025):
  thread = threading.Thread(target=scan_port, args=(target, port))
  threads.append(thread)
  thread.start()

# Wait for all threads
for thread in threads:
  thread.join()
```

---

## 🛠️ Implementation Details

### Architecture
```
Port Scanner
├── Main Function
│ ├── Argument Parsing
│ ├── IP Resolution
│ └── Scan Initialization
├── Scan Function
│ ├── Thread Management
│ ├── Socket Connection
│ └── Result Collection
└── Utility Functions
├── Banner Grabbing
├── Service Identification
└── Results Export
```


### Code Structure

The project follows clean coding practices:
- **Modular Design:** Separate functions for different tasks
- **Error Handling:** Try-except blocks for network errors
- **Threading Pool:** Efficient thread management
- **Results Logging:** Organized output with progress tracking

---

## 🎨 Features Explained

### 1. **Multi-Threading**
```python
class PortScanner:
def init(self, target, threads=100):
self.threads = threads
self.lock = threading.Lock()

def run_scan(self):
    threads = []
    for port in range(self.start_port, self.end_port + 1):
        thread = threading.Thread(target=self.scan_port, args=(port,))
        threads.append(thread)
        thread.start()
        
        # Limit concurrent threads
        if len(threads) >= self.threads:
            for t in threads:
                t.join()
            threads = []
```

**Why it matters:** Scanning 65,535 ports sequentially takes hours. With threading, we can scan 100 ports concurrently, reducing time to minutes.

### 2. **Banner Grabbing**

```python
def grab_banner(self, sock, port):
  try:
    if port in :
      sock.send(b"GET / HTTP/1.1\r\nHost: ...\r\n\r\n")
    else:
      sock.send(b"\r\n")
      banner = sock.recv(1024).decode('utf-8', errors='ignore')
      return banner[:50]
  except:
    return ""
```

**What it does:** Attempts to grab service information by sending probe requests and capturing responses. Helps identify running services.

### 3. **Service Identification**

```python
def get_service_name(self, port):
  services = {
21: "FTP", 22: "SSH", 23: "Telnet",
25: "SMTP", 53: "DNS", 80: "HTTP",
110: "POP3", 143: "IMAP", 443: "HTTPS",
3306: "MySQL", 5432: "PostgreSQL", 3389: "RDP"
}
  return services.get(port, "Unknown"
```

---

## 🚧 Challenges Faced

### Challenge 1: Performance

**Problem:** Single-threaded scanning was too slow  
**Solution:** Implemented multi-threading with configurable thread count  
**Learning:** Understanding concurrency and thread synchronization

### Challenge 2: Timeout Management

**Problem:** Hanging on filtered ports  
**Solution:** Set appropriate timeouts (0.5-1 second)  
**Learning:** Balancing speed vs. accuracy

### Challenge 3: Banner Grabbing Reliability

**Problem:** Different services respond differently  
**Solution:** Service-specific probes and error handling  
**Learning:** Network communication protocols and service behavior

---

## 📊 Test Results

I tested the scanner on my local network:

- **Target:** 192.168.1.0/24
- **Ports Scanned:** 1-1024
- **Time Taken:** ~2 minutes (with 100 threads)
- **Open Ports Found:** 5-10 per device
- **Services Identified:** HTTP, SSH, DNS, NetBIOS, etc.

### Sample Output
[+] Port 22: SSH (OpenSSH 7.4)
[+] Port 80: HTTP (Apache httpd 2.4.6)
[+] Port 443: HTTPS
[+] Port 53: DNS
[+] Port 3306: MySQL

---

## 🎓 Key Learnings

1. **Networking:** Understanding how TCP connections work and port status
2. **Python:** Socket programming, threading, OOP principles
3. **Cybersecurity:** Reconnaissance techniques and their importance
4. **Problem-Solving:** Debugging network issues and optimizing performance
5. **Best Practices:** Error handling, clean code, documentation

---

## ✅ CEH Alignment

This project directly supports the **CEH v13 certification**:

- **Module:** Footprinting and Reconnaissance
- **Concepts:** Network scanning, service enumeration, protocol analysis
- **Practical Skills:** Using reconnaissance tools and techniques
- **Real-World Application:** Essential first step in penetration testing

---

## 🔗 GitHub Repository

Check out the complete project on GitHub:

**[Port Scanner Project](https://github.com/SachinRajput-SSR/port-scanner-project)**

The repository includes:
- ✅ Complete source code
- ✅ Detailed README
- ✅ Usage examples
- ✅ MIT License

---

## 📈 Next Steps

This project has prepared me for:
- Advanced scanning techniques (SYN scan, UDP scanning)
- Vulnerability assessment tools
- Network security concepts
- Penetration testing methodologies

**Next Project:** Personal Website Security Audit (coming soon!)

---

## 🤝 Let's Connect

I'm excited about my cybersecurity journey and always open to:
- 💬 Technical discussions
- 🤝 Collaborations
- 📚 Knowledge sharing
- 💼 Mentorship opportunities

[💼 LinkedIn](https://www.linkedin.com/in/sachin-singh-tanwar-5582582b4/) | [📧 Email](mailto:your-email@example.com) | [🐙 GitHub](https://github.com/SachinRajput-SSR)

---

**Happy Hacking! 🎯**

*Published: {{ page.date | date: "%B %d, %Y" }}*  
*Updated: {{ page.last_modified_at | date: "%B %d, %Y" }}*
