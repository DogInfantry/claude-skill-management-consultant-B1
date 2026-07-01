# Practice Cases — Quantified & Structured

A library of practice cases re-engineered from raw interview dialogue into **structured, quantified drills**. Each case gives the problem statement, the right opening structure (issue tree), the **quantified spine** (math laid out explicitly), the recommendation, and **coaching notes** (what good looks like / red flags).

Numbers marked **[ILLUSTRATIVE]** are added to demonstrate the quantification path and should not be presented as hard data — swap in the interviewer's or client's real figures. This file complements `case-pattern-library.md` (archetypes) and `case-interview.md` (candidate playbook).

---

## Case 1 — Handheld BP Device: Sales Decline
**Archetype:** Demand-side revenue decline → channel + product diagnosis.

**Problem statement.** A healthcare-technology company (operating ~15 years across Asia) launched a handheld blood-pressure device. Sales are not picking up. Identify the reasons and recommend solutions.

### Opening structure (issue tree)
Lead with the funnel; don't discover it late:

```
Sales shortfall
├── Supply side (products reaching market?) ──► rule out first
└── Demand side
    ├── By channel
    │   ├── Pharmacies ──► meeting target
    │   └── Hospitals / doctor recommendations ──► BIGGEST DECLINE  ← focus
    └── Purchase funnel (per channel)
        ├── Need / Awareness
        ├── Affordability / Accessibility
        ├── Experience  →  Function (accuracy)  +  Design (strap)
        └── Influence / Promotion (doctor incentive)
```

### The quantified spine (the insight the dialogue half-buries)
The case hinges on **doctor economics**: the device pays a doctor ~Rs 100 per patient spread over 3 years, while a competing recommendation pays Rs 700 per year. Lay it out as a per-influencer comparison:

| Lever | Our device | Competing recommendation | Gap |
|---|---|---|---|
| Doctor payout | Rs 100 / patient over **3 yrs** ≈ **Rs 33/yr** | Rs 700 / **year** | Doctor earns **~21×** more pushing the alternative |

**Diagnosis:** the bottleneck is not patient awareness — it is the **influencer (doctor) incentive** that controls the hospital channel. That single ratio explains the channel-specific decline.

**[ILLUSTRATIVE] sensitivity:** if the hospital channel is ~40% of target volume and doctor conversion roughly tracks relative incentive, closing the payout gap toward parity is the highest-ROI lever before any product fix. Size the commission budget against incremental units.

### Second driver — product/design
- **Function:** accurate *only if* the strap is bound correctly → user-error sensitivity.
- **Design:** straps loosen after ~12 months, causing inaccurate readings → trust erosion and repeat-purchase risk.

### Recommendation
1. **Influencer economics (do first):** raise doctor commission to close the ~21× gap in the hospital channel.
2. **Product design:** re-engineer the strap for durability and easier correct fitting.
3. **Prioritise by ROI:** incentive fix is fast-payback opex; strap redesign is a longer-lead quality program.

### Coaching notes
- **What good looks like:** ring-fence supply vs demand early, isolate the *channel* before the *funnel stage*, and convert the payout figures into a **ratio** rather than restating them.
- **Red flags:** jumping to "more patient advertising" (wrong node — the doctor is the bottleneck); treating the strap as primary; never quantifying the incentive gap.

---

## Case 2 — Drone Taxi Service: Pricing & Viability
**Archetype:** Greenfield pricing with no direct competitor → cost-plus floor + value ceiling.

**Problem statement.** An airline wants to launch a drone-taxi service on a ~30-minute city-to-airport route (road alternative takes ~3 hours in peak traffic). How should it price the service, and is it viable?

### Approach selection
No direct competitor → drop competitor-based pricing. Use **cost-based pricing for the floor** and **value-based pricing for the ceiling**:
- **Value anchor:** trip time falls from ~3 hrs to ~30 min → **~85% time saved** = the willingness-to-pay story.

### The quantified spine
Inputs (monthly): drone rent **₹25L**, airport charges **₹2L**, salaries + overhead **₹5L**, fuel **₹50,000/flying-hr**; capacity **8 pax/trip**; operating window 5 hrs/day; **25 working days/month**; assume **100% occupancy**.

```
Trips:    5 round trips/day × 25 days = 125 round trips/month
Flying:   one-way 30 min → round trip = 1 flying-hour → 5 flying-hrs/day
Fuel/day: 5 × ₹50,000 = ₹2.5L
Fixed/day:(25L + 2L + 5L) / 25 = ₹1.28L
Total/day:₹2.5L + ₹1.28L = ₹3.78L
Pax/day:  5 round trips × 2 legs × 8 pax = 80 seats/day
Cost/seat:₹3.78L / 80 = ₹4,725  →  price ≈ ₹4,800 one-way (cost floor)
```

**Value check (ceiling):** road alternative ~₹800 one-way → ~₹4,800 is a **~6× premium**, defensible only for a time-rich, price-insensitive segment.

### Recommendation
- **Price ~₹4,800 one-way** at launch (cost-recovery floor at full occupancy), positioned as **premium/luxury** for peak windows only.
- **Viability caveat:** ~₹4,800 assumes **100% occupancy** — fragile. Stress-test it: at 70% occupancy cost/seat = **₹6,750**; at 50% = **₹9,450**. The real question is the *achievable* load factor, not the headline price.
- Expand to other high-traffic corridors once load factors are proven.

### Coaching notes
- **What good looks like:** drops competitor pricing with a reason, builds the cost stack cleanly, separates **cost floor** from **value ceiling**, and challenges the 100%-occupancy assumption with a sensitivity.
- **Red flags:** taking 100% occupancy at face value; pricing on cost alone without the road-fare anchor; forgetting a round trip = two revenue legs (the ×2 that yields 80, not 40, seats/day).

---

## Case 3 — Pharma: Post-Boom Revenue & Market-Share Decline
**Archetype:** Company-specific decline against a growing industry → portfolio reset.

**Problem statement.** A leading drug manufacturer boomed during a demand spike; revenue and market share then fell while the industry kept growing ~5–7%. Reverse the decline and regain share.

### The decisive early split
Industry **+5–7%** but client **declining** → **company-specific, not market-wide**. Cause: over-indexing on a temporary-demand drug category whose demand collapsed. Framing question: *how do we redeploy a demand-spike-built capacity base into growing segments?*

### Structure
```
Reverse decline & regain share
├── Demand: price | competition | product quality | segment mix
└── Supply: capacity (~95% util = industry standard) | product mix | channel
        ├── Current: mostly Rx drugs, minor OTC, mass producer
        ├── Channels: hospitals, chemists, pharmacies; exports
        └── White space: OTC + e-pharmacy (faster-than-industry growth)
```

### Quantification opportunities (frame three sized bets — figures [ILLUSTRATIVE])
1. **OTC entry:** OTC growing faster than the 5–7% base + spare/standardisable capacity → size as `addressable OTC market × realistic share × OTC margin`. A few points of a fast segment offsets the runoff.
2. **B2B / insurance bulk supply:** leverage cost leadership → `contract volume × (price − unit cost)`, low unit cost is the moat.
3. **Offshore plant:** lowers landed cost to export markets → `export volume × per-unit landed-cost saving − annualised capex`.

### Recommendation
1. Expand **OTC + e-pharmacy** (fastest growth, exploits idle capacity).
2. Strike **insurance / bulk B2B** deals on cost leadership.
3. Strengthen the strongest export region with a **local plant** to cut costs.

### Coaching notes
- **What good looks like:** nails "industry up, client down → idiosyncratic cause" fast; ties every lever to an existing asset (capacity, cost position, export base); attempts to size the OTC prize.
- **Red flags:** generic "do organic + inorganic" with no link to the root cause; recommending R&D when it's already healthy; zero quantification.

---

## Case 4 — Luxury Jewellery: Market Sizing for Entry
**Archetype:** Top-down market sizing for a premium new-market entry.

**Problem statement.** A foreign luxury-jewellery brand wants to enter a large new country market. Estimate the size of its addressable target market.

### Approach selection
New premium entrant with a strong global brand but a market where buyers traditionally trust legacy local jewellers → **top-down** sizing on the female-adult population, segmented by affluence and purchase frequency. Decide price first (via willingness-to-pay), then size volume, then multiply.

### The quantified spine (segmentation math laid out)
Assumptions: population ~138 Cr; adult females ~60 Cr; affluence split of the 60 Cr → **10% elite, 20% upper-middle, 30% middle, 40% lower-middle**. Map each segment to a buyer type and an annual purchase rate:

| Segment | Population | Buyer type | Items/yr | Annual units |
|---|---|---|---|---|
| Elite (10%) | 6 Cr | Frequent (1 item / 2 months) | 6 | 6 × 6 = **36 Cr** |
| Upper-middle (20%) | 12 Cr | Casual | 2 | part of 34.8 |
| 30% of middle | 5.4 Cr | Casual | 2 | part of 34.8 |
| Casual subtotal | 17.4 Cr | — | 2 | 2 × 17.4 = **34.8 Cr** |
| Lower-middle + 70% middle | 24 + 12.6 Cr | Non-buyers | 0 | 0 |

```
Total annual units = 36 Cr (frequent) + 34.8 Cr (casual) = ~71 Cr items/yr
Market size = 71 × (avg price per unit X) Cr
```

So the **market is ~71·X Cr/year**, where X is the price point set by the willingness-to-pay analysis. The structure — *segment → buyer type → frequency → units → × price* — is the transferable skill.

### Recommendation
- Target the **elite/affluent** segment first (the only frequent buyers), where global-brand prestige overcomes the legacy-jeweller loyalty that suppresses the mass segments.
- **Long-term:** adapt designs to local taste to widen beyond the elite.
- **Short-term:** build a personalised **digital/omnichannel** presence (buyers research and compare online before purchase).

### Coaching notes
- **What good looks like:** chooses top-down with a reason, segments by *both* affluence and purchase frequency, zeroes non-buyers explicitly, and keeps price as a variable X rather than guessing it mid-sizing.
- **Red flags:** sizing the whole adult-female population as buyers; forgetting frequency (elite buy ~6×, not once); bolting a price on before the WTP step.

---

## Case 5 — Private Equity: Invest / Pass Decision
**Archetype:** Invest-or-pass → returns math + risk screen.

**Problem statement.** A PE firm is considering investing in a target that has a technology cutting production costs **up to 25%** but needs **$200M** to build mass-production capacity. Should the firm invest? Identify the key risks.

### Given data (use it)
| Target / Industry | Value |
|---|---|
| Industry CAGR | **8%** |
| Total assets | **~1.235 Bn** |
| Current liabilities | **~0.475 Bn** |
| Latest annual income | **~0.065 Bn** |
| Funding required | **$200 M** |
| Cost-reduction tech | up to **25%** |
| Assumed hold period | **≥ 5 years** |

### The quantified spine
A returns claim must be expressed as **IRR or MOIC against a fund hurdle**, never "X% profit." Show the shape:
- `MOIC = exit equity value / entry equity value`; `IRR` solves `entry = exit / (1+IRR)^years`.
- Reference points: over a **5-yr** hold, **2.0× MOIC ≈ 15% IRR**, **2.5× ≈ 20% IRR**; over **4 yrs**, **2.0× ≈ 19% IRR**.
- So "over 20% return in 4 years" implies roughly a **2×+ MOIC** — state the assumption and pressure-test whether 8% market growth + a 25% cost edge can plausibly deliver it.

**Leverage check:** current liabilities (~0.475) vs assets (~1.235) ≈ 38%; latest income (~0.065) is small against a $200M raise → returns depend on the **new capacity scaling**, not the existing book. Flag financing risk.

### Risk screen
- **Execution:** building greenfield capacity on time/budget.
- **Demand:** is a 25% cost saving enough to win switchers?
- **Macro / working capital:** rising input costs, climbing current liabilities.
- **Exit:** realistic buyer/IPO at year 5?

### Recommendation
Invest **only if** the returns math clears the fund's hurdle (IRR/MOIC, not "20% profit") **and** execution + exit risks are mitigated; otherwise pass.

### Coaching notes
- **What good looks like:** uses the **given financials**, converts "20% profit" into **IRR/MOIC with stated assumptions**, ties invest/pass to a fund hurdle.
- **Red flags:** accepting "20% in 4 years" without defining the metric; ignoring the supplied balance-sheet data; listing risks without naming the binding one (executing the $200M build).

---

## Case 6 — Organisational Capacity Expansion
**Archetype:** "Should we expand capacity?" → demand-feasibility before supply-investment.

**Problem statement.** A manufacturer is running near full utilisation and is weighing a capacity expansion. Should it expand, and if so, how?

### Structure (the right order: demand first, then supply, then mode)
```
Expand capacity?
├── External demand check (do this FIRST)
│   ├── Market size & growth, future projections
│   ├── Demand elasticity (will lower-cost/higher-volume be absorbed?)
│   └── Supply-chain conditions (can inputs scale?)
├── Internal feasibility
│   ├── Competitive advantage, economies of scale, degree of innovation
│   └── Current utilisation & true bottleneck (machine? labour? a single line?)
└── Expansion mode (only if demand + feasibility clear)
        Organic build | M&A | Outsourcing | Improvement (people/process/technology)
```

### The quantified spine
- **Incremental capacity decision = compare added contribution vs annualised investment.**
  `Go if: incremental units × contribution margin/unit  >  annualised capex + added fixed opex` **[ILLUSTRATIVE framing]**.
- **Find the binding bottleneck before spending:** if utilisation is "95%" but only one process step is saturated, **debottlenecking that step** can add output at a fraction of a full build. Quantify capacity gained per rupee for (a) debottleneck, (b) outsource, (c) greenfield, and rank.

### Recommendation
Expand **only if** demand growth is real and elastic to the added supply **and** incremental contribution beats annualised cost; prefer the highest capacity-per-rupee mode (often debottlenecking or outsourcing before greenfield).

### Coaching notes
- **What good looks like:** checks demand *before* committing capex; locates the true bottleneck; compares expansion modes on capacity-per-rupee.
- **Red flags:** jumping straight to "build a new plant"; treating 95% utilisation as automatically meaning "need more capacity" without finding the bottleneck; ignoring whether the market can absorb the extra output.

---

## How Claude should use this file
1. **As interviewer:** pick a case, reveal data only when the candidate asks for the right node, grade against the coaching notes.
2. **As coach:** compare a candidate's structure to the issue tree, push toward the quantified spine.
3. **On a real problem:** pattern-match (BP device = influencer-economics in a channel; drone = cost-floor-vs-value-ceiling; pharma = idiosyncratic decline vs growing market; PE = returns-math discipline).
4. Tag any number you add as **[ILLUSTRATIVE]**; show the math explicitly; sanity-check order of magnitude.
