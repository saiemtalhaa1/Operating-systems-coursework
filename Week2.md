
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
[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 3](Week3.md)
