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

## Architecture Image
<img width="1536" height="1024" alt="Project Architecture" src="https://github.com/user-attachments/assets/5ae91fa8-1337-48bd-80e6-c04e8d2e3afc" />

<br>

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

---

# 🔥 Troubleshooting Scenarios

- DHCP failures and APIPA address assignment
- DNS misconfiguration and resolution failures
- Group Policy deployment and scope issues
- NTFS and file share permission troubleshooting
- Active Directory account lockouts
- Missing mapped network drives

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


<br>
<img width="1020" height="585" alt="2 2) Domain Name" src="https://github.com/user-attachments/assets/394aa91d-b6e3-4d1b-b77d-e763cc0ad501" />

<br>
<img width="1366" height="699" alt="2 6) Successfully Configured Domain Controller" src="https://github.com/user-attachments/assets/227d956f-66e9-4dc8-9e2b-6880f1d56132" />

<br>
<img width="813" height="551" alt="5) OUs structure" src="https://github.com/user-attachments/assets/5f951bd5-4174-47a3-a0a8-5177c26f57bc" />
<br>

<img width="852" height="563" alt="8) IT Group   its Members" src="https://github.com/user-attachments/assets/fd4f09b9-aeb3-4e20-aa1b-dba387b8d75f" />

<br>
## Enterprise Group Policies

* Security hardening
* User environment standardization
* Centralized policy enforcement

<img width="1019" height="551" alt="8) GPO list in GPMC" src="https://github.com/user-attachments/assets/ab957537-4971-4f8d-8428-7de6bd0356e6" />
<br>


## File Server Implementation

* Department-based shared folders
* NTFS permission layering
* Quotas and file restrictions


<br>
<img width="934" height="513" alt="1) Folder structure inside Shares Folder" src="https://github.com/user-attachments/assets/b9067675-d662-4226-8d54-0f9712da9e27" />

<br>
<img width="957" height="539" alt="2) IT Folder -  IT Users NTFS Persmissions" src="https://github.com/user-attachments/assets/330fd258-98cf-4fab-94a9-b5d0e08a6099" />

<br>
<img width="1084" height="498" alt="11 1) Copying Process has failed because of the Quota limit" src="https://github.com/user-attachments/assets/edac5aab-e7d6-4208-a72d-10f7ce69e081" />

<br>
<img width="1063" height="491" alt="12 3) Copying the mp4 video file is failed becuase a file screen blocks mp4 file types" src="https://github.com/user-attachments/assets/9fd3ff75-2a8b-4768-a6fb-875a773ed702" />
<br>


## Real Troubleshooting Scenarios

* Diagnosed DHCP failures causing APIPA addressing
* Resolved GPO wallpaper deployment issues
* Fixed DNS misconfiguration problems
* Restored file share access through NTFS troubleshooting


<br>
<img width="572" height="322" alt="1) CL01 IP Configuration" src="https://github.com/user-attachments/assets/b093b5f5-c52b-4b5e-bcb9-b9c9b393fae1" />

<br> 

<img width="1366" height="704" alt="10 9) CL01 Desktop Wallpaper" src="https://github.com/user-attachments/assets/5c1d4804-57cf-4cb1-8166-56722d4798ff" />

<br>
<img width="1029" height="551" alt="8" src="https://github.com/user-attachments/assets/2fe90cc3-7689-40d4-b0f9-08296c5a4a3b" />
<br>
<img width="1366" height="721" alt="1) Ticket - HR user unable to access shared drive" src="https://github.com/user-attachments/assets/913b9dd3-9be7-4d4d-ad26-b7afe8ae4633" />
<br>
<img width="1366" height="704" alt="1 2) Ticket - HR user unable to access shared drive" src="https://github.com/user-attachments/assets/a3d795e0-eecf-46e2-9943-757f347e05c9" />
<br>
<img width="960" height="583" alt="1 8) Ticket - HR user unable to access shared drive" src="https://github.com/user-attachments/assets/50fe59f8-5b14-44a6-9f2a-ddde51850b6c" />
<br>



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
