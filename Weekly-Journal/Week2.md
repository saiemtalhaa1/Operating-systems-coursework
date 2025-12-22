# 📘 Week 2 – Security Configuration & Remote Administration

---

## 1. Introduction

In Week 2, the focus was on securing the Linux server and enabling safe remote administration.  
Instead of managing the server only through the local console, secure remote access was prepared to allow efficient and professional system management.

Remote administration is essential in real-world environments, but it introduces additional security risks.  
This week highlighted the importance of balancing **accessibility**, **security**, and **operating system control** when administering servers.

---

## 2. Objectives for This Week

The main objectives of Week 2 were:

- Enable secure remote administration
- Verify SSH service availability
- Confirm correct network configuration
- Identify security risks related to remote access
- Define a security baseline for future hardening tasks

These objectives support later firewall configuration, access control enforcement, and intrusion detection.

---

## 3. Remote Administration Overview

### Why Remote Administration Is Needed

Remote administration allows system administrators to manage servers without physical access, which is the standard practice in data centres and cloud environments.

**Advantages:**
- Faster system management and troubleshooting
- Reduced downtime
- Real-world server administration experience using SSH

**Potential Risks:**
- Unauthorized login attempts
- Brute-force password attacks
- Increased network exposure

Because of these risks, remote access must be secured using strong authentication and restrictive access policies.

---

## 4. SSH Service Verification

Before allowing remote access, the SSH service was checked to ensure it was active and running.

The following command was used:
- `sudo systemctl status ssh`

This confirms that the SSH daemon is running and listening for incoming connections, which is required for remote system administration.

![SSH Service Status](../Screenshots/Week2/Week2_1.png)

---

## 5. Network Configuration Verification

SSH requires a valid and active network connection.  
The server’s network interface and IP address were verified using:

- `ip a`

This confirmed:
- The active network interface
- The assigned IPv4 address
- The interface state was **UP**

Correct network configuration is essential for reliable remote access and later firewall rule enforcement.

![Network Interface and IP Address](../Screenshots/Week2/Week2_2.png)

---

## 6. File Permission Configuration

Basic file permissions were reviewed to understand Linux access control at the operating system level.

A test file was created and permissions were modified using:
- `touch permissions.txt`
- `chmod 700 permissions.txt`

This configuration ensures that only the file owner has full access, supporting the principle of **least privilege** and reducing the risk of unauthorized data access.

![File Permission Change](../Screenshots/Week2/Week2_3.png)

---

## 7. File Ownership Verification

File ownership was checked and corrected where required using:
- `sudo chown user:user filename`

Correct file ownership ensures that access control policies are enforced correctly by the operating system and prevents unauthorized file manipulation by other users or processes.

![File Ownership Check](../Screenshots/Week2/Week2_4.png)

---

## 8. Threat Model and Risk Identification

Remote access introduces several operating system security threats that must be mitigated.

| Threat | Description | Impact | Mitigation Strategy |
|------|------------|--------|---------------------|
| Brute-force SSH | Repeated login attempts | Account compromise | Key-based authentication, disable passwords, fail2ban |
| Weak credentials | Simple or reused passwords | Unauthorized access | Enforce key-based SSH and restricted sudo access |
| Open services | Unnecessary exposed ports | Larger attack surface | Firewall default-deny policy and service minimisation |

These mitigation strategies are implemented and evidenced in later weeks.

---

## 9. Secure vs Insecure Access Comparison

| Feature | Secure SSH Access | Insecure Access |
|------|------------------|----------------|
| Encryption | Yes | No |
| Authentication | Mandatory | Optional or none |
| Data protection | Encrypted traffic | Plain text |
| Security level | High | Low |

This comparison highlights why SSH is essential for secure remote administration.

---

## 10. Security vs Usability Trade-off

Disabling password-based authentication improves security by preventing brute-force attacks but reduces convenience during initial access.  
This trade-off is justified because key-based SSH authentication provides stronger protection and aligns with professional server administration practices.

---

## 11. Reflection

Week 2 demonstrated that remote access must be implemented securely to protect the operating system from common attack vectors.  
While SSH enables efficient administration, improper configuration can significantly increase system risk.

The security baseline established this week provides a strong foundation for firewall configuration, access control, intrusion detection, and performance monitoring in subsequent weeks.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | Week 2 | [Week 3](Week3.md) | [Week 4](Week4.md) | [Week 5](Week5.md) | [Week 6](Week6.md) | [Week 7](Week7.md)
