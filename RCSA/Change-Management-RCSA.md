# Change Management RCSA

## 1. Overview

This RCSA assesses risks and controls associated with managing changes to IT systems, applications, infrastructure, and production environments.

Effective change management ensures that changes are appropriately requested, assessed, tested, approved, implemented, documented, and reviewed.

> **Note:** This is a fictional assessment created for educational and professional portfolio purposes.

---

## 2. RCSA Assessment

| ID     | Sub-Process                | Risk                                                                                                                            | Existing Control                                    | Control Type         | Likelihood | Impact | Inherent Risk | Control Effectiveness | Residual Risk | Treatment |
| ------ | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- | -------------------- | ---------: | -----: | ------------: | --------------------- | ------------- | --------- |
| CM-001 | Change Request             | Changes may be implemented without adequate documentation, resulting in unauthorized or poorly controlled system modifications. | Formal change request process                       | Preventive           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| CM-002 | Change Approval            | Changes may be implemented without appropriate authorization, resulting in unauthorized system modifications.                   | Change approval workflow                            | Preventive           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| CM-003 | Change Testing             | Insufficient testing may result in defective changes being introduced into production environments.                             | Testing and validation procedures                   | Preventive           |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| CM-004 | Production Changes         | Unauthorized or inappropriate production changes may affect system availability, integrity, or security.                        | Production change controls and restricted access    | Preventive           |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| CM-005 | Emergency Changes          | Emergency changes may bypass standard change controls, increasing the risk of unauthorized or poorly tested changes.            | Emergency change procedure and retrospective review | Preventive/Detective |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| CM-006 | Segregation of Duties      | The same individual may request, approve, and implement a change, reducing independent oversight.                               | Segregation of duties and approval controls         | Preventive           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| CM-007 | Post-Implementation Review | Failed or inappropriate changes may not be identified and addressed promptly due to inadequate post-implementation review.      | Post-implementation review process                  | Detective            |          2 |      4 |  8 – Moderate | Partially Effective   | Moderate      | Mitigate  |

---

# 3. Detailed RCSA Assessments

## CM-001 — Change Request

### Sub-Process

Change Request Management

### Risk

Changes may be implemented without adequate documentation, resulting in unauthorized or poorly controlled system modifications.

### Existing Control

A formal change request process requiring changes to be documented before implementation.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Changes may be implemented outside the formal process where processes are not consistently enforced.

### Impact

**4 – Major**

Poorly documented changes can affect system stability, security, integrity, and auditability.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

A formal process exists, but effectiveness may be reduced when changes are not consistently recorded or supporting documentation is incomplete.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Require all planned production changes to have documented change requests containing the business justification, scope, implementation plan, risk assessment, testing evidence, approval, and rollback procedure.

---

## CM-002 — Change Approval

### Sub-Process

Change Authorization

### Risk

Changes may be implemented without appropriate authorization, resulting in unauthorized system modifications.

### Existing Control

A formal change approval workflow requiring authorization from designated approvers.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Changes may bypass the approval process where enforcement is weak or emergency procedures are misused.

### Impact

**4 – Major**

Unauthorized changes may compromise system integrity, security, or availability.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Approval controls exist, but exceptions or incomplete evidence may weaken the control.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Enforce documented approval before production implementation and periodically review change records for evidence of appropriate authorization.

---

## CM-003 — Change Testing

### Sub-Process

Change Testing and Validation

### Risk

Insufficient testing may result in defective changes being introduced into production environments.

### Existing Control

Changes are tested in an appropriate non-production environment before production implementation.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Changes may be insufficiently tested due to time pressure, incomplete test plans, or inadequate test environments.

### Impact

**5 – Critical**

A defective change could cause significant service disruption, data integrity issues, security weaknesses, or system failure.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Testing procedures exist, but evidence of testing may be incomplete or inconsistent for some changes.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Require documented test plans and test results for production changes, including evidence that identified defects have been resolved before implementation.

---

## CM-004 — Production Changes

### Sub-Process

Production Change Implementation

### Risk

Unauthorized or inappropriate production changes may affect system availability, integrity, or security.

### Existing Controls

* Restricted production access
* Approved change requests
* Change implementation procedures
* Activity logging

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Weak enforcement of production access and change procedures may allow unauthorized changes.

### Impact

**5 – Critical**

Unauthorized changes to critical production systems could cause significant operational or security consequences.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Production controls exist, but weaknesses may remain where access restrictions, approvals, or monitoring are not consistently enforced.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Restrict production access to authorized personnel and ensure all production changes are linked to approved change records.

---

## CM-005 — Emergency Changes

### Sub-Process

Emergency Change Management

### Risk

Emergency changes may bypass standard change controls, increasing the risk of unauthorized or poorly tested changes.

### Existing Control

Emergency change procedures requiring justification, authorization, documentation, and retrospective review.

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

Emergency circumstances can result in expedited changes where normal processes are bypassed.

### Impact

**4 – Major**

Poorly controlled emergency changes can cause system instability, security weaknesses, or operational disruption.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Emergency procedures exist, but retrospective reviews or supporting documentation may not always be completed.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Require all emergency changes to have documented justification and authorization and conduct a retrospective review after implementation.

---

## CM-006 — Segregation of Duties

### Sub-Process

Change Role Separation

### Risk

The same individual may request, approve, and implement a change, reducing independent oversight and increasing the risk of unauthorized modifications.

### Existing Control

Segregation of duties between change requestors, approvers, testers, and implementers.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Conflicting responsibilities may arise where access roles are not properly designed or reviewed.

### Impact

**4 – Major**

Lack of independent oversight could allow unauthorized or inappropriate changes to be implemented without detection.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

SoD controls exist, but exceptions may occur where role assignments are not periodically reviewed.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Maintain a change-management SoD matrix and periodically review user permissions to ensure request, approval, testing, and implementation responsibilities are appropriately separated.

---

## CM-007 — Post-Implementation Review

### Sub-Process

Post-Implementation Review

### Risk

Failed or inappropriate changes may not be identified and addressed promptly due to inadequate post-implementation review.

### Existing Control

Post-implementation reviews are performed for selected changes.

### Control Type

**Detective**

### Likelihood

**2 – Unlikely**

The existence of review procedures reduces the likelihood that failed changes remain unidentified.

### Impact

**4 – Major**

Failure to identify issues following implementation could result in prolonged operational or security problems.

### Inherent Risk

**2 × 4 = 8 – Moderate**

### Control Effectiveness

**Partially Effective**

Post-implementation reviews exist, but coverage may not be consistent across all relevant changes.

### Residual Risk

**Moderate**

### Treatment

**Mitigate**

### Recommended Action

Define clear criteria for post-implementation reviews and ensure significant, failed, and emergency changes are reviewed and documented.

---

# 4. Key RCSA Observations

The assessment highlights several important principles of change management.

### 1. Authorization

Changes should be appropriately authorized before implementation.

### 2. Testing

Changes should be tested before being introduced into production environments.

### 3. Segregation of Duties

The request, approval, testing, and implementation functions should be appropriately separated.

### 4. Production Access

Production access should be restricted to authorized personnel.

### 5. Emergency Changes

Emergency procedures should not become a mechanism for routinely bypassing normal controls.

### 6. Auditability

Changes should be traceable through appropriate documentation and system logs.

### 7. Post-Implementation Review

Significant and unsuccessful changes should be reviewed to identify lessons and corrective actions.

---

# 5. Change Management Control Checklist

When assessing change management, consider:

* [ ] Is a formal change request required?
* [ ] Is the business justification documented?
* [ ] Has the change been appropriately assessed?
* [ ] Has the change been approved?
* [ ] Has testing been completed?
* [ ] Is test evidence available?
* [ ] Is there an implementation plan?
* [ ] Is there a rollback/backout plan?
* [ ] Is production access appropriately restricted?
* [ ] Are conflicting responsibilities segregated?
* [ ] Are emergency changes appropriately controlled?
* [ ] Are changes logged?
* [ ] Are failed changes investigated?
* [ ] Are significant changes subject to post-implementation review?

---

# 6. RCSA Conclusion

Effective change management reduces the likelihood that unauthorized, poorly tested, or inappropriate changes will affect production systems.

A mature change management environment should provide evidence that changes are:

**Requested → Assessed → Tested → Approved → Implemented → Monitored → Reviewed**

The effectiveness of these controls should be periodically assessed through evidence-based testing rather than simply confirming that a documented change-management procedure exists.
