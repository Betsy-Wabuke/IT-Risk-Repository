# Backup & Recovery RCSA

## 1. Overview

This RCSA assesses risks and controls associated with the backup, protection, retention, restoration, and recovery of organizational IT systems and data.

Effective backup and recovery controls help ensure that critical systems and information can be restored following events such as system failure, accidental deletion, cyberattacks, data corruption, or other operational disruptions.


---

# 2. RCSA Assessment

| ID     | Sub-Process          | Risk                                                                                                                                 | Existing Control                                                  | Control Type | Likelihood | Impact | Inherent Risk | Control Effectiveness | Residual Risk | Treatment |
| ------ | -------------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------- | ------------ | ---------: | -----: | ------------: | --------------------- | ------------- | --------- |
| BR-001 | Backup Configuration | Critical systems may not be adequately backed up, resulting in inability to recover data following system failure or disruption.     | Scheduled backup procedures                                       | Preventive   |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| BR-002 | Backup Monitoring    | Backup failures may not be detected promptly, resulting in critical data remaining unprotected.                                      | Automated backup monitoring and alerts                            | Detective    |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| BR-003 | Backup Integrity     | Backup data may be corrupted or incomplete, resulting in unsuccessful recovery attempts.                                             | Backup integrity checks and validation                            | Detective    |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| BR-004 | Backup Retention     | Backup data may not be retained for an appropriate period, limiting the organization's ability to recover from historical incidents. | Backup retention policy                                           | Preventive   |          2 |      4 |  8 – Moderate | Effective             | Moderate      | Mitigate  |
| BR-005 | Backup Security      | Backup data may be accessed, altered, or deleted by unauthorized users.                                                              | Access controls, encryption, and restricted backup administration | Preventive   |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| BR-006 | Restoration Testing  | Backup data may not be successfully restored when required due to untested recovery procedures.                                      | Periodic restoration testing                                      | Detective    |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| BR-007 | Recovery Objectives  | Recovery procedures may not meet defined business recovery requirements, resulting in prolonged service disruption.                  | RTO and RPO requirements                                          | Preventive   |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| BR-008 | Disaster Recovery    | Critical IT services may not be restored within acceptable timelines following a major disruption.                                   | Disaster recovery plans and procedures                            | Corrective   |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |

---

# 3. Detailed RCSA Assessments

## BR-001 — Backup Configuration

### Sub-Process

Backup Scheduling and Configuration

### Risk

Critical systems may not be adequately backed up, resulting in inability to recover data following system failure or disruption.

### Existing Controls

* Scheduled backups
* Backup policies
* Backup configuration standards
* Backup coverage reviews

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Backup gaps may occur where systems are not included in backup schedules or backup configurations are incorrectly implemented.

### Impact

**5 – Critical**

Loss of critical data without a recoverable backup could significantly affect business operations.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Backup procedures exist, but coverage may not be complete across all critical systems.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Maintain an approved backup inventory and periodically reconcile critical systems against backup coverage to identify systems that are not adequately protected.

---

# BR-002 — Backup Monitoring

### Sub-Process

Backup Monitoring and Alerting

### Risk

Backup failures may not be detected promptly, resulting in critical data remaining unprotected.

### Existing Control

Automated backup monitoring, notifications, and periodic review of backup status.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Backup failures may remain unnoticed where monitoring is incomplete or alerts are not reviewed promptly.

### Impact

**5 – Critical**

Undetected backup failures may result in no recoverable backup being available when required.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Monitoring exists, but effectiveness may be reduced where alerts are not consistently reviewed or failed jobs remain unresolved.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Implement centralized monitoring of backup jobs and establish escalation procedures for failed or incomplete backups.

---

# BR-003 — Backup Integrity

### Sub-Process

Backup Integrity Validation

### Risk

Backup data may be corrupted or incomplete, resulting in unsuccessful recovery attempts.

### Existing Control

Backup integrity checks and periodic validation of backup data.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Backup corruption may occur due to storage failures, software issues, configuration errors, or other technical problems.

### Impact

**5 – Critical**

Corrupted backups may prevent recovery of critical systems and information.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Integrity checks exist, but they may not cover all backup sets or may not be performed consistently.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Perform periodic integrity validation and ensure critical backup sets are tested for recoverability.

---

# BR-004 — Backup Retention

### Sub-Process

Backup Retention Management

### Risk

Backup data may not be retained for an appropriate period, limiting the organization's ability to recover from historical incidents.

### Existing Control

Documented backup retention requirements based on business and regulatory needs.

### Control Type

**Preventive**

### Likelihood

**2 – Unlikely**

Defined retention requirements reduce the likelihood of inadequate backup history.

### Impact

**4 – Major**

Insufficient retention could prevent recovery from incidents that are discovered after a significant period.

### Inherent Risk

**2 × 4 = 8 – Moderate**

### Control Effectiveness

**Effective**

Retention requirements are documented and consistently applied to critical backup sets.

### Residual Risk

**Moderate**

### Treatment

**Mitigate**

### Recommended Action

Periodically review backup retention requirements against business, regulatory, and operational needs.

---

# BR-005 — Backup Security

### Sub-Process

Backup Access and Protection

### Risk

Backup data may be accessed, altered, or deleted by unauthorized users.

### Existing Controls

* Access restrictions
* Privileged access management
* Encryption
* Restricted backup administration
* Backup activity logging

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Backup environments may be targeted by attackers because they can provide access to large volumes of organizational data.

### Impact

**5 – Critical**

Unauthorized access or deletion of backups could prevent recovery and expose sensitive information.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Security controls exist, but weaknesses may remain in privileged access, monitoring, encryption, or backup administration.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Strengthen backup security through least-privilege access, strong authentication, encryption, administrative activity logging, and periodic privileged access reviews.

---

# BR-006 — Restoration Testing

### Sub-Process

Backup Restoration Testing

### Risk

Backup data may not be successfully restored when required due to untested recovery procedures.

### Existing Control

Periodic restoration testing for critical systems and data.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Backup restoration may fail because of corrupted backups, configuration dependencies, incomplete procedures, or infrastructure changes.

### Impact

**5 – Critical**

Failure to restore critical systems could result in prolonged service disruption and data loss.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Restoration testing exists, but tests may not cover all critical systems or may not occur frequently enough.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Establish periodic restoration tests for critical systems and document test results, recovery times, issues identified, and corrective actions.

---

# BR-007 — Recovery Objectives

### Sub-Process

Recovery Time Objective and Recovery Point Objective

### Risk

Recovery procedures may not meet defined business recovery requirements, resulting in prolonged service disruption or unacceptable data loss.

### Existing Controls

* Recovery Time Objectives (RTO)
* Recovery Point Objectives (RPO)
* Business impact assessments
* Recovery procedures

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Recovery requirements may not be accurately defined or may become outdated as business systems change.

### Impact

**5 – Critical**

Failure to meet recovery objectives could significantly disrupt business operations.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Recovery objectives exist, but they may not be consistently validated through actual recovery testing.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Periodically review RTO and RPO requirements with business and system owners and validate their achievability through recovery exercises.

---

# BR-008 — Disaster Recovery

### Sub-Process

Disaster Recovery Planning and Execution

### Risk

Critical IT services may not be restored within acceptable timelines following a major disruption.

### Existing Controls

* Disaster recovery plans
* Recovery procedures
* Alternative infrastructure
* Disaster recovery exercises
* Business continuity arrangements

### Control Type

**Corrective**

### Likelihood

**3 – Possible**

Recovery may be delayed due to outdated procedures, infrastructure dependencies, insufficient testing, or unclear recovery responsibilities.

### Impact

**5 – Critical**

Prolonged unavailability of critical IT services may significantly affect organizational operations.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Disaster recovery procedures exist, but effectiveness depends on regular testing, updated documentation, and availability of required resources.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Conduct periodic disaster recovery exercises and update recovery plans based on test results, system changes, and lessons learned.

---

# 4. RPO and RTO

## Recovery Point Objective — RPO

**RPO** represents the maximum acceptable amount of data loss measured in time.

Example:

> An RPO of 4 hours means the organization should be able to recover data to a point no more than approximately four hours before the disruption.

---

## Recovery Time Objective — RTO

**RTO** represents the target time within which a system or service should be restored following a disruption.

Example:

> An RTO of 2 hours means the service should be restored within approximately two hours after the disruption.

### Simple distinction

**RPO = How much data can we afford to lose?**

**RTO = How long can we afford to be unavailable?**

---

# 5. Backup and Recovery Evidence

Examples of evidence that may be requested during control testing include:

### Backup Configuration

* Backup schedules
* Backup configuration reports
* System-to-backup reconciliation
* Backup policy

### Backup Monitoring

* Backup job reports
* Failed backup reports
* Alert notifications
* Backup monitoring dashboards

### Backup Integrity

* Integrity check reports
* Backup validation results
* Error reports

### Restoration Testing

* Restoration test plans
* Restoration test results
* Recovery screenshots/logs
* Issues and corrective actions

### RTO/RPO

* Business impact assessments
* Approved RTO/RPO requirements
* Recovery testing results

### Disaster Recovery

* DR plans
* DR exercise reports
* Recovery timelines
* Lessons learned
* Corrective action tracking

---

# 6. Backup & Recovery Control Checklist

* [ ] Are all critical systems included in backup schedules?
* [ ] Are backup jobs monitored?
* [ ] Are failed backups escalated?
* [ ] Are backups protected against unauthorized access?
* [ ] Are backups encrypted where required?
* [ ] Are backup retention requirements documented?
* [ ] Are backups periodically tested for integrity?
* [ ] Are restoration tests performed?
* [ ] Are restoration results documented?
* [ ] Are RTOs defined?
* [ ] Are RPOs defined?
* [ ] Are RTO/RPO requirements periodically reviewed?
* [ ] Are disaster recovery exercises conducted?
* [ ] Are recovery weaknesses tracked to closure?

---

# 7. Key RCSA Observations

### 1. Backup does not equal recoverability

An organization can have successful backup jobs but still fail to restore the data when required.

Therefore:

**Backup → Validation → Restoration Testing**

### 2. Monitoring is critical

Backup failures should be detected and addressed promptly.

### 3. Backups must be protected

Backups can themselves become targets during cyberattacks. Appropriate access restrictions, authentication, encryption, and monitoring are therefore important.

### 4. RPO and RTO must reflect business requirements

Recovery objectives should be determined based on business impact and service criticality.

### 5. Recovery must be tested

A recovery plan that has never been tested provides limited assurance.

---

# 8. Backup & Recovery Lifecycle

The process can be represented as:

**Identify Critical Systems**

↓

**Define RPO/RTO**

↓

**Configure Backups**

↓

**Monitor Backup Jobs**

↓

**Validate Backup Integrity**

↓

**Protect Backup Data**

↓

**Perform Restoration Tests**

↓

**Conduct Disaster Recovery Exercises**

↓

**Review Results**

↓

**Remediate Gaps**

↓

**Continuous Monitoring**

---

# 9. RCSA Conclusion

Effective backup and recovery controls provide resilience against data loss, system failure, cyber incidents, and other operational disruptions.

The RCSA should therefore assess whether the organization can demonstrate:

* Complete backup coverage
* Successful backup execution
* Appropriate retention
* Backup security
* Backup integrity
* Successful restoration
* Defined RTOs and RPOs
* Tested disaster recovery procedures
* Evidence-based remediation of identified weaknesses

The ultimate objective is not simply to prove that backups exist, but to demonstrate that **critical systems and information can actually be recovered within acceptable business requirements**.
