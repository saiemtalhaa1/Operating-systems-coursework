# 🔍 Week 7 – Security Audit & Final System Evaluation

---

## 1. Introduction

Week 7 focused on performing a **comprehensive security audit** and conducting a **final evaluation** of the Linux server environment.  
The objective was to verify that all configurations implemented throughout the coursework collectively provide a secure, stable, and well-managed system.

Rather than introducing new configurations, this week concentrated on **validation, assessment, and reflection**, which are essential stages in real-world system administration and security management.

---

## 2. Objectives for This Week

The objectives of Week 7 were to:

- Conduct a full system security audit
- Identify potential vulnerabilities and weaknesses
- Verify firewall and network exposure
- Review installed services and access controls
- Evaluate overall system readiness
- Reflect on learning outcomes and future improvements

---

## 3. Security Auditing Overview

A security audit assesses whether system configurations align with security best practices and organisational policies.

Key questions addressed during the audit:
- Are only required services running?
- Is the system properly hardened?
- Are access controls enforced correctly?
- Is the system resilient against common attack techniques?

Security auditing ensures that controls are **effective**, not just configured.

---

## 4. System Audit Using Lynis

Lynis was used as the primary auditing tool for evaluating system security.

### Purpose of Lynis
- Analyse system configuration and permissions
- Detect misconfigurations and weaknesses
- Provide hardening recommendations
- Generate a measurable security score

### Screenshot: Lynis Installation
![Lynis Installation](Screenshots/Week7/week7_1_lynis_install.png)

This screenshot shows the successful installation of Lynis using the APT package manager.

---

### Screenshot: Lynis Scan Summary
![Lynis Scan Summary](Screenshots/Week7/week7_2_lynis_scan_summary.png)

The scan summary displays:
- Hardening index score
- Number of tests performed
- Enabled security modules
- Identified improvement areas

The results confirm that core security mechanisms such as the firewall are active, while also highlighting areas for future enhancement.

---

## 5. Network Security Assessment Using Nmap

To verify exposed services and firewall effectiveness, network scanning was performed using Nmap.

### Purpose of Nmap
- Identify open ports
- Detect active services
- Confirm minimal network exposure
- Validate firewall rules

---

### Screenshot: Nmap Installation
![Nmap Installation](Screenshots/Week7/week7_3_nmap_install.png)

This screenshot confirms that Nmap was installed successfully and ready for use.

---

### Screenshot: Nmap Scan Results
![Nmap Scan Results](Screenshots/Week7/week7_4_nmap_scan.png)

The scan results show that:
- Only port **22 (SSH)** is open
- No unnecessary services are exposed
- Firewall rules are functioning as intended

This demonstrates effective network hardening and controlled service exposure.

---

## 6. Service Review and Justification

All active services were reviewed to ensure they were necessary and justified.

### Service evaluation criteria:
- Is the service required for system operation?
- Does it introduce security risks?
- Can it be safely disabled?

Only essential services such as SSH were retained, reducing the system’s attack surface.

---

## 7. Access Control Verification

User access and privilege configuration were reviewed to confirm:

- Use of non-root user accounts
- Controlled administrative access via `sudo`
- Proper group-based permission management

These checks ensure that the principle of **least privilege** is enforced across the system.

---

## 8. Final Security Evaluation Summary

The table below summarises the overall security posture of the system:

| Security Area | Status |
|--------------|--------|
| SSH configuration | Secure |
| Firewall rules | Effective |
| Intrusion prevention | Enabled |
| Automatic updates | Configured |
| Access control | Restricted |
| Monitoring | Active |

The system demonstrates a strong layered security model.

---

## 9. Strengths and Limitations

### Strengths
- Minimal exposed services
- Effective firewall enforcement
- Automated security auditing
- Stable system configuration
- Clear separation of user privileges

### Limitations
- Monitoring could be extended with alerting tools
- Performance testing could be expanded further
- Hardware resources limit scalability

These limitations highlight opportunities for future enhancement rather than critical weaknesses.

---

## 10. Key Learning Outcomes

By completing Week 7, the following skills were developed:

- Conducting structured security audits
- Interpreting vulnerability scan results
- Validating firewall and service configurations
- Evaluating system readiness
- Applying real-world system administration practices

---

## 11. Final Reflection

Week 7 served as a conclusion to the entire coursework by bringing together **security, performance, monitoring, and access control** concepts.  
The auditing process reinforced the importance of continuous evaluation and demonstrated how layered security controls work together to protect a system.

This final assessment reflects real-world practices in system administration, where validation and review are just as important as initial configuration.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 2](Week2.md) | [Week 3](Week3.md) | [Week 4](Week4.md) | [Week 5](Week5.md) | [Week 6](Week6.md)
