# 📘 Week 2 – Security Configuration & Remote Administration

---

## 1. Introduction
In Week 2, the focus was on securing the Linux server and enabling safe remote administration.  
Instead of managing the server only through the local console, secure remote access was configured to allow efficient and professional system management.

This week introduced the importance of balancing **accessibility** and **security** when administering servers.

---

## 2. Objectives for This Week
The main objectives of Week 2 were:

- Enable secure remote administration
- Verify SSH service availability
- Confirm correct network configuration
- Understand security risks related to remote access
- Prepare the system for future security hardening

---

## 3. Remote Administration Overview

### Why Remote Administration Is Needed
Remote administration allows system administrators to manage servers without physical access.

**Advantages:**
- Faster system management
- Reduced downtime
- Real-world server administration practice

**Potential Risks:**
- Unauthorized login attempts
- Brute-force password attacks
- Network exposure

Because of these risks, strong security controls are essential.

---

## 4. SSH Configuration Workflow

Server boots
↓
SSH service starts
↓
Network interface receives IP address
↓
SSH listens on port 22
↓
Remote client connects securely


This flow ensures that remote access only occurs after required system services are active.

---

## 5. Secure Shell (SSH) Configuration

Secure Shell (SSH) was selected as the remote administration method because it provides encrypted communication between systems.

### Key actions performed:
- Verified SSH service installation
- Checked service status
- Confirmed SSH starts automatically on boot

### Commands used:
- `sudo systemctl status ssh`
- `ip a`

These commands confirmed:
- SSH service was **active and running**
- The server had a valid network interface
- The system was ready for remote access

---

## 6. Network Configuration Verification

The server’s network configuration was reviewed to ensure proper connectivity.

### Information verified:
- Active network interface
- Assigned IPv4 address
- Interface operational state (UP)

This step is critical because SSH cannot function without proper network connectivity.

---

## 7. Security Risk Identification

Remote access introduces potential security threats.  
The table below outlines key risks identified during this week.

| Risk Type | Description | Potential Impact |
|---------|------------|------------------|
| Brute-force attacks | Repeated login attempts | Account compromise |
| Weak credentials | Simple passwords | Unauthorized access |
| Open services | Exposed ports | Larger attack surface |

These risks were documented and planned to be mitigated in later weeks.

---

## 8. Secure vs Insecure Access Comparison

| Feature | Secure SSH Access | Insecure Access |
|------|------------------|----------------|
| Encryption | Yes | No |
| Authentication | Required | Optional or none |
| Data protection | Encrypted traffic | Plain text |
| Security level | High | Low |

This comparison highlights why SSH is the industry-standard choice for remote administration.

---

## 9. Key Learning Outcomes

By completing this week, the following skills were developed:

- Understanding how SSH works
- Interpreting system service status outputs
- Reading network configuration information
- Identifying security risks in server environments
- Applying security-aware system administration practices

---

## 10. Reflection
Week 2 highlighted that remote access is not only about convenience but also about responsibility.  
While SSH enables efficient system management, it also introduces security risks that must be carefully controlled. This week built a strong foundation for upcoming tasks involving firewall rules, access control, and system hardening.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 3](Week3.md) | [Week 4](Week4.md) | [Week 5](Week5.md) | [Week 6](Week6.md) | [Week 7](Week7.md) |
