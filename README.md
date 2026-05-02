# 📊 Quantitative Financial Modeling — DCF & Enterprise Valuation
### NexForge Manufacturing Ltd. | 3-Statement Model | Take-Home Assessment

![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Finance](https://img.shields.io/badge/Valuation-DCF%20%7C%20EV%20%7C%20FCFF-blue?style=flat)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat)
![Errors](https://img.shields.io/badge/Formula%20Errors-Zero-brightgreen?style=flat)
![Level](https://img.shields.io/badge/Level-Intermediate-orange?style=flat)

---

## 🧾 Project Overview

This project is a fully integrated **3-statement financial model and DCF valuation** built as part of a competitive take-home assessment for an internship application. The model covers **NexForge Manufacturing Ltd.**, a fictional industrial metal components company with $480M in revenue, and projects financials from **2022 to 2027** with a DCF valuation anchored to 2025–2028 free cash flows.

All sheets are dynamically linked through a central assumptions tab — changes in inputs cascade through the Income Statement, Balance Sheet, Cash Flow Statement, and DCF automatically, with zero hardcoded values in formula cells.

---

## 🏗️ Model Architecture

```
Workbook Structure (6 Sheets)
│
├── Cover             → Project metadata, instructions, candidate info
├── Assumptions       → All input cells (blue); single source of truth
├── Income Statement  → Revenue → Gross Profit → EBITDA → Net Income
├── Balance Sheet     → Assets, Liabilities, Equity (2022–2027)
├── Cash Flow         → Operating / Investing / Financing Activities
└── DCF Valuation     → FCFF → PV of FCF → Terminal Value → EV → Share Price
```

**Color-coding convention followed:**
| Color | Meaning |
|-------|---------|
| 🔵 Blue text | Hardcoded inputs (assumptions only) |
| ⚫ Black text | All formula-driven calculations |
| 🟡 Yellow background | Key assumption cells requiring attention |

---

## 📈 Key Outputs & Valuation Summary

| Metric | Value |
|--------|-------|
| **Implied Share Price** | $14.74 |
| **Equity Value** | $1,474M |
| **Enterprise Value** | $1,433M |
| **EV / EBITDA** | ~6.9x |
| **P / E** | ~12.3x |
| **Shares Outstanding** | 100M |
| **WACC** | 10.0% |
| **Terminal Growth Rate** | 3.5% |
| **Net Debt (FY2024)** | ($41M) — net cash |

---

## 📊 Financial Projections Snapshot (2022–2027)

| Metric | 2022A | 2027E | Change |
|--------|-------|-------|--------|
| Revenue | $480M | $773M | +61% total / 10% CAGR |
| EBITDA | $120M | $206M | +72% |
| EBITDA Margin | 25.0% | 26.6% | +160 bps |
| Net Income | $63M | $120M | +90% |
| Net Margin | 13.1% | 15.5% | +240 bps |
| Free Cash Flow | ~$53M | ~$98M | +85% |
| Operating Cash Flow | $91M | $149M | +64% |
| Net Debt / (Net Cash) | $75M debt | ($298M) net cash | Full deleveraging |

---

## 🔢 DCF Valuation Build

```
Step 1 — Free Cash Flow (FCFF)
  EBIT × (1 – Tax Rate) = NOPAT
  + D&A
  – CapEx
  – Change in Working Capital
  = Free Cash Flow to Firm

Step 2 — Discount Cash Flows
  PV of FCF (2025–2028) = $221.5M
  Discount Rate (WACC)  = 10.0%

Step 3 — Terminal Value
  Terminal Value         = $1,612.7M  (Gordon Growth Model @ 3.5%)
  PV of Terminal Value   = $1,211.7M  (~70% of Enterprise Value)

Step 4 — Enterprise to Equity Bridge
  Enterprise Value       = $1,433.2M
  Less: Net Debt         = ($41.1M)   (net cash position)
  Equity Value           = $1,474.3M
  Implied Share Price    = $14.74     (÷ 100M shares)
```

---

## 📐 Key Assumptions

| Driver | Assumption | Rationale |
|--------|-----------|-----------|
| Revenue Growth | 10.0% annually | Consistent with historical trend |
| COGS % of Revenue | 60.0% (stable) | Peer-level gross margin maintained |
| SG&A % of Revenue | 15.0% → 13.4% | Operating leverage as revenue scales |
| D&A | $28M → $40.9M | Proportional to PP&E base growth |
| CapEx | $38M → $50.9M | Sustaining + growth capex blend |
| Interest Expense | $8M → $4.67M | Declining with $10M/yr debt repayment |
| Tax Rate | 25.0% | Standard corporate assumption |
| WACC | 10.0% | Reflects industrial manufacturing risk |
| Terminal Growth Rate | 3.5% | Long-run GDP proxy (conservative) |

---

## ⚠️ Risk Factors & Model Limitations

> These are identified and documented as part of the investment thesis.

1. **Terminal Value Concentration** — 70% of enterprise value lies in the terminal period, making valuation highly sensitive to WACC (±50 bps ≈ ±$2.00/share) and terminal growth rate assumptions

2. **No Cyclical Scenario Analysis** — Model assumes linear 10% revenue growth with no recession or downturn scenario; metal components manufacturing is inherently cyclical

3. **Constant WACC** — 10% discount rate held fixed across projection period; as net debt turns to net cash (~$298M by 2027), true WACC likely declines, understating intrinsic value in later years

4. **Customer Concentration Unknown** — Revenue modeled as homogeneous; no visibility on top customer concentration, contract duration, or churn risk

5. **Margin Expansion Unvalidated** — SG&A declining from 15.0% to 13.4% requires execution; no management track record data included

---

## 💡 Investment Recommendation

**Rating: HOLD / CONDITIONAL BUY @ $14.74 implied share price**

The model supports a **Hold** rating with potential upgrade to **Buy** pending:
- ✅ Management execution track record validation
- ✅ Customer contract visibility supporting 10% revenue CAGR
- ✅ Downside scenario stress-testing (recession, margin compression)
- ✅ Comparable company benchmarking (EV/EBITDA peer range: 5.5x–7.5x)

**Upside triggers:** Margin expansion confirmed, debt-free balance sheet by 2026, industry tailwinds  
**Downside risks:** Customer loss, CapEx overruns, economic slowdown, margin compression

---

## 📁 Repository Structure

```
📦 NexForge-Financial-Model
 ┣ 📊 NexForge_Financial_Model.xlsx   → Full 3-statement model + DCF
 ┣ 📄 README.md                       → This file
 ┗ 📋 Project_Description.md          → Detailed methodology writeup
```

---

## 🛠️ Skills Demonstrated

- **3-Statement Financial Modeling** (Income Statement, Balance Sheet, Cash Flow)
- **Discounted Cash Flow (DCF) Valuation** — FCFF methodology
- **Enterprise Value & Equity Bridge** — Net debt adjustment, EV/EBITDA, P/E
- **Terminal Value Analysis** — Gordon Growth Model
- **Assumption Management** — Fully dynamic, assumption-driven architecture
- **Model Quality Assurance** — Balance sheet reconciliation, zero formula errors
- **Investment Analysis** — Valuation multiples, risk identification, investment recommendation
- **Microsoft Excel** — Advanced formula construction, cross-sheet references, formatting standards

---

## 👤 Author

**Aritra Tarafdar**  
Date: April 29, 2026  
Assessment: Financial Modeling Internship Test — Intermediate Level  
Sector: Industrial Manufacturing | Currency: USD ($M)

---

*This model was built as part of a take-home assessment. NexForge Manufacturing Ltd. is a fictional company created for the purposes of this exercise.*
