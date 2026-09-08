# ISO/IEC 27001 by industry

> Which Annex A controls matter most for your sector, which standards typically go alongside 27001, and what regulation lands on top. So you know what you're walking into before you start.

If you already know 27001 is required but aren't sure which extensions to add, this file is for you. If you're still choosing between "do it or not," start with [ceo-brief.md](ceo-brief.md).

> Codes like `A.5.7` or `A.8.24` below refer to controls in Annex A of ISO/IEC 27001:2022. What each control requires and what audit-ready evidence looks like – see [annex-a-guide.md](annex-a-guide.md).

*Русская версия: [../verticals.md](../verticals.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## FinTech and banking

### Around 27001

The financial sector is the most heavily regulated. Several layers usually stack on one business:

- **DORA** (EU 2022/2554) – effective from 17 January 2025. Requires a tight incident-notification clock (initial report within 4 hours of classifying an incident as major), robust supply chain controls, TLPT testing, register of critical providers.
- **PCI DSS 4.0.1** – mandatory for anyone storing, processing or transmitting cardholder data.
- **EBA / EIOPA Guidelines** – for banking and insurance in the EU.
- **Local regulators** – National Bank of Belarus, ARDFM of Kazakhstan, Bank of England PRA in the UK, Central Bank of the UAE.

### What ISO 27001 certification delivers

In finance, 27001 works as:

1. **Foundational framework** – management system, risk management, improvement cycle. DORA, PCI DSS and EBA Guidelines all stitch onto it.
2. **B2B signal** – without 27001 you can't enter the supply chains of major banks and payment systems.
3. **Regulatory confidence** – after an incident, the certificate serves as evidence of appropriate technical and organisational measures.

### Which controls matter most

- **A.5.7 Threat Intelligence** – mandatory for CTI programs. Integrates with FS-ISAC.
- **A.5.19–A.5.23 Supplier Security** – ICT third-party management, especially post-DORA.
- **A.5.24–A.5.27 Incident Management** – wraps the 4-hour DORA timeline.
- **A.5.30 ICT Readiness for BC** – mandatory TLPT testing for large financial institutions.
- **A.8.2 Privileged Access Rights** – a banking standard.
- **A.8.24 Cryptography** – PCI DSS requirements plus local cryptographic regulations.
- **A.8.28 Secure Coding** – mandatory for in-house development of financial services.

### Mapping to DORA and PCI DSS

ISO 27001 covers 60–70% of DORA on the management side and Annex A controls; around 50–60% of PCI DSS (especially sections 8, 10 and 12). The remaining 30–40% is concrete technical requirements specific to each framework: cardholder data environment segmentation for PCI DSS, TLPT for DORA, regulator reporting.

---

## Healthcare and medical devices

### Around 27001

For healthcare, the standard pairs with **ISO/IEC 27799:2025** – *Health informatics – Information security controls in health based on ISO/IEC 27002.* 27799 applies across the whole healthcare landscape: hospitals, clinics, labs, medical devices, telehealth, electronic health records.

For the US market, add **HIPAA** (Health Insurance Portability and Accountability Act). ISO 27001 contains at least 47 controls that support HIPAA requirements, but the certificate alone **doesn't mean HIPAA compliance**. HIPAA has privacy-related controls that aren't in 27001 – PHI access logs, Business Associate Agreements, Notice of Privacy Practices.

The standard pack for US healthcare SaaS is 27001 plus 27799 plus a HIPAA Privacy Rule mapping.

### Which controls matter most

- **A.5.34 Privacy and Protection of PII** – especially for protected health information (PHI).
- **A.5.14 Information Transfer** – transfer of medical data between organisations.
- **A.7.4 Physical Security Monitoring** – hospital premises with restricted areas.
- **A.8.10 Information Deletion** – ties into retention rules for medical records.
- **A.8.11 Data Masking** – for R&D and analytics on medical data.
- **A.5.18 Access Rights** – role-based access for different medical staff.

---

## IT, SaaS and Cloud Service Providers

### Around 27001

For cloud providers and SaaS companies, the working pattern is **27001 first, extensions later**: 27017 (cloud controls), 27018 (PII in the cloud), 27701 (services with heavy PII processing). Close the ISMS baseline with 27001, then add extensions at the next surveillance audit. That reduces project risk and simplifies the first audit (see FAQ on the 27001+27017+27018+27701 package).

- **ISO 27001** – the ISMS baseline. Always starts here.
- **ISO 27017** – 7 additional cloud-specific controls: shared responsibility, virtual asset management, automated auditability, dynamic policy enforcement.
- **ISO 27018** – 25 extended controls for CSPs processing PII: consent, choice, data minimization, retention, disclosure limitation.
- **ISO 27701** – an extension for PII controllers / PII processors, with GDPR mapping.

### What certification buys you

For SaaS companies, 27001 is:

- **A sales accelerator.** Enterprise buyers check the 27001 certificate at pre-qualification.
- **A pass to enterprise marketplaces.** Microsoft SSPA, AWS Marketplace and Google Cloud Marketplace require ISO certification as a condition.
- **A cyber insurance discount.** Premiums drop by 15–25%.

### Which controls matter most

- **A.5.23 Cloud Services** – added in 2022; shared responsibility model.
- **A.8.9 Configuration Management** – IaC, hardening baselines.
- **A.8.28 Secure Coding** – mandatory for development.
- **A.8.25–A.8.27 SDLC** – Secure Development Lifecycle.
- **A.8.31 Separation of Environments** – dev / test / prod isolation.
- **A.8.16 Monitoring Activities** – observability, SIEM, alerting.

---

## HR-tech, EdTech and PII-heavy services

### Around 27001

For HR-tech, EdTech, marketplace platforms and any services doing mass processing of individuals' personal data, the primary risks are subject privacy and cross-border transfer.

What becomes critical:

- **ISO 27701 (PIMS)** – effectively a mandatory extension to 27001.
- **GDPR, UK GDPR, Law of Belarus 99-Z, Law of Kazakhstan 94-V, KVKK, UAE PDPL** – data subject rights as daily operational work.
- **Data localization** – for Kazakhstan (Law 94-V), for certain EU regions, and for Türkiye.

### Which controls matter most

- **A.5.34 Privacy and Protection of PII.**
- **A.5.14 Information Transfer** – cross-border.
- **A.8.10 Information Deletion** – right to deletion.
- **A.8.11 Data Masking** – non-prod environments.
- **A.6.3 Awareness** – training on data subject rights.
- **A.5.31 Legal Requirements** – register of applicable privacy laws.

---

## Manufacturing, supply chain and e-commerce

### Around 27001

For manufacturing and e-commerce, the primary focus shifts to supply chain management and operational resilience. Complementary standards:

- **ISO/IEC 27036** (series) – for supplier relationships, including ICT supply chain (Part 3, 2023).
- **ISO/IEC 27040:2024** – storage security; critical for e-commerce with large data stores.
- **ISO 22301** – Business Continuity (often paired with 27001).
- **NIS2** – for essential and important operators in the EU.

### Which controls matter most

- **A.5.19–A.5.23 Supplier Security** – supplier and cloud management.
- **A.5.21 Managing Information Security in the ICT Supply Chain** – supply chain risks.
- **A.5.7 Threat Intelligence** – for proactive supply chain monitoring.
- **A.5.30 ICT Readiness for BC** – resilience to logistics and systems disruption.
- **A.7.4 Physical Security Monitoring** – warehouses.
- **A.8.13 Backup** – critical for e-commerce with large catalogs.

---

## Government and critical infrastructure

### Around 27001

For government and critical infrastructure operators (energy, transport, telecom, water) heavy regulation lands on top:

- **NIS2** in the EU.
- **NESA / SIA** in the UAE for critical sectors.
- **UK NIS Regulations** – UK competent authorities by sector.
- Local critical infrastructure laws in Belarus and Kazakhstan – details vary and need to be clarified organisation by organisation.

Complementary standards:

- **ISO/IEC 27019** – for the energy sector (ISMS in energy).
- **ISO/IEC 27011** – for telecom operators.
- **ISO/IEC 27033** (series) – network security.
- **ISA/IEC 62443** – operational technology (OT) and industrial control systems (ICS / SCADA).

### Which controls matter most

- **A.5.5 Contact with Authorities** – mandatory for regulator notifications.
- **A.5.24–A.5.27 Incident Management** – wraps short regulator timelines.
- **A.5.29 + A.5.30 Continuity** – mandatory BCM for critical services.
- **A.7.5 Protection against Physical/Environmental Threats** – for industrial sites.
- **A.8.15 + A.8.16 Logging + Monitoring** – mandatory SIEM framework.

---

## Cross-sector summary table

| Industry | Base pack | Complementary standards | Critical regulation |
|---|---|---|---|
| Banks and FinTech | 27001 | 27017 (if cloud), 22301 | DORA, PCI DSS, EBA Guidelines, local central bank rules |
| Insurance | 27001 | 22301 | DORA, EIOPA, local regulators |
| Healthcare | 27001 plus 27799 | 27701 | HIPAA (US), GDPR, NIS2 (medtech in EU) |
| IT, SaaS, Cloud | 27001 plus 27017 plus 27018 | 27701 | GDPR, NIS2 for cloud providers |
| HR-tech, EdTech | 27001 plus 27701 | – | GDPR, local privacy laws |
| E-commerce, Retail | 27001 | 27040, 22301 | GDPR, PCI DSS (if accepting cards) |
| Manufacturing, Supply Chain | 27001 | 27036, 22301 | NIS2 for critical sectors |
| Energy, Utilities | 27001 plus 27019 | ISA / IEC 62443 | NIS2, UK NIS, local critical infrastructure regulators |
| Telecom | 27001 plus 27011 | 27033 | NIS2, local telecom regulators |
| Government | 27001 | 27002 plus local requirements | Local critical infrastructure laws, NIS2 (if EU) |

---

## How to pick the package

Six steps, in this order:

1. **Base ISMS to 27001** – covers 50–70% of any sectoral regulation.
2. **Sectoral extension** – 27017 / 27018 for cloud, 27799 for healthcare, 27019 for energy, 27011 for telecom.
3. **Privacy extension** – 27701, if you're doing mass PII processing.
4. **BC extension** – 22301, if operational resilience is critical.
5. **Regulatory gap analysis** – identify requirements the ISO pack doesn't cover: notification timelines, sectoral reports, specific controls.
6. **Integrate into a single ISMS** – one document register, one evidence base. Use ISO 27002:2022 attributes (Operational Capabilities, Security Domains) for mapping.

---

## Related material

- [structure.md](structure.md) – what's inside each standard in the series.
- [comparison-regulations.md](comparison-regulations.md) – detailed breakdown of each regulation.
- [annex-a-guide.md](annex-a-guide.md) – walkthrough of each control.
- [ceo-brief.md](ceo-brief.md) – financial decision for the CEO.

---

## Need help

Want to talk through the right package for your industry? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll tell you which extensions your regulation actually needs. Chat opens with a pre-filled message. First call is on us.

Website: [iso-cert.kz](https://iso-cert.kz) · Self-paced course: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/)
