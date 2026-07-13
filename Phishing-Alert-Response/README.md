# Phishing Alert Response

An incident response exercise following an organization's phishing playbook to evaluate and resolve an alert ticket. The scenario involves a phishing email with a malicious attachment sent to HR, using a file hash previously confirmed malicious through VirusTotal analysis.

📄 [View the full alert ticket](Alert%20ticket.pdf)

## Key Findings

- **Ticket status** — escalated based on multiple phishing indicators
- **Indicators identified** — mismatched sender domain (`.su` TLD vs. display name), grammatical errors in the message body, and a confirmed malicious attachment hash
- Demonstrates use of a structured phishing playbook and flowchart to guide investigation and escalation decisions
