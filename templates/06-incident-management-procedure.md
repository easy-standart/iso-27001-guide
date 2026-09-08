# Information Security Incident Management Procedure

Level 3 process regulation. Ensures rapid, effective and orderly response to information security incidents. Implements A.5.24–A.5.28 and A.6.8 of ISO/IEC 27001:2022.

| Parameter | Value |
|---|---|
| Version | 1.0 |
| Alignment | ISO/IEC 27001:2022 |
| Status | Effective |
| Owner | Information Security Officer (CISO) |
| Classification | INTERNAL |
| Approval date | [DD.MM.YYYY] |
| Approvers | [List of approver roles] |

**Notation.** Grey italic text is examples, notes and samples for the drafter – adapt them to your organisation or replace with your own data. Text in `[square brackets]` is a placeholder that must be filled in before approval.

---

## 1. Purpose and scope

The purpose of this procedure is to ensure rapid, effective and orderly response to information security (IS) incidents to minimise damage and maintain business continuity. The document defines rules for detecting, classifying, containing and investigating IS events. Mandatory for all employees, contractors and temporary staff.

> *This section legally locks in every employee's obligation to promptly report security problems. The goal isn't to "punish the guilty", it's to minimise business damage and quickly restore operations after a failure or attack.*

---

## 2. Normative references

The procedure is developed per:

- ISO/IEC 27001:2022 – controls 5.24–5.28.
- ISO/IEC 27035 – incident management principles.
- Internal documents: Trade Secret Regulation, Business Continuity Policy, Asset and Risk Register.

> *The procedure relies on ISO/IEC 27001:2022 (organisational controls 5.24–5.28) and the specialised incident management standard ISO/IEC 27035. It also links to the business continuity policy, since a major IS incident can escalate into a disaster requiring DR plan activation.*

---

## 3. Roles and responsibilities

- **Incident Response Team (IRT/SIRT).** Cross-functional team (IT, IS, Legal, HR) responsible for direct incident resolution.
- **CISO (IS Officer).** Overall process coordination, strategic decisions, reporting to top management.
- **Line managers.** Ensure staff participation and execute corrective actions in their departments.
- **Staff.** Timely reporting of any suspicious events or system weaknesses.

> *The Incident Response Team (IRT/SIRT) is the "fire brigade" of experts from IT, IS, Legal and HR that assembles to solve critical incidents. The CISO coordinates and is accountable for reporting to top management. The main duty of staff is only to report. Employees are prohibited from independently testing vulnerabilities or trying to "investigate" a breach, as this can destroy digital evidence.*

---

## 4. Incident management lifecycle

> *This section describes the algorithm from A to Z: Planning (preparation includes drills), Detection (transition from event to incident), Classification (scale assessment), Response (containment, eradication and recovery), Lessons Learned (formal closing step with a "why did this happen" analysis).*

### 4.1. Planning and preparation (A.5.24)

- Set incident management objectives and priorities.
- Maintain the Emergency Contact List (internal and external) up to date.
- Regularly conduct drills and attack simulations (phishing, DDoS) to test readiness.

### 4.2. Detection and reporting (A.6.8)

- Events are logged automatically (system logs) or manually by staff via JIRA/HelpDesk.
- Staff must report: software malfunctions, unusual system behaviour, unauthorised access attempts, policy violations.
- Independent attempts to test or confirm vulnerabilities are prohibited.

### 4.3. Classification and assessment (A.5.25)

All events are analysed to determine category and priority:

- **Critical (P1).** Mass PII breach, complete business service outage, admin account compromise.
- **High (P2).** Ransomware infection (without access loss), partial system failure.
- **Low (P3).** Single failed login attempts, clear desk policy violation.

> *Scale assessment. For example, a client PII leak always has higher priority than a single virus on a non-critical PC. Critical (P1) triggers immediate mobilisation of the full SIRT.*

### 4.4. Response and containment (A.5.26)

- **Containment.** Isolate compromised systems from the network, block accounts, disable vulnerable services.
- **Eradication.** Remove malicious code, apply patches, restore data from clean backups.
- **Recovery.** Verify system functionality before returning to production.

### 4.5. Lessons Learned (A.5.27)

- Root Cause Analysis using the "5 Whys" method.
- Update the Risk Register and Statement of Applicability (SoA) based on the experience.
- Use anonymised examples of real incidents for staff training.

> *The most important item for continual system improvement. Example of the "5 Whys" method: Why did the virus get into the network? → Employee clicked a link. Why? → They didn't know about the risks. Why? → They missed the awareness training. Corrective action: automatic email access block for those who didn't take the annual training.*

---

## 5. Evidence collection (A.5.28)

- Identify and preserve digital evidence: server logs, memory dumps, email headers.
- Maintain chain of custody so evidence can be used in court.
- Copies of electronic evidence must be identical to originals and protected from modification.

> *Annex A.5.28 requires all evidence (logs, screenshots, memory dumps) to be collected in a way that allows court use. This implies chain of custody and guarantees that data copies are identical to originals.*

---

## 6. Notification and communication

- **Internal.** Notify management, IT and HR (when staff involved).
- **External.** Notify regulators and clients within statutory deadlines per applicable law. Typical clocks: **GDPR** – 72 hours from the moment the organisation becomes aware of the breach (Art. 33(1) – "awareness", not "detection"); **NIS2** – 24-hour early warning, 72-hour incident notification to the national CSIRT (or, in some Member States, to the competent authority per national transposition), final report within one month (Art. 23(4)); **DORA** – initial notification within the earlier of 4 hours after classifying the incident as major and 24 hours from awareness; 72-hour intermediate report; final report within one month of the initial notification. References: RTS (EU) 2025/301, ITS (EU) 2025/302. Law enforcement is notified only if a specific law requires it or the organisation elects to file (e.g., where a crime is suspected) – verify by jurisdiction.
- **Public statements.** Made only by authorised persons (PR / Director).

> *If the incident involves personal data, the law may require mandatory notification to the regulator and affected persons within a short deadline. Check the applicable regulations in your jurisdiction.*

---

## 7. Control and documentation

- All incident actions are logged in the IS Incident Register.
- Category 1 backup failure incidents are subject to mandatory investigation.
- Response results are included in the annual Management Review.

---

## 8. Revision history

| Date | Version | Change description | Author |
|---|---|---|---|
| [DD.MM.YYYY] | 1.0 | Initial edition of the document | [Full name] |

---

## 9. Review and approval

| Role | Full name | Signature | Date |
|---|---|---|---|
| Drafted by: [Responsible role] | | | |
| Reviewed by: [CISO / IS Officer] | | | |
| Approved by: [Director] | | | |

---

## Appendices

> *Appendices are operational tools that help apply the incident management procedure in practice. Five appendices with templates follow.*

### Appendix 1. IS Event Registration Form

> *This is the entry ticket to the process. The form must contain timestamps and a detailed description of what the user observed. This allows SIRT to reconstruct the event timeline during investigation.*

| Parameter | Description / Value |
|---|---|
| Event number | [Auto-generated by the system] |
| Detection date and time | [DD.MM.YYYY HH:MM] |
| Reporter's full name | [Employee full name] |
| Department | [Department name] |
| Event description | [Detailed description: what happened, which systems are affected, observed symptoms] |
| Affected assets | [List of systems, servers, workstations, applications] |
| Event category | [Malware / Unauthorised access / Data breach / Denial of service / Other] |

### Appendix 2. Classification and Prioritisation Matrix

> *This is a tool for rapid decision-making. Critical (P1) triggers immediate full SIRT mobilisation and may mean full business service outage or trade secret leak. High (P2) – partial failure or suspicion of admin account compromise. Low (P3) – single policy violations without immediate threat.*

| Priority | Criterion | Response time | Example |
|---|---|---|---|
| P1 – Critical | Full business service outage, mass PII breach, admin compromise | Immediate | Ransomware attack, client base leak |
| P2 – High | Partial system failure, suspicion of breach | Within 4 hours | Virus on a development server |
| P3 – Low | Single policy violations | Within 24 hours | Password on a sticky note |

### Appendix 3. Emergency Contact List

> *The list includes not only internal staff but also external providers, police and CERT centres. This list's currency is verified annually – searching for a system administrator's number while they're on holiday in the middle of a crisis is unacceptable.*

| Role | Full name | Phone | Email |
|---|---|---|---|
| CISO | [Full name] | [+XXX XX XXX-XX-XX] | [email@company.com] |
| System administrator | [Full name] | [+XXX XX XXX-XX-XX] | [email@company.com] |
| IT Manager | [Full name] | [+XXX XX XXX-XX-XX] | [email@company.com] |
| Internet provider | [Company name] | [Hotline] | [support@provider.com] |
| CERT (response centre) | [Name] | [Phone] | [cert@example.com] |

### Appendix 4. Investigation Action Log

> *This is the detailed work log of the response team. It records: "at 14:05 server X disconnected from network, log file hash captured by employee Y". This ensures accountability and transparency of team actions.*

| Date/Time | Responsible | Action taken | Result/Notes |
|---|---|---|---|
| [DD.MM HH:MM] | [Full name] | [Action description] | [Result, hashes, screenshots] |
| [DD.MM HH:MM] | [Full name] | [Action description] | [Result, hashes, screenshots] |

### Appendix 5. Lessons Learned Report Form

> *The most important item for continual system improvement. Uses the "5 Whys" method to find the root cause. Example: Why did the virus enter the network? Employee clicked a link. Why? They didn't know about the risks. Why? They missed the awareness training. Corrective action: automatic email access block for those who didn't take the annual training.*

| Question | Answer |
|---|---|
| Incident number | [From the register] |
| What happened? | [Brief incident description] |
| What worked well? | [Team's successful actions] |
| What can be improved? | [Identified process issues] |
| Root Cause | ["5 Whys" analysis] |
| Corrective actions | [Specific measures to prevent recurrence] |
| Responsible for execution | [Full name and deadline] |
| ISMS documentation updates | [Which documents/procedures need updating] |

---

*We help companies implement an ISMS end-to-end – from gap analysis to passing the certification audit. [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) if you need help adapting this to your business.*
