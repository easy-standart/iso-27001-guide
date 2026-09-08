# Stage 1 and Stage 2 readiness checklist

> A working list of what the auditor will look at and ask about – so you find the gaps in advance, not at the audit itself.

This checklist is built around the Annex A controls in the 2022 edition. Each block has 3–5 self-assessment questions plus an example of what audit-ready evidence looks like for critical controls.

If you're just starting the project, go to [implementation-guide.md](implementation-guide.md). If you're preparing for Stage 2, this file is your companion in the final months.

*Русская версия: [../checklist.md](../checklist.md). Have a question? [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) – we'll reply personally.*

---

## Management system readiness (clauses 4–10)

This is what makes certification possible in the first place. Work through it before you call the auditor.

- [ ] **ISMS Scope Statement** approved by top management. Signed, dated.
- [ ] **Information Security Policy** approved by top management.
- [ ] **Risk Assessment Methodology** approved. Scales, risk acceptance criteria, risk ownership.
- [ ] **Asset register** completed and reviewed. With owners and classification.
- [ ] **Risk Assessment Report** – at least one full cycle of risk assessment.
- [ ] **Statement of Applicability (SoA)** with justifications for inclusion and exclusion of each control.
- [ ] **Risk Treatment Plan** with action owners, deadlines and resources.
- [ ] **Information Security Objectives** – measurable, with metrics and owners.
- [ ] **Internal audit programme** developed. Coverage of all clauses and applicable controls within the cycle.
- [ ] **At least one internal audit** conducted by an independent auditor.
- [ ] **Management Review** conducted by top management. Minutes signed, mandatory inputs and outputs recorded.
- [ ] All NCs from the internal audit are closed or being closed with an action plan.

---

## A.5 – Organizational controls

### A.5.1 Security policies

- [ ] ISMS Policy approved by top management (signed, dated).
- [ ] Annual review schedule at minimum.
- [ ] Topical policies (access, crypto, supplier, incident) approved and accessible to staff.

### A.5.7 Threat Intelligence (added in 2022)

- [ ] Who's responsible for threat intel? Documented process?
- [ ] What feed sources are used?
- [ ] How does threat intel update the risk register and policies?
- [ ] Is there evidence of intel-based actions over the last 6 months?

**Audit-ready evidence:** quarterly threat intel report plus at least 2 examples of updating the Risk Treatment Plan or a security control based on intel.

### A.5.9 Asset Inventory

- [ ] Register covers all asset types – hardware, software, SaaS, information, people.
- [ ] Each asset has an owner.
- [ ] Sensitivity classification is in place.
- [ ] Regular reconciliation with reality (at least every 6 months).

**Audit-ready evidence:** export of the register with owners and classification plus minutes of the last reconciliation.

### A.5.18 Access Rights

- [ ] Documented JML (Joiner-Mover-Leaver) process?
- [ ] Periodic access reviews conducted? Frequency? Who signs off?
- [ ] Privileged access managed separately (see A.8.2)?

**Audit-ready evidence:** records of the last access reviews with reviewer, date, specific corrections.

### A.5.19–A.5.23 Supplier Security

- [ ] Supplier register with criticality levels?
- [ ] Contracts contain security clauses (data protection, right to audit, breach notification SLA)?
- [ ] Due diligence done before engaging a new supplier?
- [ ] Cloud services covered under A.5.23 (cloud-specific requirements)?

**Audit-ready evidence:** supplier register plus 3 examples of contracts with security clauses plus DD reports from the last year.

### A.5.23 Cloud Services (added in 2022)

- [ ] Cloud Security Policy approved?
- [ ] For each cloud service – who decided to use it and on what criteria?
- [ ] Exit strategy spelled out in the contract?
- [ ] Shared responsibility model documented?

**Audit-ready evidence:** cloud register plus exit strategy for the top 3 critical providers.

### A.5.24–A.5.27 Incident Management

- [ ] Documented incident management procedure?
- [ ] Do all staff know how to report an incident?
- [ ] Recorded incidents in the last 12 months? How many?
- [ ] Post-incident reviews documented?

**Audit-ready evidence:** at least 1–2 real incident reports (even minor) with lessons learned in the last 6 months.

Auditors read "zero incidents" as "no detection," not "all quiet."

### A.5.30 ICT Readiness (added in 2022)

- [ ] ICT Continuity Plan approved?
- [ ] RTO and RPO defined for critical systems?
- [ ] DR tests done in the last 12 months? Where are the records?

**Audit-ready evidence:** the last DR test record plus ICT continuity plan plus BIA (Business Impact Analysis).

### A.5.34 Privacy and Protection of PII

- [ ] Privacy Policy approved and published?
- [ ] Registration with regulator (if required in your jurisdiction)?
- [ ] Process for handling data subject requests?
- [ ] DPIA for high-risk processing?

---

## A.6 – People controls

### A.6.1 Screening

- [ ] Candidate vetting procedure?
- [ ] Vetting level matches the role's sensitivity?
- [ ] Screening records retained?

### A.6.3 Awareness

- [ ] Every employee gets onboarding security training?
- [ ] Annual refresh for everyone?
- [ ] Coverage includes contractors?
- [ ] Content reflects current threats (phishing, AI risks, ransomware)?

**Audit-ready evidence:** training matrix with 100% coverage plus content examples.

### A.6.7 Remote Working

- [ ] Remote Work Policy approved?
- [ ] All remote devices managed via MDM?
- [ ] VPN or Zero Trust configured for corporate access?
- [ ] BYOD spelled out separately (if applicable)?

---

## A.7 – Physical controls

### A.7.4 Physical Security Monitoring (added in 2022)

- [ ] Restricted areas defined?
- [ ] What monitoring measures are deployed (CCTV, alarms, guards)?
- [ ] Video retention periods comply with local law?
- [ ] DPIA done before CCTV deployment?

**Audit-ready evidence:** zone map plus CCTV configuration plus DPIA plus retention policy.

### A.7.7 Clear Desk and Screen Lock

- [ ] Clear desk and screen lock policy approved?
- [ ] GPO or MDM enforces auto-lock?
- [ ] Walkthrough audits conducted?

A walkthrough is where the auditor walks the office looking for unlocked laptops, papers with PII on desks, sticky notes with passwords.

---

## A.8 – Technological controls

### A.8.8 Vulnerability Management

- [ ] Regular vulnerability scans (at least monthly)?
- [ ] Closure SLA defined by risk score (CVSS × asset criticality × exposure), not by flat CVSS score?
- [ ] Closure evidence retained?
- [ ] Patch management covers legacy (if any)?

ISO 27002:2022 §8.8 asks for a risk-based priority, not a raw CVE ranking.

**Audit-ready evidence:** scan report plus remediation tickets with closure dates.

### A.8.9 Configuration Management (added in 2022)

- [ ] Hardening baselines (CIS Benchmarks, STIG) approved?
- [ ] Configurations applied automatically (IaC)?
- [ ] Configuration drift monitored?
- [ ] Changes logged?

### A.8.10 Information Deletion (added in 2022)

- [ ] Data retention schedule approved?
- [ ] Secure erasure procedures cover all media (HDD, SSD, cloud)?
- [ ] Backups included in retention/deletion policy?
- [ ] Evidence of handling deletion requests under GDPR or local privacy laws?

### A.8.11 Data Masking (added in 2022)

- [ ] Production PII masked in non-prod environments?
- [ ] Masking tools configured?
- [ ] Dev teams know how to use masked datasets?

### A.8.12 Data Leakage Prevention (added in 2022)

- [ ] DLP deployed on endpoint, email, web?
- [ ] Data classification configured in the tools?
- [ ] DLP incidents from the last 6 months in logs?
- [ ] Response process to DLP alerts works?

**Audit-ready evidence:** list of DLP incidents with classification plus response records.

### A.8.13 Backup

- [ ] Backup Policy approved?
- [ ] Restore tests conducted (at least every 6 months)?
- [ ] Test restore records retained?

**Audit-ready evidence:** records of 2–3 recent test restores with dates and results.

### A.8.15 + A.8.16 Logging and Monitoring (A.8.16 added in 2022)

- [ ] Centralised logging configured?
- [ ] Log retention matches policy?
- [ ] SIEM with use-cases operating?
- [ ] Evidence of alert response over the last 6 months?

**Audit-ready evidence:** 2–3 closed incident tickets from SIEM alerts with timeline and lessons learned.

### A.8.23 Web Filtering (added in 2022)

- [ ] Web filtering operates in the office and for remote users (VPN, SASE)?
- [ ] Blocked site categories approved?
- [ ] AI services (ChatGPT etc.) – policy defined (allow, deny, conditional)?
- [ ] Periodic category reviews conducted?

### A.8.24 Cryptography

- [ ] Cryptography Policy approved?
- [ ] Key Management lifecycle defined (generation, rotation, revocation, archive)?
- [ ] Secrets aren't sitting in plaintext in Git, CI, Wiki?
- [ ] TLS certificates renewed automatically?

### A.8.28 Secure Coding (added in 2022)

- [ ] Secure Coding Standards approved?
- [ ] Mandatory peer review for all PRs to prod?
- [ ] SAST and DAST in CI/CD pipeline?
- [ ] SBoM and SCA for third-party libraries maintained?

**Audit-ready evidence:** git logs with peer review approval plus latest SAST report plus SBoM for the main product.

### A.8.32 Change Management

- [ ] Change Management Procedure approved?
- [ ] CAB or equivalent meets on schedule?
- [ ] Emergency change process defined?

---

## When the checklist is done

If you've worked through it honestly and closed every item, you're ready for Stage 1 – and Stage 2 will go more smoothly than you expect.

For any items still in the red, decide:

1. Is it a blocker or secondary?
2. How much time and money will it take to close?
3. Can you negotiate a small delay with the CB via a scope change?

Pre-audit stress is normal. The key is to not panic – just methodically close items one by one.

---

## Related material

- [implementation-guide.md](implementation-guide.md) – implementation phases end-to-end.
- [annex-a-guide.md](annex-a-guide.md) – detailed walkthrough of each control.
- [verticals.md](verticals.md) – sector-specific angles, which controls matter in your industry.

---

## Need help

If any checklist items are unclear or you need help closing them, [text us on Telegram](https://t.me/m/8NsOXRkMZmQy). We'll work through your specific case. Chat opens with a pre-filled message. First call is on us.

Website: [iso-cert.kz](https://iso-cert.kz) · Self-paced course: [iso-cert.kz/course-27001](https://iso-cert.kz/course-27001/)
