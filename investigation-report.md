# SC-200 Security Investigation Report

## Project Overview
This project demonstrates the use of Kusto Query Language (KQL) to investigate failed sign-in activity using Microsoft Sentinel and Microsoft Entra ID sign-in logs.

## Investigation Objective
Identify suspicious patterns of failed sign-in attempts that may indicate password guessing or password-spraying activity.

## Data Source
- Table: `SigninLogs`
- Investigation period: Last 24 hours

## Detection Approach
1. Filter sign-in events to the last 24 hours.
2. Identify unsuccessful sign-in attempts.
3. Group failed attempts by IP address and user account.
4. Highlight IP addresses with 10 or more failed attempts for further investigation.

## Analyst Investigation Steps
- Review the source IP address and targeted accounts.
- Check whether the activity involves multiple users.
- Review timestamps and authentication details.
- Correlate the activity with successful sign-ins and other security alerts.
- Determine whether the activity is legitimate or suspicious.

## Recommended Response
If malicious activity is confirmed:
- Investigate affected accounts.
- Follow organizational procedures for account protection and credential resets.
- Apply appropriate Conditional Access or other security controls.
- Document the incident and escalate according to SOC procedures.

## Important Note
A high number of failed sign-ins does not automatically prove an attack. Findings must be validated against available logs and organizational context.

## Skills Demonstrated
- KQL query development
- Sign-in log analysis
- Suspicious authentication detection
- Security investigation and incident documentation
