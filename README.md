# 🏢 Windows Server 2022 Enterprise Lab

## 📌 Project Overview

This project simulates a small-to-medium sized corporate IT environment using Windows Server 2022 and VirtualBox.

The lab was built to gain practical hands-on experience with:

* Active Directory Domain Services (AD DS)
* DNS & DHCP
* Group Policy Objects (GPO)
* File Services & NTFS Permissions
* FSRM (Quotas & File Screening)
* Enterprise troubleshooting workflows
* Windows infrastructure administration

The environment was intentionally designed under hardware constraints (8 GB RAM / 2 CPU cores) to simulate realistic resource optimization.

---

# 🖥️ Lab Environment

## 🔧 Hypervisor

* Oracle VirtualBox

## 💻 Virtual Machines

| Machine | Role                                  |
| ------- | ------------------------------------- |
| DC01    | Windows Server 2022 Domain Controller |
| CL01    | Tiny10 Client                         |
| CL02    | Tiny10 Client                         |

---

# 🌐 Network Architecture

| Setting           | Value           |
| ----------------- | --------------- |
| Internal Network  | CorpNet         |
| Subnet            | 192.168.10.0/24 |
| Domain Name       | corp.lab        |
| Domain Controller | DC01            |
| DC IP Address     | 192.168.10.10   |

---

# 🏗️ Architecture Image
<img width="1536" height="1024" alt="Project Architecture" src="https://github.com/user-attachments/assets/5ae91fa8-1337-48bd-80e6-c04e8d2e3afc" />

---

# 🧠 Implemented Technologies

## Identity & Infrastructure

* Active Directory Domain Services
* Organizational Units (OUs)
* Security Groups
* Domain Join

## Networking

* DNS
* DHCP
* IP Address Management
* Internal Network Segmentation

## Group Policy

* Password Policies
* Account Lockout Policies
* USB Restrictions
* Desktop Wallpaper Deployment
* Mapped Network Drives
* Control Panel Restrictions

## File Services

* Shared Folders
* NTFS Permissions
* Access-Based Enumeration (ABE)
* Quotas
* File Screening (FSRM)

## Troubleshooting & Incident Simulation

* DHCP/APIPA failures
* DNS misconfiguration
* GPO deployment issues
* Account lockouts
* File share access problems
* Missing mapped drives

---

# 📚 Project Phases

* [Phase 1 — Architecture & Base Installation](./Phase-1-Architecture)
* [Phase 2 — Active Directory, DNS & DHCP](./Phase-2-AD-DNS-DHCP)
* [Phase 3 — Group Policy Implementation](./Phase-3-GPO)
* [Phase 4 — File Services & Permissions](./Phase-4-File-Services)
* [Phase 5 — Troubleshooting & Incident Simulation](./Phase-5-Troubleshooting)

---

# 📸 Project Highlights

## Active Directory Deployment

* Domain Controller installation and configuration
* Domain creation (`corp.lab`)
* Organizational Unit structure
* User and group management

## Enterprise Group Policies

* Security hardening
* User environment standardization
* Centralized policy enforcement

## File Server Implementation

* Department-based shared folders
* NTFS permission layering
* Quotas and file restrictions

## Real Troubleshooting Scenarios

* Diagnosed DHCP failures causing APIPA addressing
* Resolved GPO wallpaper deployment issues
* Fixed DNS misconfiguration problems
* Restored file share access through NTFS troubleshooting

---

# 🎯 Skills Demonstrated

* Windows Server Administration
* Active Directory Management
* DNS & DHCP Configuration
* Group Policy Administration
* File Server Management
* Infrastructure Troubleshooting
* Root Cause Analysis
* IT Documentation
* Enterprise Environment Design

---

# 🧪 Troubleshooting Focus

One of the primary goals of this project was to simulate real-world IT support scenarios instead of only performing successful installations.

The lab included intentional fault simulation and recovery processes to strengthen troubleshooting methodology and infrastructure understanding.

---

# 📂 Repository Structure

```text
Windows-Server-2022-Enterprise-Lab/
│
├── Phase-1-Architecture/
├── Phase-2-AD-DNS-DHCP/
├── Phase-3-GPO/
├── Phase-4-File-Services/
├── Phase-5-Troubleshooting/
└── Assets/
```

---

# 🚀 Project Goal

The objective of this project was to develop practical hands-on experience with enterprise Windows infrastructure technologies and build a portfolio demonstrating:

* System administration fundamentals
* Infrastructure troubleshooting
* Enterprise configuration management
* Technical documentation skills

---

# 📌 Status

✅ Completed

This environment is fully functional and includes identity services, centralized management, file services, and simulated enterprise troubleshooting scenarios.
