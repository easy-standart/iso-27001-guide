# ISO/IEC 27001 and regulation: what one certificate actually covers

> A map of how the standard maps to laws and regulations in the EU, UK, UAE, Türkiye and Kazakhstan – and where the certificate leaves gaps that need extra steps.

One of the most common questions from a CEO: "If we get certified to ISO 27001, are we automatically compliant with GDPR? Or NIS2? Or our local data protection law?"

Short answer: no, not automatically. The certificate covers a significant share – sometimes 60–70% of the requirements. But no regulator waives specific obligations just because you hold the certificate.

This file is a detailed breakdown for companies in Kazakhstan expanding into international markets.

*Русская версия: [../comparison-regulations.md](../comparison-regulations.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## European Union

### GDPR – General Data Protection Regulation (2016/679)

**What it requires for information security.** Article 32 of GDPR requires "a level of security appropriate to the risk" – specifically pseudonymisation and encryption, ongoing confidentiality, integrity, availability and resilience of processing systems, recovery after an incident, and regular testing of how well those measures work.

**What ISO 27001 covers.** GDPR doesn't directly require ISO 27001, but the standard delivers a ready-made set of technical and organisational measures for Article 32. Regulators accept a 27001 certificate combined with 27701 as evidence that the controller has implemented appropriate technical and organisational measures under Article 32.

**What it doesn't cover.** The legal side of GDPR – lawful basis for processing, data subject rights (access, deletion, portability), DPIAs for high-risk scenarios, 72-hour breach notification, DPO, processor contracts. All of that sits with ISO/IEC 27701 (PIMS), which has a direct mapping to GDPR articles in Annex D.

More details: [full text of GDPR Article 32](https://gdpr-info.eu/art-32-gdpr/) and [the official GDPR page on EUR-Lex](https://eur-lex.europa.eu/eli/reg/2016/679/oj).

### NIS2 – Network and Information Security Directive (EU 2022/2555)

**What it regulates.** Cybersecurity for operators of essential and important services in the EU – energy, transport, banking, healthcare, digital infrastructure, ICT service providers, digital providers. Member state transposition deadline was 17 October 2024.

**What ISO 27001 covers.** [Commission Implementing Regulation (EU) 2024/2690](https://eur-lex.europa.eu/eli/reg_impl/2024/2690/oj/eng) is an Implementing Regulation that applies **directly** (no national transposition) to a specific subset of NIS2 entities: DNS providers, TLD registries, cloud/data-centre providers, CDNs, MSPs/MSSPs, online marketplaces, search engines, social networks, trust service providers. It expands Article 21 of NIS2 into more than 150 specific controls. Other NIS2 sectors follow national transpositions. ENISA published [Technical Implementation Guidance v1.0](https://www.enisa.europa.eu/sites/default/files/2025-06/ENISA_Technical_implementation_guidance_on_cybersecurity_risk_management_measures_version_1.0.pdf) in June 2025 mapping the requirements of 2024/2690 to ISO/IEC 27001:2022, ISO/IEC 27002:2022 and NIST CSF 2.0. The Excel mapping table was updated to v1.2 in September 2025.

**What it doesn't cover.** Art. 23 CSIRT notification obligations – early warning within **24 hours**, full notification within **72 hours**, **final report within 1 month** of notification (intermediate report if the incident is still ongoing). Registration in the national register. Personal accountability of executives. Specific measures from Regulation 2024/2690 across 13 control groups.

ENISA itself notes that the mapping **"should not be interpreted as a measure of equivalence."** It's a working reference, not an equals sign.

### DORA – Digital Operational Resilience Act (EU 2022/2554)

**What it regulates.** Digital operational resilience for the EU financial sector – banks, insurers, investment firms, payment providers and their critical ICT providers. Applies from **17 January 2025**.

**The five pillars of DORA:**

1. ICT risk management.
2. ICT-related incident management, classification and reporting.
3. Digital operational resilience testing, including TLPT (threat-led penetration testing).
4. ICT third-party risk management.
5. Information and intelligence sharing.

**What ISO 27001 covers.** Around 60–70% of DORA's management-side requirements and Annex A controls (industry rule of thumb, not an ENISA-blessed figure). DORA Article 28 requires financial entities to manage risk from ICT third parties and to contract only with providers meeting appropriate information security standards. In practice, a 27001 certificate (often with 27017 added for cloud providers) is the minimum signal – DORA doesn't mandate ISO certification per se, but partner banks and procurement teams increasingly treat it as required.

**What it doesn't cover.**
- **Mandatory TLPT** for large financial institutions (at least every 3 years) – RTS on TLPT.
- **Incident-reporting clock** (RTS (EU) 2025/301 + ITS (EU) 2025/302): initial notification **within the earlier of 4 hours after classifying the incident as major and 24 hours from becoming aware**; a **72-hour intermediate report** (with possible interim updates on request from the competent authority); and a **1-month final report** with root-cause analysis.
- **Register of information** on all ICT third-party arrangements (Art. 28(3); ITS (EU) 2024/2956 defines the xBRL-CSV templates) – entity-level record every financial entity must maintain, submitted annually to the competent authority.
- **Critical Third-Party Provider (CTPP) oversight** – the ESAs directly designate and supervise CTPPs under Chapter V, Section II. This is separate from the entity-level register above.
- **Provider diversification** requirements.

---

## United Kingdom

### UK GDPR plus Data Protection Act 2018

After Brexit, the UK kept its own version of GDPR – **UK GDPR** – paired with the [Data Protection Act 2018](https://www.legislation.gov.uk/ukpga/2018/12). Enforced by the [Information Commissioner's Office (ICO)](https://ico.org.uk/).

**What ISO 27001 covers.** The ICO explicitly points to ISO/IEC 27001 as a recognised route to demonstrate "appropriate technical and organisational measures" under Article 32 of UK GDPR.

**What it doesn't cover.** ICO registration and UK adequacy specifics for international data transfers.

### UK NIS Regulations

UK NIS is the national version of the European NIS Directive, covering critical service operators and digital service providers.

**What ISO 27001 covers.** The ICO explicitly lists ISO/IEC 27001 and ISO/IEC 22301 (BCM) as expected reference standards for NIS compliance. See [ICO – Security requirements](https://ico.org.uk/for-organisations/the-guide-to-nis/security-requirements/).

**What it doesn't cover.** Competent authority notification and sector-specific requirements (energy, water, transport).

### Cyber Essentials and Cyber Essentials Plus

The National Cyber Security Centre (NCSC), the UK's technical security agency, runs the **Cyber Essentials / Cyber Essentials Plus** certification scheme. Lighter than 27001, and often a prerequisite for UK government contracts.

The standard UK IT vendor package is "ISO 27001 plus Cyber Essentials Plus."

---

## United Arab Emirates

### UAE PDPL – Federal Decree-Law No. 45 of 2021

The first comprehensive federal data protection law in the UAE. Effective 2 January 2022; enforcement ramped up through 2024–2025.

**What ISO 27001 covers.** The law doesn't explicitly require certification but refers to "generally accepted security measures." Regulators recognize ISO 27001 plus 27701 as an accepted compliance framework.

**What it doesn't cover.** Specific consent requirements, DPO duties, UAE Data Office notification, and international transfer specifics.

### DIFC Data Protection Law

Dubai International Financial Centre – a Dubai financial free zone with its own jurisdiction. **DIFC Law No. 5 of 2020** has been in force since 1 July 2020 and is closely aligned with GDPR.

DIFC is a common choice of legal entity for CIS-based technology companies selling into the Gulf. ISO 27001 covers a significant share of DIFC DP obligations. Full compliance requires additional registration with the Commissioner of Data Protection in DIFC.

### NESA and SIA – Information Assurance Standards

**NESA IAS** (National Electronic Security Authority Information Assurance Standards) is a mandatory UAE framework for critical government and semi-private sectors. NESA was reorganized into **SIA** (Signals Intelligence Agency) in 2020; SIA now handles oversight and enforcement, while the NESA standards define the content.

11 domains with detailed technical controls, structurally based on ISO 27001, NIST and ISA/IEC 62443. An ISO 27001 ISMS covers 60–70% of NESA requirements. The remaining 30–40% is NESA-specific (national security priorities, SIA reporting).

---

## Türkiye

### KVKK – Law No. 6698 on Personal Data Protection

Adopted on 7 April 2016 – the first national Turkish law on personal data. Enforced by the Personal Data Protection Authority (KVKK) and the Data Protection Board.

**What ISO 27001 covers.** The law doesn't explicitly require ISO 27001, but the Board's resolutions recommend an ISMS approach for large data controllers. ISO 27001 plus 27701 covers a significant share of KVKK's technical requirements.

**What it doesn't cover.** The key difference between KVKK and GDPR is **mandatory registration of data controllers in VERBIS** (Data Controllers Registry Information System) before processing data on Turkish citizens. Registration is free but mandatory, and done through the KVKK website.

---

## Kazakhstan

### Law of the Republic of Kazakhstan No. 94-V "On Personal Data and Their Protection" (21 May 2013)

Current edition as of 18.01.2026.

**Key localisation requirement.** Databases containing personal data on Kazakhstani citizens must be located **on Kazakhstan territory**. This is a requirement on the physical placement of servers, not on the jurisdiction of the operator. Foreign companies processing Kazakhstani citizens' data are obliged to comply.

**What ISO 27001 covers.** An ISMS framework for technical and organisational measures.

**What it doesn't cover.** Localization. Consent specifics. Cryptography requirements under СТ РК (ST RK – Kazakhstani national standard).

### СТ РК ISO/IEC 27001-2023

Current national edition, equivalent to the international 2022 edition. Certification is done through bodies accredited by NCA RK. Kazakhstan hosts both local bodies and major international CBs (TÜV SÜD, Bureau Veritas, SGS, DNV, TÜV Thüringen), with offices in Almaty and Astana.

---

## Summary table: what regulation requires beyond ISO 27001

The 27001 certificate is a strong foundation. But no regulator waives specific obligations because of it.

| Regulation | What it requires beyond ISO 27001 |
|---|---|
| GDPR | Lawful basis for processing, data subject rights, DPIA, DPO, 72-hour breach notification, processor contracts. Covered by ISO 27701 |
| NIS2 (EU) | Three-stage CSIRT notification (24h early warning / 72h full notification / 1 month final report), national register registration, personal executive accountability |
| DORA (EU) | TLPT for large financial institutions, register of critical ICT providers, ESA inspection rights |
| UK GDPR + DPA 2018 | ICO registration and engagement, UK adequacy for international transfers |
| UK NIS Regulations | Competent authority notification, sector-specific requirements |
| UAE PDPL | Consent, DPO, UAE Data Office notification, transfer specifics |
| DIFC DPL | Registration with Commissioner of Data Protection, accountability, adequacy lists |
| NESA and SIA (UAE) | Mandatory for critical sectors, SIA reporting, specific controls across 11 domains |
| KVKK (Türkiye) | Mandatory VERBIS registration, consent specifics, cross-border transfer restrictions |
| Law of Kazakhstan 94-V | PD localisation on servers in Kazakhstan, СТ РК cryptography requirements |

---

## What ISO 27001 delivers beyond any regulation

The standard adds a **management layer** – the kind of thing regulations don't usually describe as a process:

- A management system with leadership, objectives, metrics and management review.
- Systematic risk management via ISO 27005.
- 93 Annex A controls as a single catalog for risk → control → evidence traceability.
- A continual improvement cycle (PDCA).
- External proof of maturity (the certificate) for B2B tenders and customer due diligence.

---

## Strategy for businesses from Kazakhstan with export plans

If you're building from Kazakhstan with EU, UK, UAE or Türkiye in sight, the typical sequence:

1. **Implement an ISMS to ISO/IEC 27001:2022.** A baseline framework recognised by all the regulators above.
2. **Extend scope with ISO/IEC 27701.** This covers privacy requirements from GDPR, UK GDPR, UAE PDPL, DIFC DPL, KVKK and Kazakh law.
3. **Adapt cryptography to the home market.** СТ РК for Kazakhstan – without this, 27001 stalls in the local jurisdiction.
4. **Fold regulator timelines into the incident management playbook.** GDPR/UK GDPR 72 hours, NIS2 three-stage clock (24h / 72h / 1 month), DORA (4h / 72h / 1 month) – in one document with a clear escalation path.
5. **For your target export market, add local-specific requirements.** UAE – NESA plus localisation in DIFC. Türkiye – VERBIS registration. UK – Cyber Essentials Plus as a pre-tender requirement.
6. **Line up supplier security to what NIS2 and DORA buyers expect.** Their checklists are becoming the standard for B2B export into the EU.

---

## What to read next

- [ceo-brief.md](ceo-brief.md) – if you want to understand how this all turns into money.
- [implementation-guide.md](implementation-guide.md) – implementation phases.
- [verticals.md](verticals.md) – sector-specific angles.
- [annex-a-guide.md](annex-a-guide.md) – detailed walkthrough of the 93 controls.

---

## Need help

Getting ready to enter the EU, UK, UAE or Türkiye and want to bundle compliance into one package? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll walk through your regulatory map. Chat opens with a pre-filled message. First call is on us.

Website: [iso-cert.kz](https://iso-cert.kz) · Self-paced course: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/)
