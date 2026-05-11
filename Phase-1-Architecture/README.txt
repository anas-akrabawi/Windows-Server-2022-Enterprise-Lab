# 🧱 Phase 1 — Architecture & Base Installation

## 📌 Overview

In this phase, the foundation of the lab environment was designed and deployed. This included defining the network architecture, configuring virtual machines, and preparing a controlled internal network to simulate a corporate environment.

---

## 🖥️ Lab Environment

### 🔧 Hypervisor

* Oracle VirtualBox

### 💻 Host Constraints

* 8 GB RAM
* 2 CPU cores

### 🖧 Virtual Machines

| Machine | Role                        | OS                  |
| ------- | --------------------------- | ------------------- |
| DC01    | Domain Controller (planned) | Windows Server 2022 |
| CL01    | Client Machine              | Tiny10 (32-bit)     |
| CL02    | Client Machine              | Tiny10 (32-bit)     |

---

## 🌐 Network Design

### 🔹 Network Type

* Internal Network (VirtualBox)
* Network Name:

```text
CorpNet
```

### 🔹 IP Scheme

| Device | IP Address       |
| ------ | ---------------- |
| DC01   | 192.168.10.10    |
| CL01   | DHCP (initially) |
| CL02   | DHCP (initially) |

### 🔹 Subnet

```text
192.168.10.0/24
```

---

## ⚙️ Initial Configuration

* Configured all VMs to use the same internal network (`CorpNet`)
* Assigned a static IP address to DC01
* Verified network adapter configuration across all machines
* Collected IP configuration using system tools

---

## 🧪 Testing & Validation

### 🔍 Initial Issue Encountered

Clients failed to obtain IP addresses automatically and were assigned APIPA addresses (`169.254.x.x`), indicating DHCP was not available.

---

### 🛠️ Troubleshooting Actions

* Verified network adapter status and configuration
* Tested DHCP renewal (failed as expected)
* Assigned static IP addresses to client machines
* Retested connectivity between clients and server

---

### ✅ Results

* Successful communication between clients and DC01 using static IPs
* Internal network confirmed functional
* Issue isolated to absence of DHCP service (planned for next phase)

---

## 📚 Key Takeaways

* Internal networks require manual service configuration (no automatic DHCP)
* APIPA addresses indicate DHCP failure, not total network failure
* Static IP assignment is useful for isolating connectivity issues
* Verifying network layer step-by-step is critical in troubleshooting

---

## 🎯 Outcome

A stable and controlled lab environment was successfully established, including:

* Functional internal network
* Properly configured virtual machines
* Verified connectivity between systems

This phase provides the foundation for deploying **Active Directory, DNS, and DHCP services** in the next stage.
