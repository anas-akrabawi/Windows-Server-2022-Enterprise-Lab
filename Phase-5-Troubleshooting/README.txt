# 🔥 Phase 5 — Troubleshooting & Incident Simulation (Chaos Monkey)

## 📌 Overview

In this phase, multiple real-world IT support scenarios were intentionally introduced into the lab environment to simulate enterprise troubleshooting workflows. The goal was to practice incident diagnosis, root cause analysis, policy validation, and service restoration using structured troubleshooting methods.

This phase focused on developing practical skills commonly required in:

* Help Desk Support
* IT Support
* Junior System Administration

---

# 🎫 Simulated Incidents

## 1️⃣ Shared Folder Access Denied

### 🧩 Scenario

A department user lost access to a shared folder that was previously accessible.

### 🔍 Root Cause

Incorrect NTFS permissions removed from the department security group.

### ✅ Resolution

* Verified folder permissions
* Restored group-based NTFS access
* Confirmed successful access after remediation

### 📚 Skills Demonstrated

* NTFS permission troubleshooting
* Access validation
* Security group usage

---

## 2️⃣ Missing Mapped Network Drive

### 🧩 Scenario

Users reported that the mapped departmental drive was no longer visible after login.

### 🔍 Root Cause

Mapped Drive GPO link was removed from the target Organizational Unit (OU).

### ✅ Resolution

* Verified GPO application status
* Re-linked the policy to the correct OU
* Forced Group Policy update and validated drive restoration

### 📚 Skills Demonstrated

* Group Policy troubleshooting
* OU-based policy management
* User environment restoration

---

## 3️⃣ User Account Lockout

### 🧩 Scenario

A user account became locked after multiple failed login attempts.

### 🔍 Root Cause

Account lockout policy triggered due to invalid password attempts.

### ✅ Resolution

* Identified locked account in Active Directory
* Unlocked account
* Verified successful authentication

### 📚 Skills Demonstrated

* Account management
* Security policy understanding
* Authentication troubleshooting

---

## 4️⃣ DNS Resolution Failure

### 🧩 Scenario

Client machine failed to access internal resources by hostname.

### 🔍 Root Cause

Incorrect DNS server manually configured on the client machine.

### ✅ Resolution

* Verified DNS misconfiguration
* Restored correct DNS server settings
* Validated internal name resolution

### 📚 Skills Demonstrated

* DNS troubleshooting
* Network diagnostics
* Client configuration validation

---

## 5️⃣ Group Policy Not Applying

### 🧩 Scenario

Security restrictions stopped applying to a user account.

### 🔍 Root Cause

User account moved outside the Organizational Unit containing the linked GPO.

### ✅ Resolution

* Verified missing GPO application
* Restored correct OU placement
* Confirmed policy enforcement after update

### 📚 Skills Demonstrated

* Active Directory administration
* GPO scope troubleshooting
* Organizational Unit management

---

## 6️⃣ File Upload Blocked by File Screening

### 🧩 Scenario

User unable to upload specific file types to shared storage.

### 🔍 Root Cause

FSRM file screening policy blocked restricted file types.

### ✅ Resolution

* Verified active file screening policy
* Confirmed restriction behavior
* Explained enforcement policy

### 📚 Skills Demonstrated

* FSRM management
* File screening validation
* Policy enforcement troubleshooting

---

# 🧠 Troubleshooting Methodology Used

The following structured approach was used throughout all incidents:

1. Reproduce the issue
2. Identify symptoms
3. Validate configuration
4. Isolate root cause
5. Apply corrective action
6. Verify resolution
7. Document findings

---

# 📚 Key Takeaways

* Troubleshooting requires structured analysis rather than trial-and-error
* Group Policy depends heavily on OU placement and scope
* DNS is critical for Active Directory functionality
* NTFS permissions should be managed using security groups
* File server controls can enforce enterprise security policies
* Root cause analysis is essential for effective support operations

---

# 🎯 Outcome

This phase transformed the lab from a static infrastructure environment into a realistic support simulation platform.

The environment was used to:

* Simulate real support tickets
* Practice incident response
* Develop troubleshooting methodology
* Improve understanding of enterprise infrastructure dependencies

This phase demonstrates practical, hands-on IT support experience using enterprise Windows infrastructure technologies.
