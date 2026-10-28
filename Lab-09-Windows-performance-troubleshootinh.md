# Lab 9: Windows Performance Troubleshooting

## Ticket Information
- **Ticket ID:** HD-009
- **Category:** Hardware / Performance
- **Priority:** Medium
- **Status:** Resolved (simulated lab)
- **Environment:** Windows 11, 8 GB RAM
- **Assigned To:** Level 1 IT Support

## Issue Description
A user reported that their Windows 11 computer was running slowly. Applications took longer than usual to open, and the computer occasionally froze for several seconds. The issue began that morning.

## Initial Findings
- User could sign in and access the desktop.
- CPU usage: 24%.
- Memory usage: 91%.
- Disk usage: 18%.
- Browser memory usage: 2.4 GB.
- Microsoft Teams memory usage: 1.1 GB.
- Other applications and system processes accounted for additional memory usage.

## Troubleshooting Steps
1. Asked the user when the issue began and whether recent changes had occurred.
2. Opened Task Manager and reviewed CPU, Memory, and Disk usage.
3. Sorted processes by memory consumption to identify resource-intensive applications.
4. Asked the user to save their work before making changes.
5. Reviewed open browser tabs and running applications with the user.
6. Closed unnecessary browser tabs and exited an application that was no longer needed.
7. Rechecked system resource usage.
8. Confirmed that the user reported improved performance and no further freezing in the simulated scenario.

## Root Cause Analysis
High memory utilization was a likely contributing factor to the reported performance degradation. Closing unnecessary applications reduced memory usage and coincided with improved responsiveness.

The exercise did not establish a definitive underlying cause beyond the observed association.

## Resolution
Reduced unnecessary application resource consumption by closing browser tabs and an application that was no longer needed.

## Before-and-After Results

| Resource | Before | After |
|---|---:|---:|
| CPU | 24% | 19% |
| Memory | 91% | 67% |
| Disk | 18% | 14% |

## Verification
- [x] Rechecked resource utilization.
- [x] Memory usage decreased from 91% to 67%.
- [x] User reported faster application launches.
- [x] User reported that brief freezing had stopped.
- [ ] Extended monitoring — not performed.

## Recommendations
- Close unnecessary applications and browser tabs when they are not needed.
- Monitor Task Manager if performance problems return.
- Investigate startup applications and recurring resource consumption if symptoms persist.
- Consider a RAM upgrade only after evaluating workload requirements and confirming that memory capacity is insufficient.

## Technician Notes
The simulated incident was resolved using basic Windows performance troubleshooting. No operating system reinstallation, hardware replacement, or disabling of security software was necessary.

## Skills Demonstrated
- Windows 11 Task Manager
- CPU, memory, and disk monitoring
- Process analysis
- Safe application management
- Performance troubleshooting
- Before-and-after verification
- Root cause analysis
- Professional ticket documentation
