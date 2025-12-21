# Week 2 – Security Configuration & Remote Administration

## Introduction
In Week 2, the focus was on **securing the Linux server** and setting up **safe remote administration**.  
Instead of working directly on the virtual machine console every time, Secure Shell (SSH) was used to manage the server remotely in a controlled and encrypted way.

This week is important because **remote access is powerful but risky** if not configured correctly.

---

## Week 2 Objectives
The main goals for this week were:

- Enable remote access using SSH
- Confirm the SSH service is running correctly
- Identify the server’s network configuration
- Understand basic security risks related to remote administration
- Prepare the system for further security hardening in later weeks

---

## Why Remote Administration Is Needed
Managing a server locally is not practical in real systems.  
Remote administration allows administrators to:

- Manage servers without physical access
- Perform updates and maintenance efficiently
- Monitor system health from another machine

However, remote access must be **secured properly** to avoid unauthorized access.

---

## What Is SSH?
SSH (Secure Shell) is a protocol that allows encrypted communication between a client and a server.

Server boots
   ↓
SSH service starts
   ↓
Network interface gets IP address
   ↓
SSH listens on port 22
   ↓
Remote client connects securely

### Key benefits of SSH:
- Encrypted data transfer
- Secure authentication
- Protection against eavesdropping
- Widely used in real-world Linux systems

Because of these benefits, SSH was chosen as the **only remote access method**.

---

## SSH Service Configuration
The SSH service was checked to ensure it was:

- Installed
- Running
- Enabled at system startup

### Commands used:
- `sudo systemctl status ssh`
- `ip a`

These commands confirmed that:
- The SSH daemon was active
- The server was listening on the default SSH port
- The network interface was correctly configured

---

## Network Configuration Check
Understanding the network configuration is essential for secure remote access.

The following information was verified:
- Network interface name
- Assigned IP address
- Network status (UP/DOWN)

This ensured that the server could communicate reliably with the workstation.

---

## Basic Security Review
Remote administration introduces several risks if left unmanaged.

### Identified risks and observations:

| Risk | Description | Status |
|----|-----------|-------|
| Brute-force login attempts | Repeated password guessing | Identified |
| Unauthorized access | Weak authentication | Reviewed |
| Service exposure | Open services on the network | Limited |
| Data interception | Unencrypted connections | Prevented by SSH |

These risks were documented and will be **further mitigated in later weeks**.

---

## Secure vs Insecure Remote Access (Comparison)

| Feature | Secure SSH | Insecure Access |
|------|-----------|----------------|
| Encryption | Yes | No |
| Authentication required | Yes | Often no |
| Data visibility | Encrypted | Plain text |
| Industry standard | Yes | No |

This comparison highlights why SSH is the correct and professional choice.

---

## Checklist – Week 2 Tasks Completed
✔ SSH service verified  
✔ Network interface checked  
✔ Remote access confirmed  
✔ Security risks identified  
✔ Preparation for hardening completed  

---

## Reflection
This week helped me understand that **security is not only about tools, but also about configuration**.  
I learned how to verify running services, interpret network information, and recognise risks related to remote access.

The work completed in Week 2 provides a strong foundation for:
- Firewall configuration
- Authentication hardening
- System auditing in later weeks

---

[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 3](Week3.md)
