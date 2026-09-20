# NIS2 Remediation Plan — TechPay Solutions
## Priority Action Plan | August 2026

## Overview
Based on the NIS2 gap analysis (39% overall compliance),
this remediation plan prioritizes actions to achieve 
80% compliance within 6 months.

---

## Priority 1 — Critical (0-30 days)

### 1.1 Enforce MFA for All Users
**Gap**: 0% MFA compliance
**Risk**: Account takeover (demonstrated in Splunk lab)
**Action**:
- Enable MFA in Microsoft Entra ID for all accounts
- Prioritize privileged accounts first
- Enforce MFA for remote access
- Deploy authenticator app to all employees

**Cost**: €0 (included in Microsoft 365 license)
**Responsible**: IT Admin + CISO
**Deadline**: 15 days

---

### 1.2 Implement Security Awareness Training
**Gap**: No training program
**Risk**: Human error — primary attack vector
**Action**:
- Deploy annual security awareness training
- Phishing simulation quarterly
- Specific training: ransomware, social engineering
- Document completion for NIS2 evidence

**Cost**: ~€500/year (KnowBe4 or similar)
**Responsible**: HR + CISO
**Deadline**: 30 days

---

### 1.3 Test Incident Response Plan
**Gap**: IR plan not tested
**Risk**: Ineffective response during real incident
**Action**:
- Conduct tabletop exercise — ransomware scenario
- Involve all IR team members
- Document lessons learned
- Update IR plan based on findings

**Cost**: Internal time only
**Responsible**: CISO + DPO
**Deadline**: 30 days

---

## Priority 2 — High (30-90 days)

### 2.1 Business Continuity Plan
**Gap**: No BCP documented
**Risk**: Extended downtime during incident
**Action**:
- Define Recovery Time Objectives (RTO) per system
- Define Recovery Point Objectives (RPO) per system
- Document manual fallback procedures
- Test backup restoration monthly

**RTO targets for TechPay**:
| System | RTO Target | RPO Target |
|---|---|---|
| Payment gateway | 4 hours | 1 hour |
| Customer database | 8 hours | 4 hours |
| Internal systems | 24 hours | 24 hours |

**Cost**: Internal time + backup solution review
**Responsible**: CTO + CISO
**Deadline**: 60 days

---

### 2.2 Vulnerability Management Program
**Gap**: No vulnerability scanning
**Risk**: Unknown security exposures
**Action**:
- Deploy vulnerability scanner (Qualys, Nessus, or free OpenVAS)
- Monthly scans of all systems
- Critical vulnerabilities patched within 72 hours
- High vulnerabilities patched within 30 days
- Document scan results for NIS2 evidence

**Cost**: OpenVAS free / Qualys ~€2,000/year
**Responsible**: SOC Lead
**Deadline**: 60 days

---

### 2.3 Supply Chain Security
**Gap**: No supplier security assessments
**Risk**: Third party breach affecting TechPay
**Action**:
- Create supplier security questionnaire
- Annual assessment of critical suppliers
- Include security clauses in all new contracts
- Review existing DPAs for security requirements

**Critical suppliers to assess**:
- Jumio (KYC provider)
- Payment network processors
- Cloud providers (Microsoft Azure)
- Mailchimp (email marketing)

**Cost**: Internal time
**Responsible**: DPO + Legal + Procurement
**Deadline**: 90 days

---

## Priority 3 — Medium (90-180 days)

### 3.1 Network Segmentation
**Gap**: Flat network architecture
**Risk**: Lateral movement during attack
**Action**:
- Segment payment systems from general network
- Implement firewall rules between segments
- Restrict access to payment systems by IP
- Monitor inter-segment traffic

**Cost**: ~€5,000 (firewall configuration)
**Responsible**: IT Admin + CTO
**Deadline**: 120 days

---

### 3.2 Formal Security Policies
**Gap**: Policies not formally approved
**Action**:
- Information Security Policy — board approved
- Acceptable Use Policy — all employees sign
- Password Policy — minimum requirements
- Remote Work Policy — security requirements
- Annual review cycle established

**Cost**: Internal time + legal review
**Responsible**: CISO + DPO + Legal
**Deadline**: 120 days

---

### 3.3 Privileged Access Management
**Gap**: No formal PAM solution
**Action**:
- Implement Just-In-Time (JIT) access for admin roles
- Review privileged accounts quarterly
- Remove standing admin access where possible
- Log all privileged actions to Sentinel

**Cost**: Included in Entra ID P2 license
**Responsible**: IT Admin + CISO
**Deadline**: 180 days

---

## Remediation Timeline

Month 1
├── MFA enforced for all users
├── Security awareness training deployed
└── IR plan tabletop exercise completed

Month 2-3
├── Business continuity plan documented
├── Vulnerability management operational
└── Supplier assessments initiated

Month 4-6
├── Network segmentation implemented
├── Formal policies board-approved
└── PAM solution deployed


## Expected Compliance After Remediation

| Article | Current | After 6 months |
|---|---|---|
| 21.2.a Risk analysis | 60% | 85% |
| 21.2.b Incident handling | 75% | 95% |
| 21.2.c Business continuity | 25% | 80% |
| 21.2.d Supply chain | 35% | 75% |
| 21.2.e Network security | 20% | 70% |
| 21.2.f Cryptography | 65% | 85% |
| 21.2.g HR security | 30% | 85% |
| 21.2.h MFA | 0% | 100% |
| **TOTAL** | **39%** | **84%** |
