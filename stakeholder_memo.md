# Stakeholder Memorandum: Botium Toys Risk Assessment

**TO:** IT Manager, Botium Toys  
**FROM:** Arthur Sousa, Cybersecurity Analyst  
**SUBJECT:** Internal Security Audit – Risk Assessment & Recommendations

## Scope
The audit covers Botium Toys' internal IT infrastructure, including the storefront, warehouse, and global e-commerce servers.

## Critical Assets
1.  **Customer PII:** Personal data of US and EU customers.
2.  **Payment Processing:** Credit card transaction systems.
3.  **Intellectual Property:** Proprietary toy designs and warehouse data.

## Risk Assessment Summary
Currently, Botium Toys operates at a **High Risk** level. The lack of data encryption and "Least Privilege" access controls makes the company highly vulnerable to data breaches. Operating in the EU without GDPR compliance exposes the company to massive legal penalties.

## Recommended Action Plan
1.  **Technical (High Priority):** Implement AES-256 encryption for all data at rest and in transit. Deploy an IDS to monitor the global storefront.
2.  **Administrative (High Priority):** Establish a "Least Privilege" access policy and a formal Disaster Recovery Plan.
3.  **Compliance:** Conduct a Gap Analysis for PCI DSS immediately to avoid transaction processing penalties.
