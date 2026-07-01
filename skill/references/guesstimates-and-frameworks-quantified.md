# Guesstimates & Case Frameworks — Quantified

Guesstimates laid out as **explicit, checkable math** (not prose), plus case-framework diagrams converted into **reusable issue trees with the levers spelled out**. Pairs with `guesstimation.md`, `frameworks.md`, and `case-types.md`. Numbers tagged **[ILLUSTRATIVE]** are demonstrative — swap in real assumptions.

---

## Part A — Guesstimates (worked)

### Guesstimate 1 — Routers sold in a large country per year
**Answer: ~10 million/year.**

**Clarify:** include both standalone routers and combo router-modems.
**Structure:** annual sales = new users (market growth) + routers replaced (end of life), split into **two demand bases**.

**Assumptions:** population 1.4 B; working population 35% = 500 M; white/grey-collar 20% of workers = 100 M; internet access 50% = 700 M; growth 10%; router lifetime 5 yrs.

```
BASE 1 — white/grey-collar workers
  on routers   = 70% of 100M = 70M
  share 10/router → existing = 70M/10 = 7.0M
  new/yr       = (7.0 × 0.10) + (7.0 / 5) = 0.7 + 1.4 = 2.1M

BASE 2 — internet-access population
  on routers   = 20% of 700M = 140M
  share 5/router → existing = 140M/5 = 28.0M
  new/yr       = (28.0 × 0.10) + (28.0 / 5) = 2.8 + 5.6 = 8.4M

TOTAL new/yr   = 2.1 + 8.4 = ~10.5M  (≈ 10 million)
```
**Reusable pattern:** `existing stock = users / sharing ratio`, then `annual flow = stock × growth + stock / lifetime`. The "growth + replacement" formula generalises to any durable good (TVs, ACs, laptops).

### Guesstimate 2 — Market size of sofas (value/year)
**Clarify:** value not volume; armchairs excluded; sofas *sold*, not produced.
**Method:** demand-side (assume no supply bottleneck).
**Assumptions:** population 1.4 B; 5 people/household → 280 M households; urban:rural 30:70; 30% urban + 1% rural own sofas → ~10% penetration; +30% for non-residential (offices, hotels, lounges).

```
Households           = 1.4B / 5          = 280M
Sofa-owning (10%)    = 28M
Replacement ~10 yrs  → buyers/yr = 28M / 10 = 2.8M households   [ILLUSTRATIVE]
Avg price ~₹20,000   [ILLUSTRATIVE]
Residential value/yr = 2.8M × ₹20,000   = ₹5,600 Cr
+30% non-residential = × 1.30            ≈ ₹7,300 Cr/yr          [ILLUSTRATIVE total]
```
**Chain to remember:** demand base → replacement cycle → price → non-residential adjustment.

**Guesstimate discipline:** state assumptions out loud; pick demand- *or* supply-side, not both; round to clean numbers; sanity-check the order of magnitude; apply an adjustment factor for edge users.

---

## Part B — Case Frameworks (issue trees with levers)

### B1. Profitability
**Profit = Revenue − Cost.** Use for declining profits, cost-benefit, scenario weighing.
**Process:** (1) get comfortable with levers, (2) drill into components, (3) **de-average & customise**, (4) recommend.
```
Profit
├── Revenue = Volume × Unit Price
│     Volume → Demand (needs, substitutes, competitors) | Supply (capacity, bottleneck)
│     Unit Price → pricing strategy, value-chain position
└── Cost
      ├── Variable: raw materials, energy, transport, labour
      └── Fixed: rent, interest, overhead, capacity utilisation, legal/regulatory
```
**Winning lever:** de-averaging — split revenue/cost by segment, channel, or product before concluding.

### B2. Market Entry
**Five core issues:** value proposition & capabilities, market size, competition, market share & revenue, costs.
**Key questions:** distinctive value prop + capabilities? geography/conditions/demand? costs & economies of scale? expected sales?
```
Market entry
├── Industry: growth rate, barriers, revenue estimates
├── Company: core assets, capabilities, resources
├── Customer: segments, needs, expectations, profiling
├── Product: current portfolio, offerings, potential
└── Costs: distribution, input, shared/sunk → entry mode (Scratch / Acquisition / JV)
```

### B3. Growth Strategy
Two levers: **customers** and **orders/billings**; two modes: **organic** vs **inorganic**.
```
Growth
├── Organic (own resources)
│   ├── Volume per customer: raise price, raise basket size, raise visit/checkout rate
│   └── New customers: new stores/franchise, extend lineup, new segment, new geography
└── Inorganic: partnerships, mergers, acquisitions
```
**Ten diagnostics:** industry avg growth; current vs target; cash + time; existing strengths; competitor right/wrong; organic vs inorganic + scale; price elasticity; new demand; threats/barriers; expected revenue & profit return.

### B4. Pricing
Three approaches: **cost-based** (floor), **value-based** (ceiling), **competitor-based** (skip if no competitor).
**Four questions:** USP? cost of production? competitor prices? value/benefit to customer?
**Spine:** cost floor → value ceiling (from benefit, e.g. time saved) → choose a point → **stress-test the volume/occupancy assumption**.

### B5. M&A
Acquisition screen: cost of the acquisition? can the client sustain itself post-deal? post-acquisition challenges for the acquirer? (Synergy + integration risk.)

### B6. Private Equity Investment
Score each dimension like a nine-box matrix:
| PE-firm fit | Industry attractiveness | Target-specific |
|---|---|---|
| Fund size, style | Market size, growth | Business model, valuation |
| Portfolio, NPV/IRR | Barriers to entry/exit | Management capability |
| Exit period | Competition, customers, supply chain, elasticity | Profitability, portfolio fit |

**Discipline:** express returns as **IRR/MOIC vs a fund hurdle**, never "X% profit." Quick reference: 5-yr hold → 2.0× MOIC ≈ 15% IRR, 2.5× ≈ 20% IRR; 4-yr → 2.0× ≈ 19% IRR.

---

## Usage rules for Claude
1. Lay guesstimate math out in **explicit steps**, not prose; sanity-check the magnitude before presenting.
2. Apply the **growth + replacement** formula to any durable-good sizing.
3. Tag any number you add as **[ILLUSTRATIVE]**.
