# Incident Response Plan — TechPay Solutions
## Version 1.0 | August 2026

## 1. Purpose and Scope
This Incident Response Plan (IRP) defines TechPay Solutions' 
procedures for detecting, containing, eradicating and recovering 
from cybersecurity incidents. It applies to all TechPay systems, 
employees and third-party providers.

## 2. Incident Response Team

| Role | Responsibility | Contact |
|---|---|---|
| CISO | Overall incident coordination | ciso@techpay.com |
| DPO | GDPR compliance and breach notification | dpo@techpay.com |
| SOC Lead | Technical detection and containment | soc@techpay.com |
| Legal Counsel | Legal obligations and law enforcement | legal@techpay.com |
| HR Manager | Employee-related incidents | hr@techpay.com |
| Communications | Internal and external communications | comms@techpay.com |

## 3. Incident Classification

| Severity | Definition | Response Time | Example |
|---|---|---|---|
| P1 — Critical | Business-stopping, data breach | 15 minutes | Ransomware, data exfiltration |
| P2 — High | Significant impact, potential breach | 1 hour | Account takeover, brute force |
| P3 — Medium | Limited impact, no breach | 4 hours | Failed phishing, policy violation |
| P4 — Low | Minimal impact | 24 hours | Spam, single failed login |

## 4. Incident Response Phases

### Phase 1 — Preparation
- Maintain updated asset inventory
- Ensure backups are tested weekly
- Train staff on phishing and social engineering
- Test IR plan quarterly

### Phase 2 — Detection & Analysis

Alert received (Splunk/Sentinel/user report)
↓
SOC Lead assesses severity (P1-P4)
↓
IR team activated if P1 or P2
↓
Evidence preserved — logs, screenshots, timestamps
↓
Scope determined — what systems affected?


### Phase 3 — Containment
**Short-term containment (immediate):**
- Isolate affected systems from network
- Disable compromised accounts
- Block malicious IPs in firewall
- Preserve forensic evidence

**Long-term containment:**
- Apply emergency patches
- Strengthen access controls
- Increase monitoring on adjacent systems

### Phase 4 — Eradication
- Remove malware or threat actor access
- Patch exploited vulnerabilities
- Reset all potentially compromised credentials
- Verify systems are clean before recovery

### Phase 5 — Recovery
- Restore systems from clean backups
- Monitor for re-infection for 30 days
- Gradually restore services with enhanced monitoring
- Document all recovery steps

### Phase 6 — Post-Incident
- Lessons learned meeting within 5 days
- Update IR plan based on findings
- Report to board and regulators as required
- Implement preventive controls

## 5. Legal and Regulatory Obligations

| Obligation | Trigger | Deadline | Authority |
|---|---|---|---|
| GDPR Art. 33 — AEPD notification | Personal data breach | 72 hours | AEPD |
| GDPR Art. 34 — Individual notification | High risk to individuals | Without undue delay | Affected persons |
| NIS2 Art. 23 — Early warning | Significant incident | 24 hours | INCIBE-CERT |
| NIS2 Art. 23 — Incident notification | Significant incident | 72 hours | INCIBE-CERT |
| NIS2 Art. 23 — Final report | Significant incident | 1 month | INCIBE-CERT |
| DORA Art. 19 — ICT incident | Major ICT incident | 4 hours initial | Banco de España |

## 6. Evidence Preservation
- Never power off affected systems — memory evidence lost
- Take forensic images before remediation
- Preserve all logs with timestamps
- Document chain of custody
- Store evidence in tamper-proof location
