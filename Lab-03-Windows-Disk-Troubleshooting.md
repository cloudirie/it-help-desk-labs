Lab 3: Windows Disk Usage Troubleshooting
Objective
Investigate high disk usage on a Windows virtual machine using Task Manager and document the findings.

Environment
Operating system: Windows
Environment: Virtual machine (VM)
Tool: Windows Task Manager
Reported Observation
During the initial investigation, disk usage fluctuated between approximately 52% and 91%.

Troubleshooting Steps
Opened Task Manager using Ctrl + Shift + Esc.
Selected the Processes tab and observed disk activity.
Observed Antimalware Service Executable, associated with Microsoft Defender Antivirus.
Restarted the Windows VM after a Windows update/restart sequence.
Reopened Task Manager and checked disk, CPU, and memory utilization.
Observed system performance again after the restart.
Results
Disk usage: 0% during the final observation.
Disk transfer rate: 0 MB/s during the final observation.
CPU usage: fluctuated between approximately 1% and 5%.
Memory in use: 2.1 GB out of 4 GB.
No screenshots were captured during this exercise.
Conclusion
Disk activity was idle during the final observation after the VM restarted. The original high disk usage did not recur during the observation period.

The root cause of the original disk usage spikes was not confirmed. Additional monitoring would be required if the issue returns.

Skills Practiced
Navigating Windows Task Manager
Monitoring disk, CPU, and memory utilization
Observing Windows Defender-related processes
Documenting troubleshooting steps and results
Distinguishing observed results from confirmed root causes
Next Steps
If high disk usage returns, identify the process responsible, record its resource usage, and investigate further before making system changes.

