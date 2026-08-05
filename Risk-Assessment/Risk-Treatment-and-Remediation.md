# Risk Treatment and Remediation

## 1. Overview

Risk treatment is the process of determining how an organization will respond to an identified risk based on its risk exposure, business objectives, risk appetite, and available controls.

Risk remediation refers to the actions taken to address a control weakness or reduce the identified risk to an acceptable level.

The overall process can be represented as:

**Identify → Assess → Treat → Remediate → Validate → Close → Monitor**

---

## 2. Risk Treatment Options

There are four commonly used risk treatment approaches:

### 2.1 Mitigate

Reduce the likelihood and/or impact of the risk by implementing or strengthening controls.

**Example:**

A generic administrative account is being used for system changes.

**Treatment:** Mitigate

**Actions:**

* Enforce named user accounts.
* Implement privileged access management.
* Enable enhanced activity logging.
* Introduce dual custody where appropriate.
* Review privileged activities periodically.

---

### 2.2 Accept

Management formally acknowledges the risk and decides that no additional treatment is required because the risk is within the organization's accepted tolerance.

Risk acceptance should be:

* Deliberate
* Documented
* Approved by the appropriate authority
* Subject to defined review periods

Risk acceptance should not simply mean that a risk has been ignored.

---

### 2.3 Transfer

Transfer some or all of the financial or operational consequences of a risk to another party.

Examples may include:

* Cyber insurance
* Outsourcing
* Contractual risk allocation
* Third-party service arrangements

Risk transfer does not necessarily eliminate the underlying risk.

---

### 2.4 Avoid

Avoid the activity, system, process, or technology creating the risk.

**Example:**

An organization may decide to discontinue a high-risk technology service that is no longer essential to business operations.

Avoidance may involve:

* Discontinuing a service
* Removing a vulnerable technology
* Ending a high-risk process
* Choosing an alternative solution

---

## 3. Treatment Decision Factors

When selecting a treatment option, consider:

* Current risk rating
* Risk appetite
* Business criticality
* Cost of treatment
* Control effectiveness
* Regulatory requirements
* Operational impact
* Available technology
* Risk exposure
* Time required for remediation

---

## 4. Risk Remediation

Once mitigation is selected, specific actions should be defined to address the underlying control weakness.

A remediation action should clearly state:

**What needs to be done + who is responsible + when it should be completed + what evidence will demonstrate completion.**

### Weak Action

> Improve access controls.

This is too vague to effectively track.

### Strong Action

> Disable inactive user accounts identified during the access review and implement a periodic reconciliation between HR records and active system accounts.

The second action is specific and can be verified.

---

## 5. Remediation Plan Components

A risk remediation plan should ideally include:

| Component          | Purpose                                          |
| ------------------ | ------------------------------------------------ |
| Risk ID            | Unique identifier for the risk                   |
| Risk Statement     | Clearly defines the risk                         |
| Root Cause         | Explains why the weakness exists                 |
| Remediation Action | Defines what needs to be done                    |
| Risk Owner         | Person accountable for managing the risk         |
| Action Owner       | Person responsible for completing the action     |
| Target Date        | Expected completion date                         |
| Status             | Tracks remediation progress                      |
| Evidence           | Demonstrates completion                          |
| Validation         | Confirms whether the remediation is effective    |
| Closure Date       | Records when the risk/action was formally closed |

---

## 6. Example Remediation Plan

### Risk

Generic administrative accounts are being used to perform system changes without sufficient individual attribution.

### Root Cause

Administrative activities are not consistently performed using uniquely assigned named accounts.

### Treatment

**Mitigate**

### Remediation Actions

1. Identify all generic administrative accounts.
2. Determine whether each account has a legitimate business requirement.
3. Replace unnecessary generic accounts with named privileged accounts.
4. Implement privileged access management for accounts that require elevated access.
5. Enable enhanced logging for privileged activities.
6. Implement dual custody for sensitive administrative activities where appropriate.
7. Review privileged account activity periodically.

### Evidence

Potential evidence may include:

* List of generic accounts
* Approved privileged access records
* PAM configuration
* System activity logs
* Access review reports
* Change records
* Screenshots or configuration reports

### Validation

The control owner or risk function should verify that:

* Generic accounts have been removed or appropriately controlled.
* Named accounts are being used.
* Privileged activities are attributable to individual users.
* Required logging is enabled.
* Evidence supports the remediation performed.

---

## 7. Remediation Status

A consistent status methodology can be used to track remediation progress.

| Status                 | Meaning                                                             |
| ---------------------- | ------------------------------------------------------------------- |
| **Open**               | Risk/action has been identified and requires remediation            |
| **In Progress**        | Remediation activities have started                                 |
| **Pending Validation** | Remediation has reportedly been completed and requires verification |
| **Closed**             | Remediation has been validated and formally closed                  |
| **Overdue**            | Target completion date has passed without satisfactory closure      |
| **Accepted**           | Risk has been formally accepted by the appropriate authority        |

---

## 8. Closure Should Be Evidence-Based

A remediation action should not automatically be considered closed simply because the responsible team states that the action has been completed.

Closure should be supported by appropriate evidence.

### Example

**Action:**

> Disable all inactive privileged accounts.

**Evidence:**

* Updated privileged account listing
* System screenshots or configuration report
* Access review results
* Relevant system logs

**Validation:**

Confirm that the identified accounts are no longer active and that the control weakness has been adequately addressed.

---

## 9. Key Takeaway

Effective risk treatment goes beyond identifying a recommendation.

A complete risk management process should establish:

> **What is the risk? → What treatment has been selected? → What action will address it? → Who owns it? → When is it due? → What evidence proves completion? → Has remediation been validated?**

The ultimate objective is to reduce the organization's exposure to an acceptable level and ensure that remediation is sustainable.
