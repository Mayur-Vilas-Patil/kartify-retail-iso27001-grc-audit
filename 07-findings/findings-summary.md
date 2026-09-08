# Kartify Retail – Audit Findings Summary

## Overview

The internal audit identified three minor nonconformities and one observation during the simulated ISO/IEC 27001:2022 internal audit.

### Audit Result

| Result                | Count |
| --------------------- | ----: |
| Conforming            |    16 |
| Minor Nonconformities |     3 |
| Major Nonconformities |     0 |
| Observations          |     1 |
| Total Tests           |    20 |

## NCR-01 – Legacy TLS Configuration

**Risk:** R04 – Payment Application Security
**Control:** A.8.24 – Use of Cryptography
**Classification:** Minor Nonconformity
**Status:** Open

### Finding

One of six payment endpoints permitted TLS 1.1 for an admin-facing payment reconciliation endpoint.

### Risk / Impact

Use of legacy TLS may increase the risk of interception or downgrade attacks and may have implications for payment security requirements.

### Root Cause

Manual provisioning occurred outside the standard deployment templates and hardening pipeline.

### Corrective Action

* Disable legacy TLS.
* Apply the standard hardening pipeline.
* Re-scan all payment endpoints.
* Verify that the insecure configuration is no longer present.

**Owner:** Engineering Lead – Payments
**Target Date:** 20-Sep-2026

---

## NCR-02 – Delayed Access Revocation

**Risk:** R08 – Seller KYC and Bank Data
**Control:** A.5.15 – Access Control
**Classification:** Minor Nonconformity
**Status:** Open

### Finding

One support staff account retained KYC download access approximately 60 days after a role change.

### Risk / Impact

Excessive access to sensitive seller KYC and banking information increases the risk of unauthorized access or disclosure.

### Root Cause

The role-change process did not include an automatic access-review trigger.

### Corrective Action

* Revoke inappropriate access.
* Introduce an automatic access-review trigger following role changes.
* Audit recent role transfers to identify similar cases.

**Owner:** Finance Manager coordinating HR/IT
**Target Date:** 15-Sep-2026

---

## NCR-03 – Database Change Approval

**Risk:** R10 – Database Change Management
**Control:** A.8.32 – Change Management
**Classification:** Minor Nonconformity
**Status:** Open

### Finding

One of ten sampled production database changes lacked a documented approval ticket.

### Risk / Impact

Insufficient change authorization evidence may increase the risk of unauthorized or uncontrolled production changes.

### Root Cause

The emergency/hotfix process allowed direct deployment without consistently enforced after-the-fact reconciliation.

### Corrective Action

* Require a retrospective change ticket within 24 hours for emergency changes.
* Perform monthly reconciliation between deployment logs and change tickets.
* Monitor compliance with the process.

**Owner:** Head of Infrastructure
**Target Date:** 20-Sep-2026

---

## OBS-01 – Privileged Access Review Sign-Off

**Risk:** R09 – Privileged Access
**Control:** A.5.18 – Access Rights
**Classification:** Observation
**Status:** Open

### Observation

The privileged AWS/system administrator access review was completed, but management sign-off occurred five days late.

No inappropriate access was identified.

### Recommendation

Introduce automated reminders and escalation for overdue privileged access review approvals.

---

## Corrective Action Closure

Findings should not be closed merely because a procedure or configuration has been changed.

Closure should require objective evidence demonstrating that:

1. The corrective action has been implemented.
2. The action is operating effectively.
3. The issue has been verified by the auditor or designated verifier.
4. Evidence of implementation and effectiveness has been recorded.

Following verification, the NCR status should be updated and the relevant risk register entries should be reviewed.
