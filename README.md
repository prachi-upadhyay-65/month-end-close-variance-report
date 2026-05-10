# Month-End Close & Variance Report — Finance Operations Simulation

> A full month-end close simulation for a fictional Indian IT services company, built to demonstrate hands-on finance operations skills: trial balance preparation, P&L reporting, budget vs actuals variance analysis, and management reporting.

---

## The Business Scenario

**Company:** TechServe India Pvt Ltd — a Bangalore-based IT services and consulting firm  
**Size:** 32 employees (22 billable engineers + PMs, 10 support & admin)  
**Period:** Month ended 31 March 2025  
**Revenue:** ₹1,31,50,000 (March actuals)  
**My Role:** Finance Analyst responsible for closing the books, preparing the P&L, running variance analysis, and issuing the management report to the CFO

The company delivers IT services to domestic clients and exports software services to international clients (USD-denominated). The close involves reconciling bank accounts, posting accruals, confirming GST liabilities, and locking the period in the ERP — then packaging the numbers into a management summary with clear recommendations.

---

## What the Numbers Revealed

### Finding 1 — Revenue Shortfall is a Timing Issue, Not a Demand Issue
March revenue came in at **₹1,31,50,000 against a budget of ₹1,35,00,000 — a ₹3,50,000 shortfall (2.6% adverse).** The entire gap traces to export revenue: USD 49,500 worth of invoices were raised on 1 April due to client approval cycles running past the month-end cut-off. The domestic pipeline is healthy with 3 active RFPs worth ₹48L in progress. This is a billing process problem, not a revenue problem.

### Finding 2 — Salary Overrun Needs a Structural Fix
Total salary cost (delivery + admin) exceeded budget by **₹3,50,000 (~8% adverse).** Two drivers: a one-time retention bonus of ₹2,00,000 paid to two senior analysts (MD-approved on 28 March), and a mid-month contract engineer hire that added ₹2,00,000 to delivery costs. Both were individually approved but neither was reflected in the budget — the issue is process, not spend control. Without a supplementary budget approval mechanism, forecast accuracy will continue to deteriorate.

### Finding 3 — DSO Deterioration is an Early Warning Signal
Days Sales Outstanding stretched to **51 days in March, up from 45 days in February** — a 13% increase in one month. The two largest customers (representing ₹9,20,000 of the AR balance) are 18–22 days past due. If this trend continues into Q1 FY26, the company will face a working capital squeeze despite healthy revenue.

---

## Recommendations to the CFO

| # | Recommendation | Owner | Due |
|---|----------------|-------|-----|
| 1 | **Tighten billing calendar** — mandate all invoices raised by the 25th of each month to eliminate end-of-month revenue timing gaps | Finance Analyst + Account Managers | 10-Apr |
| 2 | **Introduce a supplementary budget approval process** — any off-cycle hire or bonus above ₹50,000 requires Finance Manager sign-off and a budget amendment before processing | CFO + Finance Manager | 15-Apr |
| 3 | **Issue formal dunning letters to the 2 overdue customers** — escalate to BD Head if no payment confirmation within 7 days of letter; review credit terms for both accounts at next QBR | Finance Analyst → BD Head | 05-Apr |

---

## What's in the Workbook

| Tab | Contents |
|-----|----------|
| **Trial Balance** | 37 accounts across assets, liabilities, equity, revenue, COGS, OPEX, and tax — with opening balances, March transactions, closing balance formulas, and a debit/credit balance check |
| **P&L Statement** | Auto-populated from the Trial Balance via `SUMIF` — Revenue → Gross Profit → EBITDA → PBT → PAT, with % of revenue at every level. No manual copying anywhere. |
| **Budget vs Actuals** | 11 line items with budget, actuals, variance in ₹ and %, colour-coded favourable/adverse, and a full analyst commentary sentence for each variance |
| **Close Checklist** | 23 tasks covering bank reconciliation, accruals, GST, TDS, AR review, payroll reconciliation, CFO sign-off, period lock, and document archiving — each with owner, target date, status, and evidence note |
| **Management Summary** | KPI scorecard, 3 narrative takeaways written for a CFO audience, and a 5-item action register with owners and due dates |
| **6-Month Trend** | Oct 2024–Mar 2025 trend across 10 metrics: Revenue, Gross Profit, EBITDA, PAT, all four margins, headcount, revenue per head, and DSO — with auto-calculated trend arrows |

---

## Key Finance Concepts Demonstrated

- **Trial balance preparation** — double-entry structure with debit/credit balance verification
- **Month-end accruals** — salary accruals, depreciation (PP&E + Ind AS 116 ROU asset), gratuity provision
- **Revenue recognition** — milestone-based domestic billing, forex conversion for export revenue (USD → INR at RBI rate)
- **GST accounting** — output tax liability (GSTR-1), input tax credit reconciliation (GSTR-2B), net liability confirmation
- **Variance analysis** — budget vs actuals with root cause commentary, distinguishing timing differences from structural issues
- **DSO calculation** — working capital metric tracking and escalation trigger
- **Ind AS 116** — operating lease recognised as ROU asset + lease liability, monthly amortisation
- **Period close process** — ERP period lock, document archiving, CFO sign-off workflow
- **Management reporting** — translating raw numbers into actionable insights for non-finance leadership

---

## Technical Build Notes

- Built entirely in **Microsoft Excel** using `openpyxl`
- **121 live formulas** — zero hardcoded calculated values
- P&L pulls directly from Trial Balance via `SUMIF` on account codes — change any transaction figure and the entire P&L updates automatically
- Color-coded per finance industry standard: **blue = hardcoded inputs**, **black = formulas**, **green = cross-sheet links**
- Verified with **zero formula errors** (`#REF!`, `#DIV/0!`, `#VALUE!` — all clean)

---

## File

| File | Description |
|------|-------------|
| `TechServe_India_Month_End_Report_Mar2025.xlsx` | Full 6-tab workbook |

---

## About This Project

This project was built specifically to demonstrate the finance operations skills described in roles requiring month-end close ownership, statutory account consolidation, and financial reporting — including budget vs actuals variance analysis, ERP period management, and CFO-level management reporting. The scenario, company, and all figures are fictional and created for portfolio purposes.
