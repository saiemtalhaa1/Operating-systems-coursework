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

## 4. SSH Service Verification

Before allowing remote access, the SSH service was checked to ensure it was active and running.

The following command was used:
- `sudo systemctl status ssh`

This confirms that the SSH daemon is running and listening for incoming connections.

![SSH Service Status](../Screenshots/Week2/Week2_1.png)

---

## 5. Network Configuration Verification

SSH requires a valid network connection.  
The server’s network interface and IP address were verified using:

- `ip a`

This confirmed:
- The active network interface
- The assigned IPv4 address
- The interface state was **UP**

![Network Interface and IP Address](../Screenshots/Week2/Week2_2.png)

---

## 6. File Permission Configuration

Basic file permissions were reviewed to understand Linux access control.

A test file was created and permissions were modified using:
- `touch permissions.txt`
- `chmod 700 permissions.txt`

This ensures that only the file owner has full access.

![File Permission Change](../Screenshots/Week2/Week2_3.png)

---

## 7. File Ownership Verification

File ownership was checked and corrected where required using:
- `sudo chown user:user filename`

This ensures correct access rights and prevents unauthorized file manipulation.

![File Ownership Check](../Screenshots/Week2/Week2_4.png)

---

## 8. Security Risk Identification

Remote access introduces potential security threats.

| Risk Type | Description | Potential Impact |
|---------|------------|------------------|
| Brute-force attacks | Repeated login attempts | Account compromise |
| Weak credentials | Simple passwords | Unauthorized access |
| Open services | Exposed ports | Larger attack surface |

These risks will be addressed further in later weeks.

---

## 9. Secure vs Insecure Access Comparison

| Feature | Secure SSH Access | Insecure Access |
|------|------------------|----------------|
| Encryption | Yes | No |
| Authentication | Required | Optional or none |
| Data protection | Encrypted traffic | Plain text |
| Security level | High | Low |

---

## 10. Reflection
Week 2 demonstrated that remote access must be implemented securely.  
While SSH enables efficient administration, improper configuration can expose the system to serious threats.

This week provided a strong foundation for upcoming firewall configuration and access control tasks.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | Week 2 | [Week 3](Week3.md) | [Week 4](Week4.md) | [Week 5](Week5.md) | [Week 6](Week6.md) | [Week 7](Week7.md)
