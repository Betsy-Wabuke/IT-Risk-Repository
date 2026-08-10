# Security Monitoring & Logging RCSA

## 1. Overview

This RCSA assesses risks and controls associated with collecting, monitoring, protecting, retaining, reviewing, and investigating security and system logs.

Effective security monitoring enables an organization to identify suspicious activity, detect potential security incidents, maintain accountability, support investigations, and provide evidence for audit and risk management activities.



---

# 2. RCSA Assessment

| ID     | Sub-Process                    | Risk                                                                                                        | Existing Control                                 | Control Type | Likelihood | Impact | Inherent Risk | Control Effectiveness | Residual Risk | Treatment |
| ------ | ------------------------------ | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------ | ------------ | ---------: | -----: | ------------: | --------------------- | ------------- | --------- |
| SM-001 | Log Collection                 | Critical security and system events may not be captured, resulting in monitoring and investigation gaps.    | Centralized log collection and logging standards | Detective    |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| SM-002 | SIEM Monitoring                | Security events may not be detected promptly due to inadequate monitoring or alert configuration.           | SIEM monitoring and alert rules                  | Detective    |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| SM-003 | Alert Management               | Security alerts may not be investigated or escalated within defined timelines.                              | Alert triage and escalation procedures           | Detective    |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| SM-004 | Log Retention                  | Security logs may not be retained for the required period, limiting investigations and auditability.        | Log retention policy                             | Preventive   |          2 |      4 |  8 – Moderate | Effective             | Moderate      | Mitigate  |
| SM-005 | Log Integrity                  | Logs may be modified, deleted, or manipulated, compromising their reliability as evidence.                  | Restricted access and centralized log storage    | Preventive   |          2 |      5 |    10 – Major | Partially Effective   | Major         | Mitigate  |
| SM-006 | Privileged Activity Monitoring | Unauthorized or inappropriate privileged activities may not be detected promptly.                           | Privileged activity logging and monitoring       | Detective    |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| SM-007 | Monitoring Coverage            | Security monitoring may not cover all critical systems, applications, endpoints, or network infrastructure. | Monitoring coverage review                       | Detective    |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| SM-008 | Log Review                     | Important security events may not be identified due to inadequate or inconsistent log review.               | Periodic log review and monitoring procedures    | Detective    |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |

---

# 3. Detailed RCSA Assessments

## SM-001 — Log Collection

### Sub-Process

Security and System Log Collection

### Risk

Critical security and system events may not be captured, resulting in monitoring and investigation gaps.

### Existing Controls

* Centralized log collection
* Logging standards
* System logging configuration
* Log source inventory

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Logs may not be collected where systems are incorrectly configured, log sources are not onboarded, or logging is disabled.

### Impact

**5 – Critical**

Missing logs can prevent detection of suspicious activity and limit incident investigation.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Centralized logging exists, but not all relevant systems may consistently send logs to the monitoring platform.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Maintain an approved log-source inventory and periodically reconcile it against critical IT assets to identify systems that are not forwarding required logs.

---

# SM-002 — SIEM Monitoring

### Sub-Process

Security Information and Event Monitoring

### Risk

Security events may not be detected promptly due to inadequate monitoring or alert configuration.

### Existing Control

SIEM platform configured to collect, correlate, and generate alerts from relevant security events.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Monitoring gaps may occur where rules are incomplete, improperly configured, or not regularly reviewed.

### Impact

**5 – Critical**

Failure to detect suspicious activity promptly may increase the likelihood and impact of security incidents.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

SIEM monitoring exists, but detection effectiveness depends on log coverage, correlation rules, alert tuning, and analyst review.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Periodically review SIEM coverage and detection rules and validate that critical security events generate appropriate alerts.

---

# SM-003 — Alert Management

### Sub-Process

Security Alert Triage and Escalation

### Risk

Security alerts may not be investigated or escalated within defined timelines.

### Existing Controls

* Alert triage procedures
* Security analyst review
* Incident escalation procedures
* Alert severity classification

### Control Type

**Detective**

### Likelihood

**3 – Possible**

High alert volumes, unclear priorities, or insufficient staffing may result in delayed alert investigation.

### Impact

**5 – Critical**

Delayed investigation of significant alerts may allow malicious activity to continue undetected.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Alert management procedures exist, but response times may not consistently meet defined expectations.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Establish alert severity levels, response SLAs, escalation criteria, and monitoring of unresolved alerts.

---

# SM-004 — Log Retention

### Sub-Process

Log Retention and Archiving

### Risk

Security logs may not be retained for the required period, limiting investigations and auditability.

### Existing Control

Documented log retention requirements and centralized log storage.

### Control Type

**Preventive**

### Likelihood

**2 – Unlikely**

Defined retention requirements reduce the likelihood of logs being deleted prematurely.

### Impact

**4 – Major**

Insufficient retention may prevent investigation of incidents discovered after a significant period.

### Inherent Risk

**2 × 4 = 8 – Moderate**

### Control Effectiveness

**Effective**

Retention requirements are documented and generally applied to critical log sources.

### Residual Risk

**Moderate**

### Treatment

**Mitigate**

### Recommended Action

Periodically review retention configurations and ensure they align with organizational policy, regulatory requirements, and investigative needs.

---

# SM-005 — Log Integrity

### Sub-Process

Log Protection and Integrity

### Risk

Logs may be modified, deleted, or manipulated, compromising their reliability as evidence.

### Existing Controls

* Restricted log access
* Centralized log storage
* Privileged access controls
* Audit trails

### Control Type

**Preventive**

### Likelihood

**2 – Unlikely**

Access restrictions reduce the likelihood of unauthorized log modification.

### Impact

**5 – Critical**

Manipulated logs may conceal unauthorized activity and compromise incident investigations.

### Inherent Risk

**2 × 5 = 10 – Major**

### Control Effectiveness

**Partially Effective**

Access controls exist, but effectiveness depends on proper privileged access management and monitoring of administrative activity.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Restrict administrative access to logging platforms, monitor privileged activities, and implement appropriate mechanisms to protect logs from unauthorized modification or deletion.

---

# SM-006 — Privileged Activity Monitoring

### Sub-Process

Privileged User Activity Monitoring

### Risk

Unauthorized or inappropriate privileged activities may not be detected promptly.

### Existing Controls

* Privileged account logging
* PAM
* SIEM monitoring
* Administrative activity monitoring

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Privileged activity may not be adequately monitored where administrative accounts are excluded from logging or monitoring rules are incomplete.

### Impact

**5 – Critical**

Misuse of privileged access can significantly affect critical systems and sensitive information.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Privileged activity logging exists, but gaps may remain where generic accounts or unmanaged administrative activities are used.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Require privileged activities to be attributable to named users wherever possible and configure monitoring for high-risk administrative activities.

---

# SM-007 — Monitoring Coverage

### Sub-Process

Security Monitoring Coverage

### Risk

Security monitoring may not cover all critical systems, applications, endpoints, or network infrastructure.

### Existing Control

Monitoring coverage reviews and log-source inventories.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

New systems, applications, or infrastructure may be deployed without being incorporated into monitoring.

### Impact

**5 – Critical**

Unmonitored systems can provide blind spots that attackers may exploit.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Monitoring exists, but coverage may not always align with the complete IT asset inventory.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Reconcile the security monitoring inventory against the organization's IT asset register and investigate systems that are not appropriately monitored.

---

# SM-008 — Log Review

### Sub-Process

Security Log Review

### Risk

Important security events may not be identified due to inadequate or inconsistent log review.

### Existing Control

Periodic review of security logs and monitoring alerts.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

High volumes of logs may make manual review difficult, while poorly configured alerts may result in important events being overlooked.

### Impact

**4 – Major**

Failure to identify suspicious activity may result in delayed incident response.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Log review procedures exist, but effectiveness depends on monitoring coverage, alert quality, and analyst capacity.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Prioritize automated detection and correlation of high-risk events while maintaining documented review procedures for critical logs and alerts.

---

# 4. Security Monitoring Lifecycle

A mature monitoring process should follow:

**Identify Critical Systems**

↓

**Identify Required Log Sources**

↓

**Configure Logging**

↓

**Centralize Logs**

↓

**Correlate Events**

↓

**Generate Alerts**

↓

**Triage Alerts**

↓

**Investigate Suspicious Activity**

↓

**Escalate Incidents**

↓

**Record Evidence**

↓

**Remediate**

↓

**Review & Improve Detection Rules**

---

# 5. Critical Events to Monitor

Examples of events that may require monitoring include:

### Authentication

* Multiple failed login attempts
* Successful login after repeated failures
* Login from unusual locations
* Disabled account activity
* New account creation

### Privileged Access

* Administrator login
* Privilege escalation
* Creation of privileged accounts
* Changes to administrator permissions
* Administrative configuration changes

### System Changes

* Security configuration changes
* Firewall rule changes
* Endpoint security changes
* Critical system modifications

### Network Activity

* Unusual outbound connections
* Suspicious network traffic
* Connections to known malicious infrastructure
* Unexpected remote access

### Data Activity

* Unusual data transfers
* Mass file access
* Large data exports
* Unauthorized access attempts

---

# 6. Security Monitoring Evidence

Examples of evidence that may be requested during control testing include:

### Log Collection

* Log source inventory
* SIEM ingestion reports
* System logging configurations
* Log forwarding status

### Monitoring

* SIEM dashboards
* Detection rules
* Correlation rules
* Alert configurations

### Alert Management

* Alert queues
* Alert investigation tickets
* Escalation records
* SLA reports

### Log Retention

* Retention configuration
* Archived logs
* Retention policy

### Privileged Monitoring

* Administrator activity logs
* PAM reports
* Privileged access alerts

### Coverage

* Asset inventory
* SIEM onboarding list
* Monitoring coverage reports
* Unmonitored asset reports

---

# 7. Security Monitoring Control Checklist

* [ ] Are critical systems identified?
* [ ] Are critical systems forwarding logs?
* [ ] Is there an approved log-source inventory?
* [ ] Are logs centralized where appropriate?
* [ ] Are critical security events monitored?
* [ ] Are SIEM detection rules configured?
* [ ] Are alerts assigned severity levels?
* [ ] Are alerts investigated within defined timelines?
* [ ] Are critical alerts escalated?
* [ ] Are logs protected from unauthorized modification?
* [ ] Are privileged activities monitored?
* [ ] Are logs retained according to policy?
* [ ] Is monitoring coverage reconciled against the asset inventory?
* [ ] Are detection rules periodically reviewed and improved?

---

# 8. Important IT Risk Connection

Security monitoring should not operate as an isolated activity.

The flow should be:

**Asset Inventory**

↓

**Monitoring Coverage**

↓

**Log Collection**

↓

**SIEM Detection**

↓

**Security Alert**

↓

**Incident Investigation**

↓

**Risk Identification**

↓

**IT Risk Tracker**

↓

**Remediation**

↓

**Risk Closure**

This is an important connection between **IT Security Operations and IT Risk Management**.

---

# 9. RCSA Conclusion

Effective security monitoring provides visibility into activity occurring across the organization's technology environment.

The RCSA should assess whether the organization can demonstrate:

* Appropriate log coverage
* Effective monitoring
* Timely alert investigation
* Appropriate escalation
* Adequate log retention
* Protection of log integrity
* Privileged activity monitoring
* Complete monitoring coverage
* Evidence-based incident investigation

The objective is not simply to have a SIEM or logging platform, but to demonstrate that the organization can **detect, investigate, respond to, and learn from significant security events**.
