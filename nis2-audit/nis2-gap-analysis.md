# NIS2 Directive Gap Analysis — TechPay Solutions
## EU Directive 2022/2555 | August 2026

## Company Classification
TechPay Solutions S.L. qualifies as an **Important Entity** 
under NIS2 Directive Art. 3 because it provides digital 
payment services and operates in the financial sector.

As an Important Entity, TechPay must comply with:
- Art. 21 — Cybersecurity risk management measures
- Art. 23 — Incident reporting obligations
- Art. 24 — Use of certified ICT products and services

---

## NIS2 Art. 21 — Risk Management Requirements

### 21.2.a — Policies on risk analysis and information security

| Requirement | Status | Evidence | Gap |
|---|---|---|---|
| Risk analysis policy documented | ✅ Partial | ISO 27001 ROPA | No formal risk register |
| Information security policy | ✅ Yes | Azure Policy | Not formally approved |
| Policy review annually | ❌ No | — | No review process defined |

**Gap score: 60% compliant**

---

### 21.2.b — Incident handling

| Requirement | Status | Evidence | Gap |
|---|---|---|---|
| Incident response plan | ✅ Yes | ir-plan.md | Not tested |
| Incident classification | ✅ Yes | P1-P4 matrix | — |
| Ransomware playbook | ✅ Yes | ransomware-playbook.md | — |
| IR team defined | ✅ Yes | IR team roles | — |
| Incident drills conducted | ❌ No | — | No tabletop exercises |

**Gap score: 75% compliant**

---

### 21.2.c — Business continuity and crisis management

| Requirement | Status | Evidence | Gap |
|---|---|---|---|
| Business continuity plan | ❌ No | — | Not documented |
| Backup and recovery procedures | ✅ Partial | Azure backups | Not tested |
| Crisis management procedures | ❌ No | — | Not documented |
| Recovery time objectives (RTO) defined | ❌ No | — | Not defined |

**Gap score: 25% compliant**

---

### 21.2.d — Supply chain security

| Requirement | Status | Evidence | Gap |
|---|---|---|---|
| Third party processor register | ✅ Yes | ROPA third party list | — |
| Supplier security assessments | ❌ No | — | No formal assessment |
| Contractual security requirements | ✅ Partial | DPAs signed | No security clauses |
| Supplier monitoring | ❌ No | — | No ongoing monitoring |

**Gap score: 35% compliant**

---

### 21.2.e — Security in network and information systems

| Requirement | Status | Evidence | Gap |
|---|---|---|---|
| Network segmentation | ❌ No | — | Flat network |
| Access control policy | ✅ Yes | Entra ID RBAC | — |
| Vulnerability management | ❌ No | — | No scan schedule |
| Patch management | ❌ No | — | No formal process |
| Endpoint protection | ❌ No | — | Not documented |

**Gap score: 20% compliant**

---

### 21.2.f — Policies on use of cryptography

| Requirement | Status | Evidence | Gap |
|---|---|---|---|
| Encryption policy | ✅ Partial | Key Vault RSA 2048 | Not formally documented |
| Key management policy | ✅ Yes | key-management-policy.md | — |
| Encryption in transit | ✅ Yes | TLS 1.3 | — |
| Encryption at rest | ✅ Partial | Azure encryption | Not verified on all systems |

**Gap score: 65% compliant**

---

### 21.2.g — Human resources security and access control

| Requirement | Status | Evidence | Gap |
|---|---|---|---|
| Security awareness training | ❌ No | — | No training program |
| Background checks | ❌ No | — | Not documented |
| Privileged access management | ✅ Partial | Entra ID roles | No PAM solution |
| Offboarding procedure | ✅ Partial | Leaver process | Not formally tested |

**Gap score: 30% compliant**

---

### 21.2.h — Multi-factor authentication

| Requirement | Status | Evidence | Gap |
|---|---|---|---|
| MFA for all users | ❌ No | — | Not enforced |
| MFA for privileged accounts | ❌ No | — | Not enforced |
| MFA for remote access | ❌ No | — | Not enforced |

**Gap score: 0% compliant** ⚠️ Critical gap

---

## Overall NIS2 Compliance Score

| Article | Requirement | Compliance |
|---|---|---|
| 21.2.a | Risk analysis | 60% |
| 21.2.b | Incident handling | 75% |
| 21.2.c | Business continuity | 25% |
| 21.2.d | Supply chain | 35% |
| 21.2.e | Network security | 20% |
| 21.2.f | Cryptography | 65% |
| 21.2.g | HR security | 30% |
| 21.2.h | MFA | 0% |
| **TOTAL** | **Overall** | **39%** |

---

## Critical Gaps (Must Fix Immediately)

1. **MFA not enforced** — 0% compliance, highest risk
2. **No business continuity plan** — regulatory requirement
3. **No vulnerability management** — network exposure unknown
4. **No security awareness training** — human risk unmitigated
5. **No supplier security assessments** — supply chain risk

---

## NIS2 Art. 23 — Incident Reporting Obligations

| Report Type | Deadline | Content |
|---|---|---|
| Early warning | 24 hours | Incident occurred, suspected cause |
| Incident notification | 72 hours | Detailed impact assessment |
| Intermediate report | On request | Progress update |
| Final report | 1 month | Full analysis, measures taken |

**Reporting authority for Spain**: INCIBE-CERT
**Portal**: `incibe-cert.es`
