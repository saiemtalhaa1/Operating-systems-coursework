# 📊 Week 3 – Performance Testing & Monitoring

---

## 1. Introduction
Week 3 focused on understanding how a Linux system behaves under different workloads.  
Instead of only configuring services, this week analysed **system performance** by generating controlled stress on CPU, memory, disk, and network resources.

Performance testing is essential to identify system limits, bottlenecks, and stability before deploying real services.

---

## 2. Objectives for This Week
The main objectives of Week 3 were:

- Understand system resource usage
- Perform basic performance testing
- Monitor CPU, memory, disk, and network activity
- Analyse how workloads affect system behaviour
- Prepare the system for optimisation and tuning

---

## 3. Performance Testing Overview

Performance testing helps answer questions such as:
- How much load can the system handle?
- Which resource becomes a bottleneck first?
- How does the system respond under stress?

### Key Performance Areas Tested:
- CPU performance
- Memory usage
- Disk I/O activity
- Network throughput

---

## 4. Performance Testing Workflow

The following workflow was followed during testing:

Select test tool
↓
Generate workload
↓
Monitor system resources
↓
Observe performance impact
↓
Analyse results


This structured approach ensures controlled and meaningful performance testing.

---

## 5. CPU Performance Testing

### Purpose
CPU testing measures how well the processor handles intensive computation.

### Actions Performed:
- Generated CPU-intensive workloads
- Observed CPU usage during execution
- Monitored process behaviour

### Key Metrics Observed:
- CPU utilisation percentage
- Process execution time
- Load average

---

## 6. Memory Performance Testing

### Purpose
Memory testing evaluates how the system handles RAM allocation and usage.

### Actions Performed:
- Created memory stress conditions
- Observed memory consumption
- Checked swap behaviour (if applicable)

### Metrics Observed:
- Used vs free memory
- Memory pressure
- Stability under load

---

## 7. Disk I/O Performance Testing

### Purpose
Disk testing identifies how fast the system can read and write data.

### Actions Performed:
- Generated disk read/write operations
- Observed disk throughput
- Monitored I/O wait times

### Why Disk I/O Matters:
- Slow disks affect application performance
- High I/O wait increases response times
- Critical for databases and servers

---

## 8. Network Performance Testing

### Purpose
Network testing measures data transfer speed and stability.

### Actions Performed:
- Tested network throughput
- Observed latency and bandwidth usage
- Verified reliable communication between systems

---

## 9. Monitoring Strategy

To understand performance impact, multiple monitoring tools were used.

### Monitoring Focus Areas:
- CPU load
- Memory usage
- Disk activity
- Network traffic

### Why Monitoring Is Important:
- Helps detect bottlenecks
- Prevents system overload
- Improves troubleshooting accuracy

---

## 10. Performance Test Summary Table

| Resource | Test Purpose | Observed Behaviour |
|-------|-------------|-------------------|
| CPU | Stress processing power | CPU usage increased during load |
| Memory | Test RAM allocation | Memory usage rose as expected |
| Disk | Measure read/write speed | Disk activity increased under I/O |
| Network | Test throughput | Stable data transfer observed |

---

## 11. Performance vs Stability Comparison

| Aspect | Low Load | High Load |
|-----|--------|----------|
| CPU usage | Low | High |
| Memory usage | Stable | Increased |
| System response | Fast | Slight delay |
| Stability | Normal | Maintained |

This comparison shows that the system remained stable even under increased load.

---

## 12. Key Learning Outcomes

By the end of Week 3, the following skills were developed:

- Understanding performance metrics
- Generating controlled system workloads
- Monitoring live system behaviour
- Identifying performance bottlenecks
- Analysing system stability under stress

---

## 13. Reflection
Week 3 demonstrated how system performance directly impacts reliability and user experience.  
Performance testing provided valuable insight into how different system components interact under load. This knowledge will be essential for future optimisation, monitoring, and security hardening tasks.

---

### 🔗 Navigation
[Back to Index](INDEX.md) | [Week 1](Week1.md) | [Week 2](Week2.md) | [Week 4](Week4.md) | [Week 5](Week5.md) | [Week 6](Week6.md) | [Week 7](Week7.md) |



