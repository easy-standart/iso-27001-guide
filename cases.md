# Public ISO/IEC 27001 certification cases

> Who's actually certified, what they did, how they used the certificate in sales and compliance.

This file is for those who want to see specific examples, not theory. All cases come from open sources: corporate compliance pages, press releases, certification body reports.

*Русская версия: [../cases.md](../cases.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## How many certificates exist worldwide

Per **ISO Survey 2024** (published in 2025 – latest available edition):

- About **96,700 valid ISO/IEC 27001 certificates** (around 179,900 certified sites).
- Nearly two-fold growth vs. 2023 – partly explained by a complete methodology change (see below), but the underlying trend is consistent.
- Growth since 2006 – from around 6,000 to ~96,700. Sixteenfold over 18 years.
- Leading sectors: IT – **almost 20%** of all certificates, banking and finance, telecom, professional services.

Methodology shift. From the 2024 edition, ISO sources data directly from [IAF CertSearch](https://www.iafcertsearch.org/) – the global database of accredited certificates. Accuracy improved substantially, but direct comparison with pre-2023 numbers is misleading because the underlying source has changed.

Top countries: China now leads (~33,400 certificates, partly a result of improved data collection from CNAS). Japan, UK, India, Italy, Germany, US, Netherlands, Spain, Israel remain stable year over year.

Source: [ISO Survey of Certifications](https://www.iso.org/the-iso-survey.html).

---

## Case 1. Amazon Web Services (AWS)

### What's in place

AWS holds a valid **ISO/IEC 27001:2022** certificate issued by **EY CertifyPoint** (accredited by the Dutch Accreditation Council, IAF member).

AWS's full compliance pack includes:

- ISO/IEC 27001:2022 – ISMS.
- ISO/IEC 27017:2015 – cloud services.
- ISO/IEC 27018:2019 – PII in public clouds.
- ISO/IEC 27701:2019 – PIMS.
- ISO/IEC 22301:2019 – Business Continuity.
- ISO/IEC 20000-1:2018 – IT Service Management.
- ISO/IEC 9001:2015 – Quality.
- CSA STAR CCM v4.0.

### Scope

Covers a defined list of AWS services and data centres across specified regions. The full scope is published and updated at each recertification.

### What this means for your business

Using AWS as infrastructure provider lets you reference the AWS certificate as evidence under control **A.5.23** (cloud security). But only in the shared-responsibility "of the cloud" side – the infrastructure layer. Security "in the cloud" – configurations, data, access – stays with you and is certified separately.

Sources:

- [AWS ISO Certified](https://aws.amazon.com/compliance/iso-certified/) – official page with certificate list and scope.
- [AWS ISO/IEC 27001:2022 FAQ](https://aws.amazon.com/compliance/iso-27001-faqs/).

---

## Case 2. Microsoft Azure and Microsoft 365

### What's in place

Microsoft holds ISO/IEC 27001 certification across its cloud infrastructure: Azure, Microsoft 365 and other enterprise services.

Reports and certificates are available through the Microsoft Service Trust Portal.

### What this means for your business

Similar to AWS – if your stack is on Azure or Microsoft 365, you can reference Microsoft's certificate during your own audit prep against A.5.23. This shortens evidence collection on the infrastructure side.

An extra benefit – the Microsoft SSPA (Supplier Security and Privacy Assurance) program. To join Microsoft's supplier base, ISO 27001 is a hard requirement.

Source: [Cloudanix – ISO 27001 for AWS / Azure / GCP](https://www.cloudanix.com/blog/introduction-iso-27001-if-you-use-aws-azure-gcp-cloud).

---

## Case 3. Google Cloud Platform

### What's in place

The ISMS for Google Cloud Services is ISO/IEC 27001 certified after audit by an independent third party. In parallel, Google holds SSAE 18 / SOC 2, ISO 27017, ISO 27018, PCI DSS, FedRAMP, HIPAA.

### Scope

Covers Google Cloud, Google Workspace, Apigee. Certificates available via Compliance Reports Manager.

Sources:

- [Google Cloud – ISO/IEC 27001 Compliance](https://cloud.google.com/security/compliance/iso-27001).
- [Google Cloud – Compliance offerings](https://cloud.google.com/security/compliance/offerings).

---

## Case 4. SAP (Germany)

### What's in place

SAP – the largest European enterprise software vendor – is ISO/IEC 27001-certified for SAP Cloud products (S/4HANA Cloud, SuccessFactors, Ariba and others).

### What's interesting

SAP consistently shows the 27001 + 27017 (cloud) + 27018 (PII) + 22301 (BCM) + 27701 (PIMS) bundle – the classic enterprise pack of a European vendor. Reports and certificates are available through SAP Trust Center.

Source: [SAP Trust Center](https://www.sap.com/about/trust-center.html).

---

## Case 5. Klarna (Sweden)

### What's in place

Klarna is one of the largest European fintech players in the BNPL (Buy Now Pay Later) space. It operates under DORA, GDPR and Swedish financial regulator Finansinspektionen.

### What's interesting

At Klarna, ISO 27001 is part of a compliance stack alongside PCI DSS Level 1. A textbook example of how fintechs stitch multiple frameworks into one evidence base.

---

## Case 6. Rakuten (Japan)

### What's in place

Rakuten is Japan's largest e-commerce and fintech conglomerate. Its subsidiaries (Rakuten Bank, Rakuten Card, Rakuten Mobile, Rakuten Cloud) are ISO/IEC 27001-certified.

### What's interesting

Japan consistently ranks in the top 3 countries by ISO 27001 certificate count worldwide. Rakuten follows the typical Japanese approach: certification not for the whole group, but per business unit – giving narrow, precise scopes and easier audits.

Source: [Rakuten Information Security](https://global.rakuten.com/corp/sustainability/security/).

---

## Case 7. Booking.com (Netherlands)

### What's in place

Booking Holdings – one of the largest global travel players, HQ in Amsterdam – is ISO/IEC 27001-certified for its core products.

### What's interesting

An example of a company that under GDPR pressure and enterprise B2B clients (corporate travel) has to demonstrate IS maturity. Its cloud infrastructure is hybrid (in-house + AWS), so the certificate covers more than just the SaaS layer.

---

## Case 8. Denmark's CPR register: 8.8 million records through one contractor (2026)

> Cases 1–7 show who is certified. This one is different: it is an incident, not a certificate. We include it because it shows step by step where the requirements of ISO/IEC 27001:2022 would have worked. The investigation is still going, and details may change.

### What happened

Denmark's central population register (CPR) holds names, addresses and personal ID numbers. Access is granted to 1,039 companies that need to verify customer data: banks, insurers, telecom operators, law firms. One of them was the IT company Pays ApS from Odense.

From 10 September 2026 a bulk extraction ran through its access. According to the Danish authorities, names, addresses and CPR numbers of about **8.8 million people** (including deceased and emigrated) were obtained, with more than **14 million** query attempts over roughly ten days. Access stayed open for 21 days and 17 hours in total.

The register itself was not hacked. No vulnerability in the system was used: every request was formally within the company's rights. There were simply far too many of them.

It was noticed on 2 October, and not by a security system. While invoicing for September, the register's side saw an unusually large bill for the contractor's queries. Access was closed, and on 5 October the ministry announced the leak.

### What is confirmed and what is not

**Confirmed** (authorities, the company, Danish media): the legitimate access of Pays ApS was misused; the volume of requests was out of proportion to its business; the leak was found through the bill. Pays confirmed to TV 2 that its access had been misused.

**Reported by Politiken**: at least three Pays profiles, including an administrator one, used the password "123456".

**Claimed by the hacker, not confirmed by the authorities**: entry via a leaked password of a former Pays employee; the bulk-query program was written by AI (two experts who saw the code agreed). It is not publicly established whether two-factor authentication was enabled on these accounts.

### Where the chain could have been broken

We do not claim that an ISO 27001 certificate would have prevented this attack. Below are the requirements that cover the scenarios described. Annex A of ISO/IEC 27001:2022 contains 93 controls.

| Step in the chain | Control |
|---|---|
| Weak or leaked password | **5.17** Authentication information, **8.5** Secure authentication |
| Access of a person who no longer works at the company | **5.18** Access rights, **6.5** Responsibilities after termination or change of employment |
| Administrator accounts | **8.2** Privileged access rights |
| A contractor with access to your data | **5.19** Information security in supplier relationships, **5.22** Monitoring, review and change management of supplier services |
| 14 million requests from a small company | **8.16** Monitoring activities (new in the 2022 edition) |

The login to the register was checked; the volume of requests was not. After the leak, the register's administration wrote to all 1,039 companies with new requirements: a person responsible for security, regular review of which employees have access, and a monthly count of CPR requests to spot abuse. For an organisation with a working ISMS this is a familiar list. In Denmark it appeared after the leak.

### What this means for your business

Three questions every company that gives contractors access to data can ask this week:

- How many external companies have access to our data, and does any of them see more than the work requires?
- What happens if a contractor makes fourteen million requests instead of a hundred? Will we notice ourselves, or from an invoice?
- Does the same apply to AI assistants and automations connected to client data? In practice they are the same contractor with a key: fast, round the clock, and with the same questions about ownership, logging and monitoring.

Sources:

- [TV 2 – live coverage of the leak](https://nyheder.tv2.dk/live/samfund/2026-10-05-uvedkommende-har-faaet-adgang-til-88-millioner-cpr-numre) (in Danish).
- [DR/Ritzau – 1,039 companies receive stricter security requirements](https://www.dr.dk/nyheder/politik/1039-virksomheder-har-faaet-indskaerpet-sikkerhed-efter-cpr-laek) (in Danish).
- [Søg og Hør, citing Politiken – at least three profiles used "123456"](https://www.seoghoer.dk/nyheder/nye-detaljer-om-cpr-laek-mindst-tre-profiler-brugte-123456-adgangskode) (in Danish).
- [TV 2 Fyn – artificial intelligence used in the leak](https://www.tv2fyn.dk/fyn/kunstig-intelligens-blev-brugt-i-omfattende-cpr-laek-e6a7e) (in Danish).
- [Copenhagen Post – "123456" password used in the CPR breach](https://cphpost.dk/2026-10-10/general/123456-password-used-in-massive-danish-cpr-data-breach/).
- [CSIS – analysis of the CPR breach](https://www.csis.com/csis-tech-blog/the-hub/cpr-breach-denmark).
- [WorkOS – third-party API access and the CPR breach](https://workos.com/blog/denmark-cpr-breach-third-party-api-access).

---

## Pattern across cases

All the certification examples above (cases 1–7) – from the three hyperscalers to European and Asian players – show the same pattern. If you're building a cloud, fintech, e-commerce or SaaS business and want to repeat the success – learn from them:

### Certification is never alone

Alongside 27001 come the extensions: 27017 (cloud), 27018 (PII in cloud), 27701 (PIMS). This is the global "cloud maturity" standard in 2026.

### The certification body is always international with IAF MLA on 27001

EY CertifyPoint, BSI, Schellman – specific names. It's not coincidence. Only a certificate from a CB accredited under IAF MLA for ISMS is recognised by enterprise buyers in the US, EU and UK.

### Public scope

The list of services and data centres is open, updated at recertification. It's part of the enterprise sale: "here's our scope, check that your service is in it".

### Self-service evidence access

Microsoft Service Trust Portal, Google Cloud Compliance Reports Manager, AWS Artifact. No need to email security@... and wait a week.

That's a marketing focus smaller companies often miss. A certificate that's hard to show loses to a certificate visible in 30 seconds.

---

## Real-world certification timelines

Per [Secureframe](https://secureframe.com/hub/iso-27001/certification-timeline) and [ISMS.online](https://www.isms.online/iso-27001/certification/how-long-does-certification-take/):

| Profile | Duration |
|---|---|
| From scratch, no security practice | 9–18 months |
| With existing security processes | 4–9 months |
| With mature ISO 27001:2013 (transition) | 3–6 months |

### Phase breakdown

| Phase | Duration | What happens |
|---|---|---|
| Gap analysis | 1–4 weeks | Comparing current state with standard requirements |
| Risk assessment + SoA | 4–8 weeks | Asset identification, risk, control selection, SoA approval |
| Control implementation | 8–16 weeks | Documentation, technical control rollout |
| Internal audit | 2–4 weeks | Preparation and execution |
| Management review | 1–2 weeks | Formal top management review |
| Stage 1 audit | 1–2 days | Documentation and Stage 2 readiness |
| Gap between Stage 1 and Stage 2 | 4–8 weeks | Closing Stage 1 findings |
| Stage 2 audit | 2–10 days | Depends on organisation size and scope |
| Certification decision | 4–8 weeks | After Stage 2 |

### Maintaining the certificate

- **Surveillance audit** – end of year 1 and year 2, usually 1–3 days.
- **Recertification audit** – end of year 3, usually scope close to Stage 2.

Full 3-year cycle: Stage 1 → Stage 2 → Surveillance 1 → Surveillance 2 → Recertification. After recertification the cycle restarts.

---

## Related material

- [certified-companies.md](certified-companies.md) – who's certified in Kazakhstan.
- [ceo-brief.md](ceo-brief.md) – cost and financial justification.
- [implementation-guide.md](implementation-guide.md) – implementation phases in detail.

---

## Need help

Want to discuss a case for your business? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll talk through what from the hyperscaler playbook actually applies to you. Chat opens with a pre-filled message. Free consultation, no obligation.

Website: [iso-cert.kz](https://iso-cert.kz) · Self-paced course: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/)
