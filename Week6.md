# 📈 Week 6 – Performance Evaluation & Analysis

---

## 1. Introduction
Week 6 focused on evaluating the system’s performance under different workloads and analysing how the operating system behaves when resources are stressed.  
The aim was not only to collect performance data, but also to **interpret results**, identify bottlenecks, and understand how system optimisation can improve efficiency.

This week builds directly on Week 3, moving from basic performance testing to **structured performance analysis**.

---

## 2. Objectives for This Week
The objectives of Week 6 were:

- Perform detailed performance testing
- Measure CPU, memory, disk, and network usage
- Compare baseline and stressed system behaviour
- Identify performance bottlenecks
- Analyse optimisation opportunities

---

## 3. Performance Evaluation Methodology

A structured methodology was followed to ensure consistent and meaningful results.

### Testing Approach

Baseline measurement
↓
Apply workload
↓
Monitor system metrics
↓
Record performance data
↓
Analyse results


This approach ensures that performance changes can be clearly attributed to workload conditions.

---

## 4. Baseline Performance Testing

Baseline testing was conducted to understand normal system behaviour under minimal load.

### Metrics observed:
- CPU utilisation
- Memory usage
- Disk activity
- Network latency

Baseline results provided a reference point for later comparisons.

---

## 5. CPU Performance Analysis

### Purpose
CPU testing evaluates how the processor handles computational workloads.

### Observations:
- CPU usage increased significantly during stress tests
- Load average rose proportionally with workload
- System responsiveness remained stable

This indicates that the CPU was able to handle increased demand without system failure.

---

## 6. Memory Performance Analysis

### Purpose
Memory testing examines how the system allocates and manages RAM under pressure.

### Observations:
- Memory usage increased during workload execution
- No unexpected crashes occurred
- System stability was maintained

Efficient memory management is essential for multitasking and service reliability.

---

## 7. Disk I/O Performance Analysis

### Purpose
Disk I/O testing evaluates how quickly the system can read and write data.

### Observations:
- Disk activity increased under load
- Higher I/O wait times were observed during heavy disk operations
- Disk performance directly affected overall system responsiveness

Disk I/O was identified as a potential bottleneck during intensive operations.

---

## 8. Network Performance Analysis

### Purpose
Network testing measures data transfer speed and latency.

### Observations:
- Network throughput remained stable
- Latency increased slightly under load
- SSH connections remained reliable

This confirms that the network configuration supports remote administration even during stress.

---

## 9. Performance Data Summary

| Resource | Baseline State | Under Load |
|-------|---------------|------------|
| CPU | Low usage | High utilisation |
| Memory | Stable | Increased usage |
| Disk | Minimal activity | Heavy I/O |
| Network | Stable | Slight latency |

This table summarises the performance changes observed during testing.

---

## 10. Bottleneck Identification

Based on testing results:
- **Disk I/O** was identified as the primary bottleneck
- CPU and memory handled workloads efficiently
- Network performance remained acceptable

Identifying bottlenecks helps guide optimisation efforts.

---

## 11. Optimisation Considerations

Potential optimisation strategies include:
- Disk caching improvements
- Load scheduling during off-peak times
- Resource monitoring for early detection

These improvements aim to enhance system efficiency and reliability.

---

## 12. Key Learning Outcomes

This week developed the following skills:

- Performance measurement techniques
- System monitoring and data interpretation
- Bottleneck identification
- Performance optimisation planning
- Analytical thinking in system evaluation

---

## 13. Reflection
Week 6 demonstrated that system performance is not just about raw hardware capability, but also about how resources are managed under load.  
By analysing performance metrics and identifying bottlenecks, I gained a deeper understanding of operating system behaviour and the importance of proactive optimisation.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 2](Week2.md) | [Week 3](Week3.md) | [Week 4](Week4.md) | [Week 5](Week5.md) | [Week 7](Week7.md) |
