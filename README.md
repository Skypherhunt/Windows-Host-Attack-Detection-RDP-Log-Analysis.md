# Windows Host Attack Detection – RDP Log Analysis

## Overview
This project demonstrates **host-based attack detection** using native Windows Security logging. It focuses on identifying and analyzing failed and successful **Remote Desktop Protocol (RDP)** authentication attempts by correlating attacker activity with Windows Security Event Logs.

A controlled attack simulation was performed from a Kali Linux virtual machine against a Windows 10 virtual machine, and the resulting security events were analyzed using Windows Event Viewer.

---

## Lab Environment
- Windows 11 (Host)
- Windows 10 Virtual Machine (Target)
- Kali Linux Virtual Machine (Attacker)
- Network Configuration: Host-only adapter

---

## Key Detection Events
- **Event ID 4625** – Failed logon attempts
- **Event ID 4624** – Successful logon
- **Event ID 4688** – Process creation

---

## What This Project Demonstrates
- Host-based attack detection using Windows-native logging
- Identification of brute-force style RDP login attempts
- Correlation of attacker actions with Windows Security Event IDs
- Reconstruction of an attack timeline from authentication to post-login activity

---

## Tools and Technologies
- Windows Security Auditing
- Windows Event Viewer
- Remote Desktop Protocol (RDP)
- FreeRDP (xfreerdp)
- Kali Linux
- VirtualBox

---

## Outcome
This project shows how **Windows Security Event Logs alone** can be used to detect authentication attacks and post-compromise activity without relying on third-party security tools, reflecting real-world SOC and blue team analysis practices.
