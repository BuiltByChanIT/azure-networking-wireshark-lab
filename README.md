# Azure Networking Lab (NSGs + Wireshark)

## Project Overview
This project demonstrates Azure networking fundamentals by deploying two virtual machines within a virtual network, configuring Network Security Group (NSG) firewall rules, and analyzing network traffic using Wireshark.

The lab simulates real-world troubleshooting scenarios including connectivity validation, firewall rule testing, and packet inspection.

---

## Environment Architecture

Azure Infrastructure:

- Resource Group: `rg-ad-lab`
- Virtual Network: `vnet-ad-lab`
- Subnet: `default`
- 2 Virtual Machines:
  - `dc-01` – Windows Server 2022 (Domain Controller)
  - `client-01` – Windows client workstation
- Network Security Groups (NSGs)

Packet analysis performed using **Wireshark** installed on `client-01`.

---

## Technologies Used

- Microsoft Azure (VNets, VMs, NSGs)
- Windows Server 2022
- Wireshark
- Remote Desktop (RDP)
- TCP/IP networking protocols

---

## Deployment Workflow

1. Created Azure Resource Group
2. Created Virtual Network and subnet
3. Deployed two virtual machines within the same subnet
4. Verified network connectivity using ping (ICMP)
5. Configured NSG rules to allow and deny traffic
6. Installed Wireshark on client machine
7. Captured and analyzed network traffic
8. Filtered packets to observe specific protocols

---

## Network Traffic Analysis

### Live Packet Capture

Wireshark was used to capture live network traffic from the Azure virtual network.

![Live Capture](screenshots/01-wireshark-live-capture.png)

---

### ICMP Traffic (Ping)

Connectivity between virtual machines was tested using ping, capturing ICMP echo request and reply packets.

![ICMP Capture](screenshots/02-icmp-ping-capture.png)

---

### DNS Query Analysis

DNS traffic was captured while resolving domain names to IP addresses.

![DNS Capture](screenshots/03-dns-query-capture.png)

---

### TCP Handshake

The TCP 3-way handshake process was observed during connection establishment.

Handshake sequence:

1. SYN
2. SYN-ACK
3. ACK

![TCP Handshake](screenshots/04-tcp-handshake.png)

---

### HTTP Traffic Analysis

Unencrypted HTTP traffic was captured to analyze client-server communication.

![HTTP Capture](screenshots/05-http-traffic-capture.png)

---

### RDP Traffic

Remote Desktop Protocol traffic was captured when connecting to the virtual machine.

![RDP Capture](screenshots/06-rdp-traffic.png)

---

## Validation

Screenshots located in the `/screenshots` directory demonstrate:

- Successful network connectivity between virtual machines
- Network Security Group rule configuration
- Packet capture and protocol filtering
- Analysis of ICMP, DNS, TCP, HTTP, and RDP traffic

---

## Skills Demonstrated

- Azure networking fundamentals
- Network Security Group (NSG) firewall configuration
- Port-based traffic filtering
- Packet capture and analysis using Wireshark
- Protocol inspection (ICMP, DNS, TCP, HTTP, RDP)
- Basic network troubleshooting

---

## Purpose

This lab demonstrates practical networking and packet analysis skills commonly used by:

- IT Support Engineers
- Network Administrators
- Cybersecurity Analysts
- Security Operations Center (SOC) teams
