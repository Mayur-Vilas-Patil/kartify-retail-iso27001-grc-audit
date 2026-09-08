# Kartify Retail — ISO/IEC 27001:2022 GRC & Internal Audit Project

> **Hands-on GRC portfolio project demonstrating ISMS context, information asset management, risk assessment, Statement of Applicability, control testing, internal audit, nonconformity management and corrective action tracking.**

![ISO 27001](https://img.shields.io/badge/ISO%2FIEC%2027001%3A2022-ISMS-blue)
![GRC](https://img.shields.io/badge/Domain-GRC-orange)
![Internal Audit](https://img.shields.io/badge/Internal%20Audit-ISO%2019020%2C%20ISO%2019011-green)
![Project](https://img.shields.io/badge/Project-Fictional%20Case%20Study-lightgrey)

---

## ⚠️ Important Disclaimer

This repository is a **fictional hands-on GRC and internal-audit case study** created for professional learning and portfolio development.

All organizational information, assets, risks, audit evidence, findings and control-test results are simulated.

This project is **not evidence of an actual ISO/IEC 27001 certification audit, certification, client engagement or real organizational assessment.**

---

# 1. Project Overview

**Kartify Retail** is a fictional Indian e-commerce marketplace connecting customers with third-party sellers and supporting order management, logistics and payment processing.

The organization operates a cloud-native technology environment hosted on AWS and processes information including:

* Customer personal information
* Cardholder/payment transaction data
* Seller KYC information
* Seller bank/payout information
* Order and delivery information

The case study considers information-security and compliance requirements relevant to:

* **ISO/IEC 27001:2022**
* **India Digital Personal Data Protection (DPDP) Act 2023**
* **PCI DSS v4.0**

The project demonstrates how a GRC analyst can move from organizational context and information assets through risk assessment and control selection into internal audit and corrective action.

---

# 2. Project Objective

The objective of this project was to build a practical, traceable GRC workflow rather than produce isolated compliance documents.

The project demonstrates:

1. Understanding organizational context
2. Identifying interested parties and information-security requirements
3. Defining the ISMS scope
4. Building an information asset register
5. Identifying and assessing information-security risks
6. Mapping risks to ISO/IEC 27001:2022 Annex A controls
7. Developing a Statement of Applicability
8. Designing a risk-based internal audit
9. Testing control implementation and operating effectiveness
10. Recording nonconformities and observations
11. Developing corrective actions
12. Defining evidence-based audit closure requirements

---

# 3. GRC Lifecycle Demonstrated

```text
Organizational Context
        │
        ▼
Information Asset Register
        │
        ▼
Risk Register
        │
        ▼
Statement of Applicability
        │
        ▼
Internal Audit Planning
        │
        ▼
Control Testing
        │
        ▼
Findings / NCRs / Observations
        │
        ▼
Corrective Action Plan
        │
        ▼
Follow-up & Closure
```

The objective is to demonstrate **traceability** across the lifecycle rather than treating each document as a standalone deliverable.

---
# 4. Project Architecture

| Stage | Deliverable | Primary Purpose |
| ----- | ----------- | --------------- |
| 01 | Context of Organization | Define business context, interested parties and ISMS scope |
| 02 | Information Asset Register | Identify information and associated assets |
| 03 | Risk Register | Identify and assess information-security risks |
| 04 | Internal Audit Checklist | Define risk-based audit tests and control evaluation criteria |
| 05 | Statement of Applicability | Document control applicability, justification and risk relationship |
| 06 | Internal Audit Report | Document audit scope, testing, results and findings |
| 07 | Findings & Corrective Actions | Track NCRs, observations and corrective actions |
| 08 | Follow-up & Closure | Verify implementation and operating effectiveness |
---

# 5. Stage 01 — Context of the Organization

The Context of Organization document addresses ISO/IEC 27001:2022 Clause 4 and establishes the foundation for the ISMS.

### Key areas covered

* Internal organizational factors
* External organizational factors
* Business model
* Technology environment
* Governance structure
* Regulatory considerations
* Interested parties
* Information-security expectations
* ISMS scope
* ISMS boundaries and exclusions

### Technology environment

The fictional environment includes:

* AWS EC2
* AWS RDS
* AWS S3
* E-commerce marketplace platform
* Payment gateway integration
* Order-management system
* Logistics tracking

### Key information types

* Customer PII
* Cardholder/payment transaction data
* Seller KYC data
* Seller bank-account data
* Order and delivery data

---

# 6. Stage 02 — Information Asset Register

The Asset Register identifies information and associated assets relevant to the ISMS.

Examples include:

* AWS production environment
* Marketplace platform
* Payment gateway integration module
* Order-management and logistics system
* Customer PII
* Cardholder/payment transaction data
* Seller KYC and bank-account data
* Privileged administrative roles

The register applies a CIA-oriented impact assessment to help establish the security significance of assets.

---

# 7. Stage 03 — Risk Register

The Risk Register uses a qualitative **Impact × Likelihood** methodology.

### Risk methodology

```text
Risk = Impact × Likelihood
```

A 3 × 3 qualitative risk matrix is used to classify inherent risk.

The risk register links identified risks back to the information assets established during the previous stage.

### Key risk themes

The project considers risks involving:

* Cloud production access
* Application vulnerabilities
* Secure coding
* Payment security
* Order-management access
* Customer PII
* Cardholder/payment data
* Seller KYC and bank data
* Privileged accounts
* Database changes
* Critical third-party suppliers

---

# 8. Stage 04 — Statement of Applicability

The Statement of Applicability provides the control-selection layer between risk management and internal audit.

The SoA maps identified risks to relevant ISO/IEC 27001:2022 Annex A controls and documents:

* Control applicability
* Risk relationship
* Justification
* Policy/control intent
* Treatment direction
* Residual-risk considerations

Examples of mapped controls include:

| Risk | Annex A Control | Control Theme                         |
| ---- | --------------- | ------------------------------------- |
| R01  | A.5.18          | Access rights                         |
| R01  | A.8.9           | Configuration management              |
| R03  | A.8.8           | Vulnerability management              |
| R03  | A.8.28          | Secure coding                         |
| R04  | A.8.24          | Use of cryptography                   |
| R05  | A.5.15          | Access control                        |
| R05  | A.8.32          | Change management                     |
| R06  | A.8.15          | Logging                               |
| R09  | A.5.16          | Identity management                   |
| R12  | A.5.19 / A.5.20 | Supplier relationships and agreements |

---

# 9. Stage 05 — Internal Audit

The internal audit was designed as a **risk-driven control assessment** rather than a generic checklist exercise.

### Audit basis

* ISO/IEC 27001:2022 Clause 9.2
* ISO 19011 audit principles and methodology
* Kartify Retail Risk Register
* Statement of Applicability/control mapping
* Applicable policies and procedures
* Operational evidence

### Audit methodology

The audit approach included:

* Document review
* Interviews
* Configuration review
* Evidence sampling
* Access-right testing
* Supplier-document review
* Finding evaluation

---

# 10. Audit Scope

The simulated audit focused on:

* Access control and identity management
* Application security
* Payment security
* Data protection
* Database change management
* Critical supplier security

The audit included selected AWS production assets, marketplace/payment/order-management systems, sensitive information assets, privileged roles and the critical payment gateway supplier.

The full organization-wide Annex A applicability assessment was intentionally outside the audit scope and was treated as a separate SoA activity.

---

# 11. Audit Results

The audit contained **20 control tests**.

| Result                |  Count |
| --------------------- | -----: |
| Conforming tests      |     16 |
| Minor Nonconformities |      3 |
| Observations          |      1 |
| Major Nonconformities |      0 |
| **Total tests**       | **20** |

### Overall conclusion

> **PARTIALLY CONFORMING — CORRECTIVE ACTION REQUIRED**

The audit identified localized operating-effectiveness gaps rather than evidence of a systemic ISMS failure within the simulated audit scope.

---

# 12. Key Audit Findings

## NCR-01 — Cryptographic Control

**Control:** A.8.24 — Use of Cryptography
**Risk:** R04 — Payment Gateway Integration Module

A configuration review identified one admin-facing payment-reconciliation endpoint that permitted TLS 1.1 cipher suites instead of the required TLS 1.2+ configuration.

### Corrective action

* Disable legacy TLS ciphers
* Bring the endpoint under the standard hardening pipeline
* Re-scan payment-related endpoints
* Verify TLS 1.2+ compliance

---

## NCR-02 — Access Control

**Control:** A.5.15 — Access Control
**Risk:** R08 — Seller/Vendor KYC & Bank Account Data

One support-staff account retained download-level access to seller KYC/bank documents approximately 60 days after the employee moved to a different role.

### Corrective action

* Add an access-review trigger to the role-change workflow
* Revoke the identified access
* Review access for recent role changes
* Verify that role changes consistently trigger access adjustments

---

## NCR-03 — Change Management

**Control:** A.8.32 — Change Management
**Risk:** R10 — Production Database Changes

One of ten sampled production database changes lacked a documented change-approval ticket.

### Corrective action

* Enforce retrospective ticketing for emergency changes
* Require reconciliation within the defined period
* Introduce monthly reconciliation between deployment logs and change tickets
* Verify evidence during follow-up

---

## OBS-01 — Privileged Access Review

**Control:** A.5.18 — Access Rights
**Risk:** R09 — System Administrator

The quarterly privileged-access review was completed, but management sign-off was recorded five days after the defined target.

No inappropriate access was identified.

### Recommendation

Introduce automated reminders and escalation for overdue access-review sign-offs.

---

# 13. Corrective Action Management

A key principle demonstrated in this project is that **changing a procedure or configuration is not sufficient to close an audit finding.**

Closure requires objective evidence demonstrating:

1. The corrective action was implemented
2. The underlying root cause was addressed
3. The control is operating effectively
4. The issue has not recurred in an appropriate follow-up sample

This demonstrates the difference between:

```text
Action Implemented
        ≠
Finding Closed
```

The expected progression is:

```text
Finding
   ↓
Root Cause
   ↓
Corrective Action
   ↓
Implementation Evidence
   ↓
Effectiveness Verification
   ↓
Formal Closure
```

---

# 14. Key GRC Skills Demonstrated

### Governance

* ISMS structure
* Organizational context
* Interested-party analysis
* Scope definition
* Document control

### Risk Management

* Asset identification
* CIA impact assessment
* Risk identification
* Impact × likelihood assessment
* Risk treatment
* Risk-to-control traceability

### Compliance

* ISO/IEC 27001:2022
* Annex A control mapping
* DPDP Act considerations
* PCI DSS considerations

### Internal Audit

* Audit planning
* Risk-based scope
* Audit criteria
* Sampling
* Objective evidence
* Control testing
* Finding classification
* NCR management
* Corrective action verification

### Documentation

* Controlled documents
* Risk registers
* Asset registers
* Statement of Applicability
* Audit checklists
* Audit reports
* Corrective Action Plans

---

# 15. Evidence & Traceability

One of the main objectives of this portfolio is to demonstrate traceability.

```text
Asset
  │
  ▼
Risk
  │
  ▼
Control
  │
  ▼
Audit Test
  │
  ▼
Evidence
  │
  ▼
Finding
  │
  ▼
Corrective Action
  │
  ▼
Verification
```

Example:

```text
Seller KYC / Bank Data
        ↓
R08 — Unauthorized / Excessive Access
        ↓
A.5.15 — Access Control
        ↓
KA-13 — Access-control audit test
        ↓
8 sampled seller-support accounts
        ↓
1 account retained access after role change
        ↓
NCR-02
        ↓
Role-change access-review trigger
        ↓
Follow-up sampling
```

This traceability is a core feature of the project.

---

# 16. Repository Contents

kartify-retail-iso27001-grc-audit/
│
├── 01-context/
│   └── Kartify_Retail_Context_of_Organization.docx
│
├── 02-asset-register/
│   └── Kartify_Retail_Asset_Register.xlsx
│
├── 03-risk-register/
│   └── Kartify_Retail_Risk_Register.xlsx
│
├── 04-internal-audit-checklist/
│   └── Kartify_Retail_Internal_Audit_Checklist_PROFESSIONAL.xlsx
│
├── 05-statement-of-applicability/
│   └── Kartify_Retail_Comprehensive_SoA.xlsx
│
├── 06-internal-audit/
│   └── Kartify_Retail_Internal_Audit_Report.docx
│
├── 07-findings/
│   └── findings-summary.md
│
├── screenshots/
│
└── README.md
```

Each stage represents a logical component of the GRC lifecycle.

---

# 17. Tools & Frameworks

### Frameworks / Standards

* ISO/IEC 27001:2022
* ISO 19011
* PCI DSS v4.0
* India DPDP Act 2023

### Tools

* Microsoft Excel
* Microsoft Word
* GitHub
* Markdown
* Structured risk and audit workbooks

---

# 18. What I Learned From This Project

This project helped me understand that GRC is not simply about checking whether a control exists.

A useful GRC process must connect:

**Business context → assets → risks → controls → evidence → findings → corrective actions → verification.**

The internal audit stage also demonstrated the importance of distinguishing between:

* Control design
* Control implementation
* Operating effectiveness
* Evidence quality
* Corrective action effectiveness

---

# 19. Future Improvements

Planned improvements include:

* Formalizing the ISMS scope document
* Expanding Annex A coverage
* Adding risk treatment tracking
* Building a formal risk acceptance workflow
* Adding control-owner dashboards
* Adding KPI/KRI reporting
* Creating audit evidence indexing
* Adding corrective-action aging metrics
* Performing Stage 5 corrective-action follow-up
* Expanding the audit scope to additional technology and operational areas

---

# 20. Project Disclaimer

This repository is intended solely as a **professional learning and portfolio demonstration**.

Kartify Retail is fictional. All audit evidence, findings, risks, control assessments and organizational information are simulated.

No claim is made that Kartify Retail is ISO/IEC 27001 certified or that the author performed a real external certification audit.

---

## Author

**Mayur Vilas Patil**

GRC Analyst | ISO/IEC 27001:2022 Practice

Interested in:

* Governance, Risk & Compliance
* Information Security
* ISO/IEC 27001
* Internal Audit
* Risk Management
* Security Compliance

[LinkedIn](#) • [GitHub](#)
