# Week 1 – System Planning & Distribution Selection

---

## Introduction

This week focused on planning the operating system environment required for the Operating Systems coursework.  
The goal was to design a stable, secure, and realistic virtualised environment that could support later tasks such as remote administration, security hardening, monitoring, and performance testing.

Two virtual machines were planned:
- A **Linux server** (CLI-based) for configuration, security, and testing
- A **workstation** to act as the remote client connecting via SSH

All systems were deployed using **Oracle VirtualBox**.

---

## Virtual Machine Architecture

The system architecture consists of:

- **Ubuntu Server 24.04 LTS**  
  Used as the main server for configuration, security testing, and monitoring.

- **Workstation (host machine)**  
  Used to remotely access the server using SSH.

The server was configured without a graphical interface to reduce overhead and reflect real-world server environments.

📸 *Evidence: Virtual machine configuration in VirtualBox*

---

## Distribution Selection Justification

### Selected Distribution: Ubuntu Server 24.04 LTS

Ubuntu Server was selected for the following reasons:

- **Long-Term Support (LTS)**  
  Provides stability and security updates for 5 years.

- **Extensive documentation**  
  Ubuntu has one of the largest support communities, making troubleshooting and learning easier.

- **Package availability**  
  APT provides easy access to tools required later in the coursework (SSH, firewall, monitoring tools).

- **VirtualBox compatibility**  
  Ubuntu runs reliably in VirtualBox without additional drivers or configuration.

### Alternatives Considered

- **Debian** – Very stable but slower update cycle.
- **Fedora Server** – Cutting-edge but not ideal for long-term coursework stability.
- **CentOS Stream** – Enterprise-focused, less beginner-friendly.

Ubuntu Server offered the best balance between usability, stability, and learning value.

---

## Network Configuration Planning

The server network was configured using **NAT networking**.

Reasons for choosing NAT:
- Provides internet access for system updates
- Simple and secure default configuration
- Prevents unnecessary exposure of the server to external networks

The server received a dynamically assigned IP address, which was later used for SSH access.

📸 *Evidence: Network interface and IP address output*

---

## Initial System Verification (CLI)

Basic system checks were performed to confirm that the server was running correctly.

Commands used:
- `ip a` – Verify network interfaces and IP address
- `systemctl status ssh` – Confirm SSH service is running

These checks confirmed that:
- The network interface was active
- The SSH service was enabled and listening on port 22

📸 *Evidence: SSH service status output*

---

## Reflection

This week established the foundation for the entire coursework.  
By carefully planning the operating system, network configuration, and distribution choice, later security and performance tasks can be completed smoothly.

Using a minimal Ubuntu Server environment helped reinforce key Linux administration concepts and provided a realistic platform for future system hardening and monitoring activities.

---

[Back to Index](../INDEX.md)
