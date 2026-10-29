Help Desk Lab 10 — Active Directory & Account Management
Ticket Information
Ticket ID: HD-010
Category: Account Management / Active Directory
Priority: Medium
Status: Resolved (simulated lab)
Affected User: User A
Environment: Windows workstation, Active Directory domain
1. Issue Summary
The user was unable to access their work computer because their Active Directory account became locked after multiple unsuccessful password attempts. After the account was unlocked and the password was reset, the account repeatedly locked again.

2. Symptoms
Windows reported that the account was locked.
Subsequent login attempts reported an incorrect password.
The account locked again after a password reset.
The user could not initially access their workstation and mapped network drive.
3. Troubleshooting Performed
Verified the user’s identity and confirmed the exact login error.
Checked the account’s status in Active Directory Users and Computers.
Confirmed that the account was enabled but locked.
Unlocked the account using the approved procedure.
Investigated the password-related login failure.
Reset the password through the authorized account-management process.
Reviewed available authentication logs with a senior technician.
Identified repeated authentication attempts from the user’s workstation associated with a mapped network drive using outdated credentials.
Updated or removed the stale credentials using the approved procedure.
Tested the user’s Windows sign-in and mapped network drive access.
4. Root Cause
Outdated saved credentials associated with a mapped network drive repeatedly triggered failed authentication attempts, causing the user’s account to lock again.

5. Resolution
The account was unlocked and the password was reset through the approved process. The stale credentials associated with the mapped network drive were corrected.

6. Verification
User successfully signed in to Windows.
Mapped network drive opened successfully.
No further lockouts occurred during the initial monitoring period in the simulation.
7. Security Considerations
Verified user identity before account changes.
Followed authorized account-management procedures.
Did not request or record the user’s password.
Investigated repeated lockouts rather than repeatedly unlocking the account.
Used least-privilege principles and appropriate escalation.
8. Final Outcome
Resolved — simulated lab.

The user regained workstation and network drive access. The underlying cause of repeated account lockouts was identified and addressed.

9. Skills Practiced
Active Directory Users and Computers
Account lockout troubleshooting
Password reset procedures
Authentication log investigation
Saved credential troubleshooting
Root cause analysis
User access verification
Professional ticket documentation
