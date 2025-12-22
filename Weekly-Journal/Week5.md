# 🛡️ Week 5 – Advanced Security Controls & Monitoring Infrastructure

---

## 1. Introduction

Week 5 focused on implementing **advanced operating system security controls** and building a basic monitoring and verification infrastructure.  
These controls go beyond basic firewall protection and help detect, prevent, and report security incidents.

All configuration tasks were performed **remotely via SSH from the workstation**, in accordance with the coursework administrative constraint.

---

## 2. Objectives for This Week

The objectives of Week 5 were:

- Implement mandatory access control using AppArmor or SELinux
- Enable automatic security updates
- Configure intrusion prevention using fail2ban
- Create a security baseline verification script
- Develop a remote monitoring script
- Verify configurations using command-line evidence

---

## 3. Mandatory Access Control (AppArmor)

AppArmor was used to enforce mandatory access control policies on the system.  
It restricts what applications are allowed to access, even if they are compromised.

### Command Used
- `sudo aa-status`

This command verifies that AppArmor is enabled and actively enforcing profiles.

*(Screenshot to be added)*

---

## 4. Automatic Security Updates

Automatic updates were configured to ensure that critical security patches are applied without manual intervention.

### Command Used
- `sudo apt install unattended-upgrades`
- `sudo dpkg-reconfigure unattended-upgrades`

This reduces the risk of vulnerabilities caused by outdated packages.

*(Screenshot to be added)*

---

## 5. Intrusion Prevention with fail2ban

fail2ban was configured to protect SSH by automatically blocking IP addresses that generate repeated failed login attempts.

### Command Used
- `sudo systemctl status fail2ban`

This helps mitigate brute-force SSH attacks.

*(Screenshot to be added)*

---

## 6. Security Baseline Verification Script

A security verification script named `security-baseline.sh` was created on the server.  
This script checks whether key security controls are enabled and correctly configured.

### Example checks performed:
- SSH service status
- Firewall status
- AppArmor status
- fail2ban service status
- Automatic updates configuration

All script lines are commented to explain their function.

*(Script output screenshot to be added)*

---

## 7. Remote Monitoring Script

A remote monitoring script named `monitor-server.sh` was created on the workstation.  
The script connects to the server via SSH and collects system performance metrics.

### Metrics collected include:
- CPU usage
- Memory usage
- Disk usage
- System uptime

This supports later performance analysis in Week 6.

*(Script output screenshot to be added)*

---

## 8. Security vs Performance Trade-off

Advanced security controls can introduce minor performance overhead due to additional checks and logging.  
However, this trade-off is acceptable because improved security and visibility significantly reduce the risk of system compromise.

Security was prioritised in line with best practices for server environments.

---

## 9. Week 5 Requirement Checklist

| Requirement | Status |
|------------|--------|
| AppArmor enabled | ⬜ |
| Automatic updates configured | ⬜ |
| fail2ban configured | ⬜ |
| Security baseline script created | ⬜ |
| Remote monitoring script created | ⬜ |
| SSH-only administration | ✅ |

---

## 10. Reflection

Week 5 demonstrated how layered security controls strengthen operating system protection.  
By combining mandatory access control, automatic updates, intrusion prevention, and monitoring scripts, the system became more resilient to both known and unknown threats.

These controls provide essential security visibility and prepare the system for performance evaluation and auditing in later weeks.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 2](Week2.md) | [Week 3](Week3.md) | [Week 4](Week4.md) | Week 5 | [Week 6](Week6.md) | [Week 7](Week7.md)
