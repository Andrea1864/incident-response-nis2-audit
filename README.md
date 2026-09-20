# Incident Response Plan & NIS2 Audit — TechPay Solutions

## Project Overview
This project simulates a complete cybersecurity incident 
response and NIS2 compliance audit for a fictional fintech 
company — TechPay Solutions S.L. following a ransomware attack.
It combines technical incident response with legal and 
regulatory compliance obligations.

## Scenario
On August 10, 2026, TechPay's payment infrastructure was 
hit by a ransomware attack. This triggered a full incident 
response activation, GDPR breach notification to AEPD, 
NIS2 reporting to INCIBE-CERT, and a compliance audit 
revealing 39% NIS2 compliance.

## What This Project Covers

### Incident Response
- Complete IR plan with 6-phase methodology
- Ransomware-specific playbook with MITRE ATT&CK mapping
- GDPR Art. 33/34 breach notification procedure
- Multi-regulator notification timeline (AEPD, INCIBE-CERT, 
  Banco de España)

### NIS2 Compliance Audit
- Full gap analysis against NIS2 Art. 21 requirements
- Current compliance: 39%
- 8 control areas assessed
- Critical gaps identified: MFA, BCP, vulnerability management

### NIS2 Remediation Plan
- Priority 1 actions (0-30 days): MFA, training, IR testing
- Priority 2 actions (30-90 days): BCP, vulnerability mgmt
- Priority 3 actions (90-180 days): network segmentation, PAM
- Target compliance after 6 months: 84%

## Regulatory Framework
| Regulation | Obligations Covered |
|---|---|
| GDPR Art. 33 | Breach notification to AEPD (72h) |
| GDPR Art. 34 | Individual notification |
| NIS2 Art. 21 | Risk management requirements |
| NIS2 Art. 23 | Incident reporting to INCIBE-CERT |
| DORA Art. 19 | ICT incident reporting to Banco de España |

## NIS2 Compliance Summary
| Control Area | Current | Target (6 months) |
|---|---|---|
| Risk analysis | 60% | 85% |
| Incident handling | 75% | 95% |
| Business continuity | 25% | 80% |
| Supply chain | 35% | 75% |
| Network security | 20% | 70% |
| Cryptography | 65% | 85% |
| HR security | 30% | 85% |
| MFA | 0% | 100% |
| **Total** | **39%** | **84%** |

## Key Documents
- [IR Plan](incident-response/ir-plan.md)
- [Ransomware Playbook](incident-response/ransomware-playbook.md)
- [Breach Notification](incident-response/breach-notification.md)
- [NIS2 Gap Analysis](nis2-audit/nis2-gap-analysis.md)
- [NIS2 Remediation Plan](nis2-audit/nis2-remediation-plan.md)
- [Incident Report Template](templates/incident-report-template.md)
- [Breach Notification Template](templates/breach-notification-template.md)

## Skills Demonstrated
- Incident response planning and execution
- Ransomware response and MITRE ATT&CK mapping
- GDPR breach notification (Art. 33 and Art. 34)
- NIS2 compliance gap analysis
- Regulatory remediation planning
- Multi-regulator coordination (AEPD, INCIBE-CERT, Banco de España)
- DPO operational responsibilities

## Related Projects
- [Splunk SIEM Lab](https://github.com/Andrea1864/splunk-siem-log-analysis)
- [Microsoft Sentinel Lab](https://github.com/Andrea1864/siem-microsoft-sentinel)
- [Azure Policy + NIS2](https://github.com/Andrea1864/azure-policy-defender-cloud)
- [TechPay GDPR ROPA](https://github.com/Andrea1864/gdpr-ropa-fintech)
- [MedCore GDPR ROPA](https://github.com/Andrea1864/gdpr-ropa-healthcare)

## Author
Andrea Castillo— Law Graduate | Cybersecurity & GRC Specialist  
