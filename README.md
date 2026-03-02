# Azure Networking Lab (NSGs + Wireshark)

## Overview
Built a 2-VM networking lab in Microsoft Azure to test connectivity, configure Network Security Group (NSG) rules, and capture/analyze traffic using Wireshark.

## Architecture
- 2x Azure Virtual Machines
- Azure Virtual Network (VNet)
- Network Security Groups (NSGs)
- Wireshark installed on one VM

## Technologies Used
- Microsoft Azure (VNets, VMs, NSGs)
- Windows/Linux Virtual Machines
- Wireshark
- TCP/IP networking fundamentals

## Deployment Steps (High-Level)
1. Created Azure Resource Group and Virtual Network
2. Deployed two VMs in the same subnet
3. Validated private IP connectivity (ping tests)
4. Modified NSG rules to allow/block traffic
5. Captured and filtered traffic using Wireshark

## Validation
Screenshots in `/screenshots` demonstrate:
- Successful and failed connectivity tests
- NSG rule configuration
- Wireshark packet capture analysis

## Skills Demonstrated
- Azure networking fundamentals
- Firewall rule logic (NSGs)
- Port-based access control
- Packet capture and protocol analysis
- Basic network troubleshooting
