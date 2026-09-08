# Information Security Risk Assessment and Treatment Methodology

Risk management regulation. Defines a unified, systematic and repeatable approach to information security risk management. Meets clauses 6.1.2 and 6.1.3 of ISO/IEC 27001:2022.

| Parameter | Value |
|---|---|
| Version | 1.0 |
| Alignment | ISO/IEC 27001:2022 |
| Status | Effective |
| Owner | Information Security Officer / CISO |
| Classification | INTERNAL |
| Approval date | [DD.MM.YYYY] |
| Approvers | [List of approver roles] |

**Notation.** Grey italic text is examples, notes and samples for the drafter – adapt them to your organisation or replace with your own data. Text in `[square brackets]` is a placeholder that must be filled in before approval.

---

## 1. Purpose and scope

This Methodology defines a unified, systematic and repeatable approach to information security risk management. Developed in accordance with clauses 6.1.2 and 6.1.3 of ISO/IEC 27001:2022.

**Objectives of the Methodology:**

- Ensure identification of all relevant information security risks.
- Establish transparent and justified risk assessment criteria.
- Guarantee that risk assessment results are consistent, comparable and repeatable.
- Direct resources to protecting the most critical assets and preventing adverse events.

**Scope.** The Methodology applies to all information assets, processes, systems and sites within the ISMS boundaries defined in the "ISMS Scope Statement".

> *This section explains why risk assessment is critical for the ISMS. The standard requires the methodology to guarantee repeatability – two different analysts assessing the same risk should reach the same conclusion.*

---

## 2. Normative references

This Methodology is based on the following documents:

- ISO/IEC 27001:2022 – Information security, cybersecurity and privacy protection. Information security management systems. Requirements.
- ISO/IEC 27005:2022 – Information security. Guidance on managing information security risks.
- ISO 31000:2018 – Risk management. Guidelines.
- [List applicable national law and industry standards of your country.]

---

## 3. Roles and responsibilities

| Role | Responsibility |
|---|---|
| CEO | [Approves risk acceptance criteria (risk appetite). Approves the Risk Treatment Plan and decides on accepting residual risks.] |
| CISO / IS Officer | [Coordinates the risk assessment process. Maintains the IS Risk Register. Reports to management. Organises periodic reviews of the methodology.] |
| Risk Owners | [Department heads responsible for specific assets or processes. Assess consequences of risk realisation in their zones. Approve risk treatment measures.] |
| Asset Owners | [Persons with authority and responsibility to manage a specific information asset. Provide asset information for risk assessment.] |

> *Assigning risk owners is a key standard requirement. Every risk must have a specific responsible person able to make decisions and allocate resources.*

---

## 4. Assessment criteria (scales and measurements)

> *Before starting the risk assessment, the organisation establishes a single "measuring stick" – criteria that ensure objectivity and comparability.*

Risk assessment is based on two parameters:

- **Impact** – the scale of harm if the risk materializes.
- **Likelihood** – the frequency or probability of the risk occurring.

### 4.1. Impact scale

Impact is assessed through the CIA triad (Confidentiality, Integrity, Availability) and other harm types.

| Level | Description | Examples of harm |
|---|---|---|
| 1 – Low | Minimal business impact | Public information; service outage < 1 hour; financial loss < [amount]; minor user inconvenience. |
| 2 – Moderate | Moderate impact | Leak of internal restricted information; outage up to 4 hours; financial loss [range]. |
| 3 – Medium | Substantial impact | Leak of client confidential data; outage up to 12 hours; financial loss [range]; client complaints. |
| 4 – High | Serious impact | PII breach; regulatory non-compliance; regulator fines; outage up to 1 day; significant financial loss. |
| 5 – Critical | Catastrophic impact | Disclosure of trade secrets; mass PII breach; lawsuits; full business shutdown > 1 day; critical reputational damage; loss of licences. |

> *Adapt examples to your business. State specific financial loss amounts. For a fintech these can be millions, for a small business – thousands. Consider industry regulator requirements.*

### 4.2. Likelihood scale

Likelihood defines how often a threat may materialise considering existing controls.

| Level | Frequency | Description |
|---|---|---|
| 1 – Rare | Once in 5–10 years or less | Theoretically possible, but no incident history in the organisation or industry. Existing controls are effective. |
| 2 – Unlikely | Once in 2–5 years | Isolated cases in the industry. Controls in place but may have gaps. |
| 3 – Possible | Once in 1–2 years | Similar events in the organisation or industry regularly. Controls partially effective. |
| 4 – Likely | Several times a year | Regularly in the organisation or industry. Controls insufficient or absent. |
| 5 – Almost certain | Weekly or monthly | Constantly occurring. Vulnerabilities actively exploited (phishing, DDoS). Controls ineffective or absent. |

> *Likelihood assessment must consider existing controls. If antivirus and firewall are in place, malware infection likelihood decreases. Use your incident history and industry statistics.*

---

## 5. Risk assessment process

The risk assessment process consists of three sequential stages that ensure systematic identification, analysis and evaluation of information security risks.

### Stage 1. Risk identification

For each asset:

- **Asset.** What are we protecting?
- **Threat.** What could happen?
- **Vulnerability.** The weak spot.
- **Consequence.** Loss of CIA.
- **Risk owner.** Responsible person.

**Examples.**

- [Asset: Client database, CRM, source code, servers.]
- [Threat: Hacker attack, fire, employee error, hardware failure, phishing.]
- [Vulnerability: Unpatched software, no MFA, weak passwords, no backups.]

**Identification methods:** interviews with asset owners, incident history analysis, threat intelligence, ISO 27002 checklists.

### Stage 2. Risk analysis

For each risk:

1. **Impact.** Harm magnitude on the 1–5 scale through the CIA triad.
2. **Likelihood.** Threat realisation frequency on the 1–5 scale.
3. **Risk level.** Formula-based calculation and matrix mapping.

**Calculation formula:** `Risk (R) = Impact × Likelihood`.

**Example.** [Risk: PII leak via phishing. Impact: 4 (High – fines). Likelihood: 4 (Likely – regular). Risk level: 4 × 4 = 16 (High).]

**Visualisation.** Result mapped in a 5×5 risk matrix with colour coding (green → yellow → red).

### Stage 3. Risk evaluation

Comparison with acceptance thresholds:

- **1–4: Acceptable.** No treatment required.
- **5–9: Tolerable.** Requires monitoring.
- **10–25: Unacceptable.** Treatment mandatory.

**Decision-making.** Comparing risk level with acceptance criteria (risk appetite):

- Low risks (1–4): recorded in the Register for monitoring.
- Medium risks (5–9): Risk Owner decides on treatment considering resources.
- High/Critical (10–25): immediate treatment, Plan approved by top management.

**Stage output:** prioritised list of risks for treatment in section 6.

> *The assessment process must be documented for each asset. All three stages are captured in the Risk Register. The key standard requirement is repeatability: different analysts assessing the same risk must reach the same result.*

### Risk matrix (5×5)

| Impact ↓ / Likelihood → | 1 Rare | 2 Unlikely | 3 Possible | 4 Likely | 5 Almost certain |
|---|---|---|---|---|---|
| 5 – Critical | 5 Medium | 10 High | 15 High | 20 Critical | 25 Critical |
| 4 – High | 4 Low | 8 Medium | 12 High | 16 High | 20 Critical |
| 3 – Medium | 3 Low | 6 Medium | 9 Medium | 12 High | 15 High |
| 2 – Moderate | 2 Low | 4 Low | 6 Medium | 8 Medium | 10 High |
| 1 – Low | 1 Low | 2 Low | 3 Low | 4 Low | 5 Medium |

> *The risk matrix is a visual tool for prioritisation. Colour coding helps quickly see which risks need immediate action. Green – acceptable, red – critical.*

---

## 6. Risk treatment

| Strategy | Description and examples |
|---|---|
| 1. Modification / Mitigation | Implementing Annex A controls to reduce risk likelihood or impact. [Examples: Antivirus deployment, MFA, data encryption, backup, staff training, patch management, network segmentation.] |
| 2. Avoidance | Ending the activity or use of the asset that creates the risk. [Examples: Disabling a vulnerable port/service, dropping outdated unsupported software, ending processing of certain data types, blocking risky web resources.] |
| 3. Sharing / Transfer | Transferring risk responsibility or consequences to a third party. [Examples: Cyber risk insurance, IT infrastructure outsourcing (transfer to a cloud provider), managed security services (SOC as a Service), contracts with SLA guarantees.] |
| 4. Retention / Acceptance | Deliberate decision not to implement additional controls. Applies when treatment cost exceeds potential harm or the risk is within the organisation's risk appetite. |

> *Risk acceptance decisions must be documented and approved by an authorised person (usually top management). All accepted risks are subject to regular monitoring.*

> *ISO 27001 requires risk treatment decisions to be documented in the Risk Treatment Plan. For each risk, the selected strategy, specific Annex A controls, responsible persons, deadlines and required resources are stated.*

**Strategy selection principle.** For each risk in the Register, one strategy (or a combination – e.g., "mitigation + transfer": implement controls and insure the residual risk) is chosen. The choice is justified by "control cost – risk reduction" ratio and recorded in the Register; actions are captured in the Risk Treatment Plan.

---

## 7. Reporting and documentation

Risk management results are recorded in the following mandatory documents:

**1. Information Security Risk Register.** For each risk: ID, threat and vulnerability description, affected asset, risk owner, impact and likelihood assessment, risk level, treatment status, date of last review.

**2. Risk Treatment Plan (RTP).** For each risk requiring treatment: chosen strategy, specific Annex A controls, responsible parties, implementation deadlines, required resources (budget, staff), expected residual risk.

**3. Statement of Applicability (SoA).** Mandatory ISO 27001 document containing the list of all 93 Annex A controls with justification for inclusion or exclusion. SoA links identified risks to selected controls.

**Update frequency:**

- Risk Register – at least annually or on significant changes.
- Risk Treatment Plan – as controls are implemented and new risks emerge.
- Statement of Applicability – on ISMS scope or control changes.

---

## 8. Review and update

The Methodology and assessment results are reviewed:

- At least once a year (scheduled review).
- On significant organisational change (new processes, systems, units).
- On threat landscape change (new attack types, vulnerabilities).
- After serious IS incidents.
- On change in legal or standard requirements.

> *The risk management process must be integrated into the ISMS PDCA cycle. Risk assessment results are inputs to the Management Review.*

---

## 9. Revision history

| Date | Version | Change description | Author |
|---|---|---|---|
| [DD.MM.YYYY] | 1.0 | Initial edition of the IS Risk Assessment and Treatment Methodology | [Full name] |

---

## 10. Review and approval

The Methodology is reviewed by key stakeholders and approved by top management.

| Role | Full name | Signature | Date |
|---|---|---|---|
| Drafted by: [CISO / IS Officer] | | | |
| Reviewed by: [IT Director / CIO] | | | |
| Approved by: [CEO] | | | |

> *Critical: adapt the impact and likelihood scales to your business. State specific financial loss amounts. The risk matrix and acceptance criteria must be approved by top management and reflect the organisation's real risk appetite.*

---

*We help companies implement an ISMS end-to-end – from gap analysis to passing the certification audit. [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) if you need help adapting this to your business.*
