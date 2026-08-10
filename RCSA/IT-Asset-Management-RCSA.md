# IT Asset Management RCSA

## 1. Overview

This RCSA assesses risks and controls associated with identifying, recording, assigning, monitoring, maintaining, and disposing of organizational IT assets.

Effective IT asset management provides visibility over hardware, software, network devices, and other technology resources throughout their lifecycle.

Asset visibility is also foundational to other IT risk processes because the organization cannot effectively protect, monitor, patch, or recover assets that it does not know exist.


---

# 2. RCSA Assessment

| ID        | Sub-Process          | Risk                                                                                                                    | Existing Control                                  | Control Type         | Likelihood | Impact | Inherent Risk | Control Effectiveness | Residual Risk | Treatment |
| --------- | -------------------- | ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------- | -------------------- | ---------: | -----: | ------------: | --------------------- | ------------- | --------- |
| AM-IT-001 | Asset Inventory      | IT assets may not be accurately recorded, resulting in limited visibility of the organization's technology environment. | Centralized IT asset inventory/CMDB               | Preventive/Detective |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| AM-IT-002 | Asset Ownership      | IT assets may not have clearly assigned owners, resulting in unclear accountability for maintenance and security.       | Asset ownership assignment                        | Preventive           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| AM-IT-003 | Asset Classification | Assets may not be appropriately classified according to business criticality or information sensitivity.                | Asset classification framework                    | Preventive           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| AM-IT-004 | Asset Reconciliation | Differences between actual assets and the asset register may remain undetected.                                         | Periodic asset reconciliation                     | Detective            |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| AM-IT-005 | Unauthorized Assets  | Unauthorized or unmanaged devices may connect to the organization's network and introduce security risks.               | Network access controls and asset discovery       | Preventive/Detective |          3 |      5 |    15 – Major | Partially Effective   | Major         | Mitigate  |
| AM-IT-006 | Asset Lifecycle      | Assets may not be appropriately tracked from acquisition through retirement.                                            | Asset lifecycle management process                | Preventive           |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| AM-IT-007 | Software Inventory   | Unauthorized or unsupported software may remain installed on organizational systems.                                    | Software inventory and software approval controls | Preventive/Detective |          3 |      4 |    12 – Major | Partially Effective   | Major         | Mitigate  |
| AM-IT-008 | Asset Disposal       | Retired assets may be disposed of without adequate data sanitization, resulting in potential information exposure.      | Secure disposal and data destruction procedures   | Preventive           |          2 |      5 |    10 – Major | Partially Effective   | Major         | Mitigate  |

---

# 3. Detailed RCSA Assessments

## AM-IT-001 — Asset Inventory

### Sub-Process

IT Asset Inventory Management

### Risk

IT assets may not be accurately recorded, resulting in limited visibility of the organization's technology environment.

### Existing Control

A centralized asset inventory or configuration management database is maintained to record organizational IT assets.

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

Assets may be omitted from the inventory due to manual processes, incomplete onboarding, acquisitions, transfers, or unauthorized deployments.

### Impact

**5 – Critical**

Lack of asset visibility may prevent the organization from effectively managing vulnerabilities, patching, access, monitoring, and incident response.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

An asset inventory exists, but records may not always accurately reflect the current IT environment.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Maintain a centralized asset inventory and periodically reconcile it against network discovery, endpoint management, procurement, and other authoritative sources.

---

# AM-IT-002 — Asset Ownership

### Sub-Process

Asset Ownership and Accountability

### Risk

IT assets may not have clearly assigned owners, resulting in unclear accountability for maintenance and security.

### Existing Control

Assets are assigned to designated users, departments, system owners, or custodians.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Ownership information may become outdated when employees transfer, leave, or change responsibilities.

### Impact

**4 – Major**

Unclear ownership may delay vulnerability remediation, incident response, access reviews, and asset maintenance.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Asset ownership is recorded, but ownership records may not always be updated when organizational changes occur.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Require each critical asset to have an identified owner and periodically reconcile ownership information with HR and organizational records.

---

# AM-IT-003 — Asset Classification

### Sub-Process

Asset Classification

### Risk

Assets may not be appropriately classified according to business criticality or information sensitivity.

### Existing Control

Asset classification based on factors such as business importance, information sensitivity, and operational criticality.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Classification may be inconsistent where criteria are unclear or asset owners do not periodically review classifications.

### Impact

**4 – Major**

Incorrect classification can result in inappropriate security, monitoring, backup, or recovery controls.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Classification controls exist, but classifications may not always be current or consistently applied.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Define standardized asset classification criteria and require periodic review by asset owners.

---

# AM-IT-004 — Asset Reconciliation

### Sub-Process

Asset Reconciliation

### Risk

Differences between actual assets and the asset register may remain undetected.

### Existing Control

Periodic reconciliation between the IT asset register and physical or technical asset discovery sources.

### Control Type

**Detective**

### Likelihood

**3 – Possible**

Differences may arise due to asset transfers, disposals, acquisitions, missing records, or unauthorized devices.

### Impact

**4 – Major**

Unreconciled assets may result in security, financial, compliance, and accountability risks.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Reconciliation is performed, but discrepancies may not always be investigated and resolved promptly.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Perform periodic asset reconciliation and track discrepancies through formal remediation until resolved.

---

# AM-IT-005 — Unauthorized Assets

### Sub-Process

Unauthorized Device Detection

### Risk

Unauthorized or unmanaged devices may connect to the organization's network and introduce security risks.

### Existing Controls

* Network access control
* Endpoint management
* Network discovery
* Device monitoring
* Asset inventory reconciliation

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

Unauthorized devices may connect through unmanaged network ports, wireless networks, or other access mechanisms.

### Impact

**5 – Critical**

Unmanaged devices may introduce malware, bypass security controls, or provide unauthorized access to organizational resources.

### Inherent Risk

**3 × 5 = 15 – Major**

### Control Effectiveness

**Partially Effective**

Device discovery and network access controls exist, but unmanaged devices may not always be identified or blocked promptly.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Regularly reconcile network-connected devices against the approved asset inventory and investigate unknown or unauthorized devices.

---

# AM-IT-006 — Asset Lifecycle

### Sub-Process

IT Asset Lifecycle Management

### Risk

Assets may not be appropriately tracked from acquisition through retirement.

### Existing Control

Asset lifecycle procedures covering acquisition, assignment, maintenance, transfer, and retirement.

### Control Type

**Preventive**

### Likelihood

**3 – Possible**

Lifecycle events may not always be updated in the asset management system.

### Impact

**4 – Major**

Incomplete lifecycle tracking may result in inaccurate inventory, unsupported assets, security vulnerabilities, and financial losses.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Lifecycle processes exist, but updates may depend on manual notifications and may not occur consistently.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Define clear responsibilities for updating asset records at acquisition, assignment, transfer, repair, and retirement stages.

---

# AM-IT-007 — Software Inventory

### Sub-Process

Software Asset Management

### Risk

Unauthorized or unsupported software may remain installed on organizational systems.

### Existing Control

Software inventory, approved software lists, endpoint management, and software installation controls.

### Control Type

**Preventive / Detective**

### Likelihood

**3 – Possible**

Users or administrators may install software outside the approved software management process.

### Impact

**4 – Major**

Unauthorized or unsupported software may introduce vulnerabilities, licensing issues, malware, or compatibility problems.

### Inherent Risk

**3 × 4 = 12 – Major**

### Control Effectiveness

**Partially Effective**

Software inventory controls exist, but unauthorized installations may not always be detected promptly.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Regularly compare installed software against approved software inventories and investigate unauthorized or unsupported applications.

---

# AM-IT-008 — Asset Disposal

### Sub-Process

IT Asset Retirement and Disposal

### Risk

Retired assets may be disposed of without adequate data sanitization, resulting in potential information exposure.

### Existing Control

Secure asset disposal procedures, data wiping, destruction certificates, and authorized disposal vendors where applicable.

### Control Type

**Preventive**

### Likelihood

**2 – Unlikely**

Defined disposal procedures reduce the likelihood of data remaining on retired equipment.

### Impact

**5 – Critical**

Improperly sanitized devices may expose confidential organizational or personal information.

### Inherent Risk

**2 × 5 = 10 – Major**

### Control Effectiveness

**Partially Effective**

Disposal procedures exist, but evidence of data sanitization or destruction may not always be consistently maintained.

### Residual Risk

**Major**

### Treatment

**Mitigate**

### Recommended Action

Require documented evidence of data sanitization or destruction before retired assets are disposed of or transferred outside the organization.

---

# 4. IT Asset Lifecycle

A complete asset lifecycle should generally follow:

**Request / Acquisition**

↓

**Registration**

↓

**Classification**

↓

**Assignment**

↓

**Deployment**

↓

**Maintenance**

↓

**Transfer**

↓

**Review**

↓

**Retirement**

↓

**Secure Disposal**

---

# 5. Asset Management Evidence

Examples of evidence that may be requested during control testing include:

### Asset Inventory

* IT asset register
* CMDB records
* Asset tags
* Hardware inventory reports

### Asset Ownership

* User assignment records
* Department ownership records
* System owner records

### Asset Reconciliation

* Reconciliation reports
* Network discovery reports
* Endpoint management reports
* GLPI or CMDB records

### Unauthorized Assets

* Network access reports
* NAC reports
* Unknown device reports
* Investigation tickets

### Software Management

* Software inventory
* Approved software list
* Software installation reports
* License records

### Disposal

* Asset disposal forms
* Data destruction certificates
* Wiping reports
* Disposal vendor records

---

# 6. Asset Management Control Checklist

* [ ] Is there a centralized IT asset inventory?
* [ ] Are all critical assets recorded?
* [ ] Does each critical asset have an owner?
* [ ] Are assets classified by criticality?
* [ ] Are asset records periodically reconciled?
* [ ] Are unknown network devices investigated?
* [ ] Are unauthorized devices blocked or restricted?
* [ ] Are asset transfers recorded?
* [ ] Are retired assets removed from active inventories?
* [ ] Is unauthorized software identified?
* [ ] Are unsupported systems identified?
* [ ] Is data securely removed before disposal?
* [ ] Is evidence of disposal retained?

---

# 7. Key RCSA Observations

### 1. You cannot protect what you cannot see

Asset visibility is the foundation of effective IT risk management.

**Asset Inventory → Vulnerability Management → Security Monitoring → Incident Response**

### 2. Ownership creates accountability

Every important asset should have an accountable owner or custodian.

### 3. Reconciliation identifies gaps

An asset register should not be treated as automatically accurate.

It should periodically be compared against independent sources.

### 4. Unknown devices are a risk signal

A device connected to the organization's network but missing from the approved asset inventory should be investigated.

### 5. Asset lifecycle management prevents stale records

Assets should be tracked throughout their lifecycle rather than only when initially purchased.

### 6. Disposal is a security activity

Retiring an asset does not eliminate the information risk associated with it.

Data should be securely sanitized before disposal or transfer.

---

# 8. Asset Management and IT Risk

Asset management feeds information into several other IT risk processes:

| Asset Management Information | Related IT Risk Process  |
| ---------------------------- | ------------------------ |
| Asset inventory              | Vulnerability Management |
| Asset owner                  | Risk Ownership           |
| Asset criticality            | Risk Assessment          |
| Device status                | Security Monitoring      |
| Network presence             | Access Control           |
| Software inventory           | Vulnerability Management |
| Asset lifecycle              | IT Governance            |
| Disposal status              | Data Protection          |
| Unknown devices              | Incident Management      |

This demonstrates why asset management is an important foundational component of IT Risk.

---

# 9. RCSA Conclusion

Effective IT asset management provides the organization with reliable visibility and accountability over its technology environment.

The RCSA should therefore assess whether the organization can demonstrate:

* Complete asset visibility
* Clear ownership
* Appropriate asset classification
* Regular reconciliation
* Detection of unauthorized assets
* Lifecycle tracking
* Software visibility
* Secure asset disposal

The ultimate objective is to ensure that every relevant IT asset is **known, owned, classified, monitored, managed, and securely retired**.
