# PASTA Threat Modeling

A threat modeling exercise using the **PASTA (Process for Attack Simulation and Threat Analysis)** framework, applied to a sneaker company's e-commerce application that processes financial transactions and stores customer PII.

📄 [View the full worksheet](PASTA%20worksheet.pdf)

## Key Sections

- **Business & Security Objectives** — identifies PCI-DSS compliance and secure authentication as core requirements given the app's handling of financial transactions
- **Technical Scope** — evaluates APIs, PKI, SHA-256, and SQL as key technologies, prioritizing APIs as the largest attack surface due to their role connecting customers, sellers, and internal systems
- **Threat Analysis** — identifies SQL injection and social engineering as key threats
- **Vulnerability Analysis** — identifies lack of prepared statements and weak/reused credentials as exploitable vulnerabilities
- **Risk Analysis & Impact** — recommends MFA, principle of least privilege, prepared statements, and rate limiting as mitigating controls
