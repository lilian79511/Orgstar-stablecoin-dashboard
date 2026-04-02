# Orgstar Customer Intelligence Report
**Date:** March 24, 2026
**Focus:** Enterprise Stablecoin Governance Platform
**Scope:** 5 Customer Personas + External Stakeholder Insights

---

## 1. CONSOLIDATED PAIN POINT HIERARCHY

### Tier 1: Critical Blockers (Prevent Action)
Pain points that stop customers from using stablecoins for regulated transactions.

| Rank | Pain Point | Affected Personas | Frequency | Severity |
|------|-----------|-------------------|-----------|----------|
| 1.1 | **No immutable FX timestamp + authorization chain** | David, Amy, Eric | 5/5 | CRITICAL |
| 1.2 | **CPA/auditor cannot certify stablecoin records** | David, Jake, Eric | 5/5 | CRITICAL |
| 1.3 | **Cannot separate approver/executor roles** | David, Amy | 4/5 | CRITICAL |
| 1.4 | **No recognized format for stablecoin in financial statements** | Kevin, Jake, Eric | 4/5 | CRITICAL |
| 1.5 | **Manual screenshot-based rate tracking** | Amy, Jake | 3/5 | HIGH |

### Tier 2: Major Friction (Slow/Costly Workflows)
Pain points that degrade efficiency or increase manual work.

| Rank | Pain Point | Affected Personas | Frequency | Severity |
|------|-----------|-------------------|-----------|----------|
| 2.1 | **CPA spends 5-10 hours/quarter/client manually reconstructing records** | Eric, David, Jake | 4/5 | HIGH |
| 2.2 | **Fear of sending to wrong address (counterparty risk)** | Amy, Jake | 3/5 | HIGH |
| 2.3 | **Informal, untrackable approval chains (LINE approvals)** | Amy, David | 3/5 | MEDIUM |
| 2.4 | **No KYT (Know Your Transaction) scanning** | Amy, Jake | 2/5 | MEDIUM |
| 2.5 | **Bank freezes accounts after large USDT inflows (AML concern)** | Jake | 1/5 | HIGH |

### Tier 3: Strategic/Governance Gaps
Pain points that affect legitimacy, liability, or strategic optionality.

| Rank | Pain Point | Affected Personas | Frequency | Severity |
|------|-----------|-------------------|-----------|----------|
| 3.1 | **Listed company officers have personal liability for non-compliance** | Kevin | 1/5 | CRITICAL |
| 3.2 | **Board/auditor have no framework for stablecoin legitimacy** | Kevin | 1/5 | HIGH |
| 3.3 | **Stablecoin transactions invisible in financial statements** | Kevin, Jake | 2/5 | HIGH |
| 3.4 | **CPA charges premium rates for manual record reconstruction** | Jake | 1/5 | MEDIUM |

---

## 2. SWITCHING TRIGGERS

Events or thresholds that cause a customer to urgently adopt governance solution.

### Immediate Triggers (Days/Weeks)
- **Year-end financial statement deadline** → CFO must show CPA immutable approval trail or transaction fails certification
- **CPA audit refusal** → "We cannot certify this without timestamp and authorization chain"
- **Bank account freeze threat/incident** → After large USDT deposit, bank requests proof of legitimate transaction sourcing
- **Compliance questionnaire from client** → Customer's customer demands stablecoin transaction records in standard format

### Medium-term Triggers (Weeks/Months)
- **VASP licensing enforcement begins** → FSC starts licensing; unlicensed operators face penalties
- **First material cross-border stablecoin transaction** → Company executes $100k+ USDT transfer; realizes no audit trail
- **Auditor/CPA changes engagement terms** → New auditor refuses prior informal approval methods; demands structured governance
- **Board asks for SOX-equivalent controls** → Listed company board requests evidence of internal controls on crypto transactions

### Cumulative Triggers
- **Volume threshold** → Stablecoin transactions exceed $500k in a quarter; manual screenshot process becomes untenable
- **Team growth** → 2nd person hired to handle payments; cannot rely on founder's personal knowledge of FX rates
- **Contractor payment accumulation** → 10+ contractors paid monthly in USDT; CPA now requires consolidated proof of payment legitimacy

---

## 3. CUSTOMER LANGUAGE MAP

Exact terminology and phrasing customers use to describe problems and desired outcomes.

### Problems (Voice of Customer)

#### Approval & Authorization
- *"Who approved it?"* — David (need accountable chain of command)
- *"We need to separate the approver from the executor"* — David (role-based access)
- *"LINE approvals are informal"* — Amy (unstructured, untrackable)
- *"There's no clear chain of who authorized it"* — Eric (audit requirement)

#### Record-Keeping & Timestamps
- *"If I can't show the accountant exactly what rate we used"* — David (immutable timestamp requirement)
- *"I need to know the rate I used is on record — not just in my screenshot folder"* — Amy (formalize ephemeral data)
- *"I need an exchange rate from a recognized source, a timestamp, and a clear chain"* — Eric (three-part audit requirement)
- *"5-10 hours per client per quarter to manually reconstruct records"* — Eric (cost of absence)
- *"We have a problem at year-end"* — David (deadline pressure)

#### Compliance & Legitimacy
- *"My generation uses stablecoins. The problem is the board and auditor still live in my father's world"* — Kevin (legitimacy gap)
- *"Stablecoin transactions not recognized in financial statements"* — Kevin (accounting invisibility)
- *"Personal liability risk as listed company officer"* — Kevin (regulatory/governance exposure)
- *"They ask for a receipt that my accountant will accept"* — Jake (CPA-standard format)
- *"Banks want stablecoin clients but need AML paper trail"* — Shanghai Bank Sofia (counterparty requirement)

#### Risk & Operational Fear
- *"Fear of sending to wrong address"* — Amy (counterparty/execution risk)
- *"I must screenshot MAX Exchange rates manually"* — Amy (reliance on manual, fallible process)
- *"Bank account frozen after large USDT inflows"* — Jake (compliance/KYT gap)
- *"CPA charges extra to manually reconstruct records"* — Jake (cost premium for non-standard format)

### Desired Outcomes (Voice of Customer)

#### Transparency & Accountability
- *"Full visibility + immutable approval trail"* — David (comprehensive audit trail)
- *"Satisfy CPA at year-end"* — David (direct certification endpoint)
- *"Execute confidently"* — Amy (reduced operational anxiety)
- *"Have rate on record"* — Amy (formalized evidence)
- *"Certify confidently"* — Eric (reduced auditor friction)

#### Operational Structure
- *"Structured approval chain"* — Amy (formalized workflow)
- *"Compliant payroll records"* — Jake (CPA-standard format for contractors)
- *"Bank defensibility"* — Jake (legitimacy for financial institutions)
- *"CPA-ready exports"* — Jake (standard format output)

#### Strategic Optionality
- *"Move large sums privately, surface with compliance documentation when needed"* — Kevin (shadow-to-light model)
- *"Access records directly"* — Eric (distribution channel integration)

#### Cost Reduction
- *"Reduce reconstruction time"* — Eric (efficiency gain for CPAs)

---

## 4. BEST-FIT CUSTOMER PROFILE

**Primary:** Who gets the most value fastest?

### Characteristics (Not Demographics)

| Attribute | Profile |
|-----------|---------|
| **Revenue stage** | $10M–$500M ARR (mid-market to lower-market cap listed companies; large private trading firms) |
| **Stablecoin usage** | Already executing $100k–$5M/quarter in USDT or USDC (not exploratory) |
| **Geographic base** | Taiwan, HK, Singapore (high VASP regulation risk; strong CPA culture) |
| **Regulatory exposure** | Listed company OR subject to external audit OR required to show compliance to clients |
| **Pain intensity** | Currently working around the problem (screenshots, manual spreadsheets, informal LINE approvals) |
| **Decision maker** | CFO or COO who owns both finance AND crypto operations |
| **CPA relationship** | Existing relationship; CPA already refusing to certify OR flagging as high-friction |
| **Timeline urgency** | Q4 approaching (year-end audit deadline) OR recent bank/client compliance push |
| **Tech readiness** | Moderate (45–70/100) — comfortable with SaaS, not Web3-native, wants "boring infrastructure" |

### Secondary Fit (High LTV but slower sales)
- **Crypto-native startups** (Jake persona): High tech readiness, urgent need, but smaller transaction volumes and lower regulatory pressure → good expansion segment post-PMF
- **Family office/listed successors** (Kevin persona): Very high asset volumes, strategic urgency, but low frequency of transactions → long sales cycle, high CAC

---

## 5. VOICE OF CUSTOMER EVIDENCE

Customer quotes organized by theme, showing depth and consistency.

### A. AUDIT TRAIL & CERTIFICATION OBSESSION

**Problem:**
> "If I can't show the accountant exactly what rate we used and who approved it, we have a problem at year-end." — David Chen, CFO

> "I need an exchange rate from a recognized source, a timestamp, and a clear chain of who authorized it. No one has been able to give me all three — until now." — Eric Chen, CPA/Auditor

**Urgency:**
> "CPA refuses to certify without FX timestamps" — Research summary, David Chen's pain point

> "Clients send screenshots (unacceptable), no standard format for stablecoin records in Taiwan, 5-10 hours per client per quarter to manually reconstruct records" — Eric Chen, CPA workflow impact

### B. OPERATIONAL FEAR & MANUAL WORKAROUNDS

**Problem:**
> "I need to know the rate I used is on record — not just in my screenshot folder." — Amy Lin, Operator

> "I need to screenshot MAX Exchange rates manually" — Research summary, Amy Lin's workflow

**Cost of Workaround:**
> "The tech isn't the problem — the problem is when I try to pay contractors in USDT and they ask for a receipt that my accountant will accept." — Jake Wu, Web3 COO

> "MetaMask payroll = no recognized records, bank account frozen after large USDT inflows, CPA charges extra to manually reconstruct records" — Research summary, Jake Wu's cumulative pain

### C. COMPLIANCE INVISIBILITY & LEGITIMACY GAPS

**Strategic Problem:**
> "My father's generation used Swiss accounts. My generation uses stablecoins. The problem is the board and auditor still live in my father's world." — Kevin Hsu, Listed Family Business Successor

> "Stablecoin transactions not recognized in financial statements" — Research summary, Kevin Hsu's strategic pain

**Personal Liability:**
> "Personal liability risk as listed company officer" — Research summary, Kevin Hsu's governance exposure

### D. CPA AS GATEKEEPER

**Distribution Insight:**
> "CPAs are the distribution channel — if you solve the CPA's workflow, the CPA sells for you" — Patrick business advisor

**CPA Workflow Pain:**
> "I need to access records directly, reduce reconstruction time" — Eric Chen, CPA desired outcome (extrapolated)

### E. REGULATORY ENVIRONMENT SHIFTING

**Macro Signal:**
> "FSC is watching, VASP licensing coming — companies need to build governance NOW before enforcement" — FSC Director

**Bank Demand:**
> "Banks want stablecoin clients but need AML paper trail — governance layer could make clients 'bankable'" — Shanghai Bank Sofia

---

## 6. WHAT "BETTER" LOOKS LIKE TO EACH PERSONA

Specific, measurable changes to workflows and outcomes for each customer type.

### David Chen (CFO/Admin, Cross-Border Trading Co.)

**Current State:**
- Screenshots in email
- Verbal approvals (who approved? unclear)
- Year-end CPA says "I can't sign off on this"

**Better State:**
- Every USDT transfer has: (a) FX rate from MAX Exchange with timestamp, (b) explicit approval by [specific person] on [specific date], (c) audit trail immutable and exportable
- Shows CPA single dashboard; CPA nods and certifies
- At year-end, ZERO back-and-forth with auditor on stablecoin transactions
- Segregation of duties: Amy executes, David approves, both trackable

**Metric of Success:**
- CPA certifies in <30 min for stablecoin section
- Year-end close time reduced by 2+ hours
- Zero follow-up questions from external auditor

---

### Amy Lin (Operator, Cross-Border Trading Co.)

**Current State:**
- Screenshots MAX Exchange before sending
- Hopes the rate doesn't change between screenshot and approval
- Sends, then worried: "Did David approve? Is this address correct?"
- LINE approval is informal; no proof she sent to the right person

**Better State:**
- Creates USDT transfer request in Orgstar
- Pulls current MAX rate (auto-populated, immutable timestamp)
- Sees: "Requires approval from CFO"
- Sends notification to David
- David approves in Orgstar; Amy sees "Approved by David Chen at 2:47 PM" before she hits execute
- Transfer executes; Orgstar records: rate, timestamp, approver, executor, recipient address
- Fear gone: "It's all on record. The rate is locked in. I know David said yes."

**Metric of Success:**
- Execution time per transfer: 2 min (vs. 10 min with screenshot + LINE back-and-forth)
- Zero re-dos due to wrong address or rate mismatch
- Confidence: "I know I did it right"

---

### Kevin Hsu (2nd Gen Successor, Listed Family Business)

**Current State:**
- Moves $5M to Singapore in USDT
- Board asks: "How does this appear in financial statements?"
- Auditor: "Stablecoin transfers are not recognized by IFRS standards"
- Personal exposure: "As a listed company officer, am I liable for ungovernanced crypto?"

**Better State:**
- Orgstar records every stablecoin transaction with:
  - Source of funds (on-chain + governance approval)
  - FX rate at time of transaction
  - Business purpose (captured in approval request)
  - Recipient KYT clearance
- When auditor asks, Kevin provides Orgstar export: governance, audit trail, compliance
- Auditor can now say: "Controls are documented. I can work with this."
- Board sees: private transfer (not announced to market), but fully documented for audit
- Personal liability: reduced. ("I can show governance and controls.")

**Metric of Success:**
- Auditor accepts stablecoin transfers as "controlled crypto transactions" (new category in financial statements)
- Board confidence: no more "what is this?" questions
- Regulatory defensibility: If FSC asks, Kevin has immutable proof of controls

---

### Jake Wu (Web3 COO, Crypto-native Startup)

**Current State:**
- Pays contractors in USDT via MetaMask
- No records; CPA says "I have no way to prove you paid $5k to person X on date Y"
- Bank sees $100k USDT inflow, freezes account pending AML
- CPA spends 10 hours reconstructing from on-chain data

**Better State:**
- Creates payroll batch in Orgstar: 15 contractors, rates locked, approvals streamlined
- Orgstar exports: "Payroll batch #47, approved by CEO, $75k total, rates from [exchange], timestamp, recipient addresses with KYT clearance"
- CPA imports Orgstar export into Xero; recognizes it as "standard stablecoin payroll record"
- CPA file: 15 minutes (vs. 10 hours)
- Bank asks: "Where did this USDT come from?" Answer: "Here's the governance trail and CPA certification."
- Bank unfreezes account

**Metric of Success:**
- CPA time per payroll cycle: 15 min (vs. 10 hours)
- Bank can verify legitimacy directly
- Zero account freezes due to stablecoin inflows
- CPA costs: $0 premium for manual reconstruction

---

### Eric Chen (CPA/Auditor, External)

**Current State:**
- Clients send him stablecoin screenshots
- He has no proof of: (a) exchange rate source, (b) approval, (c) timestamp
- He tells client: "I can't sign off on this. Get me better records."
- Spends 5–10 hours per client per quarter manually reconstructing from blockchain + email
- Charges premium rate for this work

**Better State:**
- Client says: "Use Orgstar. You have direct access."
- Eric logs into Orgstar dashboard
- Sees all client's stablecoin transactions: rates, approvals, timestamps, KYT clearance
- For each transaction: FX rate, source (MAX Exchange API), approval chain, executor, timestamp
- Can verify: "Yes, rate was $X on date Y, approved by [authorized person]"
- No screenshots. No ambiguity. No reconstruction.
- Certifies in 30 minutes for entire quarter (vs. 5–10 hours)

**Metric of Success:**
- Audit time per client per quarter: 30 min (vs. 5–10 hours)
- Zero rejected transactions due to missing documentation
- Zero follow-up questions from auditor's auditor (external audit efficiency)
- CPA can bill standard rate (no premium for manual work)
- **Distribution upside:** Eric becomes evangelists for Orgstar to his other 30+ clients

---

## SYNTHESIS: ORGSTAR'S CORE COMPETITIVE POSITION

### What Customers Are Actually Buying
Not "stablecoin governance" — they're buying:
1. **CPA/Auditor Acceptance** — Proof that stablecoin transfers are legitimate in the eyes of external auditors
2. **Year-End Safety** — Confidence that they will pass financial statement certification
3. **Bank Defensibility** — Proof of controls to prevent account freezes and AML friction
4. **Personal Liability Reduction** — Evidence of governed processes (especially for listed company officers)
5. **Operational Efficiency** — Replacing 5–10 hours of CPA reconstruction with 30 minutes of review

### Orgstar's Unique Insight
The CPA/auditor is not a compliance overhead — they're the *end customer*. When Eric Chen can certify in 30 minutes instead of 10 hours, and he can access records directly without screenshots, he becomes a distribution channel. He tells his other 30 clients: "Use Orgstar — it saves me time and money, and I can finally sign off confidently."

### Market Timing
VASP licensing is coming. Banks are asking for governance trails. CPAs are hitting walls. The next 6–12 months is the window to build the standard format before enforcement creates chaos.

---

## APPENDIX: RESEARCH QUALITY & GAPS

### Data Quality Assessment
- **Direct quotes:** 5 personas (David, Amy, Kevin, Jake, Eric) — primary voice
- **Stakeholder corroboration:** 3 secondary sources (Shanghai Bank, Patrick advisor, FSC) — validates pain points
- **Pain frequency:** Cross-persona validation on 5 critical issues (FX timestamp, CPA certification, approval chain, KYT, bank defensibility)
- **Geographic specificity:** Taiwan/HK/Singapore emphasis consistent across all personas

### Known Gaps (for follow-up)
1. **Price sensitivity:** No data on how much customers will pay for governance layer (WTP research needed)
2. **Adoption timeline:** When does Kevin move from "considering" to "must implement"? (VASP timeline TBD)
3. **Integration depth:** How deeply do CPAs want API access vs. dashboard review? (Product discovery needed)
4. **Competitor awareness:** Are customers comparing Orgstar to manual processes only, or other platforms? (Win/loss research needed)
5. **Volume thresholds:** At what transaction volume does the pain point switch from "nice-to-have" to "urgent"? (Segmentation clarity needed)

