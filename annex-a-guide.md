# Annex A – 93 controls of ISO/IEC 27001:2022. An executive guide

> What the controls are, why they matter and what audit-ready evidence looks like. No copy-paste of the standard text – direct practical value only.

In the 2022 edition, Annex A was rebuilt from scratch. The previous version had 114 controls across 14 sections. Now there are 93 controls across 4 themes. This isn't cosmetic renumbering – it's **structural consolidation**: 57 old controls were merged into 24 new ones, 1 was split into 2, 11 new controls were added, and the remaining 56 stayed substantively unchanged. Full correspondence table: Annex B of ISO/IEC 27002:2022.

If you already hold a 27001:2013 certificate, most of the work carries over. If you're starting from scratch, this file explains what the standard actually asks of your business.

*Русская версия: [../annex-a-guide.md](../annex-a-guide.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## The four themes

All 93 controls fall into four buckets:

| Theme | Section | Count | What it covers |
|---|---|---|---|
| Organizational | A.5 | 37 | Policies, rules and procedures at the organisation level |
| People | A.6 | 8 | People-related measures: hiring, training, remote work, offboarding |
| Physical | A.7 | 14 | Protection of physical assets, premises and perimeter |
| Technological | A.8 | 34 | Technical and digital measures: encryption, secure development, monitoring |

The math checks out: 37 + 8 + 14 + 34 = 93.

---

## Five attributes – optional but useful

In ISO/IEC 27002:2022, each control carries five attributes. These aren't certification requirements – they're supporting "tags" for risk assessment and mapping to other frameworks.

| Attribute | Values | Why it matters |
|---|---|---|
| Control Type | Preventive, Detective, Corrective | Balance of controls across incident phases |
| Information Security Properties | Confidentiality, Integrity, Availability (CIA) | Triad coverage |
| Cybersecurity Concepts | Identify, Protect, Detect, Respond, Recover | Direct mapping to NIST CSF functions |
| Operational Capabilities | 15 values: governance, asset management, access management, etc. | Grouping by operational disciplines |
| Security Domains | Governance and ecosystem, Protection, Defence, Resilience | Strategic view |

**Practical use.** SoAs often add an attributes column for board reporting – a "30% preventive, 50% detective" split. Attributes also help you pick compensating controls when accepting residual risk.

**A note on NIST CSF 2.0.** In February 2024, NIST added a sixth function – **Govern**. The Cybersecurity Concepts attribute in 27002:2022 still uses the five original values. As of 2026 there is no official NIST- or ENISA-published mapping of Govern to ISO 27001. Working practice treats Govern as covering clauses 4–5 of ISO 27001 (context and leadership), with partial coverage of 6–7. This is a **working reference for compliance teams**, not an "official mapping".

---

## Connection to the management part

Annex A doesn't stand apart from clauses 4–10. Each clause tells you "how"; Annex A tells you "with what".

| Clause | Purpose | Where Annex A shows up |
|---|---|---|
| 4 Context | Understanding the organisation, interested parties, scope | Defines which assets and processes are in scope for controls |
| 5 Leadership | Top management commitments, security policy | A.5.1 (security policy) and A.5.2 (roles) operationalize clause 5 |
| 6 Planning | Risk assessment and treatment, objectives, change planning | **The main entry point to Annex A.** Clause 6.1.3 requires selecting controls based on risk assessment; 6.1.3(d) requires the SoA |
| 7 Support | Resources, competencies, awareness | A.6.1–A.6.3 (hiring, screening, training), A.5.37 (operating procedures) |
| 8 Operation | Operational planning, control implementation | Where Annex A controls actually live day-to-day |
| 9 Performance | Monitoring, internal audit, management review | A.5.35–A.5.36 (independent review, compliance), A.8.15–A.8.16 (logging, monitoring) |
| 10 Improvement | Nonconformities, corrective actions, continual improvement | Applies to all controls |

The 2022 edition also added clause **6.3 Planning for changes** – formal requirements for managing changes to the ISMS.

---

## The 11 new controls of 2022 – what matters

These controls are the main focus for first-time certification or transition from 2013.

### A.5.7 Threat Intelligence

Collect threat information, analyze it at three levels – strategic, tactical, operational – and act on it.

**Common mistake.** Subscribing to a CTI feed without any process to handle it. Data flows in; the risk register doesn't move. Auditors log this as "control declared, not operationalized."

**Audit-ready evidence.** Quarterly threat intel report plus at least 2 examples of updating the Risk Treatment Plan in response to new TTPs.

### A.5.23 Cloud Services

Security requirements across the **full lifecycle** of cloud services: acquisition, use, management, exit.

**Common mistake.** Assuming the provider handles all the security – a shared-responsibility failure. AWS covers security *of* the cloud; the customer covers security *in* the cloud.

**Audit-ready evidence.** Cloud register plus an exit strategy for the top 3 critical providers.

### A.5.30 ICT Readiness for Business Continuity

The ICT-specific layer of the broader BCM program. Narrow focus on technology readiness for recovery.

**Common mistake.** ICT readiness is declared on paper, but real DR tests haven't run in years.

**Audit-ready evidence.** Report from the most recent DR test, plus an ICT continuity plan and a BIA.

### A.7.4 Physical Security Monitoring

Monitoring of physically secured zones via CCTV, alarms and guards.

**Common mistake.** Falling foul of GDPR or local data protection law – CCTV deployed with no DPIA, no defined retention period.

**Audit-ready evidence.** Zone map, CCTV configuration, DPIA and retention policy.

### A.8.9 Configuration Management

Full lifecycle management for configurations of hardware, software, services and networks.

**Common mistake.** Hardening standards exist on paper but aren't enforced. Actual production configurations drift from baseline.

**Audit-ready evidence.** Hardening baselines (CIS Benchmarks, STIG), IaC with code review, configuration drift monitoring.

### A.8.10 Information Deletion

Delete data when it's no longer needed – to comply with privacy laws (GDPR Right to Erasure and equivalents).

**Common mistake.** Forgotten copies in cloud storage and backups. GDPR requires deletion everywhere – policies often skip over that.

**Audit-ready evidence.** Data retention schedule plus secure erasure procedures for all media types.

### A.8.11 Data Masking

Mask data to limit exposure. Pseudonymization, anonymization, encryption.

**Common mistake.** Production PII sitting in test and dev environments. The single most common finding.

**Audit-ready evidence.** Data masking policy plus configured tooling in non-prod environments.

### A.8.12 Data Leakage Prevention

Measures to prevent and detect unauthorized transfer of data outside the perimeter.

**Common mistake.** DLP left in "monitor only" mode for years. Alerts fire; nobody responds.

**Audit-ready evidence.** List of DLP incidents with classification, plus response records.

### A.8.16 Monitoring Activities

Monitoring of networks, systems and applications for anomalous behavior.

**Common mistake.** Logs are collected (A.8.15) but nobody looks at them. SIEM is "configured" but reports are empty.

**Audit-ready evidence.** 2–3 closed incident tickets from SIEM alerts, with timeline and lessons learned.

### A.8.23 Web Filtering

Manage user access to external websites.

**Common mistake.** Filtering works in the office only – remote users without VPN aren't covered. Categories aren't reviewed – AI services, for example, become a channel for uncontrolled data exfiltration.

**Audit-ready evidence.** Web filtering policy plus evidence the filter is actually running.

### A.8.28 Secure Coding

Secure development principles across the software development lifecycle.

**Common mistake.** Standards exist on paper, without enforcement through mandatory peer review. Third-party libraries pulled in without SBoM or SCA.

**Audit-ready evidence.** Git logs with peer-review approvals, SAST/DAST in CI/CD, and an SBoM for the main product.

---

## All 93 controls – quick reference

Names come from ISO/IEC 27002:2022. The "essence" column is a paraphrase to avoid copyright issues. The "risk" column is an expert estimate of the risk of not having the control in place (H – high, M – medium, L – low). Actual risk for your company comes out of your own risk assessment.

### A.5 Organizational controls (37)

| Control | Name | Essence | Risk |
|---|---|---|---|
| A.5.1 | Policies for information security | Approved set of security policies | H |
| A.5.2 | Information security roles and responsibilities | ISMS role allocation | H |
| A.5.3 | Segregation of duties | Separation of authority | M |
| A.5.4 | Management responsibilities | Top management duties | H |
| A.5.5 | Contact with authorities | Contacts with regulators | M |
| A.5.6 | Contact with special interest groups | Contacts with CERT, security associations | L |
| **A.5.7** | **Threat intelligence** (added in 2022) | Threat intel collection and analysis | H |
| A.5.8 | Information security in project management | Security requirements in project management | M |
| A.5.9 | Inventory of information and other associated assets | Asset register with owners | H |
| A.5.10 | Acceptable use of information and other associated assets | Rules of use | M |
| A.5.11 | Return of assets | Asset return at termination | M |
| A.5.12 | Classification of information | Information sensitivity classification | H |
| A.5.13 | Labelling of information | Labelling per classification | M |
| A.5.14 | Information transfer | Information transfer protection | H |
| A.5.15 | Access control | Access control policy | H |
| A.5.16 | Identity management | Identity management | H |
| A.5.17 | Authentication information | Authentication management | H |
| A.5.18 | Access rights | Access rights management, JML, reviews | H |
| A.5.19 | Information security in supplier relationships | Supplier security principles | H |
| A.5.20 | Addressing information security within supplier agreements | Security clauses in contracts | H |
| A.5.21 | Managing information security in the ICT supply chain | ICT supply chain risks | M |
| A.5.22 | Monitoring, review and change management of supplier services | Supplier services monitoring | M |
| **A.5.23** | **Information security for use of cloud services** (added in 2022) | Security across cloud service lifecycle | H |
| A.5.24 | Information security incident management planning and preparation | Incident preparation | H |
| A.5.25 | Assessment and decision on information security events | Event assessment | M |
| A.5.26 | Response to information security incidents | Incident response | H |
| A.5.27 | Learning from information security incidents | Lessons learned | M |
| A.5.28 | Collection of evidence | Evidence gathering | M |
| A.5.29 | Information security during disruption | Security during business disruption | H |
| **A.5.30** | **ICT readiness for business continuity** (added in 2022) | ICT continuity readiness | H |
| A.5.31 | Legal, statutory, regulatory and contractual requirements | Legal compliance | H |
| A.5.32 | Intellectual property rights | IP protection | M |
| A.5.33 | Protection of records | Record protection | M |
| A.5.34 | Privacy and protection of PII | Privacy and PII protection | H |
| A.5.35 | Independent review of information security | Independent security review | M |
| A.5.36 | Compliance with policies, rules and standards | Policy compliance check | M |
| A.5.37 | Documented operating procedures | Documented SOPs | M |

### A.6 People controls (8)

| Control | Name | Essence | Risk |
|---|---|---|---|
| A.6.1 | Screening | Candidate vetting | M |
| A.6.2 | Terms and conditions of employment | Security clauses in employment contracts | H |
| A.6.3 | Information security awareness, education and training | Awareness and training | H |
| A.6.4 | Disciplinary process | Disciplinary process for violations | M |
| A.6.5 | Responsibilities after termination or change of employment | Post-termination duties | M |
| A.6.6 | Confidentiality or non-disclosure agreements | NDAs with staff and third parties | M |
| A.6.7 | Remote working | Remote work security | H |
| A.6.8 | Information security event reporting | Incident reporting channels | H |

### A.7 Physical controls (14)

| Control | Name | Essence | Risk |
|---|---|---|---|
| A.7.1 | Physical security perimeters | Physical perimeters | M |
| A.7.2 | Physical entry | Physical access control | M |
| A.7.3 | Securing offices, rooms and facilities | Premises protection | M |
| **A.7.4** | **Physical security monitoring** (added in 2022) | Secured zones monitoring | M |
| A.7.5 | Protecting against physical and environmental threats | Environmental threats protection | M |
| A.7.6 | Working in secure areas | Rules for secure areas | M |
| A.7.7 | Clear desk and clear screen | Clear desk and screen lock policy | L |
| A.7.8 | Equipment siting and protection | Equipment placement and protection | M |
| A.7.9 | Security of assets off-premises | Off-site asset security | M |
| A.7.10 | Storage media | Media management | M |
| A.7.11 | Supporting utilities | Supporting utilities | M |
| A.7.12 | Cabling security | Cable network security | L |
| A.7.13 | Equipment maintenance | Equipment maintenance | L |
| A.7.14 | Secure disposal or re-use of equipment | Secure disposal | M |

### A.8 Technological controls (34)

| Control | Name | Essence | Risk |
|---|---|---|---|
| A.8.1 | User end point devices | End point device security | H |
| A.8.2 | Privileged access rights | Privileged access management | H |
| A.8.3 | Information access restriction | Information access restriction | H |
| A.8.4 | Access to source code | Source code protection | M |
| A.8.5 | Secure authentication | Secure authentication methods | H |
| A.8.6 | Capacity management | Capacity management | M |
| A.8.7 | Protection against malware | Malware protection | H |
| A.8.8 | Management of technical vulnerabilities | Vulnerability management | H |
| **A.8.9** | **Configuration management** (added in 2022) | Configuration management | H |
| **A.8.10** | **Information deletion** (added in 2022) | Information deletion | H |
| **A.8.11** | **Data masking** (added in 2022) | Data masking | M |
| **A.8.12** | **Data leakage prevention** (added in 2022) | Leakage prevention | H |
| A.8.13 | Information backup | Backup | H |
| A.8.14 | Redundancy of information processing facilities | Infrastructure redundancy | M |
| A.8.15 | Logging | Logging | H |
| **A.8.16** | **Monitoring activities** (added in 2022) | Activity monitoring | H |
| A.8.17 | Clock synchronisation | Clock sync | L |
| A.8.18 | Use of privileged utility programs | System utilities control | M |
| A.8.19 | Installation of software on operational systems | Software installation on prod | M |
| A.8.20 | Networks security | Network security | H |
| A.8.21 | Security of network services | Network services security | M |
| A.8.22 | Segregation of networks | Network segmentation | M |
| **A.8.23** | **Web filtering** (added in 2022) | Web filtering | M |
| A.8.24 | Use of cryptography | Cryptography use | H |
| A.8.25 | Secure development life cycle | Secure SDLC | H |
| A.8.26 | Application security requirements | Application security requirements | M |
| A.8.27 | Secure system architecture and engineering principles | Secure architecture principles | M |
| **A.8.28** | **Secure coding** (added in 2022) | Secure coding | H |
| A.8.29 | Security testing in development and acceptance | Security testing | H |
| A.8.30 | Outsourced development | Outsourced development management | M |
| A.8.31 | Separation of development, test and production environments | Environment separation | M |
| A.8.32 | Change management | Change management | H |
| A.8.33 | Test information | Test data protection | M |
| A.8.34 | Protection of information systems during audit testing | Systems protection during audits | L |

---

## What auditors actually check at Stage 2

The 20 items reviewed most closely:

1. Clause 6.1.2 – Risk Assessment.
2. Clause 6.1.3 plus SoA.
3. Clause 9.2 – Internal audit.
4. Clause 9.3 – Management review.
5. Clause 6.2 – Information security objectives.
6. A.5.9 Asset inventory.
7. A.5.18 Access rights.
8. A.5.19–A.5.23 Supplier security.
9. A.5.24–A.5.27 Incident management.
10. A.6.3 Awareness training.
11. A.8.2 Privileged access rights.
12. A.8.5 Secure authentication.
13. A.8.8 Vulnerability management.
14. A.8.13 Backup.
15. A.8.15 plus A.8.16 Logging plus Monitoring.
16. A.8.24 Cryptography.
17. A.8.28 Secure coding (for developers).
18. A.8.32 Change management.
19. A.5.30 ICT readiness.
20. A.5.34 Privacy and protection of PII.

---

## Typical major nonconformities

A major NC is a serious nonconformity that **blocks certificate issuance** or suspends it. The 10 most common ones auditors report:

1. Risk assessment missing or applied inconsistently (clause 6.1.2).
2. Risk treatment plan not implemented, no link to SoA (clause 6.1.3).
3. SoA incomplete or inaccurate (clause 6.1.3(d)).
4. Internal audit not done, or done by a non-independent auditor (clause 9.2).
5. Management review skipped or missing mandatory inputs/outputs (clause 9.3).
6. Security objectives aren't measurable or aren't monitored (clause 6.2).
7. Incident management never exercised – no evidence of real incidents or lessons learned (A.5.24–A.5.27).
8. Periodic access reviews not done, or done as a formality (A.5.18, A.8.2).
9. Supplier security not managed (A.5.19–A.5.23).
10. BCM / ICT readiness not tested (A.5.29, A.5.30).

## Typical minor nonconformities

A minor NC doesn't block certification but requires correction:

1. Incomplete asset inventory (A.5.9, A.8.1).
2. Gaps in training records (A.6.3).
3. Password policy not applied to all systems (A.5.17, A.8.5).
4. Inconsistent supplier due diligence (A.5.19).
5. Visitor logs and physical controls are partial (A.7.2, A.7.6).
6. Weak removable media policy (A.7.10).
7. ISMS documents lacking version, owner, review date (clause 7.5).
8. No test restore records for backups (A.8.13).
9. Gaps in cryptographic key management (A.8.24).
10. Walkthrough catches clear desk violations (A.7.7).

---

## When minor becomes major

Three scenarios:

1. **Complete absence.** A requirement isn't met at all (e.g., management review has never been conducted).
2. **Process failure.** Backup is documented as "daily" but actually runs a couple of times a month at random.
3. **Unclosed minor from the previous audit.** A minor from the previous surveillance audit automatically escalates to major.

---

## Related material

- [checklist.md](checklist.md) – working readiness checklist per theme.
- [implementation-guide.md](implementation-guide.md) – implementation phases in detail.
- [glossary.md](glossary.md) – ISMS terminology.

---

## Need help

Preparing for Stage 2 or working through the SoA? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll walk through your case. Chat opens with a pre-filled message. First call is on us.

Website: [iso-cert.kz](https://iso-cert.kz) · Self-paced course: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/)
