# 🛡️ Phase 3 — Group Policy (GPO) Implementation

## 📌 Overview

In this phase, centralized management was implemented using **Group Policy Objects (GPOs)** to enforce security, standardize user environments, and simulate real-world enterprise controls across departments.

---

## ⚙️ Implemented Policies

### 🔐 Password Policy

* Enforced minimum password length
* Enabled complexity requirements
* Configured password expiration

---

### 🔒 Account Lockout Policy

* Lockout after multiple failed attempts
* Temporary lockout duration configured
* Reset counter defined

---

### 🖼️ Desktop Wallpaper Policy

* Enforced a standardized corporate wallpaper
* Deployed using a shared network path
* Ensured consistent user environment across domain

---

### 🔌 USB Storage Restriction

* Blocked access to removable storage devices
* Prevented data exfiltration and unauthorized file transfers

---

### 🗂️ Mapped Network Drive

* Mapped shared network drive to users
* Provided centralized access to department resources

---

### 🚫 Control Panel Restriction

* Restricted access to Control Panel for specific users
* Prevented unauthorized system configuration changes

---

## 🏢 GPO Design & Scope

* User-based policies linked to:

  * IT OU
  * HR OU
  * Finance OU

* Computer-based policies linked to:

  * Computers OU

* Policies applied based on **Active Directory structure and role separation**

---

## 🧪 Validation & Testing

* Verified GPO application using system tools
* Confirmed password and lockout enforcement
* Validated wallpaper deployment on client machines
* Tested USB restriction behavior
* Confirmed mapped drive availability
* Verified Control Panel access restrictions

---

## ⚠️ Issues Encountered & Resolution

### Wallpaper Not Applying (Black Screen)

**Cause:**

* Initially used mapped drive and local paths

**Resolution:**

* Switched to UNC path (`\\DC01\Wallpapers\...`)
* Verified share and NTFS permissions
* Confirmed correct GPO scope (User Configuration)

---

## 🎯 Outcome

* Centralized policy enforcement successfully implemented
* Improved system security and user environment control
* Demonstrated real-world Group Policy design and troubleshooting

This phase establishes a strong foundation for **file services, access control, and enterprise-level management** in the next phase.
