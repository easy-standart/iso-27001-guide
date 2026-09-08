# Statement of Applicability (SoA)

Mandatory ISO/IEC 27001:2022 document (clause 6.1.3(d)). Comprehensive record of the organisation's position on each of the 93 controls listed in Annex A.

| Parameter | Value |
|---|---|
| Version | 2.0 |
| Alignment | ISO/IEC 27001:2022 |
| Status | Effective |
| Owner | Information Security Officer / CISO |
| Classification | CONFIDENTIAL |
| Approval date | [DD.MM.YYYY] |
| Approvers | [List of approver roles] |

**Notation.** Grey italic text is examples, notes and samples for the drafter – adapt them to your organisation or replace with your own data. Text in `[square brackets]` is a placeholder that must be filled in before approval.

---

## 1. Purpose

This "Statement of Applicability" (SoA) is a mandatory requirement of clause 6.1.3(d) of ISO/IEC 27001:2022 and provides an exhaustive description of the position of [Organisation name] on each of the 93 information security controls listed in Annex A.

**Objectives:**

- Link risk assessment results with actually implemented or planned controls.
- Ensure traceability between the Risk Register, the Risk Treatment Plan and the implemented controls.
- Give ISO 27001 auditors a full "checklist" to verify conformance with the standard.
- Justify the exclusion of controls not applicable to the organisation.

> *The SoA is a "living" document that is updated on every significant change in risk management processes or when new controls are implemented. This is the main document studied by the auditor at the certification audit.*

---

## 2. Justification codes (legend)

For brevity and consistency, the following standard justification codes are used in the applicability table:

| Code | Description |
|---|---|
| RR | **Risk Management** – the control is selected based on IS risk assessment results. There is a direct reference to a specific risk in the Risk Register. |
| LR | **Legal Requirements** – the control is required by national or international law (e.g., GDPR, industry standards, local personal data laws). |
| BR | **Business Requirements** – the control is required to fulfil client contracts, achieve strategic business objectives or ensure competitiveness. |
| BP | **Best Practice** – the control is adopted as a recognised industry standard or best practice for business process reliability and resilience. |

> *A single control may have several justification codes at once. For example: "RR, LR" means the control is needed both to reduce risk and to meet legal requirements.*

---

## 3. Applicability table (Annex A)

### 3.1. Section 5: Organizational controls (37)

| # | Control | Applicable? | Justification | Status | Internal document |
|---|---|---|---|---|---|
| 5.1 | Policies for information security | Yes | LR, RR. Baseline requirement (clause 5.2) | Implemented | [IS Policy] |
| 5.2 | Information security roles and responsibilities | Yes | LR, RR. Baseline requirement (clause 5.3) | Implemented | [RACI matrix] |
| 5.3 | Segregation of duties | Yes | RR. Reducing abuse and error risk | [Implemented / In progress] | [RACI matrix] |
| 5.4 | Management responsibilities | Yes | LR, RR. Standard clause 5.1 | Implemented | [IS Policy] |
| 5.5 | Contact with authorities | Yes | LR. Regulator incident notification | [Implemented / In progress] | [Incident Management Procedure] |
| 5.6 | Contact with special interest groups | [Yes/No] | BP. Peer community exchange | [Implemented / Planned] | [Doc ID] |
| 5.7 | Threat intelligence | [Yes/No] | RR. Proactive defence against new attacks | [Implemented / In progress / Planned] | [Threat Intelligence Policy] |
| 5.8 | Information security in project management | [Yes/No] | BR, RR. Embedding IS in projects | [Implemented / In progress] | [Doc ID] |
| 5.9 | Inventory of information and other associated assets | Yes | RR. Baseline for asset management | Implemented | [Asset Management Policy] |
| 5.10 | Acceptable use of information and other associated assets | Yes | RR, BP. Rules for corporate assets | Implemented | [Asset Management Policy] |
| 5.11 | Return of assets | Yes | RR. Asset protection on offboarding | Implemented | [Asset Management Policy] |
| 5.12 | Classification of information | Yes | RR, LR. Differentiated protection by sensitivity | Implemented | [Classification Policy] |
| 5.13 | Labelling of information | Yes | RR. Supporting classification | Implemented | [Classification Policy] |
| 5.14 | Information transfer | Yes | RR, LR. Protection during data exchange | [Implemented / In progress] | [Classification Policy] |
| 5.15 | Access control | Yes | RR, LR. Core protection mechanism | Implemented | [Access Control Policy] |
| 5.16 | Identity management | Yes | RR. Account lifecycle | Implemented | [Access Control Policy] |
| 5.17 | Authentication information | Yes | RR, LR. Credential protection | Implemented | [Access Control Policy] |
| 5.18 | Access rights | Yes | RR. Control and periodic review of rights | Implemented | [Access Control Policy] |
| 5.19 | Information security in supplier relationships | Yes | RR, LR. Supplier risk management | [Implemented / In progress] | [Supplier Policy] |
| 5.20 | Addressing information security within supplier agreements | Yes | LR, RR. Legal protection via contracts | [Implemented / In progress] | [Supplier Policy] |
| 5.21 | Managing information security in the ICT supply chain | [Yes/No] | RR. Supply chain risk protection | [In progress / Planned] | [Supplier Policy] |
| 5.22 | Monitoring, review and change management of supplier services | Yes | RR. Service quality control | [Implemented / In progress] | [Supplier Policy] |
| 5.23 | Information security for use of cloud services | [Yes/No] | BR, RR. Applicable when using AWS/Azure/GCP | [Implemented / In progress] | [Supplier Policy] |
| 5.24 | Information security incident management planning and preparation | Yes | LR, RR. Incident readiness | Implemented | [Incident Management Procedure] |
| 5.25 | Assessment and decision on information security events | Yes | RR. Incident triage | Implemented | [Incident Management Procedure] |
| 5.26 | Response to information security incidents | Yes | LR, RR. Baseline procedure | Implemented | [Incident Management Procedure] |
| 5.27 | Learning from information security incidents | Yes | RR, BP. Continual improvement | [Implemented / In progress] | [Incident Management Procedure] |
| 5.28 | Collection of evidence | Yes | LR. Legal weight of evidence | [Implemented / In progress] | [Incident Management Procedure] |
| 5.29 | Information security during disruption | [Yes/No] | BR, RR. Continuity | [In progress / Planned] | [BCP] |
| 5.30 | ICT readiness for business continuity | [Yes/No] | BR, RR. Critical for SLA | [Implemented / Planned] | [DR Plan] |
| 5.31 | Legal, statutory, regulatory and contractual requirements | Yes | LR. Baseline requirement | Implemented | [Legal Register] |
| 5.32 | Intellectual property rights | [Yes/No] | LR. Software licence compliance | [Implemented / Not applicable] | [Licence Register] |
| 5.33 | Protection of records | Yes | LR, RR. Log and archive preservation | Implemented | [Incident log] |
| 5.34 | Privacy and protection of PII | Yes | LR. GDPR / local privacy laws | [Implemented / In progress] | [Privacy Policy] |
| 5.35 | Independent review of information security | Yes | LR, BP. Internal or external audit | [Implemented / In progress] | [Audit Programme] |
| 5.36 | Compliance with policies, rules and standards for information security | Yes | RR, LR. Compliance monitoring | [Implemented / In progress] | [Internal Audit Report] |
| 5.37 | Documented operating procedures | Yes | RR, BP. Reducing operational risk | [Implemented / In progress] | [Procedure IDs] |

### 3.2. Section 6: People controls (8)

| # | Control | Applicable? | Justification | Status | Internal document |
|---|---|---|---|---|---|
| 6.1 | Screening | Yes | LR, RR. Reducing insider threat | Implemented | [HR Policy] |
| 6.2 | Terms and conditions of employment | Yes | LR. Employee IS legal obligations | Implemented | [Employment contract] |
| 6.3 | Information security awareness, education and training | Yes | LR, RR. Baseline requirement | Implemented | [Training Matrix] |
| 6.4 | Disciplinary process | Yes | LR. Sanctions for violations | Implemented | [Disciplinary Policy] |
| 6.5 | Responsibilities after termination or change of employment | Yes | RR. Access control on offboarding | Implemented | [Asset Management Policy] |
| 6.6 | Confidentiality or non-disclosure agreements | Yes | LR, RR. Legal protection of trade secrets | Implemented | [NDA template] |
| 6.7 | Remote working | [Yes/No] | BR. Applicable if remote staff exist | [Implemented / Not applicable] | [Mobile Devices Policy] |
| 6.8 | Information security event reporting | Yes | LR, RR. Incident communication channels | Implemented | [Incident Management Procedure] |

### 3.3. Section 7: Physical controls (14)

| # | Control | Applicable? | Justification | Status | Internal document |
|---|---|---|---|---|---|
| 7.1 | Physical security perimeters | Yes | RR. Office/server room perimeter protection | Implemented | [Physical Security Policy] |
| 7.2 | Physical entry | Yes | RR. Zone access control | Implemented | [Physical Security Policy] |
| 7.3 | Securing offices, rooms and facilities | Yes | RR. Physical protection of workspaces | Implemented | [Physical Security Policy] |
| 7.4 | Physical security monitoring | Yes | RR. CCTV, access logs | Implemented | [Physical Security Policy] |
| 7.5 | Protecting against physical and environmental threats | Yes | RR. Fire suppression, climate control | Implemented | [Physical Security Policy] |
| 7.6 | Working in secure areas | Yes | RR. Rules for working in server rooms | Implemented | [Physical Security Policy] |
| 7.7 | Clear desk and clear screen | Yes | RR, BP. Minimising accidental disclosure | Implemented | [Workspace Security Policy] |
| 7.8 | Equipment siting and protection | Yes | RR. Protection from water, dust, heat | Implemented | [Physical Security Policy] |
| 7.9 | Security of assets off-premises | [Yes/No] | RR. Off-site laptop/mobile protection | [Implemented / Not applicable] | [Mobile Devices Policy] |
| 7.10 | Storage media | Yes | RR. Removable media management, disposal | Implemented | [Asset Management Policy] |
| 7.11 | Supporting utilities | Yes | RR. UPS, HVAC, power | Implemented | [Physical Security Policy] |
| 7.12 | Cabling security | Yes | RR. Protection from eavesdropping and damage | Implemented | [Physical Security Policy] |
| 7.13 | Equipment maintenance | Yes | RR. Regular maintenance, contractor control | Implemented | [Physical Security Policy] |
| 7.14 | Secure disposal or re-use of equipment | Yes | RR, LR. Guaranteed data deletion | Implemented | [Asset Management Policy] |

### 3.4. Section 8: Technological controls (34)

| # | Control | Applicable? | Justification | Status | Internal document |
|---|---|---|---|---|---|
| 8.1 | User end point devices | Yes | RR. Protection of workstations and laptops | Implemented | [Mobile Devices Policy] |
| 8.2 | Privileged access rights | Yes | RR. Admin account control | Implemented | [Access Control Policy] |
| 8.3 | Information access restriction | Yes | RR. Least privilege principle | Implemented | [Access Control Policy] |
| 8.4 | Access to source code | [Yes/No] | RR. Applicable to software development | [Implemented / Not applicable] | [Secure Development Policy] |
| 8.5 | Secure authentication | Yes | RR. MFA for critical systems | Implemented | [Access Control Policy] |
| 8.6 | Capacity management | Yes | RR, BR. Performance planning | [Implemented / In progress] | [Procedure ID] |
| 8.7 | Protection against malware | Yes | RR, LR. Baseline malware protection | Implemented | [Malware Protection Policy] |
| 8.8 | Management of technical vulnerabilities | Yes | RR. Regular scanning and patching | Implemented | [Vulnerability Report] |
| 8.9 | Configuration management | Yes | RR, BP. System hardening per CIS benchmarks | [Implemented / In progress] | [Procedure ID] |
| 8.10 | Information deletion | Yes | LR. GDPR / local right to erasure | [Implemented / In progress] | [Asset Management Policy] |
| 8.11 | Data masking | [Yes/No] | RR. PII protection in test environments | [Implemented / Planned] | [Procedure ID] |
| 8.12 | Data leakage prevention (DLP) | [Yes/No] | RR. Exfiltration protection | [Implemented / Planned] | [DLP Policy] |
| 8.13 | Information backup | Yes | RR, BR. Recovery from disruption | Implemented | [Backup Policy] |
| 8.14 | Redundancy of information processing facilities | Yes | BR. Infrastructure resilience | [Implemented / Planned] | [DR Plan] |
| 8.15 | Logging | Yes | RR, LR. Audit trails for investigations | Implemented | [Access Control Policy] |
| 8.16 | Monitoring activities (SIEM) | Yes | RR. Anomaly and attack detection | [Implemented / In progress] | [SIEM Policy] |
| 8.17 | Clock synchronisation (NTP) | Yes | RR. Correct log timestamps | Implemented | [NTP Configuration] |
| 8.18 | Use of privileged utility programs | Yes | RR. Control over system utilities | Implemented | [Access Control Policy] |
| 8.19 | Installation of software on operational systems | Yes | RR. Application installation control | Implemented | [Software Policy] |
| 8.20 | Networks security | Yes | RR. Firewalls, IDS/IPS | Implemented | [Network Policy] |
| 8.21 | Security of network services | Yes | RR. SLA for network services | Implemented | [Network Policy] |
| 8.22 | Segregation of networks | Yes | RR. VLANs, DMZ, critical segment isolation | Implemented | [Network Policy] |
| 8.23 | Web filtering | Yes | RR. Malicious sites protection | Implemented | [Proxy Policy] |
| 8.24 | Use of cryptography | Yes | RR, LR. Data protection at rest and in transit | Implemented | [Cryptography Policy] |
| 8.25 | Secure development life cycle | [Yes/No] | RR. Applicable to software development (Secure SDLC) | [Implemented / Not applicable] | [Secure Development Policy] |
| 8.26 | Application security requirements | [Yes/No] | RR. Applicable to software development | [Implemented / Not applicable] | [Secure Development Policy] |
| 8.27 | Secure system architecture and engineering principles | [Yes/No] | RR. Applicable to software development | [Implemented / Not applicable] | [Secure Development Policy] |
| 8.28 | Secure coding | [Yes/No] | RR. Applicable to software development, OWASP Top-10 | [Implemented / In progress] | [Secure Development Policy] |
| 8.29 | Security testing in development and acceptance (SAST/DAST) | [Yes/No] | RR. Applicable to software development | [Implemented / In progress] | [Secure Development Policy] |
| 8.30 | Outsourced development | [Yes/No] | RR. Applicable when using external developers | [Implemented / Not applicable] | [Supplier Policy] |
| 8.31 | Separation of development, test and production environments | [Yes/No] | RR. Applicable to software development | [Implemented / Not applicable] | [Secure Development Policy] |
| 8.32 | Change management | Yes | RR, BR. Change management process | Implemented | [CM Procedure] |
| 8.33 | Test information (Test data) | [Yes/No] | RR. PII protection in test data | [Implemented / In progress] | [Procedure ID] |
| 8.34 | Protection of information systems during audit testing | Yes | RR. Audit activity isolation | [Implemented / In progress] | [Procedure ID] |

---

## 4. Justification of exclusions

If any Annex A control is deemed non-applicable, the exclusion justification must be specific, detailed and convincing. Exclusion of a control is a critical audit checkpoint.

**Exclusion justification requirements:**

- The justification must show that the control is objectively not applicable (not just difficult or expensive to implement).
- Specific facts about the organisation's activities must be stated.
- The exclusion must be consistent with risk assessment results.

**Exclusion justification example:**

> Control 5.32 (Intellectual property rights) – NO, not applicable.
>
> Justification: The organisation does not use third-party proprietary software with licensing restrictions. All software used is open-source (Apache, MIT licences) or developed in-house. The organisation does not create objects of copyright for external commercialisation. Risks related to IPR violations were not identified in the risk assessment.

> *Weak or missing exclusion justification is one of the most common causes of non-conformities at ISO 27001 certification audits.*

---

## 5. Revision history

| Date | Version | Change description | Author |
|---|---|---|---|
| [DD.MM.YYYY] | 2.0 | Update to ISO/IEC 27001:2022 (93 Annex A controls) | [Full name] |

---

## 6. Review and approval

The Statement of Applicability must be approved by top management as a key ISMS document.

| Role | Full name | Signature | Date |
|---|---|---|---|
| Drafted by: [CISO / IS Officer] | | | |
| Reviewed by: [Approver role] | | | |
| Approved by: [CEO] | | | |

> *Critical: the SoA is the main audit document. Every excluded control must have a convincing justification. Implementation statuses must match reality. The SoA must be updated on every significant change in the RTP or Risk Register. A missing or incorrectly filled SoA is the main cause of non-conformities at certification audits.*

---

*We help companies implement an ISMS end-to-end – from gap analysis to passing the certification audit. [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) if you need help adapting this to your business.*
