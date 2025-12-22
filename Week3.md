# 📊 Week 3 – Performance Testing & Monitoring
---

## 1. Introduction

Week 3 focused on analysing how the Linux server behaves during normal operation by observing system performance in real time.  
Rather than changing configurations, this week concentrated on **monitoring**, **process analysis**, and **resource usage evaluation**.

Understanding performance behaviour is essential for identifying bottlenecks and ensuring long-term system stability.

---

## 2. Objectives

The objectives of this week were:

- Monitor CPU and memory usage
- Observe active system processes
- Analyse system load and stability
- Understand how Linux reports performance metrics
- Prepare the system for optimisation and tuning

---

## 3. Performance Monitoring Overview

Performance monitoring allows administrators to:

- Identify resource-intensive processes
- Detect abnormal system behaviour
- Verify system stability
- Make informed optimisation decisions

Key system components monitored:
- CPU
- Memory
- Active processes
- Load average

---

## 4. Process Analysis Using `ps`

### Purpose
The `ps aux` command was used to display all running processes on the system.  
This provides a detailed snapshot of system activity, including background services and user-level processes.

![Process List Output](Screenshots/Week3/week3_1.png)

The screenshot shows multiple system services running under the root user, confirming that essential background processes are active and stable.

---

## 5. Real-Time Monitoring Using `top`

### Purpose
The `top` command provides a live view of system performance and updates continuously.

It displays:
- CPU utilisation
- Memory usage
- Load average
- Running and sleeping processes

![Top Command Output](Screenshots/Week3/week3_2.png)

This screenshot demonstrates real-time monitoring of system activity, showing low CPU usage and stable memory consumption during normal operation.

---

## 6. Enhanced Monitoring Using `htop`

### Purpose
`htop` was used as an enhanced alternative to `top` for clearer performance visualisation.

Advantages of `htop` include:
- Colour-coded resource usage
- Visual CPU and memory bars
- Easier process navigation

![htop Monitoring](Screenshots/Week3/week3_3.png)

The screenshot clearly visualises CPU and memory usage, making system performance easier to interpret.

---

## 7. Monitoring Workflow

The following workflow was followed during monitoring:

1. Boot the server normally  
2. Observe baseline activity  
3. Run monitoring tools (`ps`, `top`, `htop`)  
4. Analyse CPU and memory usage  
5. Confirm system stability  

This structured approach ensured consistent and meaningful observations.

---

## 8. Performance Observation Summary

| Resource | Observation |
|--------|------------|
| CPU | Mostly idle during normal use |
| Memory | Stable with sufficient free RAM |
| Processes | Mainly system services |
| Load Average | Low and consistent |

The results confirm that the system operates efficiently under standard conditions.

---

## 9. System Stability Analysis

During monitoring:
- No CPU spikes were detected
- Memory usage remained controlled
- No system lag or instability occurred
- Background services functioned normally

This indicates that the system is stable and ready for further configuration and testing.

---

## 10. Key Learning Outcomes

By the end of Week 3, the following skills were developed:

- Monitoring live system performance
- Interpreting CPU and memory statistics
- Analysing running processes
- Understanding system stability indicators
- Applying performance-aware administration practices

---

## 11. Reflection

Week 3 demonstrated the importance of continuous performance monitoring.  
Even without heavy workloads, monitoring tools provide valuable insight into system health and behaviour.

These skills will be essential for later tasks involving optimisation, logging, and system hardening.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 2](Week2.md) | [Week 4](Week4.md) | [Week 5](Week5.md) | [Week 6](Week6.md) | [Week 7](Week7.md)
