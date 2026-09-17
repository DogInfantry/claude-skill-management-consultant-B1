# Stats & Capital-Budgeting Primer — Reading an A/B Test and Judging an Investment

Two numeracy toolkits that analyst, PM and consulting interviews test directly:
1. **Business statistics**, framed around what you actually do with it: read an experiment result and say whether to ship.
2. **Capital budgeting**, framed around the decision: invest or not, and which project wins.

Every formula has a worked mini-example with the math shown. For broader modelling see `references/quantitative-toolkit.md` and `references/tools-and-analysis.md`. For experiment design inside product cases see `references/product-sense-casebank.md` (Part D1).

---

## Part A — Business statistics

### A1. Descriptive vs. inferential
- **Descriptive** statistics summarise data you have, e.g. average daily sales by weekday.
- **Inferential** statistics use a **sample** to draw conclusions about a **population**, e.g. predicting how a new product will sell from a test market.
- **Random, representative sampling** is what makes the leap from sample to population legitimate.

### A2. Variable types
- **Numerical.** Discrete (orders per day) or continuous (delivery time).
- **Categorical.** Ordinal (education level, with an order) or nominal (city, payment method, no order).
- **Why it matters.** The type decides the summary and the test: a mean for numerical data, a mode or proportion for categorical, a χ² test for categorical vs. categorical.

### A3. Central tendency: pick the right "average"
| Measure | Definition | Use when |
|---|---|---|
| **Mean** | Sum ÷ count | Symmetric data without outliers |
| **Median** | Middle value: half the observations lie above it, half below | Skewed data (income, order values, time to deliver) |
| **Mode** | Most frequent value | Categorical data (most common payment method) |

*Mini-example.* Order values of ₹200, ₹220, ₹250, ₹260 and ₹5,000 have a mean of ₹1,186 but a median of ₹250. **Report the median** for a skewed metric, or segment out the whale order.

### A4. Dispersion
- **Variance** is the average squared deviation from the mean, in squared units.
- **Standard deviation (SD)** is √variance, in the original units. A low SD means values cluster near the mean; a high SD means they are spread out (in finance, riskier).
- **Normal rule of thumb.** ~68% of values lie within 1 SD of the mean, ~95% within 2 SD and ~99.7% within 3 SD.
- **Standard error (SE)** = SD ÷ √n. It measures the uncertainty of a *mean*, not the spread of the data. People confuse SD and SE constantly.

### A5. Distributions you'll meet
- **Normal.** Continuous, symmetric metrics such as heights and measurement errors. Large-sample averages also behave this way (the central limit theorem).
- **Binomial.** The count of successes in n yes/no trials: conversions, defects, selections.
- **Frequency distributions** are shown as histograms (numerical) or bar and pie charts (categorical). Always look at the shape before choosing mean vs. median.

### A6. Hypothesis testing in five steps
1. **State H₀ and H₁.** H₀ is "no difference / no effect". H₁ is two-sided (≠) unless you committed to a direction *before* seeing the data.
2. **Pick α**, the significance level, usually 0.05. It is your tolerated false-positive rate.
3. **Compute the test statistic** (z, t or χ²) and its **p-value**: the probability of a result at least this extreme *if H₀ were true*.
4. **Decide.** If p < α, reject H₀. Otherwise **fail to reject** H₀ (never say "accept").
5. **Interpret in business terms.** Report the effect size and its interval, not just "significant".

**Worked example: a jury-selection bias check.** The pool is 50% women. A 50-person jury has 36 women. Is selection biased?
```
H₀: p = 0.5   H₁: p ≠ 0.5   α = 0.05
P(X ≥ 36 | n = 50, p = 0.5) = Σ C(50,k)/2⁵⁰ for k = 36..50 ≈ 0.0013   (one tail)
Two-sided p ≈ 2 × 0.0013 = 0.0026 < 0.05 → reject H₀: selection looks biased.
```
*Note.* 0.0013 is the **one-sided** tail. With a two-sided H₁, double it. The conclusion doesn't change here, but it can near the threshold.

### A7. Which test?
| Question | Test | Statistic |
|---|---|---|
| One sample mean vs. a known value (σ known or n large) | z-test | z = (x̄ − μ) ÷ (σ/√n) |
| Two group means (e.g. AOV control vs. variant) | Two-sample t-test (Welch) | t = (x̄₁ − x̄₂) ÷ √(s₁²/n₁ + s₂²/n₂) |
| Two conversion rates | Two-proportion z-test | z = (p₁ − p₂) ÷ √(p̄(1−p̄)(1/n₁ + 1/n₂)) |
| Two categorical variables independent? (e.g. plan type × churned) | χ² test of independence | χ² = Σ (O − E)² ÷ E |

*The denominator is the standard error.* It combines the variances, s₁²/n₁ + s₂²/n₂, under one square root. It is **not** the sum of σ/√n terms.
*Critical values (two-sided, α = 0.05).* |z| > 1.96; for t the threshold is slightly larger with small samples. Compare the **absolute** value of the statistic.

### A8. Reading an A/B test: two worked readouts
**(i) Conversion.** Control: 10,000 users and 500 orders (5.0%). Variant: 10,000 users and 560 orders (5.6%).
```
Pooled p̄ = 1,060 / 20,000 = 0.053
SE = √(0.053 × 0.947 × (1/10,000 + 1/10,000)) ≈ 0.00317
z = (0.056 − 0.050) / 0.00317 ≈ 1.89  → two-sided p ≈ 0.058 > 0.05
```
**Decision.** Not significant at 5%. The +12% relative lift is promising but unproven. The fix is to **extend to the pre-planned sample**, not to declare a win or peek repeatedly.

**(ii) Average order value.** Control mean ₹400 (SD ₹150, n = 2,000). Variant mean ₹410 (SD ₹160, n = 2,000).
```
SE = √(150²/2,000 + 160²/2,000) = √(11.25 + 12.80) ≈ 4.90
t = (410 − 400) / 4.90 ≈ 2.04  → p ≈ 0.041 < 0.05  → significant
```
**Decision.** Significant, but check **guardrails** (conversion, refunds) before shipping. A +₹10 AOV that costs conversion is a net loss.

### A9. Sample size before you start
Rule of thumb for α = 0.05 and 80% power, comparing two proportions:

**n per arm ≈ 16 · p(1 − p) ÷ δ²**, where δ is the absolute lift you want to detect.

*Example.* Baseline 5% and a target of +10% relative (δ = 0.5 pp): n ≈ 16 × 0.05 × 0.95 ÷ 0.005² ≈ **30,400 per arm**. Halving δ quadruples n. That is why tiny lifts need huge tests.

### A10. Experiment pitfalls interviewers probe
- **Peeking.** Stopping when p first dips below 0.05 inflates false positives. Fix the duration in advance, or use sequential methods.
- **Many metrics or variants.** Twenty metrics at α = 0.05 give about one false "win" by chance. Pre-register a primary metric and adjust for multiple comparisons.
- **Novelty and primacy effects.** Run at least 1–2 full weekly cycles.
- **Network interference.** Social and marketplace features leak between treatment and control. Randomise by cluster or by market.
- **Sample-ratio mismatch.** A 50/50 split that arrives as 52/48 means the bucketing is broken. Don't trust the readout.
- **Statistical ≠ practical significance.** Always convert the lift into ₹ or users and set that against the cost of shipping.

---

## Part B — Capital budgeting

### B1. Opportunity cost & time value of money
- **Opportunity cost** = return on the best forgone option − return on the chosen option. It is used in decisions, not in accounting profit.
- **Future value:** FV = PV × (1 + i/n)^(n·t), where n is compounding periods per year.
  *Example.* ₹1,00,000 at 8% compounded quarterly for 5 years = 1,00,000 × 1.02²⁰ ≈ **₹1,48,595**.
- A rupee today is worth more than a rupee later, because it can be invested now.

### B2. The four decision metrics, on one project
Project: invest **₹100** today and receive **₹30 a year for 5 years**. The discount rate (cost of capital) is **10%**.
```
PV of inflows = 30 × annuity factor(10%, 5y) = 30 × 3.7908 ≈ ₹113.7
NPV  = 113.7 − 100                        ≈ +₹13.7   → accept (NPV > 0)
PI   = PV inflows ÷ investment = 113.7/100 ≈ 1.14    → accept (PI > 1)
IRR  = rate where NPV = 0                  ≈ 15.2%   → accept (IRR > 10%)
Payback (simple)     = 100 ÷ 30            ≈ 3.3 years
Payback (discounted) = cumulative PV ≥ 100 ≈ 4.3 years
```

| Metric | Formula | Rule | Blind spot |
|---|---|---|---|
| **NPV** | Σ CFₜ/(1+r)ᵗ − C₀ | Accept if > 0; among mutually exclusive projects pick the highest | Needs a discount rate; absolute, not per ₹ invested |
| **IRR** | r such that NPV = 0 | Accept if IRR > cost of capital | Misleads on scale and timing; multiple IRRs if cash flows change sign more than once |
| **PI** | PV of inflows ÷ C₀ | Accept if > 1; **rank by PI when capital is rationed** | Ignores absolute size |
| **Payback** | Time to recover C₀ (simple: C₀ ÷ average annual CF) | Shorter is safer | Simple version ignores the time value of money; ignores all cash after payback |
| **Benefit–cost ratio** | PV benefits ÷ PV costs | > 1 is justified; used for public and social projects | Classification of costs vs. negative benefits changes the ratio |

### B3. When the metrics disagree (the classic probe)
Mutually exclusive projects at a 10% cost of capital:
```
A: −₹100 today, +₹150 in 1 year   → NPV = 150/1.1 − 100   = +₹36.4 ; IRR = 50% ; PI = 1.36
B: −₹1,000 today, +₹1,300 in 1 year → NPV = 1,300/1.1 − 1,000 = +₹181.8 ; IRR = 30% ; PI = 1.18
```
- **IRR and PI favour A; NPV favours B.** With no capital constraint, **pick B**: NPV measures value created, and B creates 5× more.
- If capital is rationed and the spare ₹900 can fund other projects with PI above 1.18, ranking by **PI** across the whole portfolio is right.

### B4. Cost–benefit analysis in a case
1. List **all** costs and benefits, including indirect and intangible ones: training time, disruption, brand and risk.
2. Monetise them where you defensibly can. Name the rest qualitatively.
3. Discount to present value.
4. Decide on NPV (or BCR for public projects), then run a **sensitivity** on the one or two assumptions that flip the answer.

Use it for projects, hires, policies, change initiatives and social programmes (see `references/public-sector-government-defense.md`).

### B5. Balance sheet & cash flow: a 60-second read
- **Accounting equation.** Assets = Liabilities + Shareholders' equity. Equity = share capital + retained earnings − treasury stock.
- **Assets.**
  - Current (convert within 12 months): cash, receivables, inventory.
  - Non-current: property, equipment, patents.
  - Tangible vs. intangible: brand, goodwill, IP.
- **Liabilities.**
  - Current (due within 12 months): payables, short-term loans, accrued expenses.
  - Non-current: bonds, long-term leases, deferred tax.
  - **Contingent liabilities** (lawsuits, warranties): record a provision when an outflow is **probable and can be reliably estimated**. Otherwise disclose it in the notes.
- **Cash-flow statement.**
  - **CFO** (operations): the quality check on earnings.
  - **CFI** (investing): capex and acquisitions.
  - **CFF** (financing): debt, equity, dividends.
- **Free-cash-flow measures.**
  - **FCFF** = cash available to all capital providers (valuation, unlevered).
  - **FCFE** = cash left for equity holders after reinvestment and debt flows.
- **Fast diagnostics.**
  - Profit rising while CFO falls suggests working capital is soaking up cash; check receivables and inventory days.
  - Negative equity means liabilities exceed assets, a solvency flag.
  - Persistent negative CFO funded by CFF means the business runs on external money.

For deeper diagnostics see `references/quantitative-analysis.md` and `references/corporate-restructuring-financial-distress.md`.
