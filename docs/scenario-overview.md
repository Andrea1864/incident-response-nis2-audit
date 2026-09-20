# Scenario Overview — TechPay Solutions IR & NIS2 Lab

## Company Profile
- **Name**: TechPay Solutions S.L.
- **Sector**: Financial Technology (Fintech)
- **Employees**: 50
- **Location**: Barcelona, Spain
- **Services**: Digital payment processing, peer-to-peer 
  transfers, virtual card issuing
- **NIS2 Classification**: Important Entity (Art. 3.2)

## Incident Scenario
On August 10, 2026, TechPay's payment infrastructure 
was hit by a ransomware attack. The incident triggered:
- Full IR plan activation (P1 Critical)
- GDPR Art. 33 breach notification to AEPD
- NIS2 Art. 23 incident reporting to INCIBE-CERT
- DORA incident notification to Banco de España
- NIS2 compliance audit revealing 39% compliance

## Regulatory Obligations Triggered
| Regulation | Obligation | Deadline |
|---|---|---|
| GDPR Art. 33 | Notify AEPD | 72 hours |
| GDPR Art. 34 | Notify individuals | Without undue delay |
| NIS2 Art. 23 | Early warning INCIBE-CERT | 24 hours |
| NIS2 Art. 23 | Full notification | 72 hours |
| DORA Art. 19 | ICT incident report | 4 hours initial |

## Key Documents Produced
- Incident Response Plan (ir-plan.md)
- Ransomware Playbook (ransomware-playbook.md)
- Breach Notification Procedure (breach-notification.md)
- NIS2 Gap Analysis (nis2-gap-analysis.md)
- NIS2 Remediation Plan (nis2-remediation-plan.md)

docs/lessons-learned.md

markdown
# Lessons Learned — Ransomware Incident
## TechPay Solutions | August 2026

## Incident Summary
- **Type**: Ransomware attack on payment infrastructure
- **Duration**: 18 hours of service disruption
- **Data affected**: Payment logs, customer records
- **Financial impact**: ~€150,000 (downtime + recovery)
- **Regulatory impact**: AEPD notification filed

## What Went Wrong

### 1. No MFA enforced
The ransomware gained initial access via a phished 
employee account. MFA would have prevented this.
**Fix**: MFA enforced within 15 days (Priority 1.1)

### 2. No network segmentation
Once inside, the attacker moved laterally to the 
payment server within 2 hours.
**Fix**: Network segmentation within 120 days

### 3. IR plan not tested
The team had never practiced the IR plan. First 
30 minutes were chaotic — unclear who to call first.
**Fix**: Quarterly tabletop exercises

### 4. Backup not tested recently
Last backup test was 6 months ago. Recovery took 
18 hours instead of the expected 4.
**Fix**: Monthly backup restoration tests

### 5. No security awareness training
The phishing email that initiated the attack was 
not sophisticated. Training would have prevented it.
**Fix**: Mandatory annual training + quarterly phishing simulations

## What Went Well
- SOC team detected the attack within 15 minutes
- CISO made correct decision NOT to pay ransom
- DPO filed AEPD notification within 72 hours
- Legal team preserved forensic evidence correctly
- Communication to customers was clear and timely

## Action Items

| Action | Owner | Deadline | Status |
|---|---|---|---|
| Enforce MFA | IT Admin | 15 days | In progress |
| Test IR plan quarterly | CISO | 30 days | Planned |
| Monthly backup tests | IT Admin | 30 days | Planned |
| Security awareness training | HR + CISO | 30 days | Planned |
| Network segmentation | CTO | 120 days | Planned |
| Vulnerability scanning | SOC Lead | 60 days | Planned |

## NIS2 Compliance Impact
The incident revealed TechPay is only 39% NIS2 compliant.
The remediation plan targets 84% compliance within 6 months.
This incident will be referenced in the NIS2 final report
to INCIBE-CERT as evidence of continuous improvement.
