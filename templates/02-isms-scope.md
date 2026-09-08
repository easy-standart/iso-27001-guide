# ISMS Scope Statement

Management-level document. Defines the physical, organisational and technological boundaries of the Information Security Management System. Meets clause 4.3 of ISO/IEC 27001:2022.

| Parameter | Value |
|---|---|
| Version | 1.0 |
| Alignment | ISO/IEC 27001:2022 |
| Status | Effective |
| Classification | INTERNAL |
| Owner | [Responsible role] |
| Approval date | [DD.MM.YYYY] |
| Approvers | [List of approver roles] |

**Notation.** Grey italic text is examples, notes and samples for the drafter – adapt them to your organisation or replace with your own data. Text in `[square brackets]` is a placeholder that must be filled in before approval.

---

## 1. Purpose

This document defines the physical, organisational and technological boundaries of the Information Security Management System (ISMS) in accordance with clause 4.3 of ISO/IEC 27001:2022.

The document establishes:

- the perimeter of information asset protection;
- units, processes and sites covered by the ISMS;
- technological components of the infrastructure;
- points of interaction with external parties;
- justified exclusions of controls from Annex A.

> *This section can be kept as-is or adapted to your specifics. The core purpose is to state that the document defines the ISMS boundaries per the standard.*

---

## 2. Grounds for defining the scope

When establishing the ISMS boundaries, the following factors were considered per clauses 4.1–4.3 of ISO/IEC 27001:2022:

**External and internal factors.** [State key external factors: technology trends, regulator requirements, geopolitical situation, industry state. Internal: scale, organisational structure, technology, strategic objectives.]

**Interested parties and their requirements.** [List parties: clients, shareholders, employees, regulators, suppliers. State their key IS requirements. Example: "Clients require ISO 27001 conformance, regulators require compliance with the Data Protection Law".]

**Legal and regulatory requirements.** [State applicable law of your country. Example: personal data law, trade secret law, industry standards. For an EU business – GDPR.]

**Interdependencies with external organisations.** [State key external dependencies: cloud providers (Azure, AWS, Google Cloud), outsourcing partners, landlords (for leased offices), software and hardware suppliers.]

**Climate change impact (2024 update).** [If applicable, state how climate factors can affect IS: risks of power outage, extreme weather affecting the data centre, etc. If not applicable – state: "Climate change impact on the ISMS is assessed as negligible".]

---

## 3. ISMS boundaries

The ISMS scope is defined through three boundary types: organisational, physical and technological.

### 3.1. Organisational boundaries

The ISMS covers the following units and business processes:

[List units: IT Department, Development, Support, HR, Finance, etc.]

**Key business processes in scope:**

- [Software development]
- [Customer technical support]
- [IT infrastructure management]
- [Employee personal data processing]

**Processes excluded from the ISMS scope:**

[List processes not in scope: e.g., marketing, physical security (if outsourced), etc. State the exclusion reason.]

### 3.2. Physical boundaries

The following premises and sites are in scope:

**Controlled zones:**

- [Server rooms (specify locations)]
- [Archives of paper documents]
- [Workstations with access to confidential information]

**Remote workplaces.** [If staff work from home permanently, state: "Remote workplaces of staff using corporate hardware". If not – "Not applicable".]

### 3.3. Technological and logical boundaries

The following information assets and technological components are protected:

**Network infrastructure:**

- [Office LAN]
- [VPN for remote access]
- [Guest Wi-Fi (if applicable)]
- [Firewalls and perimeter defence tools]

**Information systems:**

- [CRM: specify]
- [Project management: Jira, Asana, etc.]
- [Corporate email: Microsoft 365, Google Workspace, etc.]
- [Database management systems]
- [ERP and other corporate systems]

**Cloud environments and services:**

- [Microsoft Azure / AWS / Google Cloud – list what you use]
- [Google Drive / Dropbox / OneDrive for document storage]
- [SaaS applications: list critical services]

**Workstations and mobile devices:**

- [Corporate laptops and desktops]
- [Mobile devices (phones, tablets) accessing corporate data]
- [Removable media (if allowed)]

---

## 4. Interfaces and dependencies

The organisation interacts with external parties through the following control points and dependencies:

**Services provided by external parties:**

- [Physical security and fire safety (if outsourced to landlord or contractor)]
- [IT infrastructure support (outsourcing)]
- [Internet service providers]
- [Cloud providers (AWS, Azure, Google Cloud)]

**Information exchange with clients and partners:**

- [Data transfer channels: secure APIs, SFTP, email, etc.]
- [Security requirements to partners: NDAs, security audits, etc.]

**Dependence on software and hardware suppliers.** [List critical suppliers: Microsoft, Cisco, hardware manufacturers, etc. Describe how supply and update security is ensured.]

---

## 5. Exclusions from Annex A

The organisation applies all clauses 4–10 of ISO 27001:2022 without exclusion.

For Annex A controls, the following justified exclusions are established:

[Example: Control A.7.13 "Equipment maintenance" – Not applicable in full, the organisation runs on IaaS-hosted infrastructure and does not maintain its own server hardware in the corporate physical premises. Equipment maintenance is covered by the provider under its own 27001 certification; responsibility is confirmed in the contract.]

[List other exclusions if any. If all controls apply, state: "All Annex A controls are applicable to the ISMS scope".]

> *A detailed applicability matrix of all 93 controls is in the separate "Statement of Applicability" (SoA).*

---

## 6. Revision history

The document is reviewed at least once a year or upon organisational, technological or legal changes.

| Date | Version | Change description | Author |
|---|---|---|---|
| [DD.MM.YYYY] | 1.0 | Initial edition | [Full name] |

---

## 7. Review and approval

The document is reviewed by the person responsible for information security (CISO) and approved by top management.

| Role | Full name | Signature | Date |
|---|---|---|---|
| Drafted by: [CISO / IS Specialist] | | | |
| Reviewed by: [IT Director / CIO] | | | |
| Approved by: [CEO] | | | |

---

*We help companies implement an ISMS end-to-end – from gap analysis to passing the certification audit. [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) if you need help adapting this to your business.*
