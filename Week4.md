# 🔐 Week 4 – Network Services & Firewall Configuration

---

## 1. Introduction
Week 4 focused on implementing **network security controls** to protect the Linux server from unauthorised access.  
While earlier weeks concentrated on planning and basic configuration, this week introduced **active security enforcement** through firewall rules and controlled service exposure.

The main goal was to ensure that only **essential services** were accessible and that all other traffic was restricted by default.

---

## 2. Objectives for This Week
The objectives of Week 4 were:

- Identify essential network services running on the server
- Configure a firewall using UFW (Uncomplicated Firewall)
- Restrict network access to required services only
- Reduce the system’s attack surface
- Verify firewall rules and behaviour

---

## 3. Network Services Overview

A network service is any application that listens for incoming network connections.  
Unnecessary services increase security risks and should be disabled or blocked.

### Services reviewed on the server:
- **SSH (port 22)** – required for remote administration
- No additional public services enabled

By limiting exposed services, the system becomes easier to secure and monitor.

---

## 4. Firewall Concept and Purpose

A firewall acts as a **traffic control mechanism**, deciding which network packets are allowed or blocked.

### Key firewall principles applied:
- **Default deny policy** – block everything unless explicitly allowed
- **Least privilege** – allow only what is necessary
- **Controlled access** – restrict services to trusted connections

UFW was selected due to its simplicity, reliability, and integration with Ubuntu.

---

## 5. Firewall Configuration Workflow

The following workflow was used to configure firewall rules:

Identify required services
↓
Enable firewall
↓
Allow SSH traffic
↓
Block all other incoming connections
↓
Verify firewall status and rules



This structured process ensures that security rules are applied logically and safely.

---

## 6. UFW Firewall Configuration

The firewall was configured using UFW with the following steps:

### Key actions performed:
- Enabled UFW firewall
- Allowed SSH connections (port 22)
- Verified default deny behaviour

### Commands used:
- `sudo ufw enable`
- `sudo ufw allow ssh`
- `sudo ufw status verbose`

These commands confirmed that:
- The firewall was active
- SSH traffic was explicitly allowed
- All other incoming connections were blocked by default

---

## 7. Before vs After Firewall Comparison

| Aspect | Before Firewall | After Firewall |
|-----|----------------|----------------|
| Incoming connections | Unrestricted | Restricted |
| Service exposure | Higher | Minimal |
| Attack surface | Large | Reduced |
| Security posture | Weak | Strong |

This comparison highlights the effectiveness of firewall rules in improving system security.

---

## 8. Security Impact Analysis

Implementing firewall rules significantly improved system security by:
- Preventing unauthorised network access
- Limiting exposed services
- Reducing the risk of automated attacks

Firewall configuration is a critical defence layer and complements other security mechanisms such as SSH hardening and user privilege management.

---

## 9. Week 4 Requirement Checklist

| Requirement | Status |
|-----------|--------|
| Network services reviewed | ✅ Completed |
| Firewall installed and enabled | ✅ Completed |
| SSH access allowed | ✅ Completed |
| Default deny policy applied | ✅ Completed |
| Firewall rules verified | ✅ Completed |

---

## 10. Reflection
Week 4 demonstrated how simple security measures can significantly strengthen a system.  
By enabling a firewall and restricting network traffic, the server was transformed from an open system into a controlled and protected environment.

This week reinforced the importance of **defence in depth**, where firewalls act as a critical first line of protection against external threats.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 3](Week3.md) | [Week 5](Week5.md)

