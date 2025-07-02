# yoyoyoyo

# 🛠️ Fundamental Network Troubleshooting (Module 2)

## 📘 Overview

This hands-on project is designed to build essential skills in diagnosing and resolving common network issues in a Windows environment. You’ll learn how to use command-line tools to analyze IP configurations, test connectivity, troubleshoot DNS resolution, and simulate basic firewall behaviors — all within a controlled VirtualBox lab setup.

---

## 🧰 Tools & Technologies

- **OS Environment**: Windows 10 (Client)
- **Virtualization**: Oracle VirtualBox
- **Utilities**: Command Prompt (CMD)

---

## 🚦 Learning Objectives

By the end of this project, you will be able to:

- Examine and interpret IP configurations using `ipconfig`
- Release, renew, and flush DNS settings to resolve IP or name issues
- Test network connectivity using tools like `ping`, `tracert`, and `nslookup`
- Simulate firewall-related connectivity issues
- Understand NAT and port forwarding behavior in virtualized environments

---

## 🧪 Lab Walkthrough

### 🔹 Part 1: Network Configuration Analysis

**Command: `ipconfig`**

- Displayed both basic and detailed configuration: IP Address, Subnet Mask, Default Gateway, and DNS servers.

<p align="center">
<img src="https://i.imgur.com/31.png" height="80%" width="80%" alt="IPConfig Basic and All"/>
</p>

**Command: `ipconfig /release`, `ipconfig /renew`, `ipconfig /flushdns`**

- Released and renewed IP addresses from the DHCP server.
- Cleared the DNS cache to remove outdated or corrupted entries.

<p align="center">
<img src="https://i.imgur.com/32.png" height="80%" width="80%" alt="IPConfig Release Renew FlushDNS"/>
</p>

---

### 🔹 Part 2: Testing Network Connectivity

**Command: `ping`**

- Tested various points of connectivity:
  - `127.0.0.1` (loopback)
  - Default gateway
  - Public IP (`8.8.8.8`)
  - Domain (`google.com`)

<p align="center">
<img src="https://i.imgur.com/33.png" height="80%" width="80%" alt="Ping Tests"/>
</p>

**Commands: `tracert`, `nslookup`**

- `tracert` was used to visualize the route taken by packets to reach a target.
- `nslookup` verified DNS resolution and queried specific DNS servers.

<p align="center">
<img src="https://i.imgur.com/34.png" height="80%" width="80%" alt="Tracert and Nslookup"/>
</p>

---

### 🔹 Part 3: Simulating Firewall Behavior

**Scenario: ICMP Block via Windows Defender Firewall**

- Inbound ICMP rules were disabled to simulate a blocked ping.
- Host-to-VM ping resulted in “Request timed out,” mimicking real-world firewall behavior.

<p align="center">
<img src="https://i.imgur.com/35.png" height="80%" width="80%" alt="Firewall Blocking Ping"/>
</p>

> 🔧 **To-Do**: Set up NAT port forwarding in VirtualBox and test inbound ping success.
>  
> ✅ Add screenshots and success confirmation once configured.

---

## 🧠 Skills Demonstrated

### 🖥️ Windows Administration
- IP configuration & DHCP lease control
- DNS cache troubleshooting
- Local firewall rule management

### 🌐 Networking Fundamentals
- TCP/IP model understanding
- DNS query resolution
- ICMP and packet routing analysis
- NAT and virtualized network mapping

### 🔒 Security Awareness
- Understanding firewall behavior
- Simulating access control scenarios (ping blocking)
- Recognizing effects of blocked inbound traffic

### 📟 Command-Line Proficiency
- `ipconfig`
- `ping`
- `tracert`
- `nslookup`

### ☁️ Virtualization
- Virtual machine setup in VirtualBox
- NAT mode networking
- Port forwarding (pending completion)

---

## 📁 Repository Structure


