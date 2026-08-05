# Risk Identification

## 1. Overview

Risk identification is the process of recognizing and documenting events, conditions, control weaknesses, or vulnerabilities that could negatively affect an organization's technology environment or business objectives.

Effective risk identification should move beyond simply documenting an observation. The identified issue should be analyzed to determine the underlying control weakness, potential risk, and possible business impact.

## 2. Risk Identification Approach

A practical approach is:

**Observation → Control Weakness → Risk → Impact**

### Observation

What was identified during an assessment, review, monitoring activity, audit, or control test?

### Control Weakness

What control is missing, inadequate, inconsistently implemented, or not operating effectively?

### Risk

What could happen because of the control weakness?

### Impact

What could be the consequence to the organization if the risk materializes?

## 3. Example

### Observation

A generic administrative account was used to perform a system change.

### Control Weakness

The activity was not performed using a uniquely assigned named user account, limiting individual accountability.

### Risk

The use of generic administrative accounts may prevent individual attribution of system changes, increasing the risk of unauthorized or inappropriate changes being performed without accountability.

### Potential Impact

* Unauthorized system changes
* Reduced accountability
* Difficulty during investigations
* Audit findings
* Increased operational and security risk

### Recommended Control

All system changes should be performed using uniquely assigned named user accounts. Where generic or shared administrative accounts are necessary, appropriate compensating controls such as privileged access management, dual custody, enhanced logging, and periodic activity reviews should be implemented.

## 4. Common Sources of IT Risks

IT risks can be identified through:

* Risk and Control Self-Assessments (RCSA)
* Internal audits
* External audits
* Vulnerability assessments
* Penetration testing
* Access reviews
* Security monitoring
* Incident investigations
* Compliance assessments
* Change management reviews
* IT asset reviews
* Business continuity testing
* Third-party assessments
* Control testing
* Management observations

## 5. Risk Statement Structure

A useful risk statement can follow this structure:

> **Because of [cause/control weakness], there is a risk that [risk event], which could result in [impact].**

### Example

> Because privileged activities are performed using shared administrative accounts, there is a risk that system changes cannot be attributed to individual users, which could result in unauthorized changes remaining undetected.

## 6. Risk Identification Checklist

When identifying an IT risk, consider:

* [ ] What was observed?
* [ ] What control should exist?
* [ ] Is the control missing, poorly designed, or ineffective?
* [ ] What could happen if the weakness is exploited or remains unresolved?
* [ ] What business objective could be affected?
* [ ] What is the potential impact?
* [ ] Who or what is exposed?
* [ ] Is there existing mitigation?
* [ ] Is the issue already recorded elsewhere?
* [ ] Is the issue significant enough to enter the IT Risk Register or Tracker?

## 7. Key Takeaway

A strong IT Risk professional should be able to move from an observation to a clearly articulated risk.

The goal is not simply to say:

> "A control is missing."

The goal is to explain:

> **What is wrong → why it matters → what could happen → how it should be addressed.**
