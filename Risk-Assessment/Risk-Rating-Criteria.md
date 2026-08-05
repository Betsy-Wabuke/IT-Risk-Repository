# Risk Rating Criteria

## 1. Purpose

Risk rating criteria provide a consistent basis for evaluating the likelihood and impact of identified IT risks.

The criteria help ensure that similar risks are assessed consistently and that higher-priority risks receive appropriate management attention.

> **Note:** The criteria below are an example methodology for this portfolio. Actual organizations should use their formally approved risk assessment methodology.

---

## 2. Likelihood Rating

Likelihood measures how probable it is that a risk event will occur.

| Score | Rating         | Description                                                                                |
| ----: | -------------- | ------------------------------------------------------------------------------------------ |
| **1** | Rare           | The event is highly unlikely to occur under normal circumstances.                          |
| **2** | Unlikely       | The event could occur, but there is limited evidence or opportunity for occurrence.        |
| **3** | Possible       | The event could reasonably occur and there is some evidence or opportunity for occurrence. |
| **4** | Likely         | The event is expected to occur or there is significant opportunity for occurrence.         |
| **5** | Almost Certain | The event is highly likely to occur or is already occurring frequently.                    |

### Factors to Consider

When determining likelihood, consider:

* Frequency of exposure
* Previous incidents
* Threat activity
* Vulnerability of the affected environment
* Effectiveness of existing controls
* Number of users/assets/systems exposed
* Ease with which the risk event could occur

---

## 3. Impact Rating

Impact measures the potential consequence if the risk materializes.

| Score | Rating        | Description                                                                                                                                                      |
| ----: | ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1** | Insignificant | Minimal impact with little or no disruption to business operations.                                                                                              |
| **2** | Minor         | Limited impact that can be managed through normal operational processes.                                                                                         |
| **3** | Moderate      | Noticeable operational, financial, compliance, or security impact requiring management attention.                                                                |
| **4** | Major         | Significant impact that may disrupt important business operations or result in substantial financial, security, regulatory, or reputational consequences.        |
| **5** | Critical      | Severe impact that could significantly affect critical business operations, regulatory obligations, financial stability, security, or organizational reputation. |

---

## 4. Risk Score

The risk score is calculated as:

**Risk Score = Likelihood × Impact**

For example:

> Likelihood = 4
> Impact = 5
> Risk Score = 4 × 5 = **20**

The resulting score should then be mapped to the organization's approved risk-rating bands.

---

## 5. Example Risk Rating Bands

For this portfolio, the following example bands can be used:

|     Score | Rating   | General Priority                           |
| --------: | -------- | ------------------------------------------ |
|   **1–4** | Low      | Routine monitoring                         |
|   **5–9** | Moderate | Management attention and planned treatment |
| **10–16** | Major    | Prioritized remediation and monitoring     |
| **17–25** | Critical | Urgent management attention and treatment  |

> These thresholds are illustrative and should not be treated as a universal standard. An organization's approved risk methodology takes precedence.

---

## 6. Example

### Scenario

A critical vulnerability exists on an internet-facing production server and remediation has been significantly delayed.

### Likelihood

**4 – Likely**

The system is exposed to external threats and the vulnerability remains unremediated.

### Impact

**5 – Critical**

Successful exploitation could result in compromise of a critical production system and potentially affect business operations and information security.

### Risk Score

**4 × 5 = 20**

### Example Rating

**Critical**

### Recommended Treatment

Prioritize remediation and implement appropriate compensating controls until the vulnerability is resolved.

---

## 7. Important Considerations

Risk scores should not be considered purely mathematical.

A risk with a lower numerical score may still require immediate management attention if it involves:

* Critical systems
* Regulatory requirements
* Sensitive information
* Privileged access
* Significant legal exposure
* Potential fraud
* Material business disruption

Risk assessment should therefore combine quantitative scoring with professional judgment and organizational context.

---

## 8. Key Takeaway

A consistent risk-rating methodology enables organizations to:

* Compare risks consistently
* Prioritize remediation
* Allocate resources effectively
* Escalate significant risks
* Monitor risk trends
* Support management decision-making

The objective is not simply to calculate a number. The objective is to determine **which risks require the greatest attention and why.**
