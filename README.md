# 🔐 Cybersecurity Internship – Task 2: UFW Firewall Configuration

This repository contains the implementation of a basic host-based firewall using UFW (Uncomplicated Firewall) on Kali Linux.

---

## 🛡️ Task Objective
The goal of this task is to secure the system by configuring a firewall to:
1. **Allow SSH (Port 22)** for secure remote management.
2. **Deny HTTP (Port 80)** to block unencrypted web traffic.

## 💻 Implementation
An automated Bash script (`ufw_task.sh`) was used to perform the configuration:
- Reset existing rules to ensure a clean state.
- Set default policies to `deny incoming` and `allow outgoing`.
- Applied specific rules for SSH and HTTP traffic.

## 📊 Firewall Status
Following the configuration, the active firewall rules are successfully applied as shown below:

```text
Status: active
To                         Action      From
--                         ------      ----
22/tcp                     ALLOW IN    Anywhere
80/tcp                     DENY IN     Anywhere
