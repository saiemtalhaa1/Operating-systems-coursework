# Week 2 – Security Configuration & Remote Administration

## Introduction
This week focused on securing the Linux server and enabling safe remote administration.  
The main objective was to configure Secure Shell (SSH) correctly, reduce attack surfaces, and apply basic system hardening techniques while maintaining usability for administrative tasks.

---

## Objectives
- Enable secure remote access using SSH
- Verify SSH service status and network availability
- Apply basic security hardening practices
- Understand risks associated with remote administration

---

## SSH Configuration Overview
Secure Shell (SSH) was used as the primary method for remote administration. SSH provides encrypted communication between client and server, protecting credentials and session data from interception.

### Key configuration goals:
- Ensure SSH service is running and enabled at boot
- Confirm correct network interface configuration
- Verify server accessibility using IP addressing

---

## SSH Service Verification
The SSH service status was checked using system management tools to confirm that the service was active and listening for incoming connections.

### Commands used:
- `sudo systemctl status ssh`
- `ip a`

These commands confirmed:
- SSH daemon was running
- The server had a valid IP address assigned
- Port 22 was open and listening

---

## Security Considerations
Remote access introduces security risks if not properly configured. The following considerations were reviewed:

| Risk | Description | Mitigation |
|----|----|----|
| Brute-force attacks | Automated login attempts | Strong passwords, later hardening |
| Unauthorized access | Weak authentication | Limited user access |
| Network exposure | Open services | Minimal services enabled |

These risks were noted for further mitigation in later weeks.

---

## Comparison: Secure vs Insecure Remote Access

| Feature | Secure SSH | Insecure Access |
|------|-----------|----------------|
| Encryption | Yes | No |
| Authentication | Required | Often none |
| Data protection | Encrypted traffic | Plain text |
| Administrative control | Auditable | Uncontrolled |

This comparison highlights why SSH is the preferred method for system administration.

---

## Reflection
This week improved my understanding of Linux security fundamentals and the importance of controlled remote access.  
I learned how to verify running services, interpret network configuration output, and evaluate security risks associated with remote administration. These skills form a foundation for more advanced hardening techniques in later weeks.

---

[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 3](Week3.md)

