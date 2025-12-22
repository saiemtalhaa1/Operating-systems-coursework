# 📈 Week 6 – Performance Monitoring, Stress Testing & System Analysis

---

## 1. Introduction
Week 6 focused on **evaluating system performance** under both idle and stressed conditions.  
Rather than only observing raw statistics, this week emphasised **interpretation**, **comparison**, and **understanding operating system behaviour** when system resources are placed under load.

Performance monitoring is essential for identifying bottlenecks, ensuring stability, and planning future optimisation.  
This week builds upon earlier system configuration and introduces **real-world performance evaluation techniques** used in production environments.

---

## 2. Objectives
The objectives of this week were to:

- Measure system uptime and baseline performance
- Monitor CPU behaviour during idle and stressed states
- Analyse memory usage and allocation
- Evaluate disk I/O performance
- Test basic network latency and reliability
- Interpret collected performance data

---

## 3. Performance Evaluation Methodology

A structured testing methodology was followed to ensure consistent results:

Baseline measurement (idle system)  
↓  
Apply controlled workload  
↓  
Monitor system metrics  
↓  
Capture performance output  
↓  
Analyse and compare results  

This approach ensures that observed performance changes are **directly linked to applied workloads**.

---

## 4. System Uptime and Baseline State

Before stress testing, system uptime was checked to confirm stability and normal operation.

### Screenshot: System uptime
![Uptime](Screenshots/Week6/week6_1_uptime.png)

The output confirms:
- The system is running normally
- No unexpected restarts occurred
- Load averages are low

This establishes a reliable baseline for further testing.

---

## 5. CPU Performance – Idle State

CPU usage was monitored while the system was idle using the `top` command.

### Screenshot: CPU idle state
![Top idle](Screenshots/Week6/week6_2_top_idle.png)

**Observations:**
- CPU usage remained very low
- Most CPU time was spent in the idle state
- No background processes were consuming excessive resources

This indicates efficient CPU utilisation when no workload is applied.

---

## 6. Stress Tool Installation

The `stress` utility was installed to simulate CPU and memory workload.

### Screenshot: Installing stress
![Install stress](Screenshots/Week6/week6_3_install_stress.png)

Using controlled tools like `stress` allows realistic performance testing without damaging the system.

---

## 7. CPU Performance – Under Load

CPU stress testing was conducted to observe behaviour under heavy computation.

### Screenshot: CPU under stress
![CPU stress](Screenshots/Week6/week6_3_cpu_stress_top.png)

**Analysis:**
- CPU utilisation increased significantly
- Load average rose proportionally
- System remained responsive and stable

This demonstrates that the processor can handle increased workloads without system failure.

---

## 8. Memory Usage Analysis

Memory usage was monitored in both idle and active conditions.

### Screenshot: Memory usage (idle)
![Memory idle](Screenshots/Week6/week6_3_memory_idle.png)

### Screenshot: Memory usage (under load)
![Memory top](Screenshots/Week6/week6_3_memory_top.png)

**Observations:**
- Memory usage increased during stress testing
- No memory exhaustion occurred
- Swap usage remained minimal

This indicates effective memory management by the operating system.

---

## 9. Disk I/O Performance

Disk performance was evaluated by comparing idle and write-intensive states.

### Screenshot: Disk idle
![Disk idle](Screenshots/Week6/week6_4_disk_idle.png)

### Screenshot: Disk write activity
![Disk IO start](Screenshots/Week6/week6_4_disk_iostart.png)

**Analysis:**
- Disk activity increased significantly during write operations
- I/O wait time became noticeable
- Disk I/O had the greatest impact on overall system performance

Disk I/O was identified as a **potential bottleneck** during intensive operations.

---

## 10. Network Performance Testing

Network latency was tested using the `ping` command.

### Screenshot: Network ping test
![Network ping](Screenshots/Week6/week6_5_network_ping.png)

**Results:**
- Stable connectivity was maintained
- Minor latency variation observed
- No packet loss affecting connectivity

This confirms reliable network performance during system load.

---

## 11. Performance Comparison Summary

| Resource | Idle State | Under Load |
|--------|-----------|-----------|
| CPU | Very low usage | High utilisation |
| Memory | Stable | Increased usage |
| Disk | Minimal activity | Heavy I/O |
| Network | Stable | Slight latency |

This comparison clearly shows how workloads affect different system components.

---

## 12. Bottleneck Identification

Based on testing results:
- **Disk I/O** showed the highest performance impact
- CPU and memory handled workloads efficiently
- Network performance remained reliable

Identifying bottlenecks is essential for future optimisation planning.

---

## 13. Optimisation Considerations

Potential optimisation strategies include:
- Using faster storage (SSD)
- Disk caching improvements
- Scheduling heavy tasks during off-peak hours
- Continuous performance monitoring

These measures improve efficiency and reliability in real deployments.

---

## 14. Learning Outcomes
This week improved understanding of:
- Performance monitoring tools
- Stress testing techniques
- Resource utilisation analysis
- Bottleneck identification
- System optimisation planning

---

## 15. Reflection
Week 6 demonstrated that system performance depends not only on hardware, but also on how resources are managed under load.  
By combining monitoring tools with analytical interpretation, a deeper understanding of operating system behaviour was achieved.

This week highlighted the importance of **proactive performance analysis** in maintaining stable and efficient systems.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week `](Week1.md) | [Week 2](Week2.md) | [Week 3](Week3.md) | [Week 4](Week4.md) | [Week 5](Week5.md) | [Week 7](Week7.md) 
