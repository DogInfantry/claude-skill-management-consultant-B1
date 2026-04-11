# Worked Case Studies — MBB Management Consultant Skill

> Three fully worked consulting cases — exactly how a McKinsey/Bain/BCG senior consultant would approach them. Each case includes the problem prompt, structuring approach, analysis path, and final recommendation. Use these to learn, practice, or as templates for your own problem-solving.

---

## How to Use These Cases

**For case interview practice**: Read the prompt, pause, structure your own approach on paper, then compare to the worked solution. Use the scoring rubric in `INSTALL.md`.

**For learning consulting thinking**: Read each case in full to internalize the reasoning pattern — hypothesis first, structured analysis, synthesis-led recommendation.

**With the Claude skill**: Paste any prompt into Claude (with the skill installed) and ask Claude to run it as an interactive case. Claude will play the interviewer, reveal data progressively, and give you structured feedback.

---

## Case 1: The Falling Star (Profitability Decline)

### The Prompt

> "StarBev is an $800M specialty beverage company with a premium portfolio (craft spirits, premium mixers, botanical waters). Their EBITDA margin has fallen from 22% to 13% over the past three years — a 9 percentage point decline that has alarmed the board. Revenue grew 4% over the same period. The CEO has hired your team to diagnose the root cause and build a turnaround plan. Where do you start?"

---

### How a McKinsey Consultant Structures This

**Step 1 — Problem Statement Clarity**

Before building any framework:
- *Complication*: 9pp margin decline despite revenue growth — cost-driven, not volume-driven (we know revenue grew 4%)
- *Question*: What is driving the margin collapse, and what do we do about it?
- *Key constraint*: Board urgency suggests we need a 90-day action plan, not a 2-year study

**Day 1 Hypothesis**: Given revenue grew, the issue is almost certainly cost-driven — either COGS inflation, mix shift to lower-margin products, or fixed cost deleveraging. Revenue-side issues (price erosion, volume weakness) are secondary hypotheses.

**Step 2 — Issue Tree**

```
Why is EBITDA margin declining from 22% to 13%? (−9pp)
│
├── Revenue-side drivers (margin erosion through mix/price)
│   ├── Price realization declining?
│   │   └── Are we discounting more? Competitive pricing pressure?
│   └── Mix shift to lower-margin products?
│       └── Premium SKU share declining vs. standard SKUs?
│
└── Cost-side drivers (costs growing faster than revenue)
    ├── Variable costs (COGS) increasing?
    │   ├── Raw material/ingredient cost inflation?
    │   ├── Packaging cost inflation?
    │   └── Manufacturing labor costs up?
    └── Fixed costs increasing?
        ├── Overhead growing faster than revenue?
        └── New capacity / facilities added ahead of demand?
```

**Step 3 — Prioritize**

Leading with the cost hypothesis (Day 1 Answer: 70% probability this is cost-driven, given revenue growth). The revenue mix sub-hypothesis is also worth testing quickly.

**Step 4 — Data Analysis**

*Data revealed progressively during the case:*

| Metric | 3 Years Ago | Today | Change |
|--------|-------------|-------|--------|
| Revenue | $769M | $800M | +4% |
| Gross Margin % | 54% | 47% | −7pp |
| COGS/unit (indexed) | 100 | 118 | +18% |
| Price/unit (indexed) | 100 | 106 | +6% |
| Premium SKU Mix | 60% | 45% | −15pp |
| EBITDA Margin | 22% | 13% | −9pp |
| Competitor avg. price increase | — | +14% | — |

**Step 5 — Synthesis**

The 9pp EBITDA margin decline is driven by two simultaneous forces:

**Force 1 — Cost Inflation (accounts for ~6pp of the 9pp decline)**
- COGS/unit increased 18% over 3 years (raw materials, packaging)
- StarBev only raised prices 6% — a 12pp gap between cost push and price recovery
- Competitors raised prices 14% — StarBev under-reacted competitively
- The "fix": Price catch-up of 8-10pp is needed immediately to restore margin

**Force 2 — Mix Shift (accounts for ~3pp of the 9pp decline)**
- Premium SKU share fell from 60% to 45% — a 15pp shift to lower-margin standard products
- Premium products carry ~65% gross margins vs. ~38% on standard products
- This alone reduces blended gross margin by ~4pp
- The "fix": Reverse mix shift through premium portfolio reinvestment and demand generation

**Step 6 — Recommendation**

*Governing Thought*: StarBev's margin collapse is a pricing and mix problem, not a volume problem. The turnaround requires a three-pronged response: immediate price recovery, portfolio remix toward premium, and structural procurement reform.

**Recommendation 1 — Pricing Catch-Up (Q1)**
- Implement 8-10% price increases on standard and premium SKUs
- Use category data to demonstrate value to retailers (justify the increase)
- Expected impact: +4-5pp EBITDA margin within 12 months
- Risk: Some volume loss — but the margin math is favorable at price elasticity < 1.0x

**Recommendation 2 — Premium Portfolio Reinvestment (Q2-Q3)**
- Reinvest $15M in marketing behind top 5 premium SKUs (craft spirits, botanical waters)
- Launch 2 limited-edition premium variants to reignite trade excitement
- Target: Return premium mix to 55%+ over 18 months
- Expected impact: +2-3pp blended gross margin improvement

**Recommendation 3 — Procurement Transformation (Q2-Q4)**
- Consolidate to 3-4 strategic raw material suppliers (currently 12+)
- Hedge 60% of commodity exposure using forward contracts
- Should-cost the top 10 input categories
- Expected impact: +1-2pp COGS improvement, $8-12M savings

**Total expected margin recovery: 7-10pp over 18 months, returning to 20-23% EBITDA margin**

---

### Case Debrief

**What strong candidates do well:**
- Lead with the hypothesis ("this is cost-driven") rather than covering all branches equally
- Identify the mix shift as a revenue-side cost driver (nuanced — it's not price or volume)
- Recognize the competitive pricing gap ($6% vs. $14%) and call it out explicitly
- Quantify the expected margin recovery by initiative

**Common mistakes:**
- Spending too much time on revenue hypotheses before testing cost
- Describing the data ("margins declined") instead of synthesizing it ("under-pricing vs. competitors is the primary driver")
- Recommending a study instead of a recommendation

---

## Case 2: New Frontier (Market Entry Strategy)

### The Prompt

> "FitWear is a $1.2B European athletic apparel brand known for premium sustainable materials and European design aesthetic. They've dominated Northern Europe for a decade but have never entered the US market. The CEO wants to know: should they enter the US? And if so, how?"

---

### How a Bain Consultant Structures This

**Step 1 — Problem Statement Clarity**

- *Complication*: FitWear is facing growth saturation in Europe; the US represents a major opportunity but also a graveyard for European brands
- *Question*: Go/No-Go, and if Go, what entry mode minimizes risk while maximizing long-term position?
- *Constraints*: Available capital of €40-60M; no existing US infrastructure; no brand awareness in the US

**Day 1 Hypothesis**: US entry is worth pursuing — the US athletic apparel market is massive and growing, and premium sustainable apparel is under-served by incumbents. But entry mode matters enormously — a capital-light entry (partnerships, selective retail) is more appropriate than a full DTC launch.

**Step 2 — Issue Tree**

```
Should FitWear enter the US market?
│
├── Is the market attractive?
│   ├── Market size and growth? (Is the prize worth the investment?)
│   ├── Competitive intensity? (Can a new player realistically gain share?)
│   └── Structural trends? (Is the sustainable premium segment growing?)
│
├── Does FitWear have a right to win?
│   ├── Differentiation vs. US incumbents?
│   ├── Sustainable price premium — will US consumers pay it?
│   └── Manufacturing / supply chain — can it work in the US at scale?
│
└── What is the optimal entry strategy?
    ├── Entry mode: DTC vs. wholesale vs. partnership vs. acquisition?
    ├── Geographic sequencing: which US markets first?
    └── Resource requirements and risk-adjusted return profile?
```

**Step 3 — Data Analysis**

*Market Attractiveness:*

| Metric | Data |
|--------|------|
| US athletic apparel market size | ~$70B, growing ~7% annually |
| Premium sustainable segment | ~$8B, growing ~18% annually |
| Key incumbents | Nike, Adidas, Lululemon, Under Armour |
| Lululemon US revenue | ~$7B (profitable, premium, women-led) |
| Consumer willingness to pay premium for sustainability | 45% of 25-40 demographic (McKinsey survey) |

*FitWear's Right to Win:*

| Factor | Assessment |
|--------|------------|
| Product differentiation | Strong: certified sustainable materials (GOTS, bluesign), European aesthetic not in US |
| Brand awareness in US | Zero — complete cold start |
| Manufacturing | European-based; US tariffs add ~6-8% COGS |
| Retail relationships | No US relationships yet; but REI has expressed interest |
| Price premium | FitWear prices 30-40% above Nike, similar to Lululemon |

*Entry Mode Options:*

| Mode | Capital Required | Speed | Risk | Long-term Upside |
|------|-----------------|-------|------|-----------------|
| Wholesale only (REI + specialty) | €10-15M | Fast | Low | Low |
| Wholesale + DTC eCommerce | €25-35M | Moderate | Medium | Medium |
| Flagship store + DTC | €50-80M | Slow | High | High |
| Acquire US sustainable brand | €150-300M | Fast | Very High | High |

**Step 4 — Synthesis**

**The market is attractive.** US athletic apparel is $70B and growing. The sustainable premium sub-segment ($8B, +18%) is the fastest-growing pocket — exactly where FitWear plays. Nike and Adidas have sustainability marketing but not sustainability products; Lululemon is premium but not sustainability-led. There is a genuine white space.

**FitWear has a conditional right to win.** Product is differentiated and credible. But US cold-start with zero brand awareness and 6-8% tariff drag is a real headwind. They must build demand before scaling supply.

**The entry strategy must be capital-efficient and sequenced.** A full DTC flagship strategy risks €60M+ with no validated demand. A pure wholesale strategy limits long-term brand building. The answer is a phased approach.

**Step 5 — Recommendation**

*Governing Thought*: FitWear should enter the US — but in a sequenced, capital-light manner that validates demand before scaling investment. Enter through REI, build DTC in parallel, and define clear go/no-go triggers.

**Phase 1 — Validate (Months 1-12): REI Partnership**
- Launch in 120 REI stores (premium, sustainability-conscious buyer base)
- Invest €8M in US brand marketing (digital, influencer, sustainability PR)
- Target: $25M Year 1 revenue; track sell-through rates and NPS
- **Kill criterion**: If sell-through < 60% in 6 months, reassess entry thesis

**Phase 2 — Amplify (Months 12-24): DTC Layer**
- Launch DTC eCommerce platform ($2M build)
- Add 3-5 additional specialty wholesale partners (Outdoor Voices, REI Co-op)
- Enter 3 urban markets (NYC, LA, San Francisco)
- Target: $75M Year 2 revenue at 12% EBITDA margin

**Phase 3 — Scale (Year 3+): Expand if Validated**
- If Phase 1-2 targets met: open 3 flagships in top markets
- Evaluate DTC-only segments, wholesale rationalization
- Target: $200M US revenue by Year 5 at 15%+ EBITDA

**Total 3-year investment: €35-45M | NPV: €85-120M at 15% cost of capital**

---

### Case Debrief

**What strong candidates do well:**
- Separate the Go/No-Go question from the How question — answer them in sequence
- Identify the sustainable premium white space (not just "the market is big")
- Recommend a phased entry with explicit kill criteria — shows judgment
- Quantify the expected return on the investment

**Common mistakes:**
- Saying "it depends" without committing to a recommendation
- Recommending a flagship store launch (too capital-intensive for an unproven market)
- Ignoring the tariff headwind and cold-start brand awareness problem

---

## Case 3: The Big Question (Market Sizing — PE Due Diligence)

### The Prompt

> "A private equity firm is considering acquiring PawProtect, a leading US pet insurance provider with $280M in premiums and 18% market share. They've asked your team a simple question before proceeding: how big is the US pet insurance market, and where is it going?"

---

### How a BCG Consultant Structures This

**Step 1 — Problem Statement Clarity**

This is a market sizing case with a specific purpose: informing a PE investment thesis. The answer isn't just a number — it's a number with a growth outlook and a view on whether PawProtect's position is defensible.

**Day 1 Hypothesis**: The US pet insurance market is significantly underpenetrated vs. the UK (50% pet insurance penetration vs. ~4% in the US) — suggesting massive growth runway. PawProtect's $280M / 18% share implies a current market of ~$1.5B, which feels small. We should size it from scratch to validate.

**Step 2 — Sizing Approach**

Use both top-down and bottom-up. Triangulate.

**Top-Down Approach — From US Pet Population:**

```
Step 1: How many insurable pets are there in the US?
  - US dogs: ~90 million
  - US cats: ~94 million
  - Total dogs + cats: ~184 million

Step 2: What % are currently insured?
  - Dogs: ~4% insured (industry data)
  - Cats: ~1% insured (lower — cats see vets less)
  - Insured pets: (90M × 4%) + (94M × 1%) = 3.6M + 0.94M = 4.54M pets

Step 3: What is the average annual premium?
  - Dogs: ~$600/year average
  - Cats: ~$350/year average
  - Blended (80% dog, 20% cat in insured pool): ~$550/year

Step 4: Current market size
  - 4.54M insured pets × $550 avg premium = $2.5B

Step 5: Sanity check
  - PawProtect claims $280M revenue, 18% share
  - Implied market: $280M / 0.18 = $1.56B
  - Gap: Our sizing ($2.5B) vs. PawProtect's implied share ($1.56B)
  - Resolution: PawProtect's market share may be based on policies, not premiums, or the market has grown since their last reporting. $2-2.5B is the better estimate.
```

**Bottom-Up Approach — From Veterinary Spend:**

```
- US annual veterinary spending: ~$38B (APPA data)
- % of vet spend that is insurable (unexpected illness/injury): ~40% = $15B
- Pet insurance typically covers 70-80% of eligible costs
- Expected claims: $15B × 75% = $11.3B
- Loss ratio for pet insurance: ~70-75%
- Implied premium volume: $11.3B / 0.72 = ~$15.7B (at full penetration)
- Current penetration: ~16% of the bottom-up potential
- Current market: $15.7B × 16% = ~$2.5B ✓ (confirms top-down)
```

**Step 3 — Growth Outlook**

| Driver | Impact | Evidence |
|--------|--------|---------|
| Pet ownership growth | +2-3% annually | Pandemic-driven pet adoption lasting |
| Penetration rate growth (4% → 25%) | 6-7x market | UK at 50%+; US historically 10 years behind UK trends |
| Premium inflation | +4-5% annually | Vet cost inflation running 6-8% p.a. |
| New entrants driving awareness | Accelerates adoption | Lemonade, Spot, Embrace entering aggressively |

**Step 4 — Synthesis**

**Current market: $2.5B, growing ~20% annually**

If US penetration reaches 25% (still well below UK at 50%) over the next 8-10 years:
- Insured pets: 184M × 25% = 46M pets
- Average premium (inflated): ~$850/year
- **Future market size: $39B**

This represents a ~15x growth from today — one of the most compelling growth runways in consumer financial services.

**Step 5 — PE Investment Implications**

*Governing Thought*: The US pet insurance market is structurally underpenetrated and growing 20%+ annually toward a $15-40B potential — making PawProtect's 18% share in an early-stage consolidating market highly attractive for a PE buyout thesis.

**Bull case for PawProtect:**
- Market leader position in a winner-take-most market (brand trust, scale efficiencies)
- Vet partnership network creates defensible distribution moat
- Data advantage: 8+ years of claims data = better pricing → better loss ratios → lower prices → more customers (flywheel)

**Key risks to validate:**
- Loss ratios: Is PawProtect's 68% loss ratio sustainable as claims inflation runs hot?
- Competitive intensity: Lemonade entered 2023; ASPCA partnership locked in — how durable?
- Churn: What is annual policy churn? Pet insurance churn runs 20-30% — CAC payback matters
- Regulatory: Is any state-level rate regulation risk?

**Recommended valuation range**: 4-6x premiums ($1.1-1.7B enterprise value) given growth trajectory, conditional on claims data validation and loss ratio deep-dive in due diligence.

---

### Case Debrief

**What strong candidates do well:**
- Run both top-down and bottom-up sizing and explicitly triangulate
- Immediately flag the discrepancy between PawProtect's implied share and their estimate — shows intellectual curiosity
- Connect the sizing to the PE investment thesis (not just "the market is $2.5B")
- Identify the specific due diligence workstreams that would stress-test the thesis

**Common mistakes:**
- Using only one sizing approach (no triangulation)
- Not sanity-checking the answer ($2.5B — does that feel right? Yes, given the industry context)
- Stopping at "the market is big" without connecting to risk/return for the PE investor
- Missing the penetration rate growth story (the biggest value driver)

---

## Case 4: The Compounder's Dilemma ⭐ *Real Engagement*

> **Client:** Apollo Hospitals Enterprise Ltd (NSE: APOLLOHOSP, ~₹1.05 L Cr mcap)
> **Engagement:** APEX-2026-01 | April 2026 | 6 weeks
> **Methodology:** MBB hypothesis-driven (SCQA → Issue Tree → Recommendation)
> **Full deliverables:** [case-studies/apollo-hospitals-FY27/](case-studies/apollo-hospitals-FY27/)

**Problem:** Apollo is at peak operating leverage (PAT +35% YoY, 58–71x P/E) but faces a classic capital allocation trilemma heading into FY27: it cannot simultaneously maximise ₹8,300 Cr bed expansion, Apollo 24|7 digital burn, and shareholder returns. The market is paying for execution certainty — any of three failures (capex overrun, 24|7 bleed, HealthCo delay) breaks the multiple.

**Original Framework — The APEX Trilemma™:** Maps every capital allocation decision as tension between three vertices: Growth Capex, Digital Optionality, and Shareholder Returns. The winning position is not at any vertex but at a calibrated point that matches the company's lifecycle stage. Apollo at FY27 inflection belongs at Growth + Returns — using the HealthCo demerger to harvest digital optionality without burning cash.

**Issue Tree with Kill Criteria:** Three paths modelled (Accelerate Growth / Disciplined Compounder / Return Capital) with explicit kill criteria: if bed expansion ROIC < WACC+300bps → rebalance; if 24|7 cannot show path to ₹100 Cr EBITDA by FY28 → divest; if HealthCo demerger value < ₹20,000 Cr → reconsider structure. All three pass in the base case.

**Recommendation — APEX Capital Allocation Waterfall:** ₹14,000 Cr of FY27–30 FCF allocated in strict priority: maintenance capex → committed beds (₹5,000 Cr) → 24|7 burn cap (≤₹450 Cr, hard gate Q2 FY27) → HealthCo demerger (Q3 FY27) → shareholder returns (25–30% residual FCF) → brownfield M&A (18% IRR hurdle). Projected TSR CAGR: **17%** vs 8–10% for alternatives.

**Apollo 24|7 Deep Dive:** Reverse-engineered unit economics (Apollo does not disclose CAC or cohort data) showed CAC collapsed ₹360 → ₹95 (73%), LTV/CAC improved <1x → 9x, payback 240 → 27 months. Recommended a 2-of-3 binding gate (contribution margin/user ≥₹65, EBITDA ≥₹0, private label ≥15%) with pre-committed Plan B (reverse-merge into HealthCo NewCo, implied value ₹3,000–4,000 Cr).

**Key Numbers:**
- Base case equity value: ₹9,760/share (~32% upside vs ₹7,400)
- HealthCo unlock: ₹25,000–35,000 Cr
- Downside (capped): ₹450 Cr burn + ₹500–800 Cr residual assets
- 70% of valuation sensitivity sits in two variables: hospital margin trajectory and HealthCo multiple

**Skills demonstrated:** SCQA structuring · Original framework development · Capital allocation strategy · SOTP valuation · Unit economics reverse-engineering · Scenario modelling · Board-level communication · CEO decision memo

---

## Practice with Claude

Install the management consultant skill and try these prompts:

```
"Run me through the StarBev profitability case as an interviewer.
Give me information progressively and score my structure and synthesis."
```

```
"I'm preparing for a Bain first-round interview next week.
Give me a market entry case and play the interviewer role."
```

```
"Size the US telemedicine market for a PE firm considering
an acquisition of a digital health platform."
```

```
"I need to diagnose why my company's gross margin has dropped
8pp over 18 months despite 15% revenue growth."
```

---

*These cases are part of the [MBB Management Consultant Skill for Claude](./README.md). Install the full skill for interactive case coaching, industry verticals, and 80+ reference files.*
