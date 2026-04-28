# Botium Toys: Comprehensive Security Audit Report

## 1. Introduction & Scope
**Project Objective:** To perform an internal security audit of Botium Toys' end-to-end infrastructure, ensuring alignment with the NIST Cybersecurity Framework (CSF) and international data regulations.

**Scope:** 
*   Physical storefront and warehouse location (US).
*   Internal corporate network and legacy systems.
*   Global e-commerce platform and cloud-hosted databases.

## 2. Current Posture Assessment
Based on the internal review, Botium Toys currently maintains a **Weak** security posture with significant gaps in technical and administrative controls.

### Existing Controls
*   **Firewall:** Basic perimeter defense is active.
*   **Antivirus:** Endpoint protection is deployed on corporate workstations.
*   **Physical:** CCTV and door locks are functional at the storefront.

### Identified Gaps (Critical Risk)
*   **Data Protection:** Plaintext storage of PII and credit card data.
*   **Access Management:** No documented "Least Privilege" or MFA policies.
*   **Monitoring:** Absence of an IDS/IPS system for network traffic analysis.
*   **Recovery:** No Disaster Recovery Plan (DRP) to handle business continuity.

## 3. NIST CSF Alignment
This audit evaluated the infrastructure across the five core functions of the NIST CSF:

*   **IDENTIFY:** Assets were identified, but the risk to EU customer data was previously underestimated.
*   **PROTECT:** Severe lack of encryption and access control protocols.
*   **DETECT:** Zero visibility into malicious lateral movement or external probes.
*   **RESPOND:** Incident response is currently ad-hoc without formal playbooks.
*   **RECOVER:** Recovery time objectives (RTO) cannot be guaranteed without a DRP.

## 4. Compliance Gap Analysis
| Standard | Status | Risk Description |
| :--- | :--- | :--- |
| **GDPR** | 🔴 Non-Compliant | High exposure to fines due to unencrypted EU resident data. |
| **PCI DSS** | 🔴 Non-Compliant | Violation of Requirement 3 (Protect Stored Cardholder Data). |
| **SOC2** | 🔴 Non-Compliant | Missing logical access controls and audit logging. |

## 5. Remediation Roadmap (Recommendations)
1.  **Encryption (Immediate):** Implement AES-256 for all databases and enforce TLS 1.3 for all web traffic.
2.  **Access Hardening:** Deploy a centralized IAM system with MFA and "Least Privilege" role-based access.
3.  **Network Visibility:** Integrate an Intrusion Detection System (IDS) and log all traffic to a centralized SIEM.
4.  **Resilience Planning:** Establish a Disaster Recovery Plan and conduct an annual security audit to maintain compliance.
