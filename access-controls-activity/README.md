# Access Controls Activity

This folder is part of my **Google Cybersecurity Certificate** portfolio. It contains my work for the activity **"Improve authentication, authorization, and accounting for a small business"** from **Course 5: Assets, Threats, and Vulnerabilities**.

## Scenario

A small business discovered a **fraudulent payroll deposit** sent to an unknown account labeled `FAUX_BANK`. As the analyst, I investigated the incident using a Windows **event log** and the company's **employee directory** to identify the threat actor and the underlying access-control weaknesses that made the attack possible.

## What I did

- Reviewed the event log entry for the fraudulent payroll event (Event ID 1227, `AdsmEmployeeService`).
- Correlated the source IP address (`152.207.255.255`) and access timestamp (10/03/2023, 8:29:57 AM) against the employee directory.
- Identified the threat actor and documented the authentication, authorization, and accounting (AAA) failures that allowed the incident.
- Recommended mitigations grounded in security best practices (offboarding, least privilege, MFA, and access audits).

## Files

| File | Description |
| --- | --- |
| `README.md` | This overview of the activity. |
| `Access control worksheet.pdf` | The completed worksheet: notes identifying the threat actor, the access-control issues found, and recommended mitigations. |

## Key takeaway

The incident was enabled by two classic access-control failures: **access was never revoked at offboarding** (a contractor's admin account stayed active years after his contract ended) and a **violation of the principle of least privilege** (every employee held blanket Admin authorization). Strong AAA controls — timely offboarding, role-based least-privilege access, MFA, and regular access audits — would have prevented or quickly detected this fraud.
