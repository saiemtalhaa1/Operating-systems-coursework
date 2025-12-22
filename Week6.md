# 📈 Week 6 – Performance Monitoring & Stress Testing

---

## 1. Introduction
Week 6 focused on **monitoring system performance** and analysing how the server behaves under different workloads.  
Both idle and stressed conditions were observed to understand CPU, memory, disk, and network behaviour.

---

## 2. Objectives
The objectives of this week were:

- Monitor system uptime and baseline state
- Observe CPU and memory usage when idle
- Apply CPU stress testing
- Analyse disk I/O behaviour
- Test basic network performance

---

## 3. System Uptime

Uptime was checked to confirm system stability.

### Screenshot: Uptime
![Uptime](Screenshots/Week6/week6_1_uptime.png)

This confirms the system is running normally.

---

## 4. Baseline CPU State (Idle)

CPU usage was observed while the system was idle.

### Screenshot: CPU idle
![Top idle](Screenshots/Week6/week6_2_top_idle.png)

Low CPU usage indicates no heavy background processes.

---

## 5. Installing Stress Tool

The `stress` utility was installed to generate artificial workload.

### Screenshot: Install stress
![Install stress](Screenshots/Week6/week6_3_install_stress.png)

This tool is commonly used for performance testing.

---

## 6. CPU Stress Testing

CPU stress testing was performed to observe load behaviour.

### Screenshot: CPU stress
![CPU stress](Screenshots/Week6/week6_3_cpu_stress_top.png)

CPU usage increased significantly under load, as expected.

---

## 7. Memory Usage Analysis

Memory usage was observed in both idle and active states.

### Screenshot: Memory idle
![Memory idle](Screenshots/Week6/week6_3_memory_idle.png)

### Screenshot: Memory under load
![Memory top](Screenshots/Week6/week6_3_memory_top.png)

Memory usage increased but remained stable.

---

## 8. Disk I/O Analysis

Disk activity was tested under idle and write-heavy conditions.

### Screenshot: Disk idle
![Disk idle](Screenshots/Week6/week6_4_disk_idle.png)

### Screenshot: Disk I/O active
![Disk IO](Screenshots/Week6/week6_4_disk_iostart.png)

Disk activity increased during write operations.

---

## 9. Network Performance Test

Network latency was tested using `ping`.

### Screenshot: Network ping
![Network ping](Screenshots/Week6/week6_5_network_ping.png)

The results show stable connectivity with minor latency.

---

## 10. Performance Summary

| Resource | Idle | Under Load |
|-------|------|-----------|
| CPU | Low | High |
| Memory | Stable | Increased |
| Disk | Minimal | Heavy I/O |
| Network | Stable | Slight delay |

---

## 11. Key Observations
- CPU and memory handled stress efficiently
- Disk I/O showed the most impact
- Network remained reliable
- System stability was maintained

---

## 12. Reflection
Week 6 provided practical insight into system performance behaviour.  
Monitoring under load helps identify bottlenecks and improves understanding of real-world server operation.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 5](Week5.md) | [Week 7](Week7.md)
