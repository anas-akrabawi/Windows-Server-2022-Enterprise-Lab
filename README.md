# Windows Server 2022 Enterprise Lab

## 📌 Overview

This project simulates a small-to-medium sized corporate IT environment using Windows Server 2022 and VirtualBox.

The environment includes:

* Active Directory Domain Services
* DNS
* DHCP
* Group Policy
* File Services
* NTFS Permissions
* FSRM (Quotas & File Screening)
* Enterprise-style OU Structure
* Troubleshooting & Incident Simulation

The objective of this lab is to gain practical hands-on experience with Windows infrastructure administration, troubleshooting, and enterprise configuration.

---

## 🖥️ Environment

### Hypervisor

* Oracle VirtualBox

### Hardware Constraints

* 8 GB RAM
* 2 CPU cores

### Virtual Machines

| Machine | Role                                  |
| ------- | ------------------------------------- |
| DC01    | Windows Server 2022 Domain Controller |
| CL01    | Tiny10 Client                         |
| CL02    | Tiny10 Client                         |

---

## 🌐 Network Design

| Setting | Value           |
| ------- | --------------- |
| Network | CorpNet         |
| Subnet  | 192.168.10.0/24 |
| Domain  | corp.lab        |
| DC IP   | 192.168.10.10   |

---

## 📚 Implemented Technologies

* Active Directory
* DNS
* DHCP
* Group Policy Objects (GPO)
* File Shares
* NTFS Permissions
* FSRM
* Access-Based Enumeration
* Organizational Units
* Security Groups

---

## 🔥 Troubleshooting Scenarios

Simulated incidents include:

* DHCP failure / APIPA assignment
* DNS misconfiguration
* GPO deployment failures
* Account lockouts
* File share permission issues
* Missing mapped drives
* FSRM file blocking

---

## 🎯 Skills Demonstrated

* Windows Server Administration
* Active Directory Management
* DNS & DHCP Configuration
* Group Policy Administration
* File Server Management
* Network Troubleshooting
* Root Cause Analysis
* IT Documentation

---

## 📸 Documentation

Each phase includes:

* Technical summary
* Configuration screenshots
* Troubleshooting notes
* Validation testing
