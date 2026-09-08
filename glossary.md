# ISMS glossary

> A dictionary of core terms for the information security management system. So you can speak the same language as your consultant, auditor and partner – no interpretation required.

All definitions marked with † are taken from **ISO/IEC 27000:2018** – the official vocabulary standard for the series. It's the only document in the family ISO distributes for free. Download it if you haven't already: [iso.org/standard/73906.html](https://www.iso.org/standard/73906.html).

Other definitions follow the wording of the standards themselves: [ISO/IEC 27001:2022](https://www.iso.org/standard/27001) (ISMS requirements) and [ISO/IEC 27002:2022](https://www.iso.org/standard/75652.html) (descriptions of the 93 Annex A controls).

*Русская версия: [../glossary.md](../glossary.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## The basic triad

**Information security.** Preservation of confidentiality, integrity and availability of information.† The CIA triad on which the whole standard is built.

**Confidentiality.** Property that information is not made available or disclosed to unauthorised parties.†

**Integrity.** Property of accuracy and completeness – information has not been modified or destroyed without authorisation.†

**Availability.** Property of being accessible and usable upon demand by an authorised party.†

---

## The management system

**ISMS (Information Security Management System).** A systematic approach to managing sensitive company information. Covers people, processes and technology. It's not a single program or regulation – it's the whole system of how an organisation manages information security.

**Management system.** Set of interrelated elements of an organisation used to establish policies, objectives and processes to achieve those objectives.†

**Top management.** Person or group of people who direct and control the organisation at the highest level.† In practice – CEO, board of directors, or CEO plus CFO plus COO. The standard mentions them often: management review, policy approval, clause 5 commitments.

**Scope.** ISMS boundaries – which units, sites, data types and processes are covered. Mandatory under clause 4.3.

**Interested party.** Person or organisation that can affect the ISMS, be affected by it, or perceive itself to be affected by its decisions.† In practice – clients, regulators, shareholders, suppliers, employees.

---

## Risk management

**Asset.** Anything of value to the organisation. In an ISMS context – information, software, equipment, services, reputation.

**Threat.** Potential cause of an unwanted incident that may harm a system or organisation.†

**Vulnerability.** Weakness of an asset or control that can be exploited by a threat.†

**Risk.** Effect of uncertainty on objectives. In information security – a combination of the likelihood and the consequences of an unwanted event.

**Risk owner.** Person or entity with accountability and authority to manage a risk.† Not "the security team" – a specific named person. That precision matters – auditors ask by name.

**Risk assessment.** Process of identifying, analyzing and evaluating risk. One of the heaviest documents in the implementation project.

**Risk treatment.** Process of selecting and implementing measures to modify risk. Four options: avoid, modify, transfer, accept.

**Residual risk.** The level of risk remaining after treatment.† Accepted by top management with a signature and date.

**Control.** A measure that modifies risk.† Includes policies, procedures and technical means. In an ISMS, a control isn't "we put something in place" – it's a formal measure with an owner and evidence.

---

## Documentation and audit

**Statement of Applicability (SoA).** A document listing the applicable Annex A controls, justification for their inclusion or exclusion, and implementation status. Mandatory evidence under clause 6.1.3(d). No SoA, no certification.

**Documented information.** Information required to be controlled and maintained by an organisation, and the medium it lives on.† The new name for "documents and records." Can live in Confluence, Notion, on paper – what matters is version control, date, owner and review process.

**Audit.** Systematic, independent, documented process for obtaining audit evidence and evaluating it objectively.† Independence is critical. An auditor can't audit their own work.

**Management review.** Formal review of the ISMS by top management, with mandatory inputs and outputs under clause 9.3. Not "a meeting where they talked" – a record with specific decisions and top-management signatures.

---

## Nonconformities and improvements

**Nonconformity.** Non-fulfilment of a requirement.†

- **Major NC** – serious nonconformity that prevents the certificate from being issued (or suspends it if active).
- **Minor NC** – a single deviation that doesn't block certification but requires correction within set deadlines.
- A minor NC not closed by the next audit automatically escalates to a major.

**Corrective action.** Action to eliminate the cause of a detected nonconformity.† Not "we fixed the symptom" – "we found and removed the cause."

**Continual improvement.** Recurring activity to enhance performance.† Covered by clause 10 of the standard.

---

## Cloud and privacy (for the 27017, 27018 extensions and the 27701 standalone standard)

**PII (Personally Identifiable Information).** Any information relating to an identified or identifiable natural person. In Russian usage – "personal data."

**PII Controller.** Party that determines the purposes and means of processing personal data. GDPR calls this the "controller"; Kazakh law calls it the "operator."

**PII Processor.** Party processing personal data on behalf of the controller. Typical examples – cloud providers, outsourced development, marketing agencies.

**Cloud service customer / provider.** Parties to a cloud contract in the terminology of ISO/IEC 17788. Used in 27017 for the shared responsibility model.

**DPIA (Data Protection Impact Assessment).** Assessment of impact on personal data protection. Mandatory for high-risk processing under GDPR and equivalent local laws. In practice – a formal document describing the processing, risks and measures.

**DPO (Data Protection Officer).** A role responsible for personal data protection. Mandatory in certain cases under GDPR; recommended in any company doing mass processing of personal data.

---

## Audit and certification

**Stage 1 audit.** First stage of the certification audit. 1–2 days. Documentation and ISMS readiness review. Usually followed by 4–8 weeks to close findings.

**Stage 2 audit.** Second stage. 2–10 days. Operational audit – staff interviews, evidence checks in systems, walkthroughs of physical sites. The certification decision is made based on the outcome.

**Surveillance audit.** Interim audit. Conducted once a year during the 3-year cycle. Typically 1–3 days. Purpose: confirm the ISMS is maintained and evolving.

**Recertification audit.** Final audit of the cycle. Conducted at the end of year 3, comparable in scope to Stage 2. After it, the cycle restarts.

**Certification Body (CB).** The body that performs the audit. Only an accredited CB can issue a certificate recognised in the IAF system. Accreditation is granted by national accreditation bodies.

**IAF MLA (Multilateral Recognition Arrangement).** Agreement among national accreditation bodies on mutual recognition of certificates. A certificate issued by a CB in an MLA signatory country is recognised in other signatory countries. This is what "international recognition" means in practice.

---

## Regulation and market

**GDPR (General Data Protection Regulation, EU 2016/679).** The EU's core data protection law. In force since May 2018. Requires lawful basis for processing, data subject rights, 72-hour breach notification, DPIA for high-risk processing. Fines (Art. 83) are two-tier: up to **EUR 10M or 2%** of worldwide annual turnover (Art. 83(4), "less severe" infringements – e.g. controller/processor obligations under Arts. 8, 11, 25–39) and up to **EUR 20M or 4%** (Art. 83(5), "more severe" – processing principles, data subject rights, international transfers). Both tiers apply **whichever is higher**.

**NIS2 (Network and Information Security Directive 2, Directive EU 2022/2555).** EU directive on cybersecurity for essential and important entities. Transposition deadline 17 October 2024. Incident notification timeline (Art. 23): early warning within **24 hours** of becoming aware of a significant incident; full notification with initial assessment within **72 hours**; **final report within 1 month** of the incident notification. If the incident is still ongoing at the 1-month mark, an intermediate report is filed instead, and the final report follows once resolved. Plus intermediate updates on CSIRT/competent authority request. Separately – personal accountability of executives.

**DORA (Digital Operational Resilience Act, Regulation EU 2022/2554).** EU regulation on digital operational resilience for the financial sector. In force from 17 January 2025. Five pillars: ICT risk management, incident logging, resilience testing (including TLPT), ICT third-party risk management, information sharing.

**PCI DSS (Payment Card Industry Data Security Standard).** Industry standard for organisations that store, process or transmit payment card data. Current version 4.0.1. Mandatory by contract with acquirers and card schemes, not by law.

**HIPAA (Health Insurance Portability and Accountability Act).** US law protecting health information (PHI). Privacy Rule and Security Rule apply to covered entities (hospitals, insurers, clearinghouses) and their business associates.

**ISO 27001 vs SOC 2 Type II.** Both frameworks address information security. 27001 is an international certificate covering a management system; SOC 2 is a US report by an independent auditor against 5 Trust Service Criteria (security, availability, processing integrity, confidentiality, privacy). Many companies pursue both: 27001 for the EU and Asia, SOC 2 for the US.

**CTPP (Critical Third-Party Provider).** An ICT service provider critical to the stability of the EU financial sector. Designated and supervised directly by the ESAs under DORA Chapter V, Section II. The list of CTPPs is published separately.

**Register of information (DORA Art. 28(3)).** A mandatory register that every financial entity maintains for all ICT third-party arrangements. Separate from CTPP designations.

**CTI (Cyber Threat Intelligence).** Operational information about active threats, adversaries and tactics. Control A.5.7 in 27001:2022. Typically delivered through specialized services (Recorded Future, Mandiant, FS-ISAC for financial services).

**GRC tools (Governance, Risk, Compliance).** Software platforms automating evidence collection, risk register maintenance, control monitoring and audit preparation. Common options – Vanta, Drata, Sprinto, Secureframe, Hyperproof, TrustCloud. They save 40–60% of internal FTE hours but require an annual subscription from around USD 15,000.

**Microsoft SSPA (Supplier Security and Privacy Assurance).** Microsoft's supplier program – mandatory annual self-assessments and ISO 27001 attestation. Without SSPA, Microsoft contracts cannot be renewed.

**M&A (Mergers and Acquisitions).** Merger and acquisition deals. In due diligence, a buyer checks security maturity: an ISO 27001 certificate cuts security DD by 50–70% and reduces cyber risk in the valuation.

**FTE (Full-Time Equivalent).** Standard unit for headcount – 1 FTE = 1 full-time employee working a standard week. Used to size ISMS implementation effort ("2 FTEs for 6 months") and compare projects across companies of different sizes.

**CSIRT (Computer Security Incident Response Team).** The organisational unit that receives, triages and coordinates response to security incidents. Under NIS2, notifications go to a national CSIRT designated by each Member State.

**TLPT (Threat-Led Penetration Testing).** Intelligence-driven pen-testing simulating a real advanced adversary attacking a specific business function. Mandatory under DORA (RTS on TLPT) for large financial institutions at least every 3 years. Based on the TIBER-EU framework.

**PIMS (Privacy Information Management System).** The privacy management system defined by ISO/IEC 27701. From the 27701:2025 edition (published 14 October 2025), it's a standalone certifiable standard with its own management-system clauses 4–10, no longer an extension to 27001. Covers PII controller/processor obligations under GDPR-style regimes; official mapping to GDPR is in Annex D.

---

## What to read next

- [structure.md](structure.md) – if you haven't yet figured out which standard covers what.
- [annex-a-guide.md](annex-a-guide.md) – detailed walkthrough of the 93 Annex A controls.
- [implementation-guide.md](implementation-guide.md) – implementation phases tied back to this glossary.

Found a term in the repository that isn't here? Open an Issue. The glossary grows from real reader questions.

---

## Need help

Stuck on terminology or want help with your certification project? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy). Chat opens with a pre-filled message. First call is on us.

Website: [iso-cert.kz](https://iso-cert.kz) · Self-paced course: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/)
