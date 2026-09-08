# Access Control and Password Policy

Level 2 topical information security policy. Establishes rules for controlling access to information resources, data and processing devices. Implements A.5.15–A.5.18, A.8.2–A.8.5 of ISO/IEC 27001:2022.

| Parameter | Value |
|---|---|
| Version | 1.0 |
| Alignment | ISO/IEC 27001:2022 |
| Status | Effective |
| Owner | Information Security Officer / CISO |
| Classification | INTERNAL |
| Approval date | [DD.MM.YYYY] |
| Approvers | [List of approver roles] |

**Notation.** Grey italic text is examples, notes and samples for the drafter – adapt them to your organisation or replace with your own data. Text in `[square brackets]` is a placeholder that must be filled in before approval.

---

## 1. Purpose, scope and users

This Access Control and Password Policy is an L2 information security policy that establishes rules for controlling access to information resources, data and processing devices.

**Purpose.** Ensure authorised access for legitimate users and prevent unauthorised access to the organisation's information assets.

**Scope.** The Policy applies to all information systems, applications, databases and network resources within the ISMS scope. The document is mandatory for all employees, contractors, interns and external parties interacting with the organisation's IT infrastructure.

---

## 2. Normative references

The Policy is developed in accordance with ISO/IEC 27001:2022 and implements the following Annex A controls:

- A.5.15 – Access control.
- A.5.16 – Identity management.
- A.5.17 – Authentication information.
- A.5.18 – Access rights.
- A.8.2 – Privileged access rights.
- A.8.3 – Information access restriction.
- A.8.4 – Access to source code.
- A.8.5 – Secure authentication.

---

## 3. Access control principles

The organisation follows these fundamental information security principles when granting access to assets:

| Principle | Description |
|---|---|
| Need-to-know | Access is granted only to the information necessary to perform a specific task or role. A user shouldn't have data "just in case". |
| Need-to-use | Access to IT infrastructure (servers, network equipment, systems) is granted only when there's a justified need for job duties. |
| Least privilege | Users get the minimum sufficient set of rights to perform their duties. Excessive rights increase risks of abuse and errors. |
| Segregation of duties (SoD) | Conflicting responsibilities must be split between different employees. One person cannot simultaneously initiate, approve and execute a critical operation (e.g., access request, approval and provisioning). |

---

## 4. Account management (lifecycle)

### 4.1. Registration and identification (Control A.5.16)

- Every user must have a unique corporate account (User ID) uniquely tied to a specific individual.
- Shared (group) accounts are PROHIBITED, except technical service accounts (with justification and CISO approval).
- Temporary accounts (interns, contractors) are created for a limited period and automatically blocked when it expires.

### 4.2. Granting and modifying rights (Control A.5.18)

Grounds for account creation or rights change: a formal request.

- Requests are submitted through the ticketing system (e.g., JIRA, ServiceNow, HelpDesk).
- Requests are initiated by a line manager or project manager.
- Access is activated ONLY after explicit approval from the Asset Owner or an authorised manager.

### 4.3. Periodic rights review (Control A.5.18)

- Asset Owners must review user access rights at least every six months.
- Ad-hoc rights reviews are triggered by role changes or functional changes for the employee.

### 4.4. Account deactivation (Control A.5.16)

- Access must be immediately blocked on employee termination, contractor engagement end or account compromise.
- Terminated employees' accounts are deleted by the system administrator immediately after offboarding and handover are complete.

---

## 5. Privileged access management (Control A.8.2)

Privileged rights (domain admin, root, sudo) provide full control of systems and require special attention:

- Privileged rights are granted ONLY to full-time IT/IS staff with written CISO approval.
- Administrative accounts must NOT be used for everyday tasks (email, web browsing, document work). Admins must have a separate regular account for daily work.
- All actions using privileged rights must be logged in protected event logs with tamper-proof storage.
- It is PROHIBITED to remove the domain admin group from local administrators or to modify monitoring service accounts (e.g., "watcher").

> *Using privileged rights for everyday tasks is the main attack vector. If a root-enabled admin opens an infected email, malware gains full system control.*

---

## 6. Password policy and authentication (Controls A.5.17, A.8.5)

### 6.1. Password complexity requirements

All organisation passwords must meet these minimums (aligned with NIST SP 800-63B §5.1.1.2 "Memorized Secret Verifiers" – covers both ISO 27001 and typical SOC 2 Type II auditor expectations under CC6.1):

- Length – **at least 12 characters**.
- Forced composition rules (mandatory uppercase / lowercase / digit / special) are NOT applied – they reduce entropy without improving security against real attacks.
- Scheduled password rotation on a calendar basis is NOT applied. A password change is required only on suspected or confirmed compromise.
- New passwords are checked against a breach-corpus list (e.g., HaveIBeenPwned Passwords API) at setup and change.
- A new password must not fully match the previous one.

> *Compatibility with ISO 27001 and SOC 2.* ISO 27001 does not prescribe numeric password requirements – the policy must be **risk-based**, its form is at the organisation's discretion. NIST SP 800-63B §5.1.1.2 explicitly recommends the approach above. SOC 2 Type II sets no minimum under CC6.1, but most auditors expect a NIST-aligned policy. If your landscape is ISO 27001 only, plus Kazakh (ST RK) requirements, password rules may differ – keep the wording aligned with the national standard, but document the choice in the risk register.

### 6.2. Password usage and storage rules

- Password sharing with anyone else is PROHIBITED. Every user is personally accountable for actions performed under their account.
- Writing passwords on paper, sticky notes, storing plaintext in text files or spreadsheets is PROHIBITED.
- Approved password managers (1Password, KeePass, Bitwarden) with encrypted storage are allowed.
- On first login, the user must immediately change the temporary password to a permanent one.

### 6.3. Sign-in technical security settings

| Control | Requirement |
|---|---|
| Password masking | The system must hide entered password characters on screen (display asterisks *** or dots •••) |
| Brute-force protection | Account locks after 3–5 failed attempts. Unlock via admin or auto-unlock after 30 minutes |
| Session timeout | Idle session ends automatically after 15 minutes (workstations) or 10 minutes (critical systems) |
| Multi-factor authentication (MFA) | MANDATORY for: VPN access, critical systems (finance, HR, production databases), cloud services (Office 365, AWS, Azure), remote server access |

---

## 7. Monitoring and event logging

To ensure accountability and incident investigation, the organisation keeps logs of all access operations:

- System administrators must configure logging of all successful and failed sign-in attempts.
- Logs capture attempts to access confidential data, configuration changes, use of administrative utilities.
- Event logs must be protected from modification or deletion by users, including administrators (centralised log collection or WORM storage).
- All system clocks must be synchronised via NTP to ensure accurate timestamps for investigations.

> *Clock synchronisation is critical. If server A shows 14:00 and server B shows 14:30, during an incident investigation the correct sequence of events cannot be reconstructed.*

---

## 8. Accountability and sanctions

Policy violation is classified as an information security incident and may result in:

- Sharing a password with a colleague or using a shared account – written warning; repeated violation – dismissal.
- Using administrative rights for personal purposes – disciplinary action, possible dismissal.
- Deliberately providing unauthorised access to confidential data – dismissal, possible administrative or criminal charges.

All disciplinary measures follow the Labour Code and internal regulations.

---

## 9. Revision history

| Date | Version | Change description | Author |
|---|---|---|---|
| [DD.MM.YYYY] | 1.0 | Initial edition of the Access Control and Password Policy | [Full name] |

---

## 10. Review and approval

The Access Control and Password Policy must be approved by top management.

| Role | Full name | Signature | Date |
|---|---|---|---|
| Drafted by: [CISO / IS Officer] | | | |
| Reviewed by: [Approver role] | | | |
| Approved by: [CEO] | | | |

---

*We help companies implement an ISMS end-to-end – from gap analysis to passing the certification audit. [Text us on Telegram](https://t.me/m/8NsOXRkMZmQy) if you need help adapting this to your business.*
