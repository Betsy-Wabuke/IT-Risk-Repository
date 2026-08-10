# IT Third-Party / Vendor Risk RCSA

## 1. Overview

This RCSA assesses risks associated with third parties, vendors, contractors, consultants, technology providers, and other external service providers that have access to organizational systems, information, infrastructure, or services.

Third-party risk management ensures that external parties meet the organization's security, operational, regulatory, contractual, and service requirements throughout the vendor lifecycle.

> **Note:** This is a fictional assessment created for educational and professional portfolio purposes.

---

# 2. RCSA Assessment

| ID     | Sub-Process                       | Risk                                                                                                                 | Existing Control                                    | Control Type         | Likelihood | Impact | Inherent Risk | Control Effectiveness | Residual Risk | Treatment |
| ------ | --------------------------------- | -------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- | -------------------- | ---------: | -----: | ------------: | --------------------- | ------------: | --------- |
| TP-001 | Vendor Due Diligence              | Vendors may be onboarded without adequate assessment of their security, financial, operational, or compliance risks. | Vendor due diligence and risk assessment            | Preventive           |          3 |      5 |    15 – Major | Partially Effective   |         Major | Mitigate  |
| TP-002 | Vendor Security Assessment        | Vendors may not maintain adequate security controls, exposing organizational systems or data to compromise.          | Vendor security questionnaires and assessments      | Preventive           |          3 |      5 |    15 – Major | Partially Effective   |         Major | Mitigate  |
| TP-003 | Contractual Security Requirements | Vendor contracts may not clearly define security, confidentiality, incident reporting, and compliance obligations.   | Contractual security clauses                        | Preventive           |          3 |      5 |    15 – Major | Partially Effective   |         Major | Mitigate  |
| TP-004 | Vendor Access Management          | Vendor personnel may receive excessive or inappropriate access to organizational systems.                            | Third-party access controls and access reviews      | Preventive/Detective |          3 |      5 |    15 – Major | Partially Effective   |         Major | Mitigate  |
| TP-005 | Vendor Monitoring                 | Vendor compliance and performance may not be adequately monitored after onboarding.                                  | Periodic vendor reviews and performance monitoring  | Detective            |          3 |      4 |    12 – Major | Partially Effective   |         Major | Mitigate  |
| TP-006 | Vendor Incident Management        | Vendor-related security incidents may not be reported or escalated promptly.                                         | Vendor incident notification requirements           | Detective            |          3 |      5 |    15 – Major | Partially Effective   |         Major | Mitigate  |
| TP-007 | SLA Management                    | Vendors may fail to meet agreed service levels, resulting in service disruption or operational impact.               | Service Level Agreements and performance monitoring | Preventive/Detective |          3 |      4 |    12 – Major | Partially Effective   |         Major | Mitigate  |
| TP-008 | Vendor Offboarding                | Vendor access may remain active after the contractual relationship ends.                                             | Vendor termination and access revocation procedures | Preventive           |          2 |      5 |    10 – Major | Partially Effective   |         Major | Mitigate  |

---

# 3. Detailed RCSA Assessments

## TP-001 — Vendor Due Diligence

### Sub-Process

Third-Party Due Diligence

### Risk

Vendors may be onboarded without adequate assessment of their security, financial, operational, or compliance risks.

### Existing Controls

* Vendor due diligence questionnaires
* Vendor risk assessments
* Procurement review
* Compliance review
* Security assessment

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Vendors may be onboarded without sufficient assessment where due diligence requirements are unclear or inconsistently applied.

### Impact

**5 – Critical**

A high-risk vendor may introduce significant security, operational, financial, or regulatory exposure.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Due diligence procedures exist, but assessments may not always be performed consistently or at the appropriate depth.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Establish a risk-based vendor due diligence process that considers the nature of the service, data accessed, system criticality, and level of vendor access.

---

# TP-002 — Vendor Security Assessment

### Sub-Process

Third-Party Security Assessment

### Risk

Vendors may not maintain adequate security controls, exposing organizational systems or data to compromise.

### Existing Controls

* Security questionnaires
* Security certifications
* Penetration testing reports where applicable
* Security assessment
* Compliance evidence

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Vendor security weaknesses may not be identified before onboarding or during the relationship.

### Impact

**5 – Critical**

A compromised vendor may expose organizational systems, sensitive information, or services.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Security assessments exist, but their depth and frequency may vary according to vendor criticality.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Apply risk-based security assessments to vendors handling sensitive information or providing critical technology services.

---

# TP-003 — Contractual Security Requirements

### Sub-Process

Contractual Security and Compliance Requirements

### Risk

Vendor contracts may not clearly define security, confidentiality, incident reporting, and compliance obligations.

### Existing Controls

* Security clauses
* Confidentiality agreements
* Data protection requirements
* Incident notification requirements
* Audit rights

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Security requirements may be omitted or insufficiently detailed in contracts.

### Impact

**5 – Critical**

Unclear contractual requirements may make it difficult to enforce security obligations or hold vendors accountable.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Security clauses exist, but requirements may not be standardized across all vendor contracts.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Develop standard minimum security clauses for vendor contracts and require appropriate legal, procurement, IT, and security review.

---

# TP-004 — Vendor Access Management

### Sub-Process

Third-Party System Access

### Risk

Vendor personnel may receive excessive or inappropriate access to organizational systems.

### Existing Controls

* Least privilege
* Named accounts
* MFA
* Privileged access management
* Periodic access reviews
* Time-bound access

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

Vendor access may remain broader or active for longer than required.

### Impact

**5 – Critical**

Compromised or misused vendor credentials could provide unauthorized access to critical systems.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Access controls exist, but periodic review and timely revocation may not always be consistently performed.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Require vendor access to be approved, role-based, time-bound where possible, monitored, and periodically reviewed.

---

# TP-005 — Vendor Monitoring

### Sub-Process

Ongoing Vendor Monitoring

### Risk

Vendor compliance and performance may not be adequately monitored after onboarding.

### Existing Controls

* Periodic vendor reviews
* SLA monitoring
* Security assessments
* Performance reports
* Compliance reviews

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Vendor risk profiles may change after onboarding due to changes in systems, ownership, security posture, or services.

### Impact

**4 – Major**

Failure to identify changes in vendor risk may result in prolonged exposure.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Vendor monitoring exists, but frequency and scope may vary.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Establish periodic risk-based vendor reviews and track identified weaknesses through formal remediation processes.

---

# TP-006 — Vendor Incident Management

### Sub-Process

Third-Party Incident Reporting

### Risk

Vendor-related security incidents may not be reported or escalated promptly.

### Existing Control

Vendor contractual requirements for incident notification and escalation.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Vendors may not immediately notify the organization of incidents affecting shared systems or data.

### Impact

**5 – Critical**

Delayed notification may prevent the organization from responding promptly to a security incident.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Incident notification requirements exist, but compliance may not be consistently tested.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Define vendor incident notification timelines and periodically test vendor escalation and communication procedures.

---

# TP-007 — SLA Management

### Sub-Process

Vendor Service Level Management

### Risk

Vendors may fail to meet agreed service levels, resulting in service disruption or operational impact.

### Existing Controls

* Service Level Agreements
* Key Performance Indicators
* SLA monitoring
* Vendor performance reviews
* Escalation procedures

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

Service performance may deteriorate due to resource constraints, technical failures, or inadequate vendor management.

### Impact

**4 – Major**

SLA failures may disrupt critical IT services and business operations.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

SLAs exist, but performance monitoring and escalation may not always be consistently performed.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Monitor vendor performance against defined SLAs and document recurring breaches, escalation actions, and corrective measures.

---

# TP-008 — Vendor Offboarding

### Sub-Process

Vendor Termination and Offboarding

### Risk

Vendor access may remain active after the contractual relationship ends.

### Existing Controls

* Vendor termination procedures
* Access revocation
* Credential disabling
* Asset return
* Data return or destruction

### Control Type

**Preventive**

### Likelihood

**2 – Unlikely**

Formal offboarding procedures reduce the likelihood of residual vendor access.

### Impact

**5 – Critical**

Active vendor accounts after termination may provide unauthorized access to organizational resources.

### Inherent Risk

**2 × 5 = 10 – Major**

### Control Effectiveness

**Partially Effective**

Offboarding procedures exist, but coordination between procurement, business owners, and IT may result in delays.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Integrate vendor termination with IT access revocation processes and require confirmation that accounts, credentials, assets, and data access have been terminated.

---

# 4. Third-Party Risk Lifecycle

A mature vendor risk process should follow:

**Vendor Identification**

↓

**Risk Classification**

↓

**Due Diligence**

↓

**Security Assessment**

↓

**Contract Review**

↓

**Approval**

↓

**Onboarding**

↓

**Access Provisioning**

↓

**Ongoing Monitoring**

↓

**Performance Review**

↓

**Incident Management**

↓

**Periodic Risk Reassessment**

↓

**Offboarding**

↓

**Access Revocation**

↓

**Data / Asset Return**

---

# 5. Vendor Risk Classification

Vendors can be categorized according to their potential impact.

| Risk Level   | Example                                                      |
| ------------ | ------------------------------------------------------------ |
| **Critical** | Vendor hosts or manages a critical banking/enterprise system |
| **High**     | Vendor has access to sensitive data or privileged systems    |
| **Medium**   | Vendor provides important but non-critical IT services       |
| **Low**      | Vendor has limited access and minimal business impact        |

The level of due diligence and monitoring should increase with vendor risk.

---

# 6. Third-Party Risk Evidence

Examples of evidence that may be requested during control testing include:

### Due Diligence

* Vendor questionnaires
* Risk assessments
* Security assessment reports
* Vendor approval records

### Security

* Security certifications
* Penetration testing reports
* Vulnerability reports
* Security policies

### Contracts

* Vendor contracts
* Security clauses
* NDAs
* Data protection clauses
* Incident notification requirements

### Access

* Vendor user accounts
* Access approvals
* Access review reports
* PAM records
* MFA configuration

### Monitoring

* Vendor performance reports
* SLA reports
* Risk reassessments
* Review meeting minutes

### Incidents

* Vendor incident notifications
* Incident reports
* Root cause analysis
* Corrective action plans

### Offboarding

* Account revocation evidence
* Asset return records
* Data destruction certificates
* Vendor termination documentation

---

# 7. Third-Party Risk Control Checklist

* [ ] Is vendor due diligence performed before onboarding?
* [ ] Are vendors risk-rated?
* [ ] Are critical vendors subject to enhanced due diligence?
* [ ] Are vendor security controls assessed?
* [ ] Are security requirements included in contracts?
* [ ] Are incident notification requirements defined?
* [ ] Is vendor access approved?
* [ ] Is vendor access based on least privilege?
* [ ] Are vendor accounts named and attributable?
* [ ] Is MFA implemented where appropriate?
* [ ] Are vendor accounts periodically reviewed?
* [ ] Are vendor SLAs monitored?
* [ ] Are vendor security risks periodically reassessed?
* [ ] Are vendor incidents tracked?
* [ ] Is vendor access revoked upon termination?
* [ ] Are organizational assets returned?
* [ ] Is organizational data returned or securely destroyed?

---

# 8. Key RCSA Observations

### 1. Vendor risk begins before onboarding

Risk assessment should happen before granting a third party access to organizational resources.

### 2. Vendor access is organizational access

A vendor account accessing an internal system should be subject to appropriate access management controls just like an internal account.

### 3. Contracts are an important control

Security expectations should be documented and enforceable rather than relying only on informal agreements.

### 4. Vendor risk changes over time

A vendor that was low risk at onboarding may become high risk after changes to systems, services, data, ownership, or access.

### 5. Offboarding is equally important

Terminating a contract does not automatically terminate technical access.

The organization should verify:

**Contract Termination → Account Revocation → Credential Revocation → Asset Return → Data Return/Destruction**

---

# 9. Third-Party Risk and IT Risk Tracker

Vendor risks identified through due diligence or ongoing monitoring should be connected to the organization's IT Risk Management process.

Example:

**Vendor Assessment**

↓

**Risk Identified**

↓

**Risk Recorded in IT Risk Tracker**

↓

**Risk Owner Assigned**

↓

**Action Plan Defined**

↓

**Target Date**

↓

**Evidence Submitted**

↓

**Validation**

↓

**Risk Closure**

This ensures vendor risk does not remain only within procurement or vendor management documentation.

---

# 10. RCSA Conclusion

Effective third-party risk management ensures that external organizations do not introduce unmanaged security, operational, compliance, or service risks.

The RCSA should therefore assess whether the organization can demonstrate:

* Risk-based vendor due diligence
* Security assessment
* Contractual security requirements
* Controlled third-party access
* Continuous vendor monitoring
* SLA management
* Vendor incident reporting
* Periodic risk reassessment
* Secure vendor offboarding

The objective is to ensure that third-party risk is managed **before, during, and after the vendor relationship**.
