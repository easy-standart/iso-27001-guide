# Implementing an ISMS to ISO/IEC 27001:2022 – a step-by-step guide

> A hands-on reference for the process owner running the project. From kick-off to certificate.

This file is for the person who'll actually run the project. It's working material, not an academic overview. If you're a CEO who just wants the numbers and the decision, see [ceo-brief.md](ceo-brief.md). If you're the Head of Compliance or CISO launching the project – stay here.

*Русская версия: [../implementation-guide.md](../implementation-guide.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## How long it takes

Depends on the starting state:

- **From scratch, no security practice:** 9–18 months.
- **With existing security processes:** 4–9 months.
- **With a mature ISO 27001:2013 (transition):** 3–6 months. This scenario is now closed – the transition window ended on 31 October 2025, 2013-edition certificates are no longer valid.

Phase breakdown is in Part 2 of this file. Cost numbers are in [ceo-brief.md](ceo-brief.md) and [certified-companies.md](certified-companies.md).

---

## Part 1. The mandatory document set

ISO/IEC 27001:2022 requires about 20 items of "documented information" and "records" under clauses 4–10. That's the strict legal minimum.

### Mandatory documents

| Document | Clause | What it captures |
|---|---|---|
| ISMS Scope Statement | 4.3 | Boundaries of the management system |
| Information Security Policy | 5.2 | Strategic commitments of top management |
| Risk Assessment and Treatment Methodology | 6.1.2 | Rules for risk assessment and treatment |
| Statement of Applicability (SoA) | 6.1.3(d) | List of applicable Annex A controls with justifications |
| Risk Treatment Plan | 6.1.3(e), 6.2, 8.3 | Plan of actions for treating identified risks |
| Information Security Objectives | 6.2 | Measurable ISMS objectives |
| Risk Assessment and Treatment Report | 8.2, 8.3 | Outcomes of risk assessment and treatment |

### Mandatory records

| Record | Clause |
|---|---|
| Training and competence records | 7.2 |
| Monitoring and measurement results | 9.1 |
| Internal audit programme and results | 9.2 |
| Management review minutes | 9.3 |
| Corrective action results | 10.2 |

### Real-world volume – 20–25 documents

The standard strictly requires ~20 items (see clauses 4.3, 5.2, 5.3, 6.1.2, 6.1.3(d), 6.1.3(e), 6.2, 7.2, 7.5.1(b), 8.1, 8.2, 8.3, 9.1, 9.2, 9.3, 10.2). Certification bodies at Stage 2 expect an additional 5–10 "readable" artefacts on top – L2 policies. This is the de facto extended package:

- Access Control Policy and Password Policy.
- Incident Management Procedure.
- Backup Policy.
- Change Management Policy.
- Disaster Recovery Plan / ICT Continuity Plan.
- Cryptography Policy.
- Supplier Security Policy.
- Acceptable Use Policy.
- Information Classification Policy.
- Data Retention and Deletion Policy.
- Remote Working Policy.
- Secure Development Policy.
- BYOD Policy (if applicable).
- Cloud Services Policy.
- Vulnerability Management Procedure.
- Logging and Monitoring Policy.
- Privacy Policy.

Auditors apply a threefold acceptance criterion: content, format, and management process. A document without version, date, owner or review process is itself a nonconformity under clause 7.5.

---

## Part 2. The project lifecycle

### Phase 1. Preparation (4–8 weeks)

**Kick-off and top management buy-in.**

- Project approved by the board or CEO.
- CISO or Head of ISMS appointed as project owner.
- Information Security Policy signed in its first edition – even if it will evolve.

**Scope definition.**

- Which units, sites, data types and processes are in the ISMS.
- What's excluded and why – with justification, not "because it's convenient."
- The document is the ISMS Scope Statement under clause 4.3.

The mistake at this stage is trying to cover the whole company. Start narrow (one product, one unit), expand later.

**Context understanding.**

- Internal and external issues (clause 4.1).
- Interested parties and their requirements (clause 4.2).

### Phase 2. Risk management (4–8 weeks)

This is the heaviest phase. Don't cut corners here – what you lay down now shapes the rest of the work.

**Methodology approval.**

- Risk Assessment Methodology under clause 6.1.2. Approach (asset-based, scenario-based, hybrid), probability and impact scales, risk acceptance criteria, ownership.
- Lean on ISO/IEC 27005:2022 for guidance.

**Asset identification.**

- Asset register (backed by A.5.9). IT assets, information, services, reputation, people.
- Each asset gets an owner and a classification per A.5.12.

**Threat and vulnerability identification.**

- Catalog of typical scenarios, plus threat intel (A.5.7).

**Risk assessment.**

- Inherent risk calculated per scenario.
- The most significant risks identified for prioritization.

**Risk Treatment Plan plus SoA.**

- Treatment choice (modify, avoid, transfer, accept).
- Selection of Annex A controls to apply.
- The SoA under clause 6.1.3(d) with columns: control, applicable / excluded, justification, implementation status.
- Risk Treatment Plan with action owners, deadlines, resources.

### Phase 3. Control implementation (8–24 weeks)

The volume depends on the organisation's starting state and how many "new" controls apply. Parallel work across several streams:

- **Policies and procedures** – the main set of 20–25 documents.
- **Technical controls** – implementation or tuning of tools: EDR, MFA, SIEM, DLP, vulnerability scanning, IAM, MDM.
- **Process controls** – change management, incident management, periodic access reviews.
- **Awareness program** – staff training (A.6.3).
- **Supplier security** – contract review and due diligence (A.5.19–A.5.23).
- **Configuration baselines** – for the technology stack (A.8.9).

Evidence collection runs in parallel – logs, tickets, minutes. That's what you'll show the auditor.

### Phase 4. Internal audit and Management Review (4–6 weeks)

**Internal audit.**

- Audit programme (clause 9.2.2) covering all clauses 4–10 and applicable Annex A controls within the cycle.
- The auditor must be **independent**. You can't audit your own work – that's an automatic major NC at Stage 2.
- Findings are documented and closed with corrective actions.

**Management Review.**

- Formal top-management meeting under clause 9.3, with mandatory inputs (status of actions from the previous review, changes in context, NCs, audit results, risks, opportunities) and outputs (decisions and assigned actions).
- Minutes – a mandatory record.

### Phase 5. Certification audit (8–14 weeks on calendar)

**Stage 1** – 1–2 days. The auditor reviews documentation and ISMS readiness. Findings are closed within 4–8 weeks.

**Stage 2** – 2–10 days. Operational audit: staff interviews, walkthroughs of physical sites, evidence checks in systems. The auditor logs major and minor NCs.

**Certification decision** – 4–8 weeks after Stage 2. Certificate valid for 3 years.

More on timing and cost in [ceo-brief.md](ceo-brief.md) and [certified-companies.md](certified-companies.md).

---

## Part 3. Asset classification

A minimal working classification scheme:

| Level | Content | Handling |
|---|---|---|
| Public | Marketing materials, website | Unrestricted |
| Internal | Internal documents, operational data | Staff only |
| Confidential | Customer PII, financial data, commercial secrets | Least privilege, encryption |
| Strictly Confidential | Crypto keys, secrets, corporate strategy, M&A | Narrow circle, MFA, access logging |

Labelling is mandatory – users need to know what level they're handling. For electronic documents, use templates. For physical, use stamps.

---

## Part 4. Risk assessment methodology – three working approaches

### Asset-based

Starts with the inventory. For each asset, you identify threats and vulnerabilities and calculate the risk. Plus: natural ties to the asset register and to controls. Minus: heavy lifting with a wide scope (e.g., a cloud SaaS with thousands of micro-assets).

### Scenario-based

Starts with realistic attack scenarios – ransomware, supply chain compromise, insider threat. Plus: natural ties to threat intel and playbooks. Minus: takes experience to avoid being too abstract.

### Hybrid

Asset-based for critical assets, scenario-based for broad risks. In practice this is the most workable approach for mid-sized companies.

Scales are typically 5×5 (likelihood × impact) with inherent and residual risk. The main thing: fix the criteria upfront in the Risk Assessment Methodology so they apply consistently.

---

## Part 5. Seven mistakes that sink projects

### Mistake 1. Scope too wide from the start

The team tries to cover the whole company; the project bloats, loses focus, never reaches Stage 2.

**What to do.** Narrow scope the first time – one product or one unit. Get certified, then expand via a scope change at the next surveillance audit.

### Mistake 2. Template risk assessment without adaptation

Auditors spot copy-paste quickly – same assets and risks as the Advisera template. That's a major NC.

**What to do.** The methodology can be a template; assets and scenarios must be your own. Put the time into honest identification.

### Mistake 3. SoA as a "we applied everything" checklist

When all 93 controls are marked "applied" without honest assessment, the auditor asks for evidence on each – and finds gaps.

**What to do.** Honestly mark excluded controls with justification. "Not applicable because we have no physical sites" is fine. "Not applicable because we don't have resources" isn't.

### Mistake 4. Documentation without versions or signatures

Policies live in a wiki with no signatures, dates or version. That violates clause 7.5.

**What to do.** Even in Confluence or Notion, maintain version history with an explicit "approved by ... on ...".

### Mistake 5. Internal audit not independent

CISO or Head of ISMS audits their own system. Major NC.

**What to do.** Use a separate auditor – internal from a different department, or an external contractor who wasn't involved in building the ISMS.

### Mistake 6. Management Review without top management

The review is run by the CISO with one IT director. Violates clause 9.3.

**What to do.** Formally invite the CEO and the board. Minutes with signatures. This isn't a 30-minute meeting – it's a formal process.

### Mistake 7. Silence on incidents

Zero incidents in 12 months. The auditor reads that as "no detection," not "all quiet."

**What to do.** Log even minor events – phishing attempts, missed patches, login anomalies – with lessons learned. This isn't "many incidents = bad." It's "our monitoring works."

---

## Part 6. Stage 1 readiness checklist

Before Stage 1 you need at minimum:

- [ ] ISMS Scope Statement approved.
- [ ] Information Security Policy signed by top management.
- [ ] Risk Assessment Methodology approved.
- [ ] Asset register populated and reviewed.
- [ ] Risk Assessment Report – at least one full cycle.
- [ ] Statement of Applicability with justifications.
- [ ] Risk Treatment Plan with owners and deadlines.
- [ ] Information Security Objectives with metrics.
- [ ] Top 15 policies from the "extended pack" approved.
- [ ] Awareness training program delivered to everyone (records in place).
- [ ] Internal audit program developed.
- [ ] At least one internal audit conducted.
- [ ] Management Review conducted, minutes signed.
- [ ] All NCs from internal audit closed or being closed with action plans.

A more detailed checklist by Annex A control is in [checklist.md](checklist.md).

---

## What to read next

- [annex-a-guide.md](annex-a-guide.md) – detailed walkthrough of the 93 controls.
- [checklist.md](checklist.md) – working readiness checklist.
- [verticals.md](verticals.md) – sector-specific angles.
- [comparison-regulations.md](comparison-regulations.md) – which regulatory requirements you'll cover along the way.

---

## Need help

Launching an implementation project and want a second pair of eyes on the plan? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll walk through your roadmap with you. Chat opens with a pre-filled message. First call is on us.

Website: [iso-cert.kz](https://iso-cert.kz) · Self-paced course: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/)
