# DHCP Issue – Troubleshooting Notes

## Problem

CL01 and CL02 were not getting IP addresses and couldn’t reach the server (DC01).

---

## What I Observed

* `ipconfig` showed:

  ```
  169.254.x.x
  ```
* Running:

  ```
  ipconfig /renew
  ```

  returned:

  ```
  Unable to contact your DHCP server
  ```
* Ping to DC01:

  ```
  ping 192.168.10.10
  ```

  failed at first with:

  ```
  General failure
  ```

---

## What I Checked

* Network adapter was enabled
* All VMs connected to `Internal Network (CorpNet)`
* DC01 had correct static IP (`192.168.10.10`)

---

## Fix / Testing

To isolate the issue, I set a manual IP on clients:

```
IP: 192.168.10.20 / 192.168.10.21  
Subnet: 255.255.255.0  
DNS: 192.168.10.10
```

Then tested:

```
ping 192.168.10.10
```

✅ Ping worked

---

## Root Cause

There was **no DHCP server configured yet**, so clients defaulted to APIPA (`169.254.x.x`).

---

## Result

* Network between clients and server is working
* Issue was only DHCP-related
