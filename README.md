# Internal Security Audit – Botium Toys

## Project Overview
As part of a simulated cybersecurity exercise, I conducted a detailed internal security audit for **Botium Toys**, 
a fictional small U.S. business with an expanding global online presence. The objective was to identify critical security gaps and ensure compliance 
with major regulatory frameworks including **NIST CSF**, **PCI DSS**, and **GDPR**.

This audit was designed to mirror real-world practices used by cybersecurity teams in risk assessment, control evaluation, and compliance alignment.

---

## Audit Scope
The following activities were performed:

- Reviewed asset inventory and risk reports
- Evaluated implementation of key technical and administrative security controls
- Mapped controls against compliance standards (PCI DSS, GDPR, SOC)
- Delivered actionable recommendations to improve the company’s security posture

---

## Security Controls Evaluated

| Control                          | Status  | Findings Summary                                                                 |
|----------------------------------|---------|----------------------------------------------------------------------------------|
| Least Privilege                  | ✘       | All employees have access to customer data; access controls need implementation |
| Disaster Recovery Plan           | ✘       | No DR plans in place to ensure business continuity                              |
| Password Policies                | ✘       | Minimal password requirements; risk of credential-based attacks                 |
| Separation of Duties             | ✘       | CEO manages operations and payroll; role separation lacking                     |
| Firewall                         | ✔       | Firewall is active with defined security rules                                  |
| Intrusion Detection System (IDS) | ✘       | IDS is not currently implemented                                                |
| Data Backups                     | ✘       | No verified backup plan for critical data                                       |
| Antivirus Software               | ✔       | Installed and maintained by the IT team                                         |
| Legacy System Monitoring         | ✘       | No regular monitoring schedule; procedures unclear                              |
| Encryption                       | ✘       | Not used on sensitive data or payment systems                                   |
| Password Management System       | ✘       | Not implemented                                                                 |
| Physical Security (Locks, CCTV) | ✔       | Adequate locks and surveillance systems in place                                |
| Fire Detection/Prevention        | ✔       | Fire alarms and suppression systems functional                                  |

---

## Compliance Gaps Identified

### PCI DSS
- ❌ All employees have access to customer credit card data
- ❌ No encryption of stored or transmitted cardholder data
- ❌ No secure password management system

### GDPR
- ❌ E.U. customer data is not encrypted
- ✔ Incident response policy includes 72-hour breach notification
- ❌ Data is inventoried but not classified
- ✔ Basic privacy policies are enforced

### SOC (Type 1/2)
- ❌ No user access control policy or separation of duties
- ❌ No encryption for sensitive personal information
- ✔ Data integrity controls are in place

---

## Key Recommendations
To strengthen Botium Toys' cybersecurity posture and regulatory compliance:

1. Implement **Least Privilege** and **Separation of Duties** policies.
2. Create and document a **Disaster Recovery Plan**.
3. Enforce **strong password policies** and deploy a **password management system**.
4. Implement **Intrusion Detection System (IDS)** to monitor network threats.
5. Regularly **monitor and manage legacy systems**.
6. Encrypt sensitive data (PII, SPII, payment info) at rest and in transit.
7. Classify existing data assets for better control mapping.

---

## Deliverables in This Repo
- `controls-checklist.md` – Security control review and gaps
- `compliance-checklist.md` – Mapping to PCI DSS, GDPR, and SOC
- `recommendations.md` – Action plan for remediation and policy changes
- `audit-summary.pdf` – Executive-level summary (optional for presentation)

---

## Tools & Frameworks Used
- NIST Cybersecurity Framework (CSF)
- PCI DSS v3.2.1
- General Data Protection Regulation (GDPR)
- System and Organization Controls (SOC 2)

---

## What I Learned
- How to assess an organization’s security readiness using established frameworks
- Mapping technical findings to compliance requirements
- Communicating risk in clear, actionable language for stakeholders
