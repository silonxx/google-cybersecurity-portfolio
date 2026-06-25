# Access Control Worksheet

**Activity:** Improve authentication, authorization, and accounting for a small business
**Course:** Google Cybersecurity Certificate — Course 5: Assets, Threats, and Vulnerabilities
**Incident:** Fraudulent payroll deposit to an unknown account (`FAUX_BANK`)

## Event log under investigation

| Field | Value |
| --- | --- |
| Event Type | Information |
| Source | AdsmEmployeeService |
| Event ID | 1227 |
| Date / Time | 10/03/2023 — 8:29:57 AM |
| User | Legal\Administrator |
| Computer | Up2-NoGud |
| IP | 152.207.255.255 |
| Description | Payroll event added. FAUX_BANK |

## Worksheet

| Notes (identifying the threat actor) | Issues (access control problems) | Recommendations (mitigations) |
| --- | --- | --- |
| The event log IP (`152.207.255.255`) matches **Robert Taylor Jr.**, a Legal-department attorney working as a **contractor**, in the employee directory. The incident occurred on **10/03/2023 at 8:29:57 AM**, which matches his last-access timestamp — confirming his account was the source of the fraudulent `FAUX_BANK` payroll event. | Robert Taylor Jr.'s account was **still active despite his contract ending on 12/27/2019** — his access was never revoked at offboarding. He also retained **full Admin authorization** as a contractor, violating the **principle of least privilege** (every employee in the directory holds blanket Admin rights regardless of role). | Implement an **offboarding procedure** that revokes account access immediately when an employee or contractor leaves. Apply the **principle of least privilege** by granting role-based permissions instead of blanket Admin rights. Additionally, **enforce MFA** and run **regular access-control audits** to catch dormant or over-privileged accounts. |
