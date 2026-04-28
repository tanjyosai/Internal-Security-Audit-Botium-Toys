# Botium Toys: Controls and Compliance Checklist

## Security Controls Evaluation

| Control Category | Control Name | Priority | Status | Rationale |
| :--- | :--- | :--- | :--- | :--- |
| **Administrative** | Least Privilege | High | 🔴 No | Critical for preventing unauthorized lateral movement. |
| **Administrative** | Disaster Recovery Plan | High | 🔴 No | Essential for business continuity during a breach or outage. |
| **Administrative** | Password Policy | Medium | 🔴 No | Current lacks complexity requirements. |
| **Technical** | Intrusion Detection System (IDS) | High | 🔴 No | No active monitoring for malicious network traffic. |
| **Technical** | Encryption (At Rest/Transit) | High | 🔴 No | Customer PII is currently stored in plaintext. |
| **Technical** | Firewall | Medium | 🟢 Yes | Basic perimeter defense is active. |
| **Technical** | Antivirus Software | Medium | 🟢 Yes | Basic endpoint protection is deployed. |
| **Physical** | CCTV (Cameras) | Medium | 🟢 Yes | Physical monitoring of storefront and warehouse. |
| **Physical** | Security Guard | Low | 🔴 No | Not required for a single physical location at this scale. |
| **Physical** | Door Locks | Medium | 🟢 Yes | Physical access to inventory is secured. |

## Compliance Status

| Compliance Standard | Status | Risk Factor |
| :--- | :--- | :--- |
| **GDPR** (EU Protection) | 🔴 Non-Compliant | High risk of fines (4% of annual turnover) for EU customer data. |
| **PCI DSS** (Payments) | 🔴 Non-Compliant | High risk of losing ability to process credit card transactions. |
| **SOC2** (Privacy) | 🔴 Non-Compliant | Trust issues with enterprise B2B partners. |
