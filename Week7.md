# 🔍 Week 7 – Security Audit & System Evaluation

---

## 1. Introduction
Week 7 focused on conducting a **security audit** and performing a **final evaluation** of the Linux server.  
The purpose of this week was to review all configurations implemented in previous weeks and assess whether the system meets security, performance, and stability requirements.

Security auditing is essential to identify weaknesses, verify controls, and ensure that best practices have been applied consistently.

---

## 2. Objectives for This Week
The main objectives of Week 7 were:

- Perform a system security audit
- Identify potential vulnerabilities
- Review running services
- Evaluate overall system configuration
- Reflect on system readiness and improvements

---

## 3. Security Auditing Overview

A security audit examines the system from a defensive perspective to answer key questions:
- Is the system properly secured?
- Are unnecessary services running?
- Are security controls working as expected?

Auditing ensures that security measures are not only configured, but also effective.

---

## 4. System Audit Using Lynis

Lynis is a widely used security auditing tool for Linux systems.

### Purpose of Lynis:
- Analyse system configuration
- Detect security weaknesses
- Provide hardening recommendations
- Improve system security posture

Lynis was used to perform a comprehensive system scan and generate audit feedback.

---

## 5. Network Security Assessment with Nmap

Network scanning was performed to analyse exposed ports and services.

### Purpose of Nmap:
- Identify open ports
- Detect active services
- Verify firewall effectiveness
- Confirm minimal service exposure

The scan results confirmed that only essential services were accessible, demonstrating effective firewall configuration.

---

## 6. Service Review and Justification

Running services were reviewed to ensure that no unnecessary applications were active.

### Service evaluation criteria:
- Is the service required?
- Does it increase attack surface?
- Can it be disabled safely?

This review ensured that the server follows the principle of **minimal service exposure**.

---

## 7. Access Control Verification

User access and privilege management were reviewed to confirm:
- Non-root user usage
- Controlled administrative access
- Appropriate permission levels

This helps reduce the impact of account compromise and enforces least-privilege principles.

---

## 8. Overall Security Evaluation

The table below summarises the final security posture of the system:

| Security Area | Evaluation |
|-------------|-----------|
| SSH configuration | Secure |
| Firewall rules | Effective |
| Intrusion prevention | Enabled |
| Automatic updates | Configured |
| Access control | Restricted |
| Monitoring | Active |

The evaluation confirms that layered security controls were successfully implemented.

---

## 9. System Strengths and Limitations

### Strengths:
- Strong access control mechanisms
- Minimal exposed services
- Automated security responses
- Stable system performance

### Limitations:
- Performance depends on available hardware resources
- Monitoring can be expanded further
- Additional intrusion detection tools could be added

These limitations represent opportunities for future improvement.

---

## 10. Key Learning Outcomes

By completing this week, the following skills were developed:

- Conducting security audits
- Analysing vulnerability reports
- Reviewing system services critically
- Evaluating overall system readiness
- Applying security best practices

---

## 11. Final Reflection
Week 7 brought together all concepts covered throughout the coursework.  
By auditing and evaluating the system, I gained confidence in understanding how individual security controls work together to protect a server environment.

This final review demonstrated the importance of continuous security assessment and reinforced real-world system administration practices.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 2](Week2.md) | [Week 3](Week3.md) | [Week 4](Week4.md) | [Week 5](Week5.md) | [Week 6](Week6.md) |
