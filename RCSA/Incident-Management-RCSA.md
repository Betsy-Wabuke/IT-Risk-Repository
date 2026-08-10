# Incident Management RCSA

## 1. Overview

This RCSA assesses risks and controls associated with identifying, recording, classifying, escalating, investigating, responding to, and closing IT and information security incidents.

An effective incident management process enables an organization to respond to incidents promptly, minimize operational impact, preserve evidence, identify root causes, and implement corrective actions.


---

# 2. RCSA Assessment

| ID     | Sub-Process             | Risk                                                                                                                     | Existing Control                                                | Control Type         | Likelihood | Impact | Inherent Risk | Control Effectiveness | Residual Risk | Treatment |
| ------ | ----------------------- | ------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------- | -------------------- | ---------: | -----: | ------------: | --------------------- | ------------- | --------- |
| IM-001 | Incident Detection      | Security or IT incidents may not be detected promptly, resulting in prolonged exposure or operational disruption.        | Monitoring tools, alerts, and user reporting mechanisms         | Detective            |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| IM-002 | Incident Logging        | Incidents may not be recorded accurately or promptly, resulting in incomplete incident visibility and poor tracking.     | ITSM/helpdesk incident logging process                          | Preventive/Detective |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| IM-003 | Incident Classification | Incidents may be incorrectly classified, resulting in inappropriate prioritization and delayed response.                 | Incident classification and severity matrix                     | Preventive           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| IM-004 | Incident Escalation     | Critical incidents may not be escalated promptly to the appropriate teams or management.                                 | Incident escalation procedures and SLAs                         | Preventive           |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| IM-005 | Incident Response       | Inadequate response procedures may result in prolonged system compromise or service disruption.                          | Incident response procedures and response teams                 | Corrective           |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| IM-006 | Incident Investigation  | Insufficient investigation may result in failure to identify the cause, scope, or affected systems.                      | Log analysis, investigation procedures, and evidence collection | Detective            |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| IM-007 | Evidence Preservation   | Failure to preserve incident evidence may compromise investigations and prevent accurate determination of what occurred. | Evidence preservation and logging procedures                    | Preventive           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| IM-008 | Root Cause Analysis     | Root causes may not be identified, resulting in recurring incidents and unresolved control weaknesses.                   | Root cause analysis and post-incident review                    | Corrective           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| IM-009 | Incident Closure        | Incidents may be closed without adequate resolution evidence, resulting in unresolved issues remaining undetected.       | Incident closure checklist and approval                         | Detective            |          2 |      4 |  8 – Moderate | Partially Effective   | Moderate      | Mitigate  |
| IM-010 | Incident Reporting      | Management may lack timely visibility of significant incidents and incident trends.                                      | Incident dashboards and management reporting                    | Detective            |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |

---

# 3. Detailed RCSA Assessments

## IM-001 — Incident Detection

### Sub-Process

Incident Detection and Monitoring

### Risk

Security or IT incidents may not be detected promptly, resulting in prolonged exposure or operational disruption.

### Existing Controls

* Security monitoring tools
* Endpoint monitoring
* Network monitoring
* System alerts
* User reporting mechanisms
* SIEM monitoring where applicable

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Incidents may remain undetected where monitoring coverage is incomplete, alerts are misconfigured, or monitoring gaps exist.

### Impact

**5 – Critical**

Delayed detection may increase the duration and potential impact of an incident.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Monitoring controls exist, but effectiveness may be reduced where monitoring coverage is incomplete or alerts are not consistently reviewed and investigated.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Periodically review monitoring coverage and alert configurations and ensure significant alerts are investigated within defined response timelines.

---

# IM-002 — Incident Logging

### Sub-Process

Incident Recording

### Risk

Incidents may not be recorded accurately or promptly, resulting in incomplete incident visibility and poor tracking.

### Existing Control

ITSM/helpdesk system used to record incidents and track resolution.

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

Incidents may be handled outside the formal ticketing process or insufficient information may be recorded.

### Impact

**4 – Major**

Incomplete incident records can affect investigation, reporting, trend analysis, and accountability.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

An incident management system exists, but incidents may not consistently contain complete information or supporting evidence.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Require all IT and security incidents to be logged in the approved incident management platform with minimum mandatory information and supporting evidence.

---

# IM-003 — Incident Classification

### Sub-Process

Incident Classification and Prioritization

### Risk

Incidents may be incorrectly classified, resulting in inappropriate prioritization and delayed response.

### Existing Control

Incident classification and severity matrix based on factors such as business impact, affected systems, users, and urgency.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Incorrect classification may occur due to incomplete information or inconsistent interpretation of severity criteria.

### Impact

**4 – Major**

A critical incident classified as low priority may experience delayed response and escalation.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Classification criteria exist, but consistency may vary between analysts or teams.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Standardize incident severity criteria and periodically train support and security personnel on incident classification.

---

# IM-004 — Incident Escalation

### Sub-Process

Incident Escalation

### Risk

Critical incidents may not be escalated promptly to the appropriate teams or management.

### Existing Control

Incident escalation procedures, defined escalation paths, and response SLAs.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Escalation may be delayed where ownership is unclear or severity is incorrectly assessed.

### Impact

**5 – Critical**

Delayed escalation can significantly increase the impact and duration of critical incidents.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Escalation procedures exist, but escalation may not always occur within defined timelines.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Define clear escalation thresholds, responsible teams, escalation contacts, and maximum response timelines for critical incidents.

---

# IM-005 — Incident Response

### Sub-Process

Incident Response and Containment

### Risk

Inadequate response procedures may result in prolonged system compromise or service disruption.

### Existing Controls

* Incident response procedures
* Incident response team
* Containment procedures
* System isolation procedures
* Recovery procedures

### Control Type

**Corrective**

### Likelihood

**3 – Possible**

Response activities may be delayed where procedures are outdated, roles are unclear, or teams lack sufficient resources.

### Impact

**5 – Critical**

Inadequate response may allow an incident to spread and significantly affect systems or operations.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Response procedures exist, but their effectiveness may be reduced if they are not regularly tested or updated.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Conduct periodic incident response exercises and update response procedures based on lessons learned and changes in the IT environment.

---

# IM-006 — Incident Investigation

### Sub-Process

Incident Investigation and Analysis

### Risk

Insufficient investigation may result in failure to identify the cause, scope, or affected systems.

### Existing Controls

* Log analysis
* System investigation
* Endpoint analysis
* Network analysis
* Evidence collection procedures

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Investigation quality may vary based on available evidence, tools, skills, and logging coverage.

### Impact

**5 – Critical**

Failure to establish the scope or cause of an incident can allow threats to persist or recur.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Investigation procedures exist, but evidence may be incomplete due to logging gaps or insufficient investigation resources.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Strengthen investigation procedures and ensure relevant logs, system information, and evidence are available to support incident analysis.

---

# IM-007 — Evidence Preservation

### Sub-Process

Incident Evidence Collection and Preservation

### Risk

Failure to preserve incident evidence may compromise investigations and prevent accurate determination of what occurred.

### Existing Control

Evidence collection and preservation procedures.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Evidence may be overwritten, altered, or lost where preservation procedures are not followed promptly.

### Impact

**4 – Major**

Loss of evidence can limit investigations, accountability, and root-cause analysis.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Evidence preservation procedures exist, but preservation may not be consistently performed or documented.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Define evidence preservation requirements, including log retention, access restrictions, timestamps, and documented handling procedures.

---

# IM-008 — Root Cause Analysis

### Sub-Process

Root Cause Analysis and Corrective Action

### Risk

Root causes may not be identified, resulting in recurring incidents and unresolved control weaknesses.

### Existing Control

Root cause analysis and post-incident review for significant incidents.

### Control Type

**Corrective**

### Likelihood

**3 – Possible**

Investigations may focus on restoring services without adequately determining the underlying cause.

### Impact

**4 – Major**

Failure to address root causes may result in repeated incidents and continued exposure.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Root cause analysis exists, but it may not consistently be performed for all significant incidents.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Require root cause analysis for significant and recurring incidents and track corrective actions through to completion.

---

# IM-009 — Incident Closure

### Sub-Process

Incident Resolution and Closure

### Risk

Incidents may be closed without adequate resolution evidence, resulting in unresolved issues remaining undetected.

### Existing Control

Incident closure checklist and approval process.

### Control Type

**Detective**

### Likelihood

**2 – Unlikely**

Closure controls reduce the likelihood of unresolved incidents being closed prematurely.

### Impact

**4 – Major**

Premature closure may result in unresolved technical or security issues remaining in the environment.

### Inherent Risk

**2 × 4 = 8 – Moderate**

### Control Effectiveness

**Partially Effective**

Closure procedures exist, but evidence and approval may not consistently meet defined requirements.

### Residual Risk

**Moderate**

### Treatment

**Mitigate**

### Recommended Action

Require incidents to contain documented resolution details, evidence of remediation, root-cause information where applicable, and appropriate closure approval.

---

# IM-010 — Incident Reporting

### Sub-Process

Incident Reporting and Monitoring

### Risk

Management may lack timely visibility of significant incidents and incident trends.

### Existing Control

Incident dashboards, trend reports, and management reporting.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Reporting gaps may occur where incident information is incomplete, delayed, or not consolidated.

### Impact

**4 – Major**

Limited management visibility may delay strategic action and remediation of recurring issues.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Reporting exists, but its effectiveness may be reduced by incomplete data or inconsistent reporting.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Develop standardized incident reporting covering incident volumes, severity, response times, SLA breaches, root causes, recurring incidents, and outstanding corrective actions.

---

# 4. Incident Management Lifecycle

A mature incident management process should follow:

**Detection**

↓

**Logging**

↓

**Classification**

↓

**Prioritization**

↓

**Escalation**

↓

**Investigation**

↓

**Containment**

↓

**Eradication / Remediation**

↓

**Recovery**

↓

**Root Cause Analysis**

↓

**Post-Incident Review**

↓

**Closure**

---

# 5. Incident Management Evidence

Examples of evidence that may be reviewed during control testing include:

### Detection

* Monitoring alerts
* SIEM alerts
* Endpoint detection alerts
* Network monitoring records

### Logging

* Incident tickets
* Helpdesk records
* Incident registration forms

### Classification

* Incident severity matrix
* Ticket priority
* Business impact assessment

### Escalation

* Escalation records
* Notification emails
* Incident timelines
* SLA reports

### Investigation

* Investigation reports
* System and network logs
* Endpoint analysis
* Security tool evidence

### Evidence Preservation

* Log retention configuration
* Evidence collection records
* Investigation timelines

### Root Cause Analysis

* RCA reports
* Post-incident reviews
* Corrective action plans

### Closure

* Resolution evidence
* Closure approvals
* Validation results

---

# 6. Incident Management Metrics

Useful metrics for monitoring incident management include:

| Metric                      | Purpose                              |
| --------------------------- | ------------------------------------ |
| Number of incidents         | Understand incident volume           |
| Critical incidents          | Monitor high-impact events           |
| Mean Time to Detect (MTTD)  | Measure detection speed              |
| Mean Time to Respond (MTTR) | Measure response efficiency          |
| SLA breaches                | Identify response weaknesses         |
| Recurring incidents         | Identify systemic problems           |
| Open incidents              | Monitor unresolved exposure          |
| Incidents by category       | Identify trends                      |
| Incidents by severity       | Understand risk exposure             |
| Root cause completion       | Measure quality of corrective action |

---

# 7. Key RCSA Observations

### 1. Detection is not the same as response

An organization may detect an incident but still have a weak response process.

### 2. Incident classification drives prioritization

Incorrect severity classification can cause critical incidents to receive insufficient attention.

### 3. Evidence matters

Incident records should provide enough information to reconstruct what happened, when it happened, and what actions were taken.

### 4. Resolution is not the same as root-cause remediation

Restoring a service does not necessarily eliminate the underlying cause.

### 5. Closure should be evidence-based

Incidents should not be closed simply because the affected service is operational again.

### 6. Recurring incidents indicate control weaknesses

Repeated incidents should trigger deeper investigation and corrective action.

---

# 8. RCSA Conclusion

An effective incident management process should enable the organization to:

* Detect incidents promptly
* Record incidents accurately
* Classify incidents consistently
* Escalate significant incidents appropriately
* Contain and remediate incidents
* Preserve relevant evidence
* Identify root causes
* Implement corrective actions
* Validate resolution
* Report trends to management

The RCSA should therefore evaluate not only whether incident management procedures exist, but whether they operate effectively and produce sufficient evidence to demonstrate timely and appropriate incident handling.
