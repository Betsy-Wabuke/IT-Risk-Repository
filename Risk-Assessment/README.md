# Risk Assessment

## 1. Overview

Risk assessment is the process of evaluating identified risks to determine their potential severity and prioritize them for appropriate treatment.

In IT Risk Management, risk assessment commonly considers:

* Likelihood
* Impact
* Existing controls
* Inherent risk
* Residual risk

## 2. Risk Assessment Process

A practical risk assessment process is:

**Identify → Assess Likelihood → Assess Impact → Determine Inherent Risk → Evaluate Controls → Determine Residual Risk**

### Step 1: Identify the Risk

Start with a clearly defined risk statement.

Example:

> Because privileged activities are performed using shared administrative accounts, there is a risk that system changes cannot be attributed to individual users, which could result in unauthorized changes remaining undetected.

### Step 2: Assess Likelihood

Determine how likely it is that the risk event will occur.

Factors that may be considered include:

* Frequency of exposure
* Existing controls
* Threat likelihood
* History of similar incidents
* Vulnerability of the affected system
* Ease of exploitation

### Step 3: Assess Impact

Determine the potential consequences if the risk materializes.

Consider impacts such as:

* Financial
* Operational
* Regulatory
* Legal
* Reputational
* Confidentiality
* Integrity
* Availability

### Step 4: Determine Inherent Risk

Inherent risk represents the level of risk **before considering the effectiveness of existing controls**.

A simple approach is:

**Likelihood × Impact = Inherent Risk Score**

### Step 5: Evaluate Existing Controls

Assess whether existing controls adequately reduce the likelihood or impact of the risk.

Consider:

* Is the control documented?
* Is the control properly designed?
* Is the control implemented?
* Is the control operating effectively?
* Is there evidence that the control operates?

### Step 6: Determine Residual Risk

Residual risk is the level of risk remaining after considering existing controls.

The residual risk helps management determine whether further risk treatment is necessary.

---

# 3. 5×5 Risk Matrix

A 5×5 risk matrix can be used to assess risk based on likelihood and impact.

| Likelihood \ Impact    |  1 |  2 |  3 |  4 |  5 |
| ---------------------- | -: | -: | -: | -: | -: |
| **5 – Almost Certain** |  5 | 10 | 15 | 20 | 25 |
| **4 – Likely**         |  4 |  8 | 12 | 16 | 20 |
| **3 – Possible**       |  3 |  6 |  9 | 12 | 15 |
| **2 – Unlikely**       |  2 |  4 |  6 |  8 | 10 |
| **1 – Rare**           |  1 |  2 |  3 |  4 |  5 |

**Risk Score = Likelihood × Impact**

The organization should define the risk rating bands that correspond to its approved risk methodology.

---

# 4. Example Risk Assessment

### Risk

Generic administrative accounts are used to perform system changes without sufficient individual attribution.

### Likelihood

**4 – Likely**

The weakness may occur whenever administrative activities are performed using shared accounts.

### Impact

**4 – Major**

A lack of individual accountability could make unauthorized or inappropriate system changes difficult to investigate and may result in operational, security, or audit consequences.

### Inherent Risk

**4 × 4 = 16**

**Inherent Risk Score: 16**

The final risk rating should be mapped to the organization's approved risk-rating thresholds.

---

# 5. Inherent vs Residual Risk

### Inherent Risk

Risk that exists **before considering existing controls**.

### Residual Risk

Risk that remains **after considering existing controls**.

For example:

> **Inherent Risk:** 16
> Existing controls: Named accounts, privileged access management, activity logging and periodic access reviews
> **Residual Risk:** To be determined based on the effectiveness of these controls.

Residual risk should not automatically be assumed to be lower than inherent risk. The reduction should be supported by an assessment of the actual control design and operating effectiveness.

---

# 6. Risk Assessment Questions

When assessing an IT risk, consider:

* [ ] How likely is the risk to occur?
* [ ] What would happen if the risk materialized?
* [ ] Which systems, processes or information could be affected?
* [ ] What existing controls are in place?
* [ ] Are the controls adequately designed?
* [ ] Are the controls operating effectively?
* [ ] Is there sufficient evidence of control operation?
* [ ] What is the inherent risk?
* [ ] What is the residual risk?
* [ ] Is further risk treatment required?

## 7. Key Takeaway

Risk assessment helps an organization distinguish between risks that require immediate attention and those that can be managed through routine monitoring.

A good assessment should therefore be **evidence-based, consistent, and aligned with the organization's approved risk methodology.**
