# Orgstar — Pencil.dev Mega Prompt
# Enterprise Stablecoin Governance System

---

## HOW TO USE THIS PROMPT

Paste the contents of any **[SCREEN PROMPT]** block directly into Pencil.dev.
For best results, generate screens in order — each screen builds on the last.
Use the **[GLOBAL DESIGN SYSTEM]** section as the base context for every generation.

---

---

# ─── GLOBAL DESIGN SYSTEM ───────────────────────────────────────────────────

```
PRODUCT: Orgstar (橙星) — Enterprise Stablecoin Governance Platform
TAGLINE: Web2 control strictness. Web3 settlement transparency.
PLATFORM: Web app (desktop-first, 1440px wide, responsive to 1280px)
INDUSTRY: B2B Fintech / Enterprise Treasury / Blockchain Compliance
TONE: Institutional trust. Clean precision. Serious but not cold.

DESIGN LANGUAGE:
- Style: Modern enterprise SaaS — clean, structured, data-dense but breathable
- NOT crypto-bro. NOT DeFi neon. Think Bloomberg Terminal meets Stripe Dashboard.
- Dark sidebar navigation, light content area
- Micro-interactions matter: status transitions, loading states, confirmation steps
- Every action that touches money must feel deliberate and safe

COLOR PALETTE:
- Primary Navy: #1B3A5C (sidebar, headers, primary buttons)
- Teal Accent: #0D6E8A (interactive elements, links, highlights)
- Orange Brand: #E07B29 (CTAs, badges, brand moments)
- Background: #F5F7FA (content area base)
- Card White: #FFFFFF
- Light Blue: #EAF4F8 (info panels, insight boxes)
- Mid Blue: #D0E8F0 (table row alternates, borders)
- Success Green: #1A7F5A
- Warning Amber: #D97706
- Error Red: #DC2626
- Text Primary: #111827
- Text Secondary: #6B7280
- Border: #E5E7EB

TYPOGRAPHY:
- Font: Inter (primary), with monospace (JetBrains Mono) for wallet addresses, tx hashes, amounts
- Heading 1: 28px / 700 / #111827
- Heading 2: 22px / 600 / #1B3A5C
- Heading 3: 16px / 600 / #111827
- Body: 14px / 400 / #374151
- Caption: 12px / 400 / #6B7280
- Mono: 13px / 500 / JetBrains Mono / #1B3A5C

GRID & SPACING:
- Layout: 16px base unit, 8px grid
- Sidebar: 240px fixed
- Content area: max-width 1160px, centered
- Card padding: 24px
- Section gaps: 32px
- Table row height: 52px

COMPONENT TOKENS:
- Border radius: 8px (cards), 6px (inputs), 4px (badges), 20px (pills)
- Shadow: 0 1px 3px rgba(0,0,0,0.08), 0 4px 16px rgba(0,0,0,0.06)
- Input height: 40px
- Button height: 40px (primary), 36px (secondary)
- Status badge: pill shape, 12px font, colored background + text

NAVIGATION STRUCTURE (Left Sidebar):
- Logo: Orgstar (橙星) + orange star icon, top left
- Section: OVERVIEW → Dashboard
- Section: TRANSACTIONS → Initiate Transfer / Transaction History / Pending Approvals
- Section: COMPLIANCE → KYT Scan / Audit Log / Accounting Export
- Section: SETTINGS → Team & Roles / Wallet Management / Company Profile
- Bottom: User avatar + role badge + logout

USER ROLES (shown as colored badges):
- Admin / CFO: Navy badge #1B3A5C
- Operator: Teal badge #0D6E8A
- Approver: Purple badge #7C3AED
- Viewer / Auditor: Gray badge #6B7280

KEY UX PRINCIPLES:
- Every irreversible action requires a 2-step confirmation modal
- Show real-time status throughout multi-step flows
- Wallet addresses always truncated: 0x1234...5678, with copy icon
- All amounts show currency symbol + stablecoin denomination (e.g. TWD / USDT)
- FX rates always timestamped (e.g. "Rate locked: 1 USDT = 31.42 TWD @ 14:32:07 CST")
- Compliance badges on every transaction row (KYT status, approval chain)
```

---

---

# ─── SCREEN 1: DASHBOARD ─────────────────────────────────────────────────────

## [SCREEN PROMPT — DASHBOARD]

```
Design a desktop web app dashboard screen (1440px) for Orgstar, an enterprise stablecoin governance platform for B2B fintech.

LAYOUT:
- Dark navy left sidebar (240px) with navigation
- Light gray content area (#F5F7FA)
- Top header bar with page title "Dashboard" and user context (role badge + company name)

SIDEBAR CONTENTS:
- Orgstar logo (orange star + wordmark) at top
- Navigation items with icons: Dashboard (active, highlighted teal), Initiate Transfer, Transaction History, Pending Approvals, KYT Scan, Audit Log, Accounting Export, Team & Roles, Wallet Management
- Active state: left border teal accent, text white, background slightly lighter navy
- Bottom: User avatar circle + "David Chen" + "CFO / Admin" navy badge

MAIN CONTENT AREA — 4 KPI CARDS (top row):
1. "Total Volume (30d)" — $2,847,500 USDT — subtitle: "↑ 12.3% vs last month" in green
2. "Pending Approvals" — 3 — subtitle: "2 require your action" in amber, with orange badge
3. "KYT Risk Flags" — 0 — subtitle: "All clear — last scan 2h ago" in green
4. "Active Wallets" — 7 — subtitle: "3 corporate / 4 operational"

Cards: white, 8px radius, subtle shadow, 24px padding, icon on top-right corner of each card (colored to match status)

MIDDLE ROW — 2 panels side by side:
LEFT PANEL (60% width): "Recent Transactions" table
- Columns: Date/Time | From → To | Amount | Currency | Status | KYT | Actions
- Show 5 rows of realistic data:
  Row 1: Mar 18 14:32 | Shanghai Office → Tokyo Supplier | 45,000 | USDT | ● Completed | ✓ Clear | View
  Row 2: Mar 18 09:15 | HQ Treasury → Payroll Pool | 280,000 | USDT | ● Completed | ✓ Clear | View
  Row 3: Mar 17 16:48 | Operations → Vendor Payment | 12,500 | USDT | ⏳ Pending Approval | ✓ Clear | Review
  Row 4: Mar 17 11:20 | Treasury → Exchange Reserve | 500,000 | USDT | ⏳ Pending Approval | ⚠ Review | Review
  Row 5: Mar 16 08:05 | Payroll Pool → Staff Wallets | 95,000 | USDT | ● Completed | ✓ Clear | View
- Status pills: Completed = green pill, Pending = amber pill
- "View all transactions →" link at bottom

RIGHT PANEL (40% width): "Approval Queue" list
- Header: "Awaiting Your Review" + count badge "2"
- 2 approval cards stacked:
  Card A: Transaction #TXN-2847 | Amy Lin (Operator) initiated | 12,500 USDT | Vendor Payment | "Initiated 3h ago" | [Approve] [Reject] buttons
  Card B: Transaction #TXN-2851 | Amy Lin (Operator) initiated | 500,000 USDT | Exchange Reserve | KYT flag warning banner | [Review KYT] [Approve] [Reject] buttons
- Each card: white background, left border teal for normal, amber for flagged

BOTTOM ROW — Full width: "Monthly Transaction Volume" bar chart
- 6-month bar chart (Oct–Mar) in teal/navy bars
- Y-axis: USDT amounts (0 to 3M)
- Clean minimal chart, no gridlines excess
- Current month bar highlighted in orange

DESIGN LANGUAGE: Modern enterprise SaaS. Inter font. Trust-inspiring. Data-dense but breathable. Dark navy sidebar, light content area. Color palette: Navy #1B3A5C, Teal #0D6E8A, Orange #E07B29, Background #F5F7FA.
```

---

---

# ─── SCREEN 2: INITIATE TRANSFER ─────────────────────────────────────────────

## [SCREEN PROMPT — INITIATE TRANSFER (OPERATOR VIEW)]

```
Design a desktop web app screen (1440px) for "Initiate Transfer" — a multi-step stablecoin transaction form for an enterprise governance platform called Orgstar.

CONTEXT: This is the Operator role's primary action. Amy Lin (Operator) is initiating a USDT cross-border payment. The form must feel controlled, deliberate, and safe — not like a crypto wallet. Like a corporate banking wire form.

LAYOUT: Same dark navy sidebar (240px) as dashboard. "Initiate Transfer" active in nav. Content area with step indicator at top.

STEP INDICATOR (horizontal, top of content):
4 steps in a progress bar style:
[1 — Transfer Details] → [2 — KYT Scan] → [3 — Review & Submit] → [4 — Pending Approval]
Currently on Step 1. Step 1 is active (teal), others are gray.

FORM CONTENT (Step 1 — Transfer Details):
White card, 760px centered, 32px padding

FORM SECTION: "From"
- Label: "Source Wallet"
- Dropdown selector showing: "HQ Treasury Wallet" with address "0x1234...5678" (monospace) and balance "USDT 2,847,000"
- Wallet balance shown as a subtle tag

FORM SECTION: "To"
- Label: "Destination Wallet"
- Toggle tabs: [Saved Wallets] [Enter Address]
- Currently on "Saved Wallets" — show a searchable list/dropdown:
  Option 1: "Tokyo Supplier — Tanaka Trading Co." / 0xAbcd...1234 / Verified ✓ (green)
  Option 2: "Vendor Payment — Chen Electronics" / 0xEfgh...5678 / Verified ✓ (green)
  Option 3: "Exchange Reserve — MAX Exchange" / 0x9876...4321 / Verified ✓ (green)

FORM SECTION: "Amount"
- Input: "45,000" with USDT denomination selector on right
- Below amount: FX Reference row:
  "FX Reference Rate (MAX Exchange): 1 USDT = 31.42 TWD  |  Equivalent: TWD 1,413,900"
  Note: "Final rate locked at moment of execution" in gray caption
  Orange info icon with tooltip text

FORM SECTION: "Transaction Purpose"
- Label: "Business Purpose (required for compliance)"
- Dropdown: [Supplier Payment] [Payroll] [Operating Expense] [Capital Transfer] [Other]
- Currently selected: "Supplier Payment"

FORM SECTION: "Reference / Notes"
- Text input: "Q1 2026 component purchase — Invoice #INV-20260318-042"
- Character count: 72/200

FORM SECTION: "Required Approval"
- Read-only info box in light blue (#EAF4F8):
  "This transfer requires CFO approval before execution. Approver: David Chen (CFO/Admin)"
  Lock icon. Text: "You will be notified when approved. After approval, you will execute the final transfer."
  This explains the loopback execution mechanism.

BOTTOM: [Cancel] [Continue to KYT Scan →] buttons. Continue is navy primary button.

DESIGN LANGUAGE: Enterprise SaaS, Inter font, deliberate and safe feel, not a crypto wallet. Same color system as dashboard.
```

---

---

# ─── SCREEN 3: KYT SCAN ──────────────────────────────────────────────────────

## [SCREEN PROMPT — KYT SCAN STEP]

```
Design a desktop screen (1440px) for Step 2 "KYT Scan" of a multi-step stablecoin transfer flow for Orgstar, an enterprise governance platform.

CONTEXT: KYT = Know Your Transaction. Before submitting for CFO approval, the system auto-scans the destination wallet against global blacklists (Chainalysis / TRM Labs). This screen shows real-time scan results. Design two states — show the "All Clear" state primarily, with a small example of what a "Flag Detected" state looks like below as a reference panel.

SAME SIDEBAR AND STEP INDICATOR as previous screen. Step 2 is now active in the progress bar.

MAIN CONTENT (760px centered white card):

TOP: Transfer Summary (recap bar, gray background):
"Sending 45,000 USDT from HQ Treasury → Tokyo Supplier (Tanaka Trading Co.) 0xAbcd...1234"

SCAN STATUS PANEL — PRIMARY STATE (All Clear):
- Large centered status icon: green checkmark circle (64px)
- Heading: "KYT Scan Complete — No Issues Found"
- Subtext: "Destination wallet has been scanned against OFAC, UN Sanctions, Chainalysis KYT, and TRM Labs blacklists."
- Scan timestamp: "Scanned at 14:32:07 CST, March 18, 2026"
- Data source badge: "Powered by Chainalysis KYT" (small gray logo area)

SCAN DETAIL TABLE (4 rows):
| Check | Source | Result | Details |
| OFAC Sanctions | US Treasury | ✓ Pass | No match |
| UN Sanctions List | United Nations | ✓ Pass | No match |
| Chainalysis KYT Risk Score | Chainalysis | ✓ Pass | Risk Score: 2/100 (Low) |
| TRM Labs Blacklist | TRM Labs | ✓ Pass | No known association |

Table: clean, alternating light blue row (#EAF4F8) / white, green check icons

BELOW TABLE: Legal disclaimer in small gray text:
"KYT scan provides risk intelligence only. Orgstar does not guarantee compliance with all applicable regulations. Final compliance responsibility rests with the corporate entity."

SECONDARY REFERENCE PANEL (below, smaller, red-tinted, labeled "Example: Flag Detected State"):
- Red warning icon, "KYT Flag Detected — Review Required"
- Risk score: 78/100 (High Risk)
- Flag reason: "Wallet associated with known mixing service activity (Chainalysis)"
- Buttons: [Block This Transaction] [Request Compliance Review] [Override with Justification]
- Override warning: "Manual override creates audit trail and requires CFO written justification"

BOTTOM NAVIGATION:
[← Back to Transfer Details] [Submit for CFO Approval →] (navy primary button)

DESIGN LANGUAGE: Trust, transparency, institutional rigor. Clear/flag states visually distinct. Same color system.
```

---

---

# ─── SCREEN 4: CFO APPROVAL VIEW ─────────────────────────────────────────────

## [SCREEN PROMPT — CFO APPROVAL REVIEW]

```
Design a desktop screen (1440px) for the CFO approval screen in Orgstar — an enterprise stablecoin governance platform. This is what David Chen (CFO/Admin) sees when he receives a transfer request for approval.

CONTEXT: Segregation of duties is critical here. The CFO is the approver ONLY — not the executor. After approval, execution authority returns to the Operator (Amy). This screen must communicate gravity and responsibility.

SAME SIDEBAR (David Chen / CFO / Admin is logged in, "Pending Approvals" is the active nav item).

PAGE HEADER: "Pending Approvals" — badge count "3"

APPROVAL REQUEST CARD (primary focus, full-width, white card with navy left border 4px):

TOP ROW of card:
- Left: Transaction ID "TXN-2847" in monospace, navy
- Right: Status pill "Awaiting CFO Approval" amber
- Submitted: "Submitted by Amy Lin (Operator) — 3 hours ago"

TRANSFER DETAILS SECTION (2-column grid inside card):
Left column:
- Source Wallet: HQ Treasury Wallet / 0x1234...5678 / Balance: 2,847,000 USDT
- Destination: Tokyo Supplier — Tanaka Trading Co. / 0xAbcd...1234
- Amount: 45,000 USDT
- TWD Equivalent: TWD 1,413,900 (at reference rate 31.42)
- Note: "Final FX rate locked at moment of execution, not at approval"

Right column:
- Business Purpose: Supplier Payment
- Reference: "Q1 2026 component purchase — Invoice #INV-20260318-042"
- KYT Status: ✓ All Clear (green badge) — Scanned 14:32 CST, Mar 18
- Chainalysis Risk Score: 2/100 (Low)

AUDIT TRAIL (timeline component, left-aligned with vertical line):
- ● Mar 18, 11:45 — Amy Lin initiated transfer request
- ● Mar 18, 14:32 — KYT scan completed (All Clear)
- ● Mar 18, 14:33 — Submitted to CFO for approval
- ○ [Pending] — CFO approval
- ○ [Pending] — Amy Lin executes final transfer
- ○ [Pending] — On-chain settlement

INFO BOX (light blue #EAF4F8, below audit trail):
Icon: lock
Text: "After your approval, Amy Lin (Operator) will be notified to execute this transfer. The CFO does not execute transfers directly — this ensures segregation of duties."

APPROVAL ACTIONS (bottom of card, right-aligned):
- [Reject Transfer] — outlined red button
- [Request More Info] — outlined gray button
- [Approve Transfer] — large navy primary button

APPROVE BUTTON → triggers a confirmation modal:
Modal title: "Confirm CFO Approval"
Body: "You are approving transfer of 45,000 USDT to Tanaka Trading Co. This action is recorded on the immutable audit log and will notify Amy Lin to execute the transfer."
Input: "CFO Signature / PIN" field (4-digit or text)
Buttons: [Cancel] [Confirm Approval]

SECONDARY: Below the main card, show 2 more smaller pending cards in a list (collapsed):
- TXN-2851: 500,000 USDT | KYT ⚠ Flag | "Expand to review"
- TXN-2839: 95,000 USDT | Payroll | KYT ✓ Clear | "Expand to review"

DESIGN LANGUAGE: Gravity and deliberateness. Every element communicates this is an irreversible decision. Dark navy accents, clear audit trail, institutional trust.
```

---

---

# ─── SCREEN 5: LOOPBACK EXECUTION ────────────────────────────────────────────

## [SCREEN PROMPT — LOOPBACK EXECUTION (OPERATOR EXECUTES AFTER CFO APPROVAL)]

```
Design a desktop screen (1440px) for the "Execute Transfer" step in Orgstar — the moment the Operator (Amy Lin) receives authority back to execute a CFO-approved transaction.

CONTEXT: This is the critical "loopback execution" mechanism. Amy initiated, CFO approved, now Amy executes. This prevents the CFO from being both approver and executor (Segregation of Duties). The FX rate is locked at THIS exact moment of execution, not at approval time.

SAME SIDEBAR (Amy Lin / Operator is logged in).

NOTIFICATION BANNER (top of page, teal background, white text):
"✓ CFO Approval Received — You may now execute Transfer TXN-2847"
[Execute Now →] button inline in banner, orange

PAGE: "Execute Transfer — TXN-2847"
Status breadcrumb: Transfer Details → KYT Scan → CFO Approval ✓ → [Execute] ← you are here → Settled

EXECUTION PANEL (760px centered white card):

TOP STATUS: Green approval badge
"Approved by David Chen (CFO) — Mar 18, 2026 at 15:47:23 CST"

FX RATE LOCK BOX (most important element — prominent):
- Heading: "Live FX Rate — Locked at Execution"
- Large display: "1 USDT = 31.47 TWD"
- Source: "MAX Exchange official rate — Mar 18, 2026 14:52:01 CST" ← timestamp
- Rate variance note: "Rate changed +0.05 TWD since approval (within 0.5% threshold ✓)"
- TWD Total: "45,000 USDT = TWD 1,416,150"
- Orange info banner: "This rate timestamp will be embedded in your accounting export for CPA certification"

PRE-EXECUTION CHECKLIST (4 items with checkboxes, all pre-checked and disabled):
✓ Source wallet balance verified: 2,847,000 USDT (sufficient)
✓ Destination wallet address confirmed: 0xAbcd...1234
✓ KYT scan valid (scanned 1h ago — within 24h window)
✓ CFO approval confirmed: David Chen, 15:47:23 CST

TRANSACTION SIMULATION (NEW — sandbox dry-run):
- Heading: "Transaction Simulation" with small "Preview" badge
- Body: "We've simulated this transaction on-chain. Estimated gas fee: 0.003 ETH (~$8.50 USD)"
- Result: "Simulation successful — no errors detected ✓"
- Small: "Simulation run at 15:51:02 CST"

FINAL EXECUTION BUTTON (centered, large):
[🔒 Execute Transfer Now] — large orange button (this is the money moment)

Below button: gray caption text
"This action is irreversible. By clicking Execute, you confirm all details above and authorize on-chain settlement. This will be recorded in the immutable audit log."

AFTER CLICK → In-progress state (show as a second sub-frame):
- Spinner animation
- "Broadcasting to blockchain... please do not close this window"
- Step indicators: [Broadcasting] → [Confirming] → [Settled]
- TX Hash appears: "0x7f3a...c291 (pending)" in monospace

DESIGN LANGUAGE: High stakes, deliberate, FX rate front and center. Orange CTA for the execute button to signal this is the brand-critical moment.
```

---

---

# ─── SCREEN 6: TRANSACTION HISTORY ──────────────────────────────────────────

## [SCREEN PROMPT — TRANSACTION HISTORY]

```
Design a desktop screen (1440px) for "Transaction History" in Orgstar — an enterprise stablecoin governance platform. This is the main ledger view.

SAME SIDEBAR. "Transaction History" active in nav.

PAGE HEADER: "Transaction History"
Right side: [Export to CSV] [Export Accounting Package] buttons

FILTER BAR (below header, full width gray bar):
- Date range picker: "Mar 1, 2026 — Mar 18, 2026"
- Status filter: [All] [Completed] [Pending] [Failed] [Rejected]
- Currency: [All] [USDT] [USDC] [DAI]
- KYT filter: [All] [Clear] [Flagged]
- [Search transactions...] input with search icon
- [Apply Filters] button teal

SUMMARY ROW (4 small stat chips inline, below filter bar):
"Showing 47 transactions | Total: 3,284,500 USDT | Completed: 44 | Pending: 3"

TRANSACTIONS TABLE (full width, alternating white/#EAF4F8 rows):
Columns:
- # (tx ID monospace small)
- Date & Time
- Initiated By
- From → To
- Amount (USDT)
- FX Rate Locked
- TWD Equivalent
- Status
- KYT
- Actions

Show 8 rows of realistic data:
TXN-2847 | Mar 18 14:52 | Amy Lin | HQ Treasury → Tanaka Trading | 45,000 USDT | 31.47 | 1,416,150 TWD | ● Completed | ✓ Clear | View / Audit
TXN-2844 | Mar 18 09:15 | Amy Lin | HQ Treasury → Payroll Pool | 280,000 USDT | 31.45 | 8,806,000 TWD | ● Completed | ✓ Clear | View / Audit
TXN-2851 | Mar 17 16:48 | Amy Lin | Operations → Vendor Payment | 12,500 USDT | — | — | ⏳ Pending | ✓ Clear | Review
TXN-2848 | Mar 17 11:20 | Amy Lin | Treasury → Exchange Reserve | 500,000 USDT | — | — | ⏳ Pending | ⚠ Flag | Review
TXN-2839 | Mar 16 15:33 | Kevin Hsu | Family Office → HK Account | 1,200,000 USDT | 31.38 | 37,656,000 TWD | ● Completed | ✓ Clear | View / Audit
TXN-2831 | Mar 15 10:07 | Amy Lin | HQ Treasury → Staff Wallets | 95,000 USDT | 31.41 | 2,983,950 TWD | ● Completed | ✓ Clear | View / Audit
TXN-2822 | Mar 14 08:45 | Amy Lin | Operations → Supplier B | 67,000 USDT | 31.44 | 2,106,480 TWD | ● Completed | ✓ Clear | View / Audit
TXN-2801 | Mar 13 17:12 | Amy Lin | HQ Treasury → Reserve Pool | 88,000 USDT | 31.39 | 2,762,320 TWD | ✗ Rejected | ✓ Clear | View

Status pills: Completed=green, Pending=amber, Rejected=red
KYT: ✓ Clear = green small badge, ⚠ Flag = orange small badge

PAGINATION: "← Previous | Page 1 of 6 | Next →"

ROW EXPAND (click a row) → shows a bottom drawer or inline expansion:
- Full audit trail timeline
- Approval chain (who initiated, who approved, execution timestamp)
- On-chain TX hash with Etherscan link
- FX rate certificate download button

DESIGN: Dense but clean data table. Monospace for financial amounts and IDs. Enterprise ledger feel.
```

---

---

# ─── SCREEN 7: ACCOUNTING EXPORT ─────────────────────────────────────────────

## [SCREEN PROMPT — ACCOUNTING EXPORT / CPA PORTAL]

```
Design a desktop screen (1440px) for "Accounting Export" in Orgstar — the feature that accountants (CPAs) use to pull certified financial records for stablecoin transactions.

CONTEXT: This is one of the most critical GTM features. The CPA (Eric, external accountant) logs in via a white-label read-only portal. They can filter by period, preview the data, and download a certified accounting package that includes FX timestamp records recognized by Taiwan FSC standards.

SAME SIDEBAR but with Viewer/Auditor role active (Eric the CPA — gray "Auditor" badge at bottom). Some nav items are grayed out (cannot initiate transfers, cannot approve).

READ-ONLY BANNER (subtle top bar, light amber):
"You are viewing as: Auditor (Read-only). You cannot initiate or approve transactions."

PAGE HEADER: "Accounting Export"
Subtitle: "Generate certified accounting packages for CPA review and financial reporting"

EXPORT CONFIGURATION CARD (white, full width, 3-column layout inside):

Column 1: "Reporting Period"
- Date range picker (calendar style): April 1, 2025 — March 31, 2026
- Preset buttons: [Q1 2026] [Q2 2025] [FY2025] [Custom]

Column 2: "Export Contents"
Checklist with toggle switches (all on by default):
✓ Transaction ledger (all transactions)
✓ FX rate certificates (with timestamps)
✓ KYT compliance scan records
✓ Approval chain audit trail
✓ On-chain transaction hash registry
✓ Wallet address register
○ Internal notes (optional)

Column 3: "Export Format"
- Radio buttons:
  ● CSV (for accounting software import)
  ○ PDF Report (for human review)
  ○ Excel (.xlsx) with pivot tables
  ○ Full Package (ZIP — all formats + raw data)
- Language: [English] [繁體中文]

[Preview Export] [Generate & Download] buttons — orange for Generate

PREVIEW TABLE (below config — shows what will be in the export):
Header: "Preview — 47 Transactions Matching Filter"
Table columns: Date | Tx ID | Description | USDT Amount | FX Rate | FX Timestamp | TWD Amount | KYT Status | Approval Chain | On-chain Hash
Show 4 rows (truncated preview)

FX CERTIFICATE CALLOUT (light blue box, important):
Icon: certificate / seal
Heading: "FX Rate Certification"
Body: "Each FX rate is captured from MAX Exchange at the exact second of blockchain settlement. Rate, timestamp, and source are cryptographically embedded in the accounting package."
Sub: "Compliant with Taiwan FSC circular for stablecoin accounting treatment (2025)"
Badge: "Taiwan FSC Reference: FSC-VASP-2025-041"

AUDIT LOG TIMELINE (right panel, 30% width):
"Recent Export Activity"
- Mar 19, 2026 09:05 — Eric Chen (Auditor) downloaded Q4 2025 report
- Mar 12, 2026 14:30 — Eric Chen (Auditor) previewed Q3 2025 data
- Feb 28, 2026 11:45 — Eric Chen (Auditor) downloaded FY2025 summary

DESIGN: Clean, trustworthy, institutional. Auditor/CPA user trusts precision above all. The FX timestamp certification element should be visually prominent.
```

---

---

# ─── SCREEN 8: TEAM & ROLES ──────────────────────────────────────────────────

## [SCREEN PROMPT — TEAM & ROLES (RBAC MANAGEMENT)]

```
Design a desktop screen (1440px) for "Team & Roles" — the RBAC (Role-Based Access Control) management page in Orgstar, an enterprise stablecoin governance platform.

SAME SIDEBAR. Admin/CFO is logged in (David Chen). "Team & Roles" active under Settings.

PAGE HEADER: "Team & Roles"
Subtitle: "Manage who can initiate, approve, and view stablecoin transactions"
Right: [Invite Team Member] button (navy primary)

ROLE PERMISSION MATRIX (top white card):
Heading: "Permission Overview"
Table with roles as columns, permissions as rows:

| Permission | Admin/CFO | Operator | Approver | Viewer/Auditor |
|---|---|---|---|---|
| Initiate Transfer | ✗ (by design) | ✓ | ✗ | ✗ |
| Approve Transfer | ✓ | ✗ | ✓ | ✗ |
| Execute Transfer | ✗ (by design) | ✓ | ✗ | ✗ |
| View Transactions | ✓ | ✓ | ✓ | ✓ |
| Export Accounting | ✓ | ✗ | ✗ | ✓ |
| Manage Wallets | ✓ | ✗ | ✗ | ✗ |
| Manage Team | ✓ | ✗ | ✗ | ✗ |
| KYT Override | ✓ | ✗ | ✗ | ✗ |

Note below table: "Admin/CFO cannot execute transfers by design — this enforces Segregation of Duties (SoD) compliance."

TEAM MEMBERS LIST (white card, below):
Heading: "Team Members (5)"

Member rows (each row: avatar + name + email + role badge + status + actions):
1. David Chen | david@orgstar.com | [Admin/CFO — Navy] | ● Active | [Edit]
2. Amy Lin | amy@orgstar.com | [Operator — Teal] | ● Active | [Edit] [Remove]
3. Michael Wang | michael@orgstar.com | [Operator — Teal] | ● Active | [Edit] [Remove]
4. Sarah Liu | sarah@orgstar.com | [Approver — Purple] | ● Active | [Edit] [Remove]
5. Eric Chen | eric@crowe.com.tw | [Viewer/Auditor — Gray] | ● Active | [Edit] [Remove]
   Sub-label under Eric: "External CPA — Crowe Taiwan"

Each row: 52px height, subtle bottom border, role badge as colored pill

INVITE MODAL (floating, show as overlay):
Title: "Invite Team Member"
Fields:
- Name
- Email
- Role: dropdown [Admin/CFO | Operator | Approver | Viewer/Auditor]
- Access Scope: [All wallets | Specific wallets only] (conditional multi-select if specific)
- Note: "An email invitation will be sent. External auditors get read-only access only."
[Cancel] [Send Invitation] buttons

ROLE INFO TOOLTIPS: Hovering any role badge shows a tooltip explaining that role's permissions in one sentence.

DESIGN: Clear hierarchy, institutional RBAC feel, security-focused. Color-code roles consistently throughout.
```

---

---

# ─── SCREEN 9: MOBILE APPROVAL NOTIFICATION ──────────────────────────────────

## [SCREEN PROMPT — MOBILE APPROVAL NOTIFICATION (CFO QUICK APPROVE)]

```
Design a mobile screen (390px iPhone-style) for a CFO approval notification in Orgstar — an enterprise stablecoin governance platform.

CONTEXT: David Chen (CFO) receives a push notification and needs to review and approve a transaction quickly from his phone. This is not the full desktop experience — it's a focused, mobile approval view. Design should feel like a serious banking app.

DESIGN: Light mode. Same color palette (navy, teal, orange). Inter font. 16px body, 14px secondary.

SCREEN: "Approve Transfer"

TOP NAV BAR:
← Back | "Review Transaction" | [Help]

TRANSACTION SUMMARY CARD (white card, full width, 16px margin):
- Header row: "TXN-2847" (monospace) + amber "Awaiting Your Approval" pill
- Orange divider line below header

Details (2-column label/value pairs, stacked):
- Initiated by: Amy Lin (Operator)
- Amount: 45,000 USDT
- Destination: Tanaka Trading Co. / 0xAbcd...1234
- Purpose: Supplier Payment
- Reference: "Q1 2026 — Invoice #042"
- KYT Status: ✓ All Clear (green)
- Submitted: 3 hours ago

KYT RESULT STRIP (teal background, white text):
"✓ KYT Scan Clear — Chainalysis | Risk Score 2/100 (Low)"

AUDIT NOTE (light blue box):
"After approval, Amy Lin will execute the transfer. You will not execute directly. FX rate locks at execution."

ACTIONS (bottom, fixed to screen bottom, 16px padding):
3 buttons stacked:
1. [Approve Transfer] — full width, navy, large, 52px height
2. [Request More Information] — full width, outlined teal
3. [Reject] — full width, outlined red

After tap on Approve → PIN confirmation screen:
- "Enter your 6-digit approval PIN"
- 6 digit circles
- Numeric keypad below
- Cancel link

SUCCESS STATE (after PIN):
- Large green checkmark animation
- "Approved ✓"
- "Amy Lin has been notified to execute"
- "Transaction reference: TXN-2847"

DESIGN: Mobile banking feel. Deliberate, high-trust, not consumer-casual. Critical financial decision UX.
```

---

---

# ─── SCREEN 10: ONBOARDING — COMPANY SETUP ───────────────────────────────────

## [SCREEN PROMPT — ONBOARDING / COMPANY SETUP]

```
Design a desktop onboarding flow screen (1440px) for Orgstar — the step where a new corporate client sets up their company profile and first wallet.

CONTEXT: A new Segment A client (Cross-Border Trading Company) has just signed up. This is Step 2 of 5 in onboarding. Clean, welcoming but still serious/institutional.

CENTERED LAYOUT (no sidebar yet — this is pre-onboarding):
- Orgstar logo top center (orange star + wordmark)
- Progress stepper: [1 Account ✓] [2 Company ←] [3 Wallets] [4 Team] [5 Launch]
- Step 2 active

FORM CARD (680px wide, centered, white, generous padding):
Heading: "Tell us about your company"
Subtext: "This information is used for KYC compliance and accounting export headers."

FIELDS:
- Company Legal Name (in country of registration): text input
- Company Registration Number: text input
- Industry: dropdown [Cross-Border Trade | Manufacturing | Technology | Financial Services | Other]
- Primary Operating Currency: dropdown [TWD | USD | HKD | JPY | SGD]
- Stablecoin(s) to use: multi-select chips [USDT] [USDC] [DAI]
- Monthly Transfer Volume (estimated): dropdown [<$100K | $100K–500K | $500K–$2M | >$2M]
- Primary Use Case: radio buttons
  ○ Cross-border supplier payments
  ○ Payroll / staff disbursements
  ○ Treasury / asset management
  ○ Multiple (describe below)

INFO BOX (light blue):
"Orgstar operates as a governance layer only. We do not hold or custodize your assets. Your stablecoins remain in your corporate wallets at all times."

BOTTOM: [← Back] [Continue to Wallet Setup →] (navy primary, right-aligned)

DESIGN: Welcoming but professional. Trust signals prominent. Clean form design. Progress is clear. First-time user shouldn't feel confused about what Orgstar does.
```

---

---

# ─── COMPONENT LIBRARY REFERENCE ─────────────────────────────────────────────

## [SCREEN PROMPT — COMPONENT LIBRARY / DESIGN SYSTEM REFERENCE SHEET]

```
Design a component library reference sheet (1440px) for Orgstar — an enterprise stablecoin governance platform. This is a design system documentation page, not a live app screen.

Show all core components on a white background with section labels. No sidebar.

SECTION 1: Buttons
- Primary (navy #1B3A5C): [Approve Transfer] [Export] [Continue →]
- Secondary (outlined teal): [Request Info] [Preview]
- Danger (outlined red): [Reject] [Delete]
- Disabled state: grayed out
- Loading state: spinner inside button
- Sizes: Large (52px), Default (40px), Small (36px)

SECTION 2: Status Badges / Pills
- Completed: green pill
- Pending Approval: amber pill
- Awaiting Execution: teal pill
- Rejected: red pill
- Draft: gray pill
- KYT Clear: green small badge with checkmark
- KYT Flag: orange badge with warning icon

SECTION 3: Role Badges
- Admin/CFO: navy #1B3A5C
- Operator: teal #0D6E8A
- Approver: purple #7C3AED
- Viewer/Auditor: gray #6B7280

SECTION 4: Cards
- Standard white card with shadow
- Info card (light blue teal background)
- Warning card (amber left border)
- Success card (green left border)
- KYT flag card (red left border)

SECTION 5: Form Elements
- Text input (default, focused, error, disabled states)
- Dropdown selector
- Multi-select checkbox group
- Toggle switch (on/off)
- Radio button group
- Date range picker

SECTION 6: Table Components
- Header row (navy background, white text)
- Default row (white)
- Alternate row (#EAF4F8)
- Selected row (teal left border)
- Expandable row (with expand arrow)

SECTION 7: Icons (16px and 24px)
- Transfer arrow, Wallet, Check/Clear, Warning, Lock, Clock, Download, User, Settings, External link, Copy (for addresses)

SECTION 8: Typography Scale
- Display all type sizes with labels: H1, H2, H3, Body, Caption, Monospace

SECTION 9: FX Rate Display Component
- The specialized "FX Rate Lock" component showing: rate, timestamp, source, TWD equivalent, variance indicator

SECTION 10: Audit Trail Timeline
- Vertical timeline with nodes, timestamps, status icons

DESIGN: Clean design system documentation. Navy, teal, orange color system. Inter + JetBrains Mono fonts.
```

---

---

# ─── USAGE NOTES FOR PENCIL.DEV ─────────────────────────────────────────────

**Screen generation order (recommended):**
1. Component Library (establishes the system)
2. Dashboard (establishes overall layout)
3. Initiate Transfer
4. KYT Scan
5. CFO Approval
6. Loopback Execution
7. Transaction History
8. Accounting Export
9. Team & Roles
10. Mobile Approval
11. Onboarding

**Pro tips:**
- If Pencil generates a screen, copy that screen's visual style description into subsequent screen prompts for consistency.
- For the sidebar, generate it once as a component and reference it in all subsequent screens.
- Specify "dark navy sidebar, light #F5F7FA content area, Inter font" in every prompt to maintain consistency.
- When generating mobile, prepend: "Mobile 390px, no sidebar, full screen, banking app feel, same color palette."

**Key design decisions to reinforce in every prompt:**
- NOT a crypto wallet. Enterprise SaaS ledger.
- FX timestamp lock is a FEATURE — always display it prominently.
- Segregation of Duties = Operator initiates, CFO approves, Operator executes. NEVER CFO executes.
- Every irreversible action = 2-step confirmation.
- KYT scan result = always visible on every transaction.
