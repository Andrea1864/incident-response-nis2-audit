# Ransomware Response Playbook — TechPay Solutions
## Scenario: Ransomware Attack on Payment Infrastructure

## Scenario Description
TechPay's payment processing server is encrypted by ransomware.
Employees cannot access the payment gateway. A ransom note 
demands 50 BTC. Customer transactions are failing.

---

## Immediate Response (0-15 minutes)

### Step 1 — Detect and Confirm

Employee reports files encrypted / ransom note visible
↓
SOC Lead confirms ransomware (NOT a false alarm)
↓
CISO and DPO notified immediately
↓
IR team activated — P1 Critical incident declared


### Step 2 — Isolate (DO NOT turn off systems)
- Disconnect affected servers from network (unplug cable)
- Disable affected user accounts in Entra ID
- Block lateral movement — isolate network segments
- Do NOT power off — forensic memory evidence preserved

### Step 3 — Preserve Evidence
- Screenshot ransom note with timestamp
- Export Splunk/Sentinel logs immediately
- Document all affected systems
- Note exact time of discovery

---

## Short-term Response (15 min — 4 hours)

### Step 4 — Assess Scope

Which systems are encrypted?
↓
Has data been exfiltrated? (double extortion?)
↓
Are backups intact and unaffected?
↓
What customer data is at risk?
↓
Is payment processing completely stopped?


### Step 5 — Activate Business Continuity
- Switch to manual payment processing if possible
- Notify key customers of service disruption
- Activate backup systems if available
- Communicate internally — do NOT email (may be compromised)

### Step 6 — Legal Notifications (critical timeline)

| Notification | Deadline | Responsible |
|---|---|---|
| NIS2 Early Warning → INCIBE-CERT | 24 hours | CISO |
| GDPR Art. 33 → AEPD | 72 hours | DPO |
| DORA → Banco de España | 4 hours initial | CISO + Legal |
| Board of Directors | 2 hours | CEO + CISO |

---

## DO NOT PAY THE RANSOM

Reasons:
- No guarantee data will be recovered
- Funds criminal organisations
- May violate sanctions (if attacker is sanctioned entity)
- Marks TechPay as a paying target
- Legal and reputational risk

---

## Recovery Phase (4 hours — 7 days)

### Step 7 — Eradication
- Identify ransomware variant (use VirusTotal, ID Ransomware)
- Remove all malware from affected systems
- Patch exploited vulnerabilities
- Reset ALL credentials (assume all compromised)

### Step 8 — Restore from Backup

Verify backup integrity BEFORE restoring
↓
Restore to clean environment (not original infected)
↓
Test restored systems before reconnecting
↓
Monitor for 30 days post-recovery
↓
Gradually restore services


### Step 9 — Post-Incident

- Lessons learned meeting within 5 days
- NIS2 Final Report → INCIBE-CERT within 1 month
- GDPR Art. 34 — assess if individuals need notification
- Update security controls based on attack vector
- Consider cyber insurance claim

---

## GDPR Breach Assessment

| Question | If YES → Action |
|---|---|
| Was personal data encrypted? | Art. 33 — Notify AEPD within 72h |
| Was personal data exfiltrated? | Art. 33 + Art. 34 — Notify individuals |
| Was special category data affected? | Higher urgency notification |
| Were payment card numbers affected? | PCI-DSS breach notification also required |

## MITRE ATT&CK — Ransomware Kill Chain
| Phase | Technique | TechPay Example |
|---|---|---|
| Initial Access | T1566 Phishing | Malicious email attachment |
| Execution | T1204 User Execution | Employee opens attachment |
| Persistence | T1547 Boot Autostart | Malware persists on restart |
| Lateral Movement | T1021 Remote Services | Spreads to payment server |
| Exfiltration | T1041 C2 Channel | Data sent before encryption |
| Impact | T1486 Data Encrypted | Files encrypted, ransom note |
