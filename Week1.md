# Week 1 – System Planning & Distribution Selection

---

## Introduction

This week focused on planning the operating system environment required for the Operating Systems coursework.  
The objective was to design a stable, secure, and realistic Linux-based virtual environment that could support later tasks such as remote administration, security hardening, monitoring, and performance evaluation.

A virtualised approach was chosen to allow safe experimentation without affecting the host system, while also reflecting real-world client–server system design.

---

## System Architecture Overview

The planned system architecture consists of two main components:

- **Ubuntu Server (CLI-based)**  
  Acts as the primary server used for configuration, security implementation, monitoring, and performance testing.

- **Workstation (host system)**  
  Used to remotely access and manage the server via Secure Shell (SSH).

This separation simulates a real-world server environment where administrative tasks are performed remotely rather than locally.

---

## System Planning Flow

The following structured planning steps were followed during system design:

1. Analyse coursework requirements  
2. Select virtualisation platform (Oracle VirtualBox)  
3. Choose an appropriate Linux server distribution  
4. Configure a minimal server installation (CLI only)  
5. Plan secure network connectivity  
6. Verify system readiness using command-line tools  

This methodical approach ensured the system was prepared for future configuration, security, and performance testing tasks.

---

## Distribution Selection Justification

### Selected Distribution: Ubuntu Server 24.04 LTS

Ubuntu Server 24.04 LTS was selected as the server operating system for the following reasons:

- **Long-Term Support (LTS)**  
  Provides stability and security updates for up to five years.

- **Extensive documentation and community support**  
  Makes learning, troubleshooting, and configuration easier, especially for academic environments.

- **Wide package availability**  
  Required tools such as SSH, firewall utilities, monitoring tools, and security scanners are easily installed via APT.

- **Strong VirtualBox compatibility**  
  Ubuntu Server runs reliably within VirtualBox without requiring additional drivers or configuration.

---

## Distribution Comparison Table

Several alternative Linux server distributions were considered before making the final selection.

| Distribution | Stability | Documentation | VirtualBox Support | Decision |
|-------------|----------|---------------|--------------------|----------|
| Ubuntu Server 24.04 LTS | Very High | Excellent | Excellent | ✅ Selected |
| Debian | Very High | Moderate | Good | Not chosen |
| Fedora Server | Medium | Moderate | Good | Not chosen |
| CentOS Stream | High | Limited | Moderate | Not chosen |

Ubuntu Server was selected due to its balance between long-term stability, ease of use, and suitability for both academic and real-world server environments.

---

## Virtual Machine Configuration

The Ubuntu Server virtual machine was configured using Oracle VirtualBox with the following specifications:

| Component | Configuration |
|---------|--------------|
| Operating System | Ubuntu Server 24.04 LTS |
| Memory | 2 GB |
| CPU | 2 vCPUs |
| Storage | 25 GB (VDI) |
| Interface | Command Line (No GUI) |

A minimal installation was intentionally chosen to reduce system overhead and improve security by limiting unnecessary services.

---

## Network Configuration Planning

The server was configured using **NAT networking**.

This configuration was chosen because it:
- Allows internet access for software updates
- Provides a simple and secure default setup
- Reduces exposure of the server to external networks

Network configuration was verified using command-line tools to ensure the server received a valid IP address and had active network interfaces.

---

## Initial System Verification

Basic system verification was performed using the command line to confirm that the server was operational and ready for remote administration.

Key checks included:
- Verifying active network interfaces and IP address
- Confirming that the SSH service was installed and running

These checks ensured that the server could be securely accessed and managed in later weeks.

---

## Week 1 Requirement Checklist

The following table confirms that all Week 1 requirements were completed:

| Requirement | Status |
|------------|--------|
| System architecture planning | ✅ Completed |
| Distribution selection and justification | ✅ Completed |
| Virtualisation platform selection | ✅ Completed |
| Network configuration planning | ✅ Completed |
| Initial system verification | ✅ Completed |
| Supporting evidence prepared | ✅ Completed |

---

## Reflection

This week highlighted the importance of careful system planning before implementation.  
By clearly defining the system architecture and selecting an appropriate operating system early, later tasks such as security configuration and performance testing become more structured and manageable.

Using a minimal Ubuntu Server environment reinforced key Linux administration concepts and provided a solid foundation for the remaining coursework activities.

---

[Back to Index](../INDEX.md)
