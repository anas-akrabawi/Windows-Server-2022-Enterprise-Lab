# 📁 Phase 4 — File Server, Permissions, Quotas & File Screening

## 📌 Overview

In this phase, a centralized **file server solution** was implemented to simulate enterprise-level storage management. This includes structured shared folders, access control using NTFS permissions, storage limits, and file type restrictions.

---

## ⚙️ Implemented Components

### 🗂️ Shared Folder Structure

A centralized share was created to host department folders:

```
\\DC01\Shares
```

Inside the share:

```
IT
HR
Finance
```

Each department has its own dedicated directory.

---

### 🔐 Access Control (NTFS Permissions)

Access was controlled using **department-based security groups**:

| Folder  | Access Group  | Permission |
| ------- | ------------- | ---------- |
| IT      | IT-Users      | Modify     |
| HR      | HR-Users      | Modify     |
| Finance | Finance-Users | Modify     |

* Administrators retain full control
* Permissions are enforced at the NTFS level

---

### 🔗 Share Permissions Strategy

* Share permissions set to **Full Control for Everyone**
* Security enforced using **NTFS permissions only**

This follows standard enterprise best practice:

> Simplify share access, enforce security via NTFS

---

### 👁️ Access-Based Enumeration (ABE)

Enabled to improve user experience and security:

* Users only see folders they have access to
* Prevents visibility of unauthorized directories

---

### 📊 Storage Quotas

Storage limits were implemented to control usage:

* Applied per department folder
* Example limit: **500MB per folder**

This prevents excessive storage consumption and simulates real-world constraints.

---

### 🚫 File Screening

File screening policies were applied to restrict unwanted file types:

* Blocked file categories:

  * Audio files (e.g., `.mp3`)
  * Executables (e.g., `.exe`)

This helps enforce data governance and reduce security risks.

---

## 🧪 Validation & Testing

The following tests were performed:

* Users can access only their department folder
* Access to other department folders is denied
* Shared folder visibility limited via ABE
* File upload blocked for restricted file types
* Storage limits enforced when quota exceeded

---

## ⚠️ Key Design Decisions

* Used **security groups** instead of assigning permissions directly to users
* Separated **share permissions** and **NTFS permissions**
* Enabled ABE for a cleaner and more secure user experience
* Implemented quotas and file screening to simulate enterprise policies

---

## 🎯 Outcome

A fully functional **enterprise-style file server** is now in place, providing:

* Centralized file storage
* Secure access control
* Controlled storage usage
* File type enforcement

This phase demonstrates practical skills in **file services, access management, and data control**, preparing the environment for real-world support and administration scenarios.
