# The ISO/IEC 27000 family – structure

> A map of how the standards around ISO/IEC 27001 fit together. So you know which document does what.

ISO/IEC 27001 isn't a standalone standard. It comes with a family of more than two dozen documents that work as a single package. One is certifiable – 27001. The rest deepen, complement or adapt the requirements for specific contexts: cloud, privacy, incidents, suppliers, healthcare, energy.

If you're new to the topic, keep this file open. You'll see references to different standards throughout the repository, and this is where each one is explained.

*Русская версия: [../structure.md](../structure.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## Who develops the standards

All documents in the 27000 series are produced by the joint technical committee **ISO/IEC JTC 1/SC 27 "Information security, cybersecurity and privacy protection"** – a joint structure of two international organisations, ISO and IEC.

The committee is based in Geneva; ANSI (USA) holds the secretariat; the chair is Wael William Diab. By 2025 more than 35 published documents covered foundational concepts, governance, trustworthiness, data quality, lifecycle processes, conformity assessment and environmental sustainability.

Committee page: [committee.iso.org/jtc1sc27](https://committee.iso.org/jtc1sc27/).

---

## Key standards – briefly

### ISO/IEC 27000:2018 – vocabulary

The "language" standard for the series. Contains official definitions of every term used elsewhere. ISO/IEC 27001:2022 directly references 27000:2018 as the normative source of terminology – the entire ISMS vocabulary comes from here.

The key point: this document is **free**. You can download it from the ISO website at no cost. Every other standard in the family is paid.

It's used at project kick-off: the implementation team downloads 27000, and from that point on every term (asset, risk, control, ISMS, scope) is understood consistently.

Source: [iso.org/standard/73906.html](https://www.iso.org/standard/73906.html).

### ISO/IEC 27001:2022 – the main standard

The one you get certified against. Published 25 October 2022. Contains 11 clauses (0–10) – the first three are introductory; clauses 4–10 set mandatory requirements for the management system. Plus Annex A – a catalog of 93 reference controls.

In February 2024, **Amendment 1: Climate action changes** was issued – short but mandatory. Exact text: clause 4.1 now adds "The organization shall determine whether climate change is a relevant issue" – the organisation is required to **determine (assess) relevance** of climate change to its context, not automatically treat it as a context factor. Plus a NOTE 2 in clause 4.2: interested parties can have climate-related requirements.

The transition from the 2013 edition ended on 31 October 2025. The only currently valid edition is 2022.

Source: [iso.org/standard/27001](https://www.iso.org/standard/27001).

### ISO/IEC 27002:2022 – code of practice

The extended reference for all 93 controls. For each one it spells out objectives, application context, typical implementation measures and expected artefacts. You certify against 27001; 27002 is the working companion you need to actually apply Annex A – without it, working with the controls is guesswork.

If your budget for buying standards is limited, buy 27002 right after 27001.

Source: [iso.org/standard/75652.html](https://www.iso.org/standard/75652.html).

### ISO/IEC 27003 – implementation guidance

Detailed analysis of how to meet the clause requirements of 27001. Doesn't set new requirements – explains existing ones. Especially useful at project launch.

### ISO/IEC 27004 – measurement and metrics

Guidance on measuring ISMS effectiveness. Used when setting up the KPI system and preparing the management review (clause 9 of ISO 27001).

### ISO/IEC 27005:2022 – risk management

The most detailed document in the series on information security risk management. Adapts the general principles of ISO 31000:2018 to the ISMS context. Covers the full cycle: identification, assessment, treatment, communication, monitoring.

The implementation team leans on this when writing its Risk Assessment Methodology – a mandatory document under clause 6.1.2 of 27001.

Source: [iso.org/standard/80585.html](https://www.iso.org/standard/80585.html).

### ISO/IEC 27017:2015 – cloud services

Code of practice for information security in cloud environments. Extends 27002 controls with cloud-specific guidance. Central idea: shared responsibility between provider and customer.

If your business is a cloud provider or a large consumer of cloud services, 27017 is the standard extension to pair with 27001. A 2nd edition (FDIS 2026) is in the pipeline, aligned with 27002:2022 – you don't need to wait; the 2015 edition is still recognised.

Source: [iso.org/standard/82878.html](https://www.iso.org/standard/82878.html).

### ISO/IEC 27018:2025 – PII in public clouds

The current 2025 edition. Controls for protecting personally identifiable information in public clouds where the provider acts as a PII processor. Tied to ISO/IEC 29100 (privacy principles).

Used by large cloud providers handling PII on behalf of their customers. Source: [iso.org/standard/27018](https://www.iso.org/standard/27018).

### ISO/IEC 27701:2025 – Privacy Information Management System (PIMS)

New edition published on 14 October 2025. Key change: 27701 is now a **standalone certifiable standard**, not an extension to 27001. It carries its own management-system clauses 4–10, tailored to privacy. Official GDPR mapping is in Annex D. Coverage of cloud services, AI processing, IoT, biometrics and health data was expanded.

Existing 27701:2019 certificates need a transition audit within the migration period (typically 24–36 months). New projects should target 27701:2025 directly.

If your business processes personal data at scale, this is the core standard for GDPR-style compliance. Source: [iso.org/standard/85819.html](https://www.iso.org/standard/85819.html).

### ISO/IEC 27035 – incident management

A four-part series:

- Part 1:2023 – principles and process
- Part 2:2023 – planning and preparation
- Part 3 – ICT incident response operations
- Part 4:2024 – coordination

Supports controls A.5.24–A.5.27 (incident management) in 27001. Useful when you're building an incident response playbook.

### ISO/IEC 27036 – suppliers

A four-part series on information security in supplier relationships:

- Part 1:2021 – overview and concepts
- Part 2:2022 – requirements
- Part 3:2023 – supply chain guidance (hardware, software, services)
- Part 4:2016 – guidance for cloud services

Unpacks controls A.5.19–A.5.23 in 27001. Especially valuable given the supply-chain pressure from NIS2 and DORA.

### ISO/IEC 27040:2024 – storage security

Technical standard on protecting storage systems (DAS, NAS, SAN, object stores, cloud storage). Supports A.8.13 (backup), A.8.10 (information deletion), A.8.24 (cryptography) for the data lifecycle.

Source: [iso.org/standard/80194.html](https://www.iso.org/standard/80194.html).

### Other documents in the series

A quick look at documents that come up less often but may matter:

| Standard | Purpose |
|---|---|
| ISO/IEC 27006 | Requirements for ISMS certification bodies |
| ISO/IEC 27007 | Guidance on conducting ISMS audits |
| ISO/IEC 27008 | Guidance on auditing security controls |
| ISO/IEC 27011 | ISMS controls for telecom operators |
| ISO/IEC 27019 | ISMS controls for the energy sector |
| ISO/IEC 27031 | ICT readiness for business continuity |
| ISO/IEC 27032 | Cybersecurity and internet services guidance |
| ISO/IEC 27033 (series) | Network security |
| ISO/IEC 27034 (series) | Application security |
| ISO/IEC 27037 | Digital forensics |
| ISO/IEC 27050 | Electronic discovery |
| ISO/IEC 27110 | Guidance for cybersecurity frameworks (the mapping of 27002 to NIST CSF leans on this) |
| ISO 27799:2025 | ISMS controls for healthcare |

---

## National adaptations

### Kazakhstan

The valid edition is **СТ РК ISO/IEC 27001-2023**, equivalent to the international 2022 edition. Certification is done by bodies accredited by NCA RK (National Accreditation Centre).

Kazakhstan has kept a local presence of the major international certification bodies: TÜV SÜD, Bureau Veritas, SGS, DNV, TÜV Thüringen. That gives a direct path to an internationally recognised 27001 certificate without going through other jurisdictions.

---

## How the standards connect

A schema to see it at a glance:

```
                    ┌──────────────────────────────────────┐
                    │  ISO/IEC 27000:2018 – vocabulary     │
                    │  (free, terms for everyone)          │
                    └──────────────────┬───────────────────┘
                                       │ normative reference
                                       ▼
       ┌───────────────────────────────────────────────────────────┐
       │  ISO/IEC 27001:2022 + Amd 1:2024 – Requirements           │
       │  (the certifiable one)                                    │
       │  Clauses 4–10  +  Annex A (93 controls)                   │
       └───────┬───────────────────────────┬───────────────────────┘
               │                           │
               │ Annex A details           │ management part
               ▼                           ▼
   ┌─────────────────────────┐   ┌────────────────────────────┐
   │ ISO/IEC 27002:2022      │   │ ISO/IEC 27003 – Guidance   │
   │ – code of practice      │   │ ISO/IEC 27004 – Measurement│
   │ – 5 attributes, 4 themes│   │ ISO/IEC 27005:2022 – Risk  │
   └─────────────────────────┘   │ ISO/IEC 27007/27008 – Audit│
                                 └────────────────────────────┘
                                       │
                                       │ sectoral and contextual
                                       ▼
   ┌─────────────┬──────────────┬──────────────┬──────────────┐
   │ 27017 cloud │ 27018 PII    │ 27701 PIMS   │ 27035 incid. │
   │ 27036 supply│ 27040 storage│ 27011 telco  │ 27019 energy │
   │ 27033 net   │ 27034 app    │ 27037 forens.│ 27799 health │
   └─────────────┴──────────────┴──────────────┴──────────────┘
```

---

## Four practical rules

**First.** Certification goes through ISO 27001 only. Any "certification under ISO 27017" or "under ISO 27701" in practice means certification against 27001 with an extended scope into the relevant standard.

**Second.** ISO 27002 is the working companion for the 93 Annex A controls. It's not certifiable on its own, but without it, applying Annex A is guesswork. If you can only buy two standards, buy 27001 and 27002.

**Third.** Grab ISO 27000 for free – it's the only one in the series ISO distributes at no cost. Without the vocabulary, a conversation with an auditor won't go anywhere.

**Fourth.** Pick extensions by business context, not by fashion. Cloud SaaS – 27017 plus 27018 plus 27701. Telecom – 27011. ICT manufacturing – 27036 plus 27034. Storage – 27040.

---

## Next

If you've made sense of the family map, the next step is [glossary.md](glossary.md) – the vocabulary to share a common language with your auditor, consultant and partner.

If you want to go straight to action, head to [implementation-guide.md](implementation-guide.md). Phases from kick-off to certificate.

---

## Need help

Questions after reading, or want help with your certification project? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy). Chat opens with a pre-filled message. First call is on us.

Website: [iso-cert.kz](https://iso-cert.kz) · Self-paced course: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/)
