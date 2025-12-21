# System Planning and Distribution Selection – Week 1

## Introduction

This week focused on planning the system architecture required for the Operating Systems coursework.  
The goal was to design a secure and realistic Linux-based environment using virtual machines, which would later be used for security configuration, monitoring, and performance testing.

A virtualised setup was chosen to allow safe experimentation, reproducibility, and isolation from the host operating system.

---

## System Architecture Overview

The system consists of two virtual machines running inside **Oracle VirtualBox**:

- **Ubuntu Server (CLI-based)** – used as the main server
- **Workstation machine** – used to remotely access and manage the server via SSH

This design simulates a real-world client–server environment.

---

## Virtual Machine Configuration

### Ubuntu Server (CMPN202-Server)

| Component | Configuration |
|--------|--------------|
| Operating System | Ubuntu Server (64-bit) |
| Memory | 2048 MB |
| CPU | 2 vCPUs |
| Storage | 25 GB (VDI) |
| Interface | Command Line (No GUI) |

The server was intentionally kept lightweight to reflect best practices for server deployments.

---

## Network Configuration

The virtual machine was configured with **NAT networking** to allow:

- Internet access for updates
- Secure SSH access from the workstation

The following command was used to confirm the network configuration:

```bash
ip a
