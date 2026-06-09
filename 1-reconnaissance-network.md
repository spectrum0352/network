
# Network Reconnaissance and Vulnerability Analysis

**Network Reconnaissance**
Network reconnaissance is the initial phase of an attack where attackers gather information about a target network. This information helps identify vulnerabilities and plan attack strategies.

**Network Vulnerability Analysis**
Network enumeration is the process of discovering hosts, services, and vulnerabilities on a network. It is a crucial step in penetration testing and security assessments.

**Network Scanning**
Network scanning is the process of identifying active devices on a network and gathering information about them.

Nmap is a valuable tool for network administrators and security professionals, but it must be used responsibly and with proper authorization. Always prioritize network security and avoid causing harm or disruption.

---

# Information Gathered During Network Reconnaissance

The following information may be collected during reconnaissance activities:

* Domain names (internal and external) — Examples: `example.com`, `mail.example.com`, `corp.local`, `hr.internal.example.com`

* IP addresses and network blocks — Examples: `192.168.1.10`, `203.0.113.25`, `10.0.0.0/16`, `192.168.1.0/24`

* Network protocols in use — Examples: TCP, UDP, HTTP, HTTPS, DNS, SMB, LDAP, SSH, FTP, SNMP

* Rogue or private websites — Examples: `http://dev-test.local`, `https://fileshare-company.xyz`, unauthorized internal admin portal

* Running TCP and UDP services — Examples: TCP 22 (SSH), TCP 80 (HTTP), TCP 443 (HTTPS), UDP 53 (DNS), UDP 161 (SNMP)

* Authentication methods — Examples: Password authentication, Multi-Factor Authentication (MFA), Kerberos, NTLM, LDAP authentication, Smart Cards

* Access control mechanisms and ACLs — Examples: Firewall ACL allowing only `10.0.0.0/24`, Role-Based Access Control (RBAC), file permissions, network segmentation rules

* VPN access points — Examples: `vpn.example.com`, Cisco AnyConnect gateway, OpenVPN server, IPsec VPN concentrator

* Intrusion Detection Systems (IDS) status — Examples: Snort detected, Suricata alerts enabled, IDS blocking scan attempts

* Analog and digital telephone numbers — Examples: `+1-555-0100`, PBX extension `1001`, VoIP/SIP endpoint `sip.example.com`

* Operating systems and software versions — Examples: Windows Server 2022, Ubuntu 22.04, Apache HTTP Server 2.4.58, OpenSSH 9.3, Microsoft SQL Server 2019


---

# Network Footprinting

Network footprinting is the process of gathering information about a target system or network.

The process of identifying a target’s operating system and software versions is known as TCP/IP fingerprinting.

---

# Performing Network Reconnaissance Using Packet Analysis

Performing network reconnaissance using packet analysis involves a structured approach combining technical tools and analytical skills.

## 1. Planning and Scope Definition

### Define Objectives

* Determine the information to gather:

  * Network topology
  * Active hosts
  * Running services
  * Potential vulnerabilities
* Define the scope:

  * Specific network segment
  * Target IP address
  * Entire environment

### Legal and Ethical Considerations

* Ensure proper authorization before conducting reconnaissance.
* Comply with all applicable laws and regulations.

---

## 2. Packet Capture

### Choose a Capture Tool

* Wireshark — GUI-based packet capture and analysis
* tcpdump — Command-line packet capture utility

### Select the Capture Interface

* Identify the network interface carrying target traffic.

### Enable Promiscuous Mode (if required)

* Allows capturing all traffic on a network segment.

### Capture the Traffic

* Start capturing traffic for sufficient duration.
* Use capture filters to reduce unnecessary data and focus on:

  * IP addresses
  * Ports
  * Protocols

---

## 3. Packet Analysis

### Filtering and Decoding

* Use display filters in Wireshark to isolate relevant traffic.
* Decode packets to analyze:

  * Network layer
  * Transport layer
  * Application layer

### Network Layer Analysis

* Identify active hosts and topology using IP addresses.
* Analyze IP headers and routing behavior.
* Detect unusual or suspicious traffic.

### Transport Layer Analysis

* Identify open ports and running services.
* Analyze TCP and UDP communication patterns.
* Detect:

  * Port scanning
  * Reconnaissance activity

### Application Layer Analysis

Analyze protocols such as:

* HTTP
* DNS
* SSH
* LDAP
* SMB

Look for:

* Unencrypted credentials
* Information leakage
* Misconfigurations

### Identifying Anomalies

Look for:

* Excessive port scanning
* Unusual protocols or services
* Unexpected host communication
* Large data transfers

---

## 4. Documentation and Reporting

### Document Findings

* Record all relevant information gathered during reconnaissance.

### Create a Report

Include:

* Summary of findings
* Identified vulnerabilities
* Security risks
* Recommendations

---

# Common Tools Used in Network Reconnaissance

* Wireshark — Detailed packet analysis
* tcpdump — Command-line packet capture
* Nmap — Network scanning and enumeration
* whois — Domain registration information lookup
* arp — View and manipulate ARP tables

---

# Services and Ports Commonly Enumerated

| Port | Protocol | Service                                      |
| ---- | -------- | -------------------------------------------- |
| 22   | TCP      | Secure Shell (SSH)                           |
| 25   | TCP      | Simple Mail Transfer Protocol (SMTP)         |
| 53   | TCP/UDP  | Domain Name System (DNS)                     |
| 135  | TCP/UDP  | Microsoft RPC Endpoint Mapper                |
| 137  | UDP      | NetBIOS Name Service (NBNS)                  |
| 139  | TCP      | NetBIOS Session Service                      |
| 161  | UDP      | Simple Network Management Protocol (SNMP)    |
| 162  | TCP/UDP  | SNMP Trap                                    |
| 389  | TCP/UDP  | Lightweight Directory Access Protocol (LDAP) |
| 445  | TCP/UDP  | SMB over TCP                                 |
| 500  | UDP      | ISAKMP / Internet Key Exchange (IKE)         |
| 2049 | TCP      | Network File System (NFS)                    |
| 3268 | TCP/UDP  | Global Catalog Service                       |

---

# Network Scanning Challenges and Limitations

## Security Devices

Firewalls, routers, proxy servers, and other security devices can:

* Block scans
* Distort results
* Provide misleading information

Scanning remote hosts outside the local network may not always produce accurate results.

## Privilege Requirements

Some advanced scanning techniques require elevated privileges such as:

* sudo
* Administrator access

---

# Ethical and Legal Considerations

## Permission is Required

Scanning networks without authorization is illegal and may result in:

* ISP complaints
* Legal action
* Government investigation

Do not scan organizations such as:

* Federal Bureau of Investigation
* United States Secret Service

without explicit authorization.

## Respect for Systems

Aggressive scanning may:

* Crash systems
* Cause downtime
* Lead to data loss

Always use caution when scanning mission-critical systems.

---

# Scanning IP Blocks

Attackers may scan IP address ranges allocated to organizations to identify:

* Active hosts
* Services
* Vulnerabilities
* Network structure

Public IP addresses are often assigned in sequential blocks, making targeted scanning easier.

---

# Port Scanning

There are:

* 65,535 TCP ports
* 65,535 UDP ports

Port scanning helps identify:

* Open ports
* Running services
* Potential attack surfaces

---

# Useful Nmap Commands

### Display Host Networking and Routing Information

```bash
nmap --iflist
```

### Trace Packets for Connectivity Troubleshooting

```bash
nmap --packet-trace 172.16.1.10
```

### Scan Using a Specific Network Interface

```bash
nmap -e eth0 172.16.1.10
```

---

# Key Considerations

* Packet analysis can expose sensitive information.
* Handle captured data securely.
* Continuously update knowledge of:

  * Network protocols
  * Security practices
  * Emerging threats

By understanding reconnaissance techniques and tools, organizations can strengthen defenses and reduce the risk of information disclosure and unauthorized access.
