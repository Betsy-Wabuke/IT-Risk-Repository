# Access Management RCSA

## 1. Overview

This RCSA assesses risks and controls associated with managing user access to organizational IT systems.

The assessment covers the access lifecycle from provisioning through modification, review, and deprovisioning.

> **Note:** This is a fictional assessment created for educational and professional portfolio purposes.

---

## 2. RCSA Assessment

| ID     | Sub-Process           | Risk                                                                                                                       | Existing Control                                     | Control Type         | Likelihood | Impact | Inherent Risk | Control Effectiveness | Residual Risk | Treatment |
| ------ | --------------------- | -------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------- | -------------------- | ---------: | -----: | ------------: | --------------------- | ------------- | --------- |
| AM-001 | User Provisioning     | Inadequate approval of user access may result in users receiving unauthorized or excessive system privileges.              | Access request and approval process                  | Preventive           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| AM-002 | User Deprovisioning   | Failure to promptly disable accounts of terminated employees may result in unauthorized access to systems and information. | Joiner-Mover-Leaver process and account deactivation | Preventive           |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| AM-003 | Privileged Access     | Excessive or inappropriate privileged access may result in unauthorized changes to critical systems.                       | PAM, privileged access reviews and approval          | Preventive/Detective |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| AM-004 | Generic Accounts      | Use of shared administrative accounts may prevent individual attribution of system activity and reduce accountability.     | PAM, audit trails and SoD                            | Preventive/Detective |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| AM-005 | Access Review         | Failure to periodically review user access may result in inappropriate or excessive privileges remaining undetected.       | Periodic user access reviews                         | Detective            |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| AM-006 | Segregation of Duties | Conflicting access privileges may allow one user to perform incompatible activities without appropriate oversight.         | Role-based access and SoD review                     | Preventive/Detective |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |

---

# 3. Detailed RCSA Assessments

## AM-001 — User Provisioning

### Sub-Process

User Access Provisioning

### Risk

Inadequate approval of user access may result in users receiving unauthorized or excessive system privileges.

### Existing Control

Access requests are submitted and approved before access is provisioned.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Inadequately approved access requests may occur where approval processes are not consistently followed or evidence is incomplete.

### Impact

**4 – Major**

Excessive or unauthorized access could result in unauthorized data access, modification, or system activity.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

The approval process exists, but control effectiveness may be reduced where approvals are inconsistent, incomplete, or not periodically reviewed.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Strengthen access provisioning controls by requiring documented approval from authorized system owners before access is granted and periodically reviewing provisioning records for compliance.

---

# AM-002 — User Deprovisioning

### Sub-Process

Employee Termination / Account Deactivation

### Risk

Failure to promptly disable accounts belonging to terminated employees may result in unauthorized access to organizational systems and information.

### Existing Controls

* Joiner-Mover-Leaver process
* HR notification to IT
* Account deactivation procedures
* Periodic account reconciliation

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Delays may occur where termination notifications are incomplete, delayed, or not properly integrated with IT processes.

### Impact

**5 – Critical**

A former employee retaining access could potentially access systems or information without authorization.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

The process exists, but effectiveness may be reduced where account deactivation depends on manual notifications or reconciliation.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Implement periodic reconciliation between HR termination records and active system accounts and ensure terminated accounts are disabled promptly.

---

# AM-003 — Privileged Access

### Sub-Process

Privileged Account Management

### Risk

Excessive or inappropriate privileged access may result in unauthorized changes to critical systems.

### Existing Controls

* Privileged Access Management
* Privileged access approval
* Periodic privileged access reviews
* Activity logging

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

Privileged access weaknesses can occur where permissions are not regularly reviewed or appropriately restricted.

### Impact

**5 – Critical**

Compromise or misuse of privileged access could significantly affect critical systems, information, and operations.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Privileged access controls exist, but weaknesses may remain where access is excessive, reviews are incomplete, or privileged activities are not adequately monitored.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Conduct periodic privileged access reviews and ensure privileged permissions are restricted according to business need and least-privilege principles.

---

# AM-004 — Generic Administrative Accounts

### Sub-Process

Shared / Generic Account Management

### Risk

Use of shared administrative accounts may prevent individual attribution of system activity and reduce accountability.

### Existing Controls

* Privileged Access Management
* Audit trails
* Segregation of Duties

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

### Impact

**4 – Major**

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Controls exist, but shared account usage limits individual accountability and traceability.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Eliminate unnecessary generic administrative accounts and require uniquely assigned named accounts for privileged activities. Where shared accounts are unavoidable, implement appropriate compensating controls.

---

# AM-005 — Access Review

### Sub-Process

Periodic User Access Review

### Risk

Failure to periodically review user access may result in inappropriate or excessive privileges remaining undetected.

### Existing Control

Periodic access reviews performed by system or application owners.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Inadequate or inconsistent access reviews may allow inappropriate access to remain undetected.

### Impact

**4 – Major**

Excessive access could result in unauthorized system activity or inappropriate access to sensitive information.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

The review process exists, but effectiveness may be reduced by incomplete reviews, inadequate evidence, or failure to remediate identified exceptions.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Standardize periodic access reviews, require documented owner approval, track identified exceptions, and monitor remediation through closure.

---

# AM-006 — Segregation of Duties

### Sub-Process

Role and Access Conflict Management

### Risk

Conflicting access privileges may allow one user to perform incompatible activities without appropriate oversight.

### Existing Controls

* Role-based access control
* Segregation of duties matrix
* Periodic access reviews
* Approval requirements

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

Conflicting access may occur where roles are not appropriately defined or SoD conflicts are not identified during access reviews.

### Impact

**4 – Major**

Conflicting privileges could facilitate unauthorized changes, fraud, or inappropriate activities.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

SoD controls exist, but conflicts may remain where role definitions are incomplete or reviews do not adequately identify and resolve incompatible privileges.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Maintain an approved SoD matrix, periodically review access conflicts, document exceptions, and ensure identified conflicts are appropriately remediated or formally approved.

---

# 4. Key RCSA Observations

The assessment identifies several recurring themes:

### 1. Access lifecycle management

Access should be managed throughout the user lifecycle:

**Joiner → Mover → Leaver**

### 2. Least Privilege

Users should receive only the access required to perform their authorized responsibilities.

### 3. Privileged Access

Administrative access requires stronger controls because privileged users can significantly affect critical systems.

### 4. Accountability

Privileged activities should be attributable to uniquely identifiable users.

### 5. Periodic Review

Access should not be considered permanently appropriate simply because it was initially approved.

### 6. Segregation of Duties

Conflicting responsibilities should be appropriately separated to reduce the risk of unauthorized or inappropriate activity.

---

# 5. RCSA Conclusion

The assessment demonstrates that access management risks can remain significant even where controls are already implemented.

Control effectiveness should therefore be assessed based on whether controls are:

* Appropriately designed
* Implemented
* Consistently operating
* Supported by evidence
* Periodically reviewed
* Corrective actions followed through to closure

The objective of the RCSA is not simply to document controls but to determine whether the controls adequately reduce the organization's risk exposure.
