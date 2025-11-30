# Discounted Cash Flow (DCF) Valuation Model

This repository contains a self-built **DCF valuation** in Excel. It demonstrates end‑to‑end cash‑flow forecasting, discounting, terminal value estimation, and enterprise value calculation using clearly stated assumptions.

> **Deliverable:** A working DCF model (Excel) that a recruiter or hiring manager can open and audit quickly.

---

## 🧠 Objective & Scope

- **Objective:** Determine the **Enterprise Value (EV)** of a hypothetical company using a DCF approach.
- **Scope:** Forecast revenue and free cash flow for a finite horizon and compute a **terminal value** using the Gordon Growth method. Discount all cash flows at **WACC** to arrive at EV.

---

## 🧩 Model Assumptions

- Projection period: **5 years**
- Revenue growth: **10%**
- Operating margin: **20%**
- Tax rate: **25%**
- Discount rate (WACC): **10%**
- Terminal growth: **3%**
- Initial revenue (Year 1): **$100 million**
- Depreciation & CapEx: **Offset each other**
- Change in Net Working Capital: **No change**

> With the *Depreciation ≈ CapEx* and *no working capital change* assumptions, **FCF ≈ NOPAT** throughout the projection period.

---

## 🔢 Methodology Overview

1. **Revenue & EBIT Forecast**  
   - Revenue grows at **10%** per year from an initial **$100m** base.  
   - **EBIT margin 20%** ⇒ EBIT = 20% of revenue.

2. **Taxes & NOPAT**  
   - Taxes at **25%** ⇒ NOPAT = EBIT × (1 − 25%).

3. **Free Cash Flow (FCF)**  
   - With Depreciation ≈ CapEx and ΔNWC ≈ 0, **FCF = NOPAT**.

4. **Discounting**  
   - Present value (PV) of each year’s FCF:  
     \[ \text{PV} = \frac{\text{FCF}_t}{(1 + r)^t} \]  
     where **r = 10% (WACC)**.

5. **Terminal Value (TV)** – Gordon Growth  
   - \[ \text{TV} = \frac{\text{FCF}_\text{final} \times (1 + g)}{r - g} \]  
     with **g = 3%**.

6. **Enterprise Value (EV)**  
   - **EV = Σ PV(FCFs) + PV(TV)**

---

## 📌 Headline Results

- **PV of Forecast Period FCFs:** ~ **$68.18m**  
- **PV of Terminal Value:** ~ **$200.65m**  
- **Enterprise Value (EV):** ~ **$268.83m**

> Units are **millions of USD** given the $100m initial revenue base.
---

### Attribution
This model and README were authored by me (the repository owner) as part of independently practicing and demonstrating corporate valuation skills.
