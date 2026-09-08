# Who's certified to ISO/IEC 27001 – bodies, registers, verification

> A map of accredited certification bodies worldwide and how to verify a certificate. So you know where to go, whom to pick, and how to check what a counterparty shows you.

This file is a practical reference for choosing a certification body (CB) and verifying issued certificates. For the global picture and hyperscaler case studies, see [cases.md](cases.md).

*Русская версия: [../certified-companies.md](../certified-companies.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## How the recognition system works

An ISO/IEC 27001 certificate is only globally recognized if the certification body that issued it is accredited under the **IAF Multilateral Recognition Arrangement (MLA)** for the ISMS scheme. IAF (International Accreditation Forum) is the global body that connects national accreditation authorities.

Chain of trust:

```
IAF MLA (global)
   └─ National Accreditation Body (UKAS, ANAB, DAkkS, RvA, etc.)
        └─ Certification Body (BSI, DNV, EY, Schellman, TÜV, etc.)
             └─ Your certificate
```

If any link in this chain is broken, the certificate may not be accepted in international tenders.

Global CB registry: [IAF CertSearch](https://www.iafcertsearch.org/).

---

## Major international certification bodies

The most active CBs for ISO 27001 globally, all with IAF MLA recognition for ISMS:

| CB | Country of origin | Accredited by | Notes |
|---|---|---|---|
| [BSI Group](https://www.bsigroup.com/) | UK | UKAS | Original developer of the standard; premium positioning |
| [DNV](https://www.dnv.com/) | Norway | RvA | Strong in energy, maritime, industrial |
| [EY CertifyPoint](https://www.ey.com/en_gl/services/assurance/certify-point) | Netherlands | RvA | Certifier for AWS 27001:2022; recognised in tech |
| [Schellman](https://www.schellman.com/) | US | ANAB | Popular for SaaS and tech companies |
| [A-LIGN](https://www.a-lign.com/) | US | ANAB | Common for cloud and SaaS |
| [TÜV SÜD](https://www.tuvsud.com/) | Germany | DAkkS | Broad geographical presence |
| [TÜV Rheinland](https://www.tuv.com/) | Germany | DAkkS | Global network |
| [SGS](https://www.sgs.com/) | Switzerland | UKAS + others | The largest TIC (Testing, Inspection, Certification) company in the world |
| [Bureau Veritas](https://www.bureauveritas.com/) | France | UKAS + others | Multi-region reach |
| [DEKRA](https://www.dekra.com/en/home/) | Germany | DAkkS | Popular in automotive and manufacturing |
| [Intertek](https://www.intertek.com/) | UK | UKAS | Global network with SMB focus |
| [BSI Americas](https://www.bsigroup.com/en-US/) | US | ANAB | BSI's US arm |

---

## Regional presence

### European Union and UK

All the major CBs above operate directly. UK-registered businesses typically prefer UKAS-accredited CBs (BSI, LRQA, Intertek). EU businesses have wide choice depending on jurisdiction; DAkkS-accredited CBs (TÜV, DEKRA) are common in the DACH region.

### United States

ANAB-accredited CBs dominate: A-LIGN, Schellman, Coalfire, BSI Americas. For B2B tech and SaaS the go-to picks are Schellman and A-LIGN, both fluent in SOC 2 as well.

### UAE and the Gulf

BSI, DNV, Bureau Veritas, SGS and Intertek all have an established local presence. For DIFC-registered entities, prefer CBs with a recognized presence in the Middle East. NESA compliance is a separate track from 27001 – see [comparison-regulations.md](comparison-regulations.md).

### Asia-Pacific

JAS-ANZ (Japan/Australia), CNAS (China), NABCB (India) and MASA (Singapore) are the regional accreditation bodies with IAF MLA. Local CBs operate through them.

### CIS region

*If you're a company based in the CIS, see the [Russian version of this repo](../certified-companies.md) for detail. In short: local certification bodies (BelGISS in Belarus, NCA-accredited bodies in Kazakhstan) are usually accepted for regional tenders. For EU, UK or US contracts, buyers often require an accredited body from those jurisdictions instead.*

---

## How to pick a CB

Three angles to consider.

### Recognition scope

Where will the certificate be used? Buyers in Europe – go with a UKAS or DAkkS-accredited CB. Mostly US-based – ANAB-accredited. For multinationals, either works, but check that the specific CB's MLA scope covers ISMS (not just quality management).

### Industry expertise

For SaaS and cloud, Schellman, A-LIGN and EY CertifyPoint have deep tech expertise and often audit hyperscalers. For manufacturing and industrial, DNV, TÜV and DEKRA. For financial services, the Big Four (Deloitte, PwC, EY, KPMG) – useful if you want to combine with SOX or SOC 1 work.

### Price and speed

Big-name CBs (BSI, DNV) charge premium rates but their brand carries weight in tenders. Mid-tier CBs (Schellman, A-LIGN) are competitive and fast. Regional CBs are usually 30–50% cheaper.

---

## How to verify a third party's certificate

If a counterparty says "we have ISO 27001," ask for the certificate number and verify it yourself. Three steps:

**1. IAF CertSearch** – [iafcertsearch.org](https://www.iafcertsearch.org/). Enter the certificate number or company name to get status (active, suspended, withdrawn) and scope confirmation.

**2. National registry** – the accreditation body in the CB's country typically maintains a public registry (UKAS, ANAB, DAkkS, RvA, etc.).

**3. Direct query to the CB** – if the first two don't give you an answer, contact the certification body directly. Contact info is usually on the certificate itself.

**Red flags:**

- The certificate is "issued" by a CB that isn't in IAF or national accreditation registries.
- The scope on the certificate doesn't match what the company actually sells.
- Issue date is in the future, or more than 3 years ago with no recertification confirmation.
- The CB's accreditation covers quality (9001) or environment (14001), but not ISMS (27001).

---

## Global certificate statistics

Per the **ISO Survey 2024** (published in 2025 – latest available edition):

- **~96,700 valid ISO/IEC 27001 certificates** (about 179,900 certified sites) – nearly a two-fold jump vs. the 2023 figure.
- Growth from ~6,000 in 2006 – roughly sixteenfold over 18 years.
- Data is now compiled directly from [IAF CertSearch](https://www.iafcertsearch.org/) – with 76 of 77 national accreditation bodies and 2,400+ CBs contributing.
- Top country: China (~33,400 certificates). Then Japan, UK, India, Italy, Germany, US, Netherlands, Spain, Israel remain stable year over year.
- **~20% IT sector**, followed by finance, telecom and professional services.

More on the data in [cases.md](cases.md).

---

## Related material

- [cases.md](cases.md) – public corporate cases (AWS, Microsoft, Google).
- [ceo-brief.md](ceo-brief.md) – cost and financial justification.
- [implementation-guide.md](implementation-guide.md) – implementation phases.

---

## Need help

Picking a certification body for your case? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll advise based on your buyers, industry and budget. Chat opens with a pre-filled message. First call is on us.

Website: [iso-cert.kz](https://iso-cert.kz) · Self-paced course: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/)
