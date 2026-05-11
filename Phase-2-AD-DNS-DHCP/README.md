# 🧱 Phase 2 — Active Directory, DNS, DHCP & Identity Setup

## 📌 Overview

In this phase, a complete **Windows domain environment** was deployed on `DC01`, including identity services, name resolution, and automatic IP management. Clients were integrated into the domain and organized using a structured OU design.

---

## ⚙️ What Was Implemented

### 🧠 Active Directory & Domain

* Installed **Active Directory Domain Services (AD DS)**
* Promoted `DC01` to Domain Controller
* Created domain:

  ```
  corp.lab
  ```
* Verified domain functionality

---

### 🌐 DNS Configuration

* DNS installed automatically with AD
* Forward lookup zone `corp.lab` created
* Clients configured to use:

  ```
  192.168.10.10
  ```
* Name resolution tested (`ping`, `nslookup`)

---

### 📡 DHCP Configuration

* Installed and authorized DHCP server
* Created scope:

  ```
  192.168.10.100 – 192.168.10.200
  ```
* Configured options:

  * DNS: `192.168.10.10`
  * Domain: `corp.lab`
* Added exclusion range:

  ```
  192.168.10.1 – 192.168.10.50
  ```
* Activated scope
* Verified clients receive IP automatically

---

### 🏢 Organizational Structure (OUs)

```
IT
HR
Finance
Computers
Servers
```

---

### 👥 Users & Groups

* Created Users
* Created security groups:

  * IT-Users
  * HR-Users
  * Finance-Users
* Assigned users to appropriate groups

---

### 💻 Client Integration

* Joined `CL01` and `CL02` to domain
* Moved clients to `Computers` OU
* Verified login using domain users

---

### 🧪 Validation & Testing

* DHCP assigning valid IPs
* DNS resolving correctly
* Domain authentication working
* Time synchronization verified
* Internal connectivity confirmed

---

### 📁 Preparation for Next Phase

* Created base shared directory:

  ```
  C:\Shares\IT
  ```

---

# ✅ Phase 2 — Final Checklist

* [x] AD installed and domain `corp.lab` created

* [x] DNS configured and resolving correctly

* [x] DHCP installed, authorized, and configured

* [x] DHCP scope (`192.168.10.100 – 200`) created

* [x] Exclusion range (`192.168.10.1 – 50`) configured

* [x] Clients receiving IP via DHCP

* [x] OUs created (IT, HR, Finance, Computers, Servers)

* [x] Users created

* [x] Security groups created (IT-Users, HR-Users, Finance-Users)

* [x] Users assigned to correct groups

* [x] Clients joined to domain

* [x] Clients moved to `Computers` OU

* [x] Domain Controller moved to `Servers` OU

* [x] DNS tested using `nslookup`

* [x] Domain login tested

* [x] Time synchronization verified

* [x] Base shared folders created (`C:\Shares\IT`)

---

## 🎯 Outcome

A fully functional **enterprise-style domain environment** is now in place, including:

* Centralized authentication (Active Directory)
* Name resolution (DNS)
* Automatic IP management (DHCP)
* Logical organization (OUs & Groups)

This environment is now ready for **Group Policy implementation (Phase 3)**.

---
