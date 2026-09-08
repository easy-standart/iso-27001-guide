# FAQ on ISO/IEC 27001

> Answers to the questions executives ask most often. If yours isn't covered here, open an Issue and we'll add it.

*Русская версия: [../faq.md](../faq.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## Is ISO 27001 a law or a voluntary standard?

ISO 27001 is a voluntary international standard. No government forces you to get certified. But enterprise buyers and regulators effectively make the certificate mandatory – without it you don't make tenders, or contracts come with extra requirements attached.

Belarus uses **СТБ ISO/IEC 27001**, Kazakhstan uses **СТ РК ISO/IEC 27001-2023**. Both national versions are identical to the international edition.

More detail in [structure.md](structure.md).

---

## What does certification actually cost?

No universal price list exists: company size, security maturity, scope width, geography and CB (Certification Body) choice push identical-looking businesses into a 3–5x range. See [ceo-brief.md](ceo-brief.md) for the 3-year cycle (Stage 1 + Stage 2, two surveillance audits, recertification) and what drives the budget.

---

## How long does it realistically take?

- From scratch, no security practice: 9–18 months.
- With existing security processes: 4–9 months.
- With a mature 27001:2013 (transition): 3–6 months. The transition window has closed; this scenario is effectively exhausted.

Phase breakdown and details in [implementation-guide.md](implementation-guide.md).

---

## Is a BelGISS certificate recognised abroad?

In most cases, yes. BelGISS registers certificates in **IAF CertSearch** – the international database. That gives international recognition through the IAF MLA system, provided BSCA's accreditation scope is signed under the MLA.

For tenders within the Eurasian Economic Union, most of Asia and CIS countries, a BelGISS certificate works out of the box. For major enterprise tenders in the US, EU or UK, buyers sometimes want a CB from their own jurisdiction – worth clarifying upfront.

More detail in [certified-companies.md](certified-companies.md).

---

## If we have a certificate, are we automatically GDPR-compliant?

No. The certificate covers 60–70% of GDPR requirements on the security side (Article 32, technical and organisational measures). But the legal side of GDPR – lawful basis for processing, data subject rights, DPIA, DPO, 72-hour breach notification – sits with **ISO/IEC 27701** (PIMS).

The typical solution is a package: 27001 plus 27701.

More detail in [comparison-regulations.md](comparison-regulations.md).

---

## What about NIS2 and DORA?

ISO 27001 covers 60–70% of NIS2 and DORA. Both add specifics that aren't in 27001:

- **NIS2** – three-stage CSIRT notification under Art. 23: 24 hours (early warning), 72 hours (full notification), 1 month (final report; intermediate report if the incident is still open). Registration in the national register. Personal accountability of executives.
- **DORA** – a tight incident-notification clock (initial report within the earlier of 4 hours after classifying an incident as major and 24 hours from becoming aware), TLPT testing, register of critical providers, ESA inspection rights.

ENISA published an official mapping of NIS2 requirements to ISO 27001 in June 2025 – a working reference for compliance teams.

More detail in [comparison-regulations.md](comparison-regulations.md).

---

## Where do we start if we've decided to implement?

Six steps, in this order:

1. Download the free **ISO/IEC 27000:2018** vocabulary standard: [iso.org/standard/73906.html](https://www.iso.org/standard/73906.html).
2. Read [structure.md](structure.md) and [glossary.md](glossary.md) to get the team on the same page.
3. Read [implementation-guide.md](implementation-guide.md) – implementation phases.
4. Run a gap analysis. It gives you a clear picture of where you stand.
5. Build the team internally. Minimum: one FTE leading the project.
6. Decide on consulting. Without an experienced CISO, going it alone takes 2–3x longer.

---

## Can we implement the ISMS on our own?

Yes, if:

- You have an experienced CISO or Head of Compliance on staff.
- The company is small (up to 100 FTE).
- Your security practice is already at a basic level.

If any of those is missing, an external consultant or fractional expert typically saves 6–12 months and 20–40% of the total project cost. A cheaper alternative to consulting is our [self-paced ISO/IEC 27001 course](https://iso-cert.kz/course-27001/).

---

## Narrow or wide scope to start?

Narrow. It's a universal rule everyone in the field agrees on.

Narrow scope (one product, one business unit) gives you:

- Initial costs 2–3x lower.
- Time-to-certification of 4–8 months instead of 12–18.
- Early commercial payoff – the certificate is usable in sales in year 1.
- A chance to learn at small scale.

Expand later through a scope change at the next surveillance audit.

The mistake that sinks projects: trying to cover the whole company on the first attempt. The team drowns in volume, the project stretches to 18–24 months, and often never reaches Stage 2.

---

## How does the certificate connect to insurance?

Cyber liability insurance is a separate market. Premiums depend on the company's risk profile. ISO 27001 certification cuts the standard premium by 15–25%. Some insurers **refuse coverage** without it.

Over the 3-year certification cycle, insurance savings alone often cover a large portion of the certification project cost.

More detail in [ceo-brief.md](ceo-brief.md).

---

## What do we do if Stage 2 finds a major NC?

Don't panic. A major NC isn't a verdict – it's a formal mechanism.

The CB gives you time to close it (usually 30–90 days). You submit a corrective action plan, implement it and report the evidence. After the CB verifies, the certificate is issued.

The key is to treat this as feedback, not a catastrophe. The best 27001 teams are the ones who went through several major NCs and learned from them.

What you should definitely NOT do: argue with the auditor or hide evidence. That breaks trust and turns "fixable" into "hopeless."

---

## How often is recertification needed?

The certificate is valid for 3 years. Within the cycle:

- Year 1: Stage 1 + Stage 2 (the certification audit itself).
- Year 2: surveillance audit.
- Year 3: surveillance audit.
- End of year 3: recertification audit.

After recertification, the cycle restarts.

It's not "one big audit every three years" – it's an ongoing process with annual checkpoints.

---

## Can we certify against 27001 + 27017 + 27018 + 27701 all at once?

Yes. For cloud providers and SaaS companies this is standard practice. Effectively it's one larger audit with extended scope, done by an accredited CB in one go.

But if you're just starting out, our advice is to close 27001 first and add extensions after. It reduces project risk and simplifies the first audit.

---

## What about SOC 2?

SOC 2 is a competing standard developed in the US. Mostly used by cloud and SaaS companies selling into the US market.

Comparison:

| Parameter | ISO 27001 | SOC 2 |
|---|---|---|
| Recognition | Global | Mostly US |
| Length of certification | 6–12 months | 3–9 months (Type 1 faster; Type 2 is 6–12 months) |
| Cost | Comparable | Comparable, sometimes cheaper |
| What's issued | Certificate | Report (Type 1 or Type 2) |
| Best fit | B2B service with global reach | B2B service focused on the US |

Many companies do both – ISO 27001 for global and European clients, SOC 2 Type 2 for US clients.

---

## Where can we get help?

Full certification cycle – from gap analysis to passing Stage 2. Text us with your specific case.

- [Telegram](https://t.me/m/8NsOXRkMZmQy) – chat opens with a pre-filled message.
- Self-paced ISO/IEC 27001 course, if you'd rather work through it yourself: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/).

---

## Didn't find your question?

Open an Issue in the repository and we'll add it to the FAQ. Your questions help us make this material more useful.
