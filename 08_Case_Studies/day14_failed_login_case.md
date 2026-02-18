# Day 14 — Failed Login Investigation Case Study

## Incident Overview
Multiple failed login attempts were detected on a user account.
This could indicate a possible brute force attack.

## Alert Details
- Alert Type: Failed login alert
- Source: Windows Security Logs
- Event ID: 4625
- Affected User: VaniLabUser
- Time Window: 10 minutes (example: 2:10 PM to 2:20 PM)


## Investigation Steps
1. Opened Event Viewer on Windows
2. Went to Windows Logs → Security
3. Filtered the log for Event ID 4625 (failed login)
4. Checked the time pattern (many fails in short time)
5. Noted the source IP and repeated attempts


## Log Analysis
I saw repeated failed logins within a short time, which looks suspicious.
Most attempts were coming from the same IP address.
This usually means someone is trying to guess the password.

## Evidence Collected
- Event ID: 4625
- Key fields checked: Account name, Source IP, Time created


## MITRE ATT&CK Mapping
- Tactic: Credential Access
- Technique: Brute Force

I mapped this to MITRE because the behavior matches password guessing attempts.

## Response Actions
- Recommended password reset
- Suggested account lockout policy
- Advised user to enable MFA

## Conclusion
This activity looks suspicious and could be an attempted brute force attack.
Monitoring and preventive controls are recommended.

## What I Learned
This case helped me understand how to investigate login alerts and document findings.
