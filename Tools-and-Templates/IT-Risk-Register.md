# IT Risk Register

## 1. Purpose

The IT Risk Register is used to document, assess, prioritize, treat, and monitor identified technology-related risks.

The examples in this register are fictional and are intended for educational and professional portfolio purposes.

---

## 2. Risk Register

| Risk ID | Risk Category                | Risk Statement                                                                                                                                                                      | Likelihood | Impact | Score | Rating   | Treatment | Status      |
| ------- | ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------: | -----: | ----: | -------- | --------- | ----------- |
| IT-R001 | Access Management            | The use of generic administrative accounts may prevent individual attribution of system changes, increasing the risk of unauthorized or inappropriate changes remaining undetected. |          4 |      4 |    16 | Major    | Mitigate  | Open        |
| IT-R002 | Identity & Access Management | Failure to promptly disable accounts belonging to former employees may result in unauthorized access to organizational systems and information.                                     |          3 |      5 |    15 | Major    | Mitigate  | Open        |
| IT-R003 | Vulnerability Management     | Delayed remediation of critical vulnerabilities may expose systems to exploitation, potentially resulting in system compromise or service disruption.                               |          4 |      5 |    20 | Critical | Mitigate  | In Progress |
| IT-R004 | Change Management            | Inadequate approval and documentation of production changes may result in unauthorized or poorly controlled changes affecting system availability or integrity.                     |          3 |      4 |    12 | Major    | Mitigate  | Open        |
| IT-R005 | Backup & Recovery            | Failure to periodically test restoration of critical backups may result in prolonged service disruption or data loss when recovery is required.                                     |          2 |      5 |    10 | Major    | Mitigate  | Open        |

---

## 3. Detailed Risk Records

### IT-R001 — Generic Administrative Accounts

**Category:** Access Management

**Risk Statement:**

The use of generic administrative accounts may prevent individual attribution of system changes, increasing the risk of unauthorized or inappropriate changes remaining undetected.

**Likelihood:** 4 – Likely

**Impact:** 4 – Major

**Risk Score:** 16

**Rating:** Major

**Treatment:** Mitigate

**Existing/Expected Controls:**

* Named user accounts
* Privileged Access Management (PAM)
* Enhanced activity logging
* Dual custody for sensitive activities
* Periodic privileged activity reviews

**Remediation Action:**

Identify generic administrative accounts, establish whether each has a legitimate business requirement, and migrate administrative activities to uniquely assigned named accounts where possible.

**Status:** Open

---

### IT-R002 — Former Employee Accounts

**Category:** Identity & Access Management

**Risk Statement:**

Failure to promptly disable accounts belonging to former employees may result in unauthorized access to organizational systems and information.

**Likelihood:** 3 – Possible

**Impact:** 5 – Critical

**Risk Score:** 15

**Rating:** Major

**Treatment:** Mitigate

**Existing/Expected Controls:**

* Joiner-Mover-Leaver process
* HR-to-IT notification process
* Periodic account reconciliation
* Access reviews
* Account deprovisioning procedures

**Remediation Action:**

Perform periodic reconciliation between employee separation records and active system accounts and disable accounts that are no longer required.

**Status:** Open

---

### IT-R003 — Critical Vulnerabilities

**Category:** Vulnerability Management

**Risk Statement:**

Delayed remediation of critical vulnerabilities may expose systems to exploitation, potentially resulting in system compromise or service disruption.

**Likelihood:** 4 – Likely

**Impact:** 5 – Critical

**Risk Score:** 20

**Rating:** Critical

**Treatment:** Mitigate

**Existing/Expected Controls:**

* Vulnerability scanning
* Patch management
* Vulnerability remediation SLA
* Risk-based prioritization
* Exception management
* Compensating controls

**Remediation Action:**

Prioritize remediation of critical vulnerabilities according to the approved remediation SLA and track outstanding vulnerabilities through the IT Risk Tracker.

**Status:** In Progress

---

### IT-R004 — Unauthorized Production Changes

**Category:** Change Management

**Risk Statement:**

Inadequate approval and documentation of production changes may result in unauthorized or poorly controlled changes affecting system availability or integrity.

**Likelihood:** 3 – Possible

**Impact:** 4 – Major

**Risk Score:** 12

**Rating:** Major

**Treatment:** Mitigate

**Existing/Expected Controls:**

* Change request documentation
* Change approval
* Testing
* Segregation of duties
* Change logs
* Post-implementation review

**Remediation Action:**

Ensure production changes are appropriately requested, tested, approved, implemented, and documented in accordance with the organization's change management process.

**Status:** Open

---

### IT-R005 — Backup Restoration Testing

**Category:** Backup & Recovery

**Risk Statement:**

Failure to periodically test restoration of critical backups may result in prolonged service disruption or data loss when recovery is required.

**Likelihood:** 2 – Unlikely

**Impact:** 5 – Critical

**Risk Score:** 10

**Rating:** Major

**Treatment:** Mitigate

**Existing/Expected Controls:**

* Scheduled backups
* Backup monitoring
* Backup retention
* Restoration testing
* Business continuity procedures

**Remediation Action:**

Perform periodic restoration tests for critical systems and document the results, identified issues, and corrective actions.

**Status:** Open

---

## 4. Risk Register Fields

The following fields should be considered when developing a complete IT Risk Register:

| Field                 | Purpose                                    |
| --------------------- | ------------------------------------------ |
| Risk ID               | Unique identifier for tracking             |
| Risk Category         | Classification of the risk                 |
| Risk Statement        | Clearly articulates the risk               |
| Risk Owner            | Person accountable for the risk            |
| Action Owner          | Person responsible for remediation         |
| Likelihood            | Probability of occurrence                  |
| Impact                | Potential consequence                      |
| Inherent Risk         | Risk before controls                       |
| Existing Controls     | Current mitigating controls                |
| Control Effectiveness | Assessment of control performance          |
| Residual Risk         | Remaining risk after controls              |
| Treatment             | Mitigate, Accept, Transfer or Avoid        |
| Remediation Action    | Action required to address the risk        |
| Target Date           | Expected remediation date                  |
| Status                | Current remediation status                 |
| Evidence              | Proof of remediation                       |
| Validation            | Confirmation that remediation is effective |
| Closure Date          | Date the risk/action was closed            |

## 5. Practical Risk Management Flow

The register should support the following process:

**Risk Identified**

↓

**Risk Documented**

↓

**Likelihood & Impact Assessed**

↓

**Inherent Risk Determined**

↓

**Controls Evaluated**

↓

**Residual Risk Determined**

↓

**Treatment Selected**

↓

**Remediation Action Assigned**

↓

**Evidence Collected**

↓

**Remediation Validated**

↓

**Risk Closed or Continuously Monitored**

## 6. Key Takeaway

A risk register should not simply be a list of problems.

It should provide a structured view of:

> **What is the risk? → How significant is it? → What controls exist? → What needs to be done? → Who is responsible? → When is it due? → Has the risk been effectively addressed?**
