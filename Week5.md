# 🛡️ Week 5 – Advanced Security & Monitoring Infrastructure

---

## 1. Introduction
Week 5 focused on implementing **advanced security controls** and introducing **basic monitoring capabilities** on the Linux server.  
While earlier weeks addressed foundational security such as SSH and firewall rules, this week strengthened the system by adding **intrusion prevention**, **automatic security updates**, and **access control mechanisms**.

The aim was to move from basic protection to a more **defensive and proactive security posture**.

---

## 2. Objectives for This Week
The objectives of Week 5 were:

- Implement intrusion prevention mechanisms
- Configure automatic security updates
- Review access control policies
- Introduce system monitoring concepts
- Improve overall system resilience against attacks

---

## 3. Intrusion Prevention Overview

Intrusion prevention systems help detect and respond to suspicious behaviour such as repeated failed login attempts.

### Why Intrusion Prevention Is Important
- Prevents brute-force SSH attacks
- Automatically blocks malicious IP addresses
- Reduces administrator workload
- Enhances server security without constant manual intervention

---

## 4. Fail2Ban Configuration

Fail2Ban was used to protect the SSH service from brute-force attacks.

### How Fail2Ban Works

Repeated failed login attempts
↓
Fail2Ban detects suspicious behaviour
↓
Offending IP address is temporarily banned
↓
Attack traffic is blocked


### Key actions performed:
- Installed Fail2Ban
- Enabled SSH protection rules
- Verified service status

Fail2Ban provides an additional layer of defence by automatically responding to attack patterns.

---

## 5. Automatic Security Updates

Keeping a system updated is critical for protecting against known vulnerabilities.

### Why Automatic Updates Matter
- Security patches are applied without delay
- Reduces exposure to known exploits
- Improves system reliability and stability

Automatic updates were configured to ensure that important security patches are applied regularly without requiring manual intervention.

---

## 6. Access Control Review

Access control determines **who can access the system and what actions they can perform**.

### Access control measures reviewed:
- Use of non-root user accounts
- Principle of least privilege
- Controlled administrative access using `sudo`

Restricting direct root access reduces the impact of potential account compromise.

---

## 7. Monitoring and System Awareness

Monitoring provides visibility into system behaviour and security status.

### Monitoring focus areas:
- Running services
- Authentication activity
- Security events
- Resource usage trends

Monitoring allows administrators to detect abnormal behaviour early and respond quickly.

---

## 8. Security Layers Overview

The following table summarises the layered security approach applied so far:

| Security Layer | Purpose |
|---------------|--------|
| SSH | Secure remote access |
| Firewall (UFW) | Network traffic control |
| Fail2Ban | Intrusion prevention |
| Automatic updates | Vulnerability mitigation |
| Access control | User privilege restriction |

This layered approach follows the principle of **defence in depth**.

---

## 9. Week 5 Requirement Checklist

| Requirement | Status |
|-----------|--------|
| Intrusion prevention implemented | ✅ Completed |
| Automatic security updates configured | ✅ Completed |
| Access control reviewed | ✅ Completed |
| Monitoring concepts applied | ✅ Completed |
| Advanced security posture achieved | ✅ Completed |

---

## 10. Reflection
Week 5 highlighted that security is not achieved through a single control, but through **multiple reinforcing mechanisms**.  
By combining firewall rules, intrusion prevention, automatic updates, and controlled access, the server became significantly more resilient to attacks.

This week reinforced the importance of proactive security management rather than reactive responses.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 4](Week4.md) | [Week 6](Week6.md)


