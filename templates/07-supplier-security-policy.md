# Supplier and Cloud Services Security Policy

Level 2 topical information security policy. Defines IS requirements for interactions with external suppliers and use of cloud services. Implements A.5.19–A.5.23 of ISO/IEC 27001:2022.

| Parameter | Value |
|---|---|
| Version | 1.0 |
| Alignment | ISO/IEC 27001:2022 |
| Status | Effective |
| Owner | Information Security Officer (CISO) |
| Classification | INTERNAL |
| Approval date | [DD.MM.YYYY] |
| Approvers | [List of approver roles] |

**Notation.** Grey italic text is examples, notes and samples for the drafter – adapt them to your organisation or replace with your own data. Text in `[square brackets]` is a placeholder that must be filled in before approval.

---

## 1. Purpose and scope

This Policy defines information security (IS) requirements for interactions with external suppliers and use of cloud services. The goal is to minimise risks related to third-party access to the Company's assets and to maintain a consistent level of information protection across the supply chain.

The Policy applies to all supplier types:

- IT developers and integrators (software vendors, system integration).
- Cloud service providers (SaaS, PaaS, IaaS) – Microsoft 365, AWS, Google Workspace and others.
- Telecommunications providers (internet, telephony, VPN).
- Outsourcing companies (accounting, HR services, call centres).
- Service staff (cleaning, logistics, security companies).

---

## 2. Normative references and related documents

The Policy is based on the following standards and internal documents:

| Standard / Document | Applicable controls / sections |
|---|---|
| ISO/IEC 27001:2022 | Group 5 controls (Organizational): A.5.19 – IS in supplier relationships; A.5.20 – Addressing IS in supplier agreements; A.5.21 – Managing IS in the ICT supply chain; A.5.22 – Monitoring, review and change management of supplier services; A.5.23 – IS for use of cloud services |
| ISO/IEC 27005 | IS risk assessment methodology (for supplier evaluation) |
| Internal ISMS documents | Asset and Risk Register, Compliance Policy, Vulnerability Analysis Instruction, IS Risk Assessment Methodology |

---

## 3. Terms and definitions

For the purposes of this Policy:

| Term | Definition |
|---|---|
| Supplier / Vendor | Any external organisation or individual providing products or services to the Company (software, cloud services, consulting, security, cleaning, etc.) |
| Cloud Service | A service providing access to information resources through the internet, where infrastructure is managed by the provider. Cloud service models: SaaS (Software as a Service) – ready software (Gmail, Salesforce); PaaS (Platform as a Service) – development platform (Heroku); IaaS (Infrastructure as a Service) – virtual infrastructure (AWS EC2, Azure VM) |
| SLA (Service Level Agreement) | A service level agreement document defining service delivery parameters (availability, response time, party responsibility). Example SLA: 99.9% uptime guarantee, incident response – 4 hours |
| Supply Chain | The network of organisations involved in delivering a product or service to the client. Includes suppliers, subcontractors, logistics companies. Example: the Company uses AWS (primary supplier), which uses Equinix data centres (subcontractor) – this is a supply chain |

---

## 4. Supplier risk assessment (Control A.5.19)

The Company applies a risk-based approach: engagement with a supplier is not possible without prior IS risk analysis per ISO/IEC 27005.

### 4.1. Risk factors

When assessing a supplier:

- Access to confidential data (trade secrets, client PII).
- Physical access to the organisation's premises (cleaning, security).
- Criticality of provided services for business (cloud email, ERP).
- Geographical location of the supplier's data centres (compliance with data localisation legislation).

### 4.2. Decision criteria

| Risk level | Decision / Actions |
|---|---|
| Low | Subject to monitoring but not immediate discontinuation. Minimal control requirements. Example: office supplies vendor. |
| Medium | NDA required, IS requirements in contracts. Regular monitoring (annual). Example: internet service provider. |
| High / Critical | Grounds for immediate discontinuation and placement on "denylist". Critical risk examples: no PII encryption; weak physical data centre protection; no IS certifications for critical services; subcontractors in countries with data transfer restrictions. |

### 4.3. Supply chain integrity

The assessment considers risks not only of the direct supplier but also of subcontractors. The Company may require disclosure of information about subcontractors and their IS certifications.

---

## 5. Supplier selection and verification requirements (Control A.5.21)

### 5.1. Compliance evidence

The Company is entitled to request compliance evidence from a potential supplier before contract signing:

| Evidence type | Description and examples |
|---|---|
| Compliance certificates | ISO/IEC 27001 – international ISMS standard; SOC 2 Type II – security audit (for cloud providers); PCI DSS – for payment card processing; TISAX – for automotive industry; GDPR compliance – European personal data regulation |
| Independent auditor reports | Results of external IS audits, penetration tests, vulnerability analysis. Example: SOC 2 Type II report from a Big Four firm (Deloitte, PwC, EY, KPMG) |
| IS policies and procedures | Copies of supplier's internal documents: IS policy, incident management procedure, business continuity plan (BCP/DR) |

### 5.2. Second-Party Audit

In critical cases (e.g., processing large volumes of client PII), the Company may initiate its own audit of the supplier's security system or engage an independent expert for on-site inspection.

> *Example: Before signing a contract with a new cloud storage provider, the CISO team visits the data centre to verify physical security (access control, CCTV, fire suppression).*

### 5.3. Approved suppliers register

The Information Security Officer (CISO) maintains and updates a centralised Approved Suppliers Register including:

- Organisation name.
- Type of services provided.
- Risk level (Low / Medium / High).
- IS certifications held.
- Date of last review.
- Date of next scheduled review.

---

## 6. Contract requirements with suppliers (Control A.5.20)

All contracts with suppliers having access to the organisation's information assets must contain mandatory IS sections. This is a control A.5.20 requirement.

**Mandatory contract provisions:**

- list of information assets and systems to which access is granted;
- data confidentiality level (with reference to the Classification Policy);
- technical security requirements (encryption, access control, logging);
- confidentiality obligations (NDA) with duration after contract termination;
- accountability for IS incidents, including financial sanctions and right of recourse;
- the organisation's right to audit supplier's IS compliance;
- IS incident notification requirements (deadline: no more than 24 hours from detection);
- procedures on contract termination (asset return/destruction, access revocation).

**Contract review.** The contract draft with IS section is reviewed by the CISO before signing. Without this review, the contract is not forwarded for approval.

---

## 7. Monitoring and change management of supplier services (Control A.5.22)

Supplier services are subject to regular monitoring to confirm alignment with agreed service levels (SLA) and IS requirements. This is a control A.5.22 requirement.

**Monitoring parameters:**

- SLA metrics (availability, response time, recovery time);
- IS metrics (currency of supplier's SOC 2 / ISO 27001 certifications, incident reports);
- compliance with obligations on updates, patch management, configurations;
- regular supplier reports (at least quarterly for critical suppliers).

**Change management.** Any changes in supplier services (technology stack switch, expansion of processed data scope, infrastructure migration) must be coordinated with the organisation. Changes undergo IS risk assessment before implementation (see section 4).

**Termination and reassessment.** Contracts are reviewed at least annually. Grounds for termination: systemic SLA violations, repeat IS incidents, absence of active certifications, loss of trust based on audit results.

---

## 8. Information security for use of cloud services (Control A.5.23)

Use of cloud services (IaaS/PaaS/SaaS – AWS, Azure, Google Cloud, local providers) is subject to specific IS requirements per control A.5.23 (added in ISO/IEC 27001:2022).

**Cloud provider selection principles:**

- the provider must have an active ISO/IEC 27001 or SOC 2 Type II certificate;
- the Shared Responsibility Model must be documented;
- physical data placement must comply with legislation (for personal data – servers in countries with adequate protection level per local regulation);
- the provider provides tools for access management, logging, encryption.

**Mandatory technical measures for cloud use:**

- data encryption in transit (TLS 1.2+) and at rest (AES-256);
- MFA for all accounts with cloud management console access;
- role separation and least privilege principle (IAM);
- regular backup of critical data to local infrastructure or another cloud region (see the Backup Policy);
- cloud configuration monitoring (CSPM tools) to detect misconfiguration.

**Cloud service exit strategy.** On termination of provider use: data migration within approved timelines, documented confirmation of data deletion by the provider, access revocation.

---

## 9. Revision history

| Date | Version | Description | Author |
|---|---|---|---|
| [DD.MM.YYYY] | 1.0 | Initial edition of the document | [Full name] |

---

## 10. Review and approval

| Role | Full name | Signature | Date |
|---|---|---|---|
| Drafted by: [Responsible role] | | | |
| Reviewed by: [CISO / IS Officer] | | | |
| Approved by: [Director] | | | |

---

*We help companies implement an ISMS end-to-end – from gap analysis to passing the certification audit. [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) if you need help adapting this to your business.*
