# 🔐 Week 4 – Network Services & Firewall Configuration

---

## 1. Introduction

Week 4 focused on implementing **network-level security controls** to protect the Ubuntu Server from unauthorised access.  
Unlike previous weeks that concentrated on monitoring and analysis, this week applied **active protection mechanisms** to control incoming network traffic.

The main objective was to minimise the system’s attack surface by allowing only essential services.

---

## 2. Objectives for This Week

The objectives of Week 4 were:

- Review active network services
- Understand mounted filesystems and disk structure
- Configure firewall rules using UFW
- Restrict network access to required services
- Verify system security and stability

---

## 3. Filesystem and Mount Point Analysis

Before configuring network security, the system’s mounted filesystems were reviewed to understand storage structure.

![Mounted Filesystems](Screenshots/Week4/Week_4_3_mount.png)

This output shows:
- Active mount points
- Filesystem types
- Read/write permissions

Understanding mounted filesystems helps ensure system integrity and prevents misconfiguration.

---

## 4. Disk Usage Verification

Disk usage was analysed to confirm available storage and ensure no abnormal usage patterns existed.

![Disk Usage df -h](Screenshots/Week4/Week_4_df-h.png)

This confirmed:
- Adequate available disk space
- Correct mounting of logical volumes
- No unexpected storage consumption

Stable disk usage is essential before enabling firewall and security services.

---

## 5. Network Services Overview

A network service is any process listening for incoming network connections.  
Unnecessary services increase security risks and should be restricted.

### Services identified:
- **SSH (port 22)** – required for remote administration
- No additional externally exposed services

This limited exposure improves overall system security.

---

## 6. Firewall Concept and Purpose

A firewall controls which network traffic is allowed or blocked.

Key principles applied:
- **Default deny policy**
- **Least privilege**
- **Explicit service allowance**

UFW (Uncomplicated Firewall) was chosen due to its simplicity and integration with Ubuntu Server.

---

## 7. Firewall Configuration Using UFW

The firewall was configured using UFW to enforce strict access control.

![Firewall Configuration](Screenshots/Week4/week_4_1.png)

### Commands used:
- `sudo ufw enable`
- `sudo ufw allow ssh`
- `sudo ufw status verbose`

These commands ensured:
- The firewall was active
- SSH access was permitted
- All other incoming connections were blocked

---

## 8. Security Impact Analysis

After firewall configuration:
- Network exposure was significantly reduced
- Only essential services remained accessible
- The system became more resistant to automated attacks

Firewall configuration provides a critical first layer of defence.

---

## 9. Before vs After Firewall Comparison

| Aspect | Before Firewall | After Firewall |
|------|----------------|---------------|
| Incoming traffic | Unrestricted | Restricted |
| Exposed services | Multiple | SSH only |
| Attack surface | Large | Reduced |
| Security posture | Weak | Strong |

---

## 10. Week 4 Requirement Checklist

| Requirement | Status |
|------------|--------|
| Filesystem reviewed | ✅ Completed |
| Disk usage verified | ✅ Completed |
| Firewall enabled | ✅ Completed |
| SSH allowed | ✅ Completed |
| Default deny policy applied | ✅ Completed |

---

## 11. Reflection

Week 4 demonstrated how enforcing simple firewall rules can dramatically improve system security.  
By restricting network access and allowing only essential services, the server transitioned into a controlled and protected environment.

This week reinforced the importance of proactive security configuration in real-world systems.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 2](Week2.md) | [Week 3](Week3.md) | Week 4 | [Week 5](Week5.md) | [Week 6](Week6.md) | [Week 7](Week7.md)
