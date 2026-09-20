# GDPR Breach Notification Procedure — TechPay Solutions

## Overview
This document defines TechPay's procedure for notifying 
the AEPD and affected individuals following a personal 
data breach, as required by GDPR Art. 33 and Art. 34.

---

## Decision Tree — Do We Need to Notify?

Personal data breach confirmed?
↓ YES
Is it unlikely to result in risk to individuals?
↓ NO (there IS risk)
→ Notify AEPD within 72 hours (Art. 33)
↓
Is the risk HIGH to individuals?
↓ YES
→ Also notify affected individuals (Art. 34)


**Key principle**: When in doubt, notify. The cost of 
late notification far exceeds the cost of unnecessary 
notification.

---

## AEPD Notification (Art. 33)

### Deadline
72 hours from becoming aware of the breach.
If notification is delayed, reasons must be documented.

### How to Notify
1. Go to AEPD portal: `sedeagpd.gob.es`
2. Select "Notificación de brechas de seguridad"
3. Complete the online form

### What to Include (Art. 33.3)
- Nature of the breach (what happened)
- Categories and approximate number of data subjects affected
- Categories and approximate number of records affected
- Contact details of DPO
- Likely consequences of the breach
- Measures taken or proposed to address the breach

---

## Individual Notification (Art. 34)

### When Required
When the breach is likely to result in HIGH RISK to 
the rights and freedoms of individuals.

### High Risk Examples at TechPay
- Payment card data exfiltrated → financial fraud risk
- KYC/identity documents leaked → identity theft risk
- Account credentials stolen → account takeover risk

### How to Notify Individuals
- Direct communication (email, letter, SMS)
- Clear and plain language
- Must include:
  - What happened
  - What data was affected
  - Likely consequences
  - Steps taken to address
  - Contact for more information (DPO)

---

## Breach Notification Timeline — Ransomware Scenario

| Time | Action | Responsible |
|---|---|---|
| T+0 | Breach detected | SOC Lead |
| T+15min | IR team activated | CISO |
| T+1h | Scope assessment complete | SOC Lead |
| T+2h | Board notified | CEO + CISO |
| T+4h | DORA initial notification → Banco de España | CISO + Legal |
| T+24h | NIS2 early warning → INCIBE-CERT | CISO |
| T+48h | AEPD notification drafted | DPO |
| T+72h | AEPD notification submitted ⚠️ DEADLINE | DPO |
| T+72h | NIS2 full notification → INCIBE-CERT | CISO |
| T+7d | Individual notifications sent (if high risk) | DPO |
| T+30d | NIS2 final report → INCIBE-CERT | CISO |

---

## Factors That Reduce Notification Urgency
- Data was encrypted at rest (Art. 34.3.a)
- Subsequent measures eliminated high risk
- Individual notification would require disproportionate effort
  (use public communication instead)

---

## DPO Responsibilities During a Breach
1. Assess whether notification is required
2. Draft AEPD notification within 48 hours
3. Review individual notification content
4. Document all decisions and rationale
5. Maintain breach register (Art. 33.5)
6. Liaise with AEPD if they request more information
7. Coordinate with Legal on potential liability

---

## Breach Register (Art. 33.5)
TechPay must maintain an internal record of ALL breaches,
even those not notified to AEPD:

| Field | Content |
|---|---|
| Date of breach | When it occurred |
| Date discovered | When TechPay became aware |
| Nature of breach | Confidentiality / Integrity / Availability |
| Data categories | What types of personal data |
| Number of records | Approximate number affected |
| Consequences | Likely impact on individuals |
| Measures taken | How TechPay responded |
| Notified AEPD | Yes / No / Reason if No |
| Notified individuals | Yes / No / Reason if No |
