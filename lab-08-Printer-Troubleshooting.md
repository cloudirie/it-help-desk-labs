# Lab 8: Printer Troubleshooting — Printer Offline

## Ticket Information
- **Ticket ID:** HD-008
- **Category:** Hardware / Printing
- **Priority:** High
- **Status:** Resolved (simulated lab)
- **Environment:** Windows 11, network printer
- **Assigned To:** Level 1 IT Support

## Issue Description
A user reported that their network printer appeared offline in Windows 11 and they could not print an important document needed for an upcoming meeting.

## Initial Findings
- Printer was powered on.
- Printer display showed a Wi-Fi connection.
- The affected computer was connected to the company Wi-Fi.
- Other websites were accessible.
- Another user could print successfully.
- The affected print queue had Pause Printing enabled.
- The Windows printer queue also had Use Printer Offline enabled.

## Troubleshooting Steps
1. Checked printer power, connection, and status.
2. Verified network connectivity and determined that the issue affected one user's computer.
3. Inspected the print queue and identified that printing was paused.
4. Resumed printing and checked the printer status.
5. Identified and disabled Use Printer Offline.
6. Confirmed that the printer status changed to Ready.
7. Sent a test page and verified that it printed successfully.

## Root Cause
The affected Windows 11 computer had printer queue settings that prevented normal printing. The Use Printer Offline setting was enabled, and Pause Printing was also enabled during the investigation.

## Resolution
Resumed the print queue and disabled Use Printer Offline. The printer returned to Ready status, and a test page printed successfully.

## Verification
- [x] Printer status changed to Ready.
- [x] Test page printed successfully.
- [x] Printing functionality was restored in the simulated scenario.
- [ ] User confirmation of the original document printing — not recorded.

## Prevention / Recommendations
- Verify printer status before submitting important print jobs.
- Check the print queue for paused jobs or offline settings.
- Report recurring printing issues to IT support.
- Escalate persistent problems if basic troubleshooting does not resolve them.

## Technician Notes
The issue was resolved through basic Windows printer troubleshooting without replacing hardware or reinstalling drivers. The problem was isolated to the affected user's computer.

## Skills Demonstrated
- Windows 11 printer troubleshooting
- Network connectivity checks
- Problem isolation
- Print queue management
- Root cause identification
- Resolution verification
- IT ticket documentation

