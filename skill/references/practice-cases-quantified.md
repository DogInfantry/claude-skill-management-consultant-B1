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

## Case 7 — Packaged Snacks: Sizing a New-State Expansion
**Archetype:** Market sizing to set production capacity → sizing that must carry a *cost-to-serve* rider, not just a demand number.

**Problem statement.** A B2C potato-chips maker already supplies most of a large country and wants to enter one more state. It needs to estimate the addressable market in that state to set production levels for the new plant/line. Premium vs. economy positioning, shelf life, and retail mix (supermarkets vs. small kirana outlets) are open.

### Opening structure (issue tree)
```
New-state production level
├── Demand size (units/yr)
│   ├── Population of state → snacking-age % → chip-eating %
│   ├── Consumption frequency (packs/person/yr) by segment
│   └── Our realistic share (competition, distribution ramp)  ← not 100%
├── Service level required (the rider most candidates skip)
│   ├── Shelf life → replenishment cadence → safety stock
│   ├── Retail mix: many small outlets = more drops, smaller lots
│   └── Fill-rate target (stockout tolerance) → capacity buffer
└── Supply decision
    └── Production = f(demand × target service level), not demand alone
```

### The quantified spine
Size demand top-down, then **gross it up for service level** — the insight is that a low-shelf-life snack sold through thousands of tiny outlets needs capacity *above* mean demand to hit fill rates.

```
State population              = 30M            [ILLUSTRATIVE]
Snacking-age reachable (60%)  = 18M
Chip-eating penetration (40%) = 7.2M consumers
Frequency                     = 24 packs/person/yr  (2/month)
Latent demand                 = 7.2M × 24     = 173M packs/yr
Realistic share yr 1 (25%)    = 43M packs/yr   ← distribution ramps, incumbents hold shelf
Service-level gross-up (+15%) = ~50M packs/yr of capacity
  (short shelf life + fragmented kirana channel → higher safety stock & drop frequency)
```

**Diagnosis:** the "answer" is not the market number — it is **production ≈ 50M packs/yr of installed capacity**, because a perishable, high-frequency, small-lot product forces you to design for service level, not average demand. Candidates who stop at 173M (latent) or even 43M (share) miss the operational point of the question.

### Recommendation
Set capacity to serve realistic year-1 share **plus** a service-level buffer sized to shelf life and channel fragmentation; phase capacity as distribution deepens rather than building for latent demand on day one.

### Coaching notes
- **What good looks like:** anchors share below 100%, then explicitly converts demand → capacity via service level; ties the buffer to shelf life and retail structure.
- **Red flags:** presenting latent market as the production number; ignoring stockouts, shelf life, and drop-size economics; assuming instant full distribution.

---

## Case 8 — Legacy Foam-Mattress Brand: EBITDA Turnaround After a National Tax Reform
**Archetype:** Margin improvement on a mature brand **+** a structural shift (formalisation of an informal sector) that is both threat and lever.

**Problem statement.** A decades-old foam-mattress and sleep-products brand — a household name competing against a large *unorganised* (informal, often untaxed) segment — has seen EBITDA stall. A national goods-and-services tax has just been rolled out, which advantages organised players and squeezes informal ones. Recommend how to lift EBITDA, and how digital tools could pull the unorganised segment "up to par" (a channel-conversion opportunity for the brand).

### Opening structure (issue tree)
```
EBITDA improvement
├── Revenue up
│   ├── Price/mix: premiumise, bundle sleep ecosystem (pillows, frames)
│   ├── Convert informal demand now disadvantaged by the tax → organised (our) supply
│   └── Channel: e-commerce + own-brand stores vs. dealer margin leakage
└── Cost down
    ├── Input (foam/chemical) procurement & should-cost
    ├── Manufacturing footprint & freight-to-weight (bulky product)
    └── Working capital (dealer credit, inventory of a bulky SKU)

Formalisation lever (the tax-reform "aha")
└── Digitise the informal tier: GST-compliant billing, credit access,
    supply-chain onboarding → migrate their demand into the taxed, branded channel
```

### The quantified spine
Frame the tax reform as a **demand-migration** opportunity and size it against the margin bridge:

```
Assume category demand in region      = 10M mattresses/yr   [ILLUSTRATIVE]
Unorganised share pre-reform (60%)    = 6.0M units
Post-reform cost disadvantage to informal players narrows their price edge
→ Capturable migration (say 10 pts)   = 0.6M units up for grabs
Our realistic capture (1/3)           = 0.2M incremental units
Contribution/unit                     = Rs 1,500
Incremental contribution              = 0.2M × 1,500 = Rs 300M ≈ EBITDA uplift lever
Compare vs. a pure cost programme (e.g., 200 bps on Rs X revenue) to prioritise.
```

**Diagnosis:** the tax reform is not background colour — it is the **highest-leverage growth vector**, because it structurally erodes the informal segment's price advantage. Digitisation (compliant billing, financing, supplier onboarding) is the mechanism that converts that macro shift into captured, branded, taxed revenue. Pair it with a disciplined cost bridge so EBITDA moves from both sides.

### Recommendation
Run two workstreams in parallel: (1) a **demand-migration play** — use digital tooling to formalise and absorb informal-segment demand the tax now disadvantages; (2) a **margin bridge** — premiumise mix and attack input/freight cost on a bulky, freight-sensitive SKU. Sequence quick pricing/mix wins first; stage the formalisation play as distribution and financing partnerships mature.

### Coaching notes
- **What good looks like:** treats the regulatory shift as a lever, not context; quantifies the migration opportunity; keeps a two-sided (revenue + cost) EBITDA bridge; remembers freight/working-capital drag of a bulky product.
- **Red flags:** generic "cut costs / do more marketing"; ignoring the tax reform's competitive effect; hand-waving "go digital" without a demand-conversion mechanism; unable to follow the finance trail (e.g., a DuPont/EBITDA-bridge follow-up).

---

## Case 9 — Boutique Gym: Enter One City, Then Scale Nationally
**Archetype:** Market entry gated on an *underserved segment*, followed by a scale-up / decentralisation design question.

**Problem statement.** A client wants to open a gym in a large metro, then scale nationally if it works. The target locality already has three gyms across low and high price points; the local gender split is ~70:30 female, and none of the incumbents cater to women. Evaluate the entry and recommend how to scale.

### Opening structure (issue tree)
```
Enter? (this locality)
├── Demand: catchment × fitness-intent % × willingness-to-pay
├── Gap: incumbents ignore the 70% female majority  ← the wedge
└── Unit economics: memberships × price − (rent + trainers + equipment)

Scale nationally?
├── What to standardise vs. localise (the female-focused concept = the IP)
├── Decentralisation model: company-owned vs. franchise vs. hybrid
│   └── trade-off: pace of scale-up  ×  standardised experience  ×  capital
└── Replicability: is the "underserved segment" gap present in target cities?
```

### The quantified spine
Prove the wedge with a simple contribution model, then choose the scale model on an explicit trade-off, not a gut call.

```
Catchment adults              = 100,000         [ILLUSTRATIVE]
Female share (70%)            = 70,000
Fitness-intent, underserved (8%) = 5,600 prospects
Capture yr 1 (10%)           = 560 members
ARPU                         = Rs 2,000/month → Rs 24,000/yr
Revenue                      = 560 × 24,000 = Rs 13.4M/yr
Contribution after rent+staff+kit (say 30%) = ~Rs 4M/yr per club  → payback test
```

Scale-model trade-off (score, don't hand-wave):

| Model | Pace of scale-up | Standardised experience | Capital intensity |
|---|---|---|---|
| Company-owned | Slow | High | High |
| Franchise | Fast | Lower | Low |
| Hybrid (own flagships, franchise fill-in) | Medium | Medium-high | Medium |

**Diagnosis:** entry is attractive **because of a specific demand gap** (an underserved female majority), not generic "fitness is growing." The scale question is really a **standardisation-vs-speed trade-off**: the female-focused concept is the IP, so protect experience while you scale — a hybrid (owned flagships to hold the brand standard, franchised units for reach) usually dominates.

### Recommendation
Enter, positioned explicitly for the underserved segment; validate unit economics in the flagship; scale via a **hybrid** model — company-owned flagships to protect the concept, franchising to accelerate reach — and only in cities where the same segment gap exists.

### Coaching notes
- **What good looks like:** finds the segment wedge instead of sizing the whole gym market; builds a per-club contribution model; picks a scale model on an explicit 3-way trade-off.
- **Red flags:** "the fitness market is big, so enter"; recommending national franchising before the flagship proves out; standardising away the very concept that differentiates.

---

## Case 10 — Commoditised Confectionery: Volume Drop Hiding in the Last Metre of Distribution
**Archetype:** Profitability/volume decline where the answer is **not** demand or price — it's a physical distribution-push failure. The teaching case for *isolate along the value chain before you theorise about customers*.

**Problem statement.** A confectionery maker selling a low-value commodity toffee (sub-rupee price point) through third-party distributors into large, medium, and mostly small retailers (paan/kiosk shops, ~60% of volume) faces a ~20% volume decline over 2–3 months. Market size is flat; the product is a commodity. Find the cause.

### Opening structure (issue tree) — the Evolved move
Don't jump from "profit down" to a Customer/Competition/Company scan. **Isolate along the value chain first**, then ask *what changed*:

```
Volume decline (price flat, market flat)
├── Production issue?      can we make/ship as before?  → no change
├── Distribution PUSH?     do distributors/retailers stock & present it?  ← isolate here
│   ├── margins to trade vs. competitors → unchanged
│   ├── reaching paan shops? → YES, still arriving
│   └── reaching the customer FROM the paan shop? → NO  ← the break
└── Customer PULL?         has demand/preference changed?  → no (commodity, flat market)
```

### The quantified spine
Locate the 80% before theorising: which channel carries the drop?

```
Channel mix:  large 10% | medium 30% | small (paan) 60%
Observed:     the entire volume decline sits in the paan-shop channel (~60% of volume)
→ 80/20 says: analyse the small-retail last metre first, ignore the rest for now
Root cause:   distributor switched to jars with NARROWER NECKS
              → shopkeeper can't fish out toffees easily
              → fewer handed to customers → volume falls, though stock still "arrives"
```

**Diagnosis:** a commodity with flat price and flat market almost never has a customer-preference story. The decline is a **distribution-push mechanics failure in the last metre** — a packaging change (narrow-neck jars) throttled the retailer's ability to dispense. You only reach it by isolating Production → Distribution-push → Customer-pull and asking *what changed*, instead of benchmarking product attributes customers don't care about.

### Recommendation
Revert/redesign the jar for easy single-unit dispensing at the counter; audit any recent packaging/logistics changes as the first suspect whenever a commoditised, well-distributed product loses volume with no price or market shift.

### Coaching notes
- **What good looks like:** rules out production, tests distribution-push before customer-pull, uses channel mix (80/20) to focus on paan shops, asks "what *changed*" rather than "what *exists*."
- **Red flags:** benchmarking taste/price/packaging aesthetics on a commodity where customers are indifferent; trial-and-error guessing instead of MECE segmentation of the last metre; missing that "product arrives at the shop" ≠ "product reaches the customer."

---

## How Claude should use this file
1. **As interviewer:** pick a case, reveal data only when the candidate asks for the right node, grade against the coaching notes.
2. **As coach:** compare a candidate's structure to the issue tree, push toward the quantified spine.
3. **On a real problem:** pattern-match (BP device = influencer-economics in a channel; drone = cost-floor-vs-value-ceiling; pharma = idiosyncratic decline vs growing market; PE = returns-math discipline; packaged snacks = demand→capacity via service level; foam-mattress = regulatory shift as demand-migration lever; gym = underserved-segment wedge + standardise-vs-speed; confectionery = value-chain isolation to the last metre).
4. Tag any number you add as **[ILLUSTRATIVE]**; show the math explicitly; sanity-check order of magnitude.
