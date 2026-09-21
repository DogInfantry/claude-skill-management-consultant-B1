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

## Case 11 — Cross-Border E-Commerce Entry: Year-1 Break-Even and the Partner Choice
**Archetype:** Market entry with a hard financial gate (break even in year 1) → break-even share test, then entry mode. The teaching case for *define the margin and the year before you multiply*.

**Problem statement.** A US e-commerce major with 15 years of operating history wants to enter a fast-growing Southeast Asian archipelago market (~100M people, ~60% internet penetration [ILLUSTRATIVE]). It must break even in its first year, then grow. Two players hold the market. The local leader has 60% share, $600M revenue and a 30% margin; it has been in the market for 8 years, its profits are rising, it has opened physical pick-up stores, and it will not partner. The foreign-origin challenger has 40% share, $400M revenue and a 20% margin; it has been in the market for 4 years, its profits are declining, and it is open to a joint venture. The market is expected to grow 40% next year. The client expects a 20% share, can operate at a 20% margin and needs a $50M fixed investment. The government is raising taxes on non-domestic firms. Should the client enter, and how?

### Opening structure (issue tree)
```
Enter, and break even in year 1?
├── Market attractiveness
│   ├── Size = sum of rival revenues; growth (which year? what rate?)
│   └── Bottom-up check: internet users × spend per user
├── Financial feasibility  ← the gate
│   ├── Margin definition: contribution margin vs net profit margin  ← clarify first
│   ├── Timing: which year's market does the share target apply to?
│   └── Break-even share = fixed cost ÷ (contribution margin × market size)
├── Operational feasibility: tax on non-domestic firms, local know-how, logistics
└── Entry mode
    ├── Standalone ──► hardest (tax + two entrenched rivals)
    ├── JV / acquisition of the challenger ──► instant share, but it is foreign too
    └── Local leader ──► would neutralise the tax, but unwilling
```

### The quantified spine
Size the market from the rival table (the share column is not a size; the size is the sum of revenues), then run break-even on an explicitly defined contribution margin.

```
Market today       = $600M + $400M              = $1,000M
Market next year   = $1,000M × 1.40             = $1,400M
Client revenue     = $1,400M × 20%              = $280M
Contribution (20%) = $280M × 20%                = $56M
Less fixed         = $56M − $50M                = +$6M profit  (≈2.1% net margin)
Break-even revenue = $50M ÷ 20%                 = $250M
Break-even share   = $250M ÷ $1,400M            = 17.9%  → only 2.1 pp of cushion vs the 20% target
```

**Error fixed:** "variable cost = $280M × (100% − 20% profit margin) = $224M; add $50M fixed = $274M < $280M, so it breaks even" → treat 20% as a *contribution* margin: $56M contribution − $50M fixed = $6M profit (if 20% were a *net* profit margin, the $50M would already sit inside the costs, and adding it again double-counts it).

**Error fixed:** applying a share target set for *this* year to *next* year's grown market → state the year. On today's $1,000M market, 20% share gives $200M revenue and $40M contribution, a $10M loss; break-even would need 25% share.

**Error fixed:** expensing the whole $50M "fixed investment" in year 1 → separate capex from the P&L. If the $50M is capex depreciated over 5 years [ILLUSTRATIVE], the accounting charge is $10M/yr (break-even revenue only $50M); the cash test is payback, $50M ÷ $56M ≈ 0.9 years. Ask which break-even the client means before answering.

**Error fixed:** reading the 60%/40% column as market sizes → those are shares; the size is the revenue sum, $1,000M.

The growth assumption flips the verdict. If "40% growth" describes the last two years rather than next year's forecast, the annual rate is √1.4 − 1 ≈ 18.3%:

| Year-1 market | Revenue at 20% | Contribution at 20% | Profit after $50M | Break-even share |
|---|---|---|---|---|
| $1,000M (no growth / "this year") | $200M | $40M | −$10M | 25.0% |
| $1,183M (18.3%/yr) | $236.6M | $47.3M | −$2.7M | 21.1% |
| $1,400M (40% in one year) | $280M | $56M | +$6M | 17.9% |

**Bottom-up sanity check:** 100M × 60% = 60M internet users → $1,000M ÷ 60M ≈ $16.7 of e-commerce spend per user per year today, ≈ $23.3 next year. That is plausible for an early-stage market, so the top-down size holds; refresh population and penetration before real use.

**Rival read-across:** the challenger's 20% margin on $400M is $80M. If it is "bleeding money", that 20% must be a gross or contribution margin and its fixed costs must exceed $80M. That is also the clue to how the client's own 20% should be read.

### Recommendation
- **Go, conditionally:** year-1 break-even holds only if next year's market really grows ~40% *and* the client wins ≥17.9% share. With 2.1 pp of cushion, any slip in growth or share (see table) turns year 1 into a loss. Present it as a knife-edge, not a clear yes.
- **Entry mode:** a JV with, or acquisition of, the challenger buys 40% share and a running operation immediately, which is the only realistic way to reach ~18–20% in year 1. But the challenger is also foreign, so the tie-up **does not escape the non-domestic tax**; only the (unwilling) local leader would. Re-run the economics on the JV basis: the challenger's share, its fixed-cost base (above $80M), the price paid and the tax uplift.
- **Go-to-market:** fix the pain points customers report with both incumbents, apply the client's 15 years of assortment and logistics capability, and evaluate pick-up stores (the leader's differentiator) once the base is profitable.

### Coaching notes
- **What good looks like:** defines contribution vs net margin before multiplying; pins the share target to a specific year; expresses the result as a break-even share and a cushion; uses the unused population and penetration data as a sanity check; notices that the tax argument does not favour a foreign partner.
- **Red flags:** "$280M > $274M, so it breaks even" with fixed costs counted twice; financials built for a standalone entry while recommending a JV; ignoring that the partner is also non-domestic; missing that a rival with a "20% margin" that is losing money points to a definitional problem.

---

## Case 12 — Renewable Developer Entering Li-ion Battery-Pack Assembly: Market Size and Entry Mode
**Archetype:** Adjacent-market entry → market sizing with unit conversion and stock-vs-flow discipline, then an entry-mode choice driven by timing.

**Problem statement.** India's fastest-growing private solar and wind developer builds, owns and operates utility-scale projects for commercial and industrial buyers. It wants to enter Li-ion batteries and hold at least 20% share within five years. It has no battery know-how, so it would start at pack assembly (not cells or materials). Base-year data [ILLUSTRATIVE; refresh before use]:
- **Stationary storage:** 150 GW of installed renewable capacity, growing 10%/yr; 10% of capacity paired with 2-hour storage.
- **Pack price:** $120/kWh, falling 10%/yr.
- **Vehicles:** 30M built per year, growing 3%/yr. 80% are 2/3-wheelers with 10 kWh packs; 20% are 4-wheelers with 35 kWh packs.
- **EV adoption:** 2% share, growing 75%/yr.

Organic entry needs 3 years to build expertise plus 1 year to build a plant; an acquisition or alliance can start almost immediately. Size the market and recommend an entry route.

### Opening structure (issue tree)
```
Enter pack assembly, and how?
├── Market size (annual GWh and $)
│   ├── Stationary storage: NEW renewable capacity × pairing % × hours  (flow)
│   │     └── plus retrofit of the INSTALLED base spread over N years   (stock ÷ N)
│   ├── EV packs: vehicles built × EV share × kWh per pack               (flow)
│   └── $ = GWh × 1,000,000 kWh/GWh × $/kWh
├── Target-year view: the 20% share is measured in YEAR 5 → size year 5, not the base year
├── Profit pool: an assembler earns value-add, not pack price (cells dominate pack cost)
└── Entry mode: organic (4 yrs to first sale) | acquisition (~1 yr) | JV (technology partner)
```

### The quantified spine
**Base year, done right:**
```
Stationary stock  = 150 GW × 10% × 2 h                       = 30 GWh  (installed base: a one-off backlog)
EV flow           = 30M × 80% × 2% × 10 kWh = 4.8 GWh
                  + 30M × 20% × 2% × 35 kWh = 4.2 GWh        = 9 GWh/yr
Stationary flow   = 15 GW added × 10% × 2 h                  = 3 GWh/yr
Annual market     = 9 + 3 = 12 GWh/yr × $120/kWh             = $1.44B/yr
Retrofit backlog  = 30 GWh ($3.6B) → if retrofitted over 10 yrs [ILLUSTRATIVE], +3 GWh/yr
```

**Error fixed:** "30 GWh × $120/kWh = $360M" → **$3.6B** (30 GWh = 30,000,000 kWh; × $120 = $3.6B). This is a 10× slip. The tell is a line item that disagrees with its own total ($4,680M = $3,600M + $1,080M).

**Error fixed:** adding 30 GWh of storage for the whole installed base (a stock) to 9 GWh of one year's vehicle production (a flow) to get "39 GWh, $4.68B per year" → an annual market uses annual additions: ~12 GWh ≈ $1.44B. Show the retrofit backlog separately, spread over a realistic timeline.

**Error fixed:** sizing only the base year when the target is five years out → project year 5 from the growth inputs:
```
Vehicles          = 30M × 1.03^5                                   = 34.8M
EV share          = 2% × 1.75^5                                    = 32.8%
Avg pack          = 80% × 10 + 20% × 35                            = 15 kWh
EV flow           = 34.8M × 32.8% × 15 kWh                         ≈ 171.3 GWh
Stationary flow   = (150 × 1.1^5 − 150 × 1.1^4) GW × 10% × 2 h     ≈ 4.4 GWh
Year-5 market     ≈ 175.7 GWh × ($120 × 0.9^5 = $70.9/kWh)         ≈ $12.45B  (≈8.6× the base year in value)
20% share         ≈ 35.1 GWh/yr of assembly capacity               ≈ $2.49B of pack revenue
```

**Error fixed:** compounding EV share at 75%/yr indefinitely → 2% × 1.75^7 ≈ 100.5%, so the share passes 100% in year 7. Cap it with an S-curve for anything beyond year 5.

**Sanity checks that change the size:**
- **Pack size:** 10 kWh is high for two-wheelers (typically a few kWh; only three-wheelers approach the upper end). At 3 kWh [ILLUSTRATIVE], base-year EV flow is 5.6 GWh, not 9.
- **Uniform EV share:** 2/3-wheelers electrify far faster than 4-wheelers; split the share by segment.
- **Profit pool:** cells are the bulk of pack cost, so an assembler's value-add is perhaps ~30% [ILLUSTRATIVE] of pack price. A 20% share in year 5 is then a ~$0.75B value-add pool, not $2.49B.

**Timing is the decision.** On the same inputs, years 1–5 sum to ~383 GWh, and year 5 alone is ~46% of that. An organic entrant sells nothing until year 5, so it misses ~54% of the five-year volume. It would also have to go from zero to ~35 GWh/yr of capacity in a single year to hit the target, which is not credible.

### Recommendation
- **Enter via acquisition (or a JV with a technology partner if no target is available at a sensible price):** the four-year organic route cannot reach 20% of a year-5 market that is ~15× the base year's annual GWh. Before committing, check target availability and valuation, cell-import dependence and domestic-manufacturing incentives.
- **Sequence:**
  - **Years 1–5:** stationary storage paired with the client's own projects (a captive anchor customer), plus 2/3-wheeler packs (the fastest-growing volume).
  - **Later:** 4-wheelers, telecom and IoT.
  - **Long term:** backward integration into cells once scale justifies it.

### Coaching notes
- **What good looks like:** converts GWh to $ with the 10^6 kWh/GWh factor written down; separates stock from flow; sizes the year the target is measured in; caps runaway compounding; sizes the assembler's value-add rather than the pack price; links entry mode to the timing of market growth.
- **Red flags:** a line item that contradicts its total; adding installed-base storage to annual production; ignoring every growth input when the objective is five years out; recommending an acquisition with no valuation or target screen; spending all the time on calculations and leaving the qualitative case thin, while the calculations themselves are wrong.

---

## Case 13 — Low-Cost Carrier In-Flight Wi-Fi: Break-Even Take Rate
**Archetype:** New ancillary product → break-even adoption rate (the ancillary version of break-even volume), with load-factor, fee and utilisation sensitivities.

**Problem statement.** A US low-cost carrier (a domestic network plus a few near-international routes) has no in-flight Wi-Fi, while its rivals do:
- **Network rival (65% of fleet equipped):** vendor-branded, vendor-priced service at ~$25/session, on a revenue share.
- **Discount rival (90% equipped):** airline-branded, free service, bought wholesale.

The client will partner with a vendor to equip all 90 aircraft. Capex is $250K per aircraft, split 40/60 between airline and vendor. The airline then pays the vendor a per-session fee to cover operating costs. Fleet data:
- **10 widebodies:** 300 seats; 2,500 flights/yr across the sub-fleet.
- **80 narrowbodies:** 100 seats; 27,500 flights/yr across the sub-fleet.

What share of passengers must buy a $10 session for the airline to break even in 2 years? Market research shows paid take rates of 5–10%.

### Opening structure (issue tree)
```
Launch Wi-Fi: break even in 2 years?
├── Investment: airline share of capex × fleet
├── Revenue base
│   ├── Passengers = seats × flights × load factor × years   ← challenge each input
│   └── Net revenue per session = price − vendor per-session fee  ← not the gross $10
├── Required take rate = airline capex ÷ (passengers × net revenue per session)
├── Take-rate drivers: flight (length, time of day, other entertainment) |
│   product (price, speed, reliability) | passenger (age, income, business vs leisure)
└── Business model: revenue share | wholesale + own pricing | free (loyalty- or sponsor-funded)
```

### The quantified spine
```
Airline capex      = $250K × 40% × 90 aircraft         = $9M   ($1M widebody + $8M narrowbody)
Passengers (2 yrs) = 300 × 2,500 × 2 = 1.5M
                   + 100 × 27,500 × 2 = 5.5M           = 7M at 100% load factor
Take rate (given)  = $9M ÷ (7M × $10)                  = 12.9%  vs 5–10% observed
```

**Error fixed:** "7M passengers × take rate × $10 = $9M" → use **net** revenue after the per-session vendor fee and a **realistic load factor**: take rate = $9M ÷ (7M × LF × ($10 − fee)). The given-data 12.9% is a floor, not the answer.

| Required take rate | LF 100% | LF 85% | LF 80% |
|---|---|---|---|
| Fee $0 (gross $10) | 12.9% | 15.1% | 16.1% |
| Fee $3 [ILLUSTRATIVE] (net $7) | 18.4% | 21.6% | 23.0% |
| Fee $5 [ILLUSTRATIVE] (net $5) | 25.7% | 30.3% | 32.1% |

Re-frame the target. At the top of the observed band (10% take, 85% LF, $3 fee), annual net revenue = 7M ÷ 2 × 85% × 10% × $7 ≈ $2.08M, so **payback ≈ 4.3 years**, not 2. With a 10+ year vendor contract, a 4-year payback may still be acceptable; the 2-year gate is what should be questioned. Put the other way, breaking even in 2 years at a 10% take rate needs **~$15.1 of net revenue per session**.

**The input that can flip the answer: aircraft utilisation.** The fleet data imply ~250 flights per widebody and ~344 per narrowbody per year, under one a day. Low-cost narrowbodies typically fly several sectors a day. At 5 sectors a day [ILLUSTRATIVE]:
```
Narrowbody flights = 80 × 5 × 365                  = 146,000/yr
Narrowbody pax     = 100 × 146,000 × 2 × 85%       ≈ 24.8M
Widebody pax       = 1.5M × 85%                    ≈ 1.3M
Total (2 yrs)                                      ≈ 26.1M
Take rate (net $7) = $9M ÷ (26.1M × $7)            ≈ 4.9%   (3.4% at a gross $10)
```
That is at or below the bottom of the observed band. Confirm whether the flight counts are per aircraft or per sub-fleet before concluding anything.

### Recommendation
- **Launch, but decide on the right base:** verify utilisation and load factor first. On the data as given, the 2-year target needs a 13–32% take rate against an observed 5–10%; at realistic utilisation it is achievable.
- **Model:** buy connectivity wholesale and keep airline branding and pricing control. That keeps the customer relationship and makes Wi-Fi a lever for loyalty and ancillary bundles. Negotiate the fee structure hard: a per-session fee lands on every sale and raises the break-even take rate by roughly 40–100% (the $3–5 rows above).
- **Pilot:** start on high-propensity routes (longer, daytime, business-heavy) to prove the take rate, then roll out. Test a free-with-loyalty-sign-up tier. A discount rival already uses free Wi-Fi as its differentiator, so "we are low-cost, so we must charge" is not self-evident.
- **Risks:**
  - **Vendor and technology lock-in:** a 10+ year contract makes vendor and technology choice the critical decision.
  - **Bandwidth ceiling:** per-aircraft bandwidth caps concurrent users, which sets a ceiling on take rate per flight.
  - **Wrong yardstick:** evaluate on NPV, not a 2-year payback.

### Coaching notes
- **What good looks like:** writes the break-even take-rate formula before computing; uses net revenue per session; runs sensitivities on load factor and fee; challenges the flight-count input; turns "13% vs 5–10%" into "which routes and models clear the bar?".
- **Red flags:** accepting 100% load factor silently; using the gross $10 while ignoring the fee; assuming one session per passenger without saying so; claiming low-cost carriers should not offer free Wi-Fi when a discount rival does exactly that; saying "keep take rates low to protect speed" instead of treating bandwidth as a capacity limit.

---

## Case 14 — Access Pricing a Once-a-Year HIV Drug in Emerging Markets
**Archetype:** Pricing where the objective is *access*, not profit maximisation → epidemiological funnel → cost-recovery floor → tiered pricing and tender channels.

**Problem statement.** The world's largest pharmaceutical company (present in 200+ countries) has a novel, patented HIV drug taken once a year. It wants an emerging-market price that ensures fast, broad access; most of its profit will come from developed markets. Emerging markets here are emerging Asia (excluding the developed Asia-Pacific economies), Africa and Latin America; the Middle East is excluded for this exercise. R&D cost was $5B, and 40% of it ($2B) should be recovered in emerging markets, with a 10% profit on top. The patent was granted 10 years ago; assume 10 years of exclusivity remain. Count adults only. Case inputs [ILLUSTRATIVE]:

| Region | Adults | Prevalence | Attainable |
|---|---|---|---|
| Emerging Asia | 3B | 0.2% | 50% |
| Africa | 300M | 9% | 70% |
| Latin America | 600M | 0.4% | 40% |

### Opening structure (issue tree)
```
EM price for an access-first drug
├── Recovery requirement: R&D share for EMs ($2B) + per-dose COGS & distribution + margin
├── Volume over the exclusivity window
│   ├── Patients = adults × prevalence × attainable %   (by region cluster)
│   ├── Doses = patients × doses/yr × years of exclusivity × uptake
│   └── Time value: discount doses sold in later years
├── Cost-recovery floor = (R&D share ÷ discounted doses) + COGS, then margin
├── Affordability & tiering: who pays (governments, donors, tenders) and how much per tier
└── Protection & competition: local patents, compulsory licensing, generics,
    incumbent daily regimens as the real reference price
```

### The quantified spine
```
Emerging Asia   = 3B × 0.2% × 50%    = 3.0M patients
Africa          = 300M × 9% × 70%    = 18.9M
Latin America   = 600M × 0.4% × 40%  = 0.96M
Total           =                      22.86M patients/yr → × 10 yrs = 228.6M doses
R&D floor       = $2B ÷ 228.6M       = $8.75/dose
+10% profit     = $9.62 (10% markup on cost)  or  $9.72 (10% margin on price): state which
```

**Error fixed:** "3M + 18.9M + 0.96M = 22.8M" → **22.86M** (≈22.9M; 228.6M doses). The gap is small here, but truncating mid-chain compounds in bigger funnels.

**Error fixed:** "price = R&D ÷ doses × 1.1 = $9.6" as the cost-based floor → the floor must also carry per-dose manufacturing and distribution cost and the time value of money:

| Floor build | $/dose |
|---|---|
| R&D share only, undiscounted, full uptake | 8.75 |
| Discount doses at 8% over 10 yrs [ILLUSTRATIVE] (annuity factor 6.71 → 153.4M discounted doses) | 13.04 |
| + COGS & distribution $2/dose [ILLUSTRATIVE] | 15.04 |
| + 10% markup | **16.54** |

The realistic floor is ~1.7× the naive $9.62. Uptake matters too: at 70% average uptake over the window [ILLUSTRATIVE], the undiscounted R&D charge alone rises from $8.75 to $12.50.

**Tiering does less than you expect.** Africa holds ~83% of patients but has the least ability to pay, so a uniform price is effectively an African price. At the full floor, the required annual recovery = $16.54 × 22.86M ≈ $378M. If Asia and Latin America pay twice the African price: 18.9M × p + 3.96M × 2p = $378M → **p ≈ $14.10** in Africa and $28.20 elsewhere. That is only ~15% below the uniform $16.54, because the higher tiers hold too few patients to cross-subsidise much. The larger lever is the recovery allocation itself: cutting the emerging-market R&D share from 40% to 20% brings the full floor to **~$9.37**.

**Value and competitive reference (the lenses to add).** The drug is novel, but patients today take daily generic regimens. The annual cost of that regimen (tens of dollars per patient-year [ILLUSTRATIVE]) is the reference a tender buyer will use. A once-a-year dose also improves adherence, so a price near the floor sits well below the drug's value; the access objective, not value, is what holds the price there.

**Protection check:**
- **Basis of exclusivity:** it comes from patents and regulatory data protection, not copyright.
- **Patent term:** it runs from filing, not grant.
- **Territory:** a home-market patent does not protect the drug in emerging markets, which need local filings.
- **Main risks:** compulsory licensing and generic entry threaten the 10-year recovery window.
- **Inputs:** the case's prevalence and population figures (e.g., a continent-wide 9% adult prevalence) are far from current epidemiology; re-base them before real use.

### Recommendation
1. **Price at a transparent cost-recovery floor (~$15–17 per annual dose on these assumptions),** not the naive ~$9.60, and publish the tier logic.
2. **Tier by income group, but recognise that the cross-subsidy is small.** If the African tier must go lower, reduce the emerging-market R&D allocation so developed markets carry more, rather than loading the small higher tiers.
3. **Sell through the real payers:** government and donor tenders and pooled procurement. Multi-year volume commitments de-risk the uptake assumption. Offer voluntary licences to generic makers in the poorest tier to pre-empt compulsory licensing while protecting the higher tiers.
4. **Drop "price below competitors" as a goal:** there is no direct competitor; the reference is the cost of existing daily regimens.

### Coaching notes
- **What good looks like:** builds a region-by-region funnel with an access (attainable) filter; ties the recovery window to remaining exclusivity; states the markup-vs-margin convention; adds COGS and discounting to the floor; tests whether tiering can actually move the low-tier price; names tenders and donors as the payers.
- **Red flags:**
  - **Funnel:** population × prevalence with no access filter; the same patients treated at 100% uptake for 10 years.
  - **Floor:** a "cost-based" price that includes only R&D.
  - **Protection and payers:** "protected by copyright"; assuming governments can "easily" fund the drug through welfare schemes.
  - **Scope:** skipping the value and competitive lenses entirely.

---

## Case 15 — B2B Industrial Pricing: A Differentiated Mulch Film Entering North America
**Archetype:** Three-lens pricing (cost floor → competitive reference → value ceiling) for a differentiated B2B product, with a landed-cost check.

**Problem statement.** A leading Asian maker of packaging, agricultural and industrial films will enter North America with a high-durability, UV-resistant mulch film. It targets large commercial farms growing berries, tomatoes and peppers.
- **Cost:** manufacturing is $12 per 200 m roll, plus $3 shipping.
- **Competition:** three established competitors price comparable film at $18–24, $20–26 and $22–28 per roll.
- **Product claims:** ~30% longer life (UV resistance), higher tensile strength (fewer replacements), biodegradability, and better heat retention (higher cold-season yields).
- **Research:** farms will pay a 15–20% premium over the average competitor price.

Set the price.

### Opening structure (issue tree)
```
Price per roll
├── Floor: landed cost (manufacturing + freight + duty) + required margin
├── Reference: closest comparable competitor price (define "average" explicitly)
├── Ceiling: economic value to the farmer (EVC)
│   ├── Reference price
│   ├── + durability value (longer life / fewer replacements per season)
│   ├── + avoided removal & disposal (biodegradable)
│   ├── + yield gain (heat retention)
│   └── − switching cost / perceived risk of a new supplier
├── Channel: distributor margin between farm-gate price and net realised price
└── Strategy: differentiation (price toward value) vs share grab (price near reference)
```

### The quantified spine
```
Cost base         = $12 + $3                         = $15/roll
Cost-plus (40%)   = $15 × 1.40                       = $21  (a 40% markup = 28.6% margin)
                    a true 40% margin would be $15 ÷ 0.60 = $25
Competitor mids   = $21, $23, $25 → reference       = $23  (also the midpoint of $18–28)
Stated-WTP band   = $23 × 1.15 to $23 × 1.20         = $26.45 – $27.60
```

**Error fixed:** "mid-range competitor price = $22, so the band is $25.30–$26.40 and $26 is optimal" → the average competitor price is **$23** (the mean of the three midpoints, and the midpoint of the full range), so the band is **$26.45–$27.60**. A $26 price sits *below* stated willingness to pay and leaves money on the table.

**Error fixed:** calling "$15 × 1.40" a 40% margin → it is a 40% **markup** (a 28.6% margin). Confirm which one the client means; here the difference is $4 per roll.

**Economic value to the farmer [ILLUSTRATIVE components]:**
```
Reference price                                   $23.00
× 1.3 for 30% longer life                         $29.90  (if longer life converts into fewer rolls per season)
+ avoided removal & disposal (biodegradable)      + $4.00
+ yield gain from heat retention                  + $3.00
− switching cost / new-supplier risk              − $2.00
EVC                                               $34.90  → differentiation value = $11.90
```
The stated-WTP band ($26.45–$27.60) implies that farmers expect to keep ~61–71% of the $11.90 and cede ~29–39% to the supplier. That is a normal split for a new entrant without a track record. Value-selling (cost per hectare per season, trial plots) is how the price moves toward the top of the band and beyond.

**Landed-cost and channel check [ILLUSTRATIVE]:**
```
Farm-gate price                                   $27.00
Net to maker after a 20% distributor margin       $21.60
Landed cost ($15 + 5% duty)                       $15.75
Unit margin                                       $5.85  (27% of net price)
```
If the cost-plus $21 were the farm-gate price, the maker would net $16.80 and keep just $1.05 per roll (≈6%). Cost-plus pricing looks fine ex-works and fails once the channel is included.

**Product-claim check:** mulch film is usually single-season, and a biodegradable film is designed to break down in the field, which conflicts with "30% longer life". Clarify this with the client. Value the durability claim as fewer tears and mid-season replacements within a season (or multi-season use if the film is not biodegradable), not as a longer calendar life.

### Recommendation
- **Price at ~$27 per roll farm-gate,** inside the corrected $26.45–$27.60 band. Position it against the premium competitor ($22–28) as the closest comparable, not against the average.
- **Differentiate, don't discount:** cost-plus ($21) already sits inside the competitive band, so cost is not the constraint. The job is to capture more of the ~$11.90 of economic value through trials, agronomic proof and cost-per-hectare selling, then move the price up.
- **Protect net realisation:** negotiate distributor margins and account for duty and FX in the landed cost. After launch, track:
  - **Commercial:** volume and adoption against plan.
  - **Product:** field-verified durability and yield.
  - **Competitors:** their price responses.
  - **Macro:** resin prices, farm subsidies and plastics rules.

### Coaching notes
- **What good looks like:** separates markup from margin; defines the competitor reference arithmetically; builds an EVC stack rather than stopping at stated willingness to pay; checks net realisation after channel and duty; flags the biodegradable-vs-durable contradiction; states the strategic stance.
- **Red flags:** a $22 "average" that is not an average; pricing below the stated WTP band while claiming to maximise value; no landed cost or distributor margin; no view of volume or elasticity; taking a single-season product's "longer life" at face value.

---

## Case 16 — PE Carve-Out of a Mega-Cap Tech Company's Flagship Smartphone Division
**Archetype:** Invest/pass on a mega-deal → financeability and dis-synergies decide the answer before returns do. The companion to Case 5.

**Problem statement.** A large global PE fund is evaluating whether to buy the flagship smartphone division of a mega-cap consumer-technology company. The parent is considering a carve-out so it can focus on software and services.
- **Scale:** the division has ~$200B of revenue (~50% of the parent) and ~25% operating margin.
- **Dependencies:** it relies heavily on the parent's proprietary operating system, app marketplace, services, brand and supply chain.
- **Outlook:** growth is expected to be modest, with some room for cost and supply-chain efficiency; the market is mature and competitive.

Is this an attractive investment?

### Opening structure (issue tree)
```
Buy the carve-out?
├── Can it be financed at all?   ← gate 1
│   ├── Entry EV = multiple × STANDALONE EBITDA
│   ├── Debt capacity = max debt/EBITDA × EBITDA (market-clearing leverage)
│   └── Equity cheque vs per-deal capacity of the largest funds
├── What is standalone EBITDA?   ← gate 2 (dis-synergies)
│   ├── Segment EBIT + D&A
│   ├── − standalone corporate costs (functions the parent provided)
│   └── − OS / IP / ecosystem licence fees to the parent
├── Returns: MOIC / IRR vs hurdle (EBITDA growth, debt paydown, exit multiple)
├── Exit: IPO or strategic sale of a $300B+ asset?
└── Alternatives: spin-off, minority / structured stake, consortium, smaller asset
```

### The quantified spine
**Error fixed:** "25% operating margin on $200B → ~$50B EBITDA" → operating margin gives **EBIT** ($50B). EBITDA adds back D&A, and a carve-out must then deduct what the parent used to provide.

**Error fixed:** "a 2% margin improvement adds ~$4B" → true only for **+2 percentage points** (25% → 27%). A 2% *relative* improvement (25% → 25.5%) adds $1B.

**Error fixed:** "5–10× EV/EBITDA → $250–500B" with no basis → the multiple is arbitrary and far below what mega-cap tech parents often trade at (20×+ [ILLUSTRATIVE]). A seller anchored there would want ~$840B for $42B of standalone EBITDA. The multiple must also be applied to *standalone* EBITDA, not segment profit.

```
Standalone EBITDA [ILLUSTRATIVE]
  Segment EBIT                           $50B
  + D&A                                  + $6B
  − standalone corporate costs (2% rev)  − $4B
  − OS/IP licence fee (5% rev)           − $10B
  = Standalone EBITDA                    $42B

Financeability [ILLUSTRATIVE]
  Entry EV at 8×                         = $336B
  Debt at 5× EBITDA                      = $210B   (interest at 8% = $16.8B → 2.5× cover)
  Equity cheque                          = $126B   (37.5% of EV)
  Largest funds ~$25B × 15% single-deal limit = ~$3.75B per deal
  → the equity alone ≈ 34 fund-sized cheques; the debt package is several times
    the largest buyout financings ever syndicated

Returns, 5-yr hold [ILLUSTRATIVE]
  Exit EBITDA  = $42B + $4B (+2 pp margin)  = $46B
  Exit EV      = 8 × $46B                   = $368B
  Net debt     = $210B − $60B paydown       = $150B
  Exit equity  = $368B − $150B              = $218B
  MOIC         = $218B ÷ $126B              = 1.73× → IRR ≈ 11.6%
  For a 20% IRR: MOIC 2.49× → exit equity $313.5B → exit EV $463.5B
               → EBITDA of ~$57.9B at 8× (+38%), or a ~10.1× exit multiple on $46B
```

Every gate fails:
- **Financing:** no fund or consortium can write the equity cheque, and the debt dwarfs any buyout financing to date.
- **Returns:** the base case misses a ~20% hurdle without heroic multiple expansion.
- **Exit:** an IPO or strategic sale of a ~$370B asset is itself a capital-markets constraint.

**Dependency cuts both ways.** The parent's services revenue rides on the device installed base, so separation weakens the parent's flywheel as well as the division's product. The parent will therefore demand licence and revenue-share terms that move value back to itself, and that fee line is exactly what shrinks standalone EBITDA.

### Recommendation
**Pass on a control buyout.** The deal cannot be financed at any credible multiple. Standalone EBITDA is materially below segment EBIT once licence fees and standalone costs are paid. Base-case returns (~12% IRR) sit well below the hurdle. If the fund still wants exposure:
- **(a) Spin-off:** propose a spin-off to the parent's shareholders, the natural route for an asset this size, with the fund as an anchor investor.
- **(b) Minority or structured stake:** e.g., preferred equity alongside the parent.
- **(c) Smaller asset:** target a smaller, genuinely separable hardware line.

Any structure needs a long-term, price-capped OS/ecosystem licence and a transition services agreement.

### Coaching notes
- **What good looks like:** checks financeability before attractiveness; distinguishes EBIT from EBITDA and segment from standalone profit; sizes the dis-synergies; computes MOIC and IRR against a hurdle; reads "2%" as percentage points vs relative change; offers structures that actually fit the deal's size.
- **Red flags:** "financially attractive, proceed with caution" on a deal no fund can finance; an unexplained 5–10× multiple; no IRR in a PE case; ignoring that the parent's own economics depend on the division; assuming an IPO exit without sizing it.

---

## Case 17 — Beverage Company: "Revenue Is Falling" Is the Wrong Premise
**Archetype:** Growth/profitability diagnosis where the stated problem is false → segment P&L, then a price-volume-mix (PVM) bridge that exposes trade-down and cannibalisation.

**Problem statement.** A leading beverage company says its growth has dropped since last year and that the issue is company-specific. It sells soda, water and other drinks (shakes, syrups, smoothies). Data in ₹M of revenue, millions of litres and ₹/L [ILLUSTRATIVE]:

| Segment | Litres Y1 → Y2 | Price/L Y1 → Y2 | Cost/L | Revenue Y1 → Y2 |
|---|---|---|---|---|
| Soda | 100 → 120 | 30 → 24 | 15 | 3,000 → 2,880 |
| Water | 30 → 33 | 25 → 25 | 12 | 750 → 825 |
| Others | 10 → 11 | 50 → 55 | 30 | 500 → 605 |

| Soda brand | Litres Y1 → Y2 | Revenue Y1 → Y2 | Price/L Y1 → Y2 |
|---|---|---|---|
| Brand A (premium) | 50 → 30 | 1,800 → 1,080 | 36 → 36 |
| Brand B | 25 → 30 | 650 → 780 | 26 → 26 |
| Value brand | 25 → 60 | 550 → 1,020 | 22 → 17 |

### Opening structure (issue tree)
```
"Growth has dropped": which metric?  ← clarify: revenue, profit or growth rate?
├── Segment P&L: revenue AND gross profit by segment (use the cost column)
├── Soda revenue bridge (PVM)
│   ├── Volume: Δlitres × old average price
│   ├── Mix: new litres at OLD brand prices − new litres at old average price
│   └── Price: new litres × (new price − old price) by brand
├── Cannibalisation test: where did Brand A's litres go?
└── Levers: value-brand price and fencing | Brand A positioning | Others' pricing power
```

### The quantified spine
**Segment P&L (₹M):**
```
Revenue       4,250 → 4,310   (+1.4%)
Gross profit  2,090 → 1,784   (−14.6%)   margin 49.2% → 41.4%
  Soda        1,500 → 1,080   (−28%)     margin 50% → 37.5%   (revenue only −4%)
  Water         390 →   429   (+10%)
  Others        200 →   275   (+37.5%)   price +10% with volume still +10%
```

**Error fixed:** "revenue has been dropping" → total revenue **rose** 1.4%; only soda revenue fell (−₹120M, −4%). The real decline is in **gross profit (−₹306M, −14.6%)**, which shows up only if the cost column is used.

**Soda PVM bridge (₹M):**
```
Volume  = (120 − 100) × ₹30                                  = +600
Mix     = (30×36 + 30×26 + 60×22) − 120×30 = 3,180 − 3,600    = −420
Price   = 60 × (17 − 22)   (A and B unchanged)               = −300
Total   = +600 − 420 − 300                                   = −120  ✓ (2,880 − 3,000)
```

**Error fixed:** "the decline is Brand A's volume loss plus the value brand's price cut" → soda volume actually **grew 20%**. The drag is **mix (−420)**, which is larger than price (−300). Brand A's loss is a shift into the value brand, not lost category demand.

**Gross-profit view (cost ₹15/L for all soda brands):** unit GP is ₹21 for A, ₹11 for B, and ₹7 → ₹2 for the value brand after the cut. The GP bridge is volume +300, mix −420, price −300 = −420 (1,500 → 1,080). The value brand's unit GP fell 71%. Every litre that moved from A to the value brand gave up ₹19 of GP, so the 20M litres A lost are worth ₹380M of GP on their own.

**Cannibalisation read:** A lost 20M L, B gained 5M L and the value brand gained 35M L. A 23% price cut drove a 140% rise in value-brand volume (an implied elasticity of about −6). That is far more than category growth explains, so most of the new volume was taken from A.

**Re-pricing test:** at ₹22/L (₹7 unit GP), the value brand needs only 120 ÷ 7 ≈ 17.1M L to earn today's ₹120M of GP. It could lose ~71% of its volume and still break even on GP, before counting any litres that return to A.

### Recommendation
1. **Reframe the problem for the client:** revenue is up; profit is down 14.6% because of a soda trade-down.
2. **Fix the value-brand price cut first:** restore the price, or fence the discount (pack sizes, channels, occasions) so it stops pulling Brand A buyers. Test elasticity in pilot markets, and track where the litres go, not just value-brand volume.
3. **Reposition Brand A only after the cannibalisation stops.** Re-targeting A will not work while a cheaper sibling is pulling its buyers down.
4. **Lean into Others,** which took a 10% price increase and still grew volume 10%. Size any new categories (low-sugar, energy) before recommending them.

### Coaching notes
- **What good looks like:** asks which metric dropped; uses the cost column; builds a PVM bridge that reconciles to the total; separates mix from price; tests for cannibalisation; quantifies the re-pricing break-even.
- **Red flags:** accepting "revenue is falling" without checking the total; treating Brand A's decline as a Brand A problem (marketing, shelf placement); raising the value brand's price without asking where the volume goes; listing new products with no sizing; ignoring the Others segment's pricing power.

---

## Case 18 — Ambulatory Surgery Centre Chain: +15% Revenue Across Six Service Lines
**Archetype:** Provider revenue growth → service-line table, lever sizing without double counting, and prioritisation on contribution and OR time rather than headline reimbursement.

**Problem statement.** A profitable US chain of six same-day surgical centres offers six service lines: orthopaedics, neurology, gastroenterology, pain management, urology and dermatology. Revenue is flat at $60M and the client wants +15%. Capacity has some headroom, and competition is typical for urban and suburban markets. Service-line data:

| Line | Avg reimbursement | Visits/yr | Revenue |
|---|---|---|---|
| Ortho | $2,500 | 4,000 | $10.0M |
| Neuro | $3,000 | 3,333 | $10.0M |
| Gastro | $1,800 | 5,556 | $10.0M |
| Pain | $2,000 | 5,000 | $10.0M |
| Urology | $2,200 | 4,545 | $10.0M |
| Derma | $1,500 | 6,667 | $10.0M |
| **Total** | **$2,062 blended** | **29,101** | **$60.0M** |

### Opening structure (issue tree)
```
+$9M revenue ($60M → $69M)
├── Volume
│   ├── New patients: marketing, referral relationships, underserved catchments
│   ├── Procedures per patient: cross-sell, bundled pathways
│   └── Capacity/services: new high-demand procedures, extended hours
├── Rate
│   ├── Negotiate commercial rates (benchmark outcomes and cost vs hospitals)
│   ├── Payer mix: grow commercial referrals (never turn away government patients)
│   └── Premium add-ons (fast-track consults, follow-up packages)
└── Prioritise by: contribution per case → contribution per OR-hour once capacity binds
                   | referral elasticity | incremental cost | compliance risk
```

### The quantified spine
**The equal-revenue trap.** Every line earns ~$10M, so a given % volume lift yields the same dollars in any line: +10% in Neuro = 333 × $3,000 ≈ $1.0M, exactly what +10% gives in any other line. "Prioritise Neuro because its rate is highest" has no revenue basis.

**Error fixed:** "5% of 29,101 visits = 1,455 × $2,000 blended = $2.9M" → the blended rate is $60M ÷ 29,101 = **$2,062**, so a uniform 5% lift = 5% × $60M = **$3.0M**.

**Error fixed:** "volume from marketing and referrals = $4.1M" → the two levers sum to $1.0M + $3.0M = $4.0M, but Neuro's share of the across-the-board lift (5% × $10M = $0.5M) is counted twice, so the de-duplicated total is **~$3.5M**. That leaves **$5.5M** to find, an 8.7% rate uplift on the ~$63.5M post-volume base, and that gap was never sized. (The premium add-on example, 400 × $200 = $80K, is under 1% of the target.)

**Prioritise on contribution, not rate [ILLUSTRATIVE cost and time inputs]:**

| Line | Rate | Variable cost | Contribution/case | OR min/case | Contribution/OR-hour |
|---|---|---|---|---|---|
| Pain | $2,000 | 25% | $1,500 | 30 | **$3,000** |
| Gastro | $1,800 | 30% | $1,260 | 30 | $2,520 |
| Derma | $1,500 | 20% | $1,200 | 30 | $2,400 |
| Urology | $2,200 | 35% | $1,430 | 45 | $1,907 |
| Ortho | $2,500 | 55% (implants) | $1,125 | 90 | $750 |
| Neuro | $3,000 | 50% | $1,500 | 150 | **$600** |

Ranking by contribution per OR-hour reverses the ranking by rate.
- **+10% Neuro (333 cases):** ~$0.50M of contribution, using ~833 OR-hours.
- **+10% Pain (500 cases, the same $1.0M of revenue):** $0.75M of contribution, using 250 OR-hours.

While capacity has headroom, rank lines by contribution per case and achievable demand; once utilisation tightens, rank by contribution per OR-hour.

**Rebuilt lever plan (each lever sized on its own base, no overlap) [ILLUSTRATIVE]:**
```
Volume +5% all lines (marketing, referrals)            5% × $60M                  $3.0M
Extra +5% on Pain + Gastro (top contribution/OR-hr)    5% × ($10M + $10M)         $1.0M
Payer mix: +5 pp commercial via commercial referrals
  (50/50 mix; government pays 0.6× commercial →
   commercial = 1.25×, government = 0.75× blended)     5% × 0.5 × $60M            $1.5M
Commercial rate +4% on the ~$37.5M commercial book     4% × $37.5M                $1.5M
New high-demand procedure                              600 cases × $2,500         $1.5M
Premium add-ons                                        2,910 visits × $200        $0.6M
Total                                                                             ≈ $9.1M  ✓ ≥ $9M
```
Justify spend on contribution, not a blended "ROI beats 15%". The two volume levers add ~$2.65M of contribution a year; against, say, $1.5M/yr of marketing [ILLUSTRATIVE], that nets ~$1.15M/yr.

### Recommendation
Hit the $9M with a sized, overlap-free portfolio:
- **~$4M from volume:** weighted toward high-contribution, short-case lines.
- **~$3M from payer mix and commercial rates:** backed by outcome and cost benchmarks against hospital settings.
- **~$2M from new procedures and premium add-ons.**

Track contribution and OR utilisation alongside revenue. Run referral partnerships and payer-mix initiatives through compliance review (referral-inducement and self-referral rules; patient-access obligations).

### Coaching notes
- **What good looks like:** notices that every line earns ~$10M; computes the blended rate instead of assuming one; removes double counting; sizes the remaining gap; ranks lines on contribution and OR time; keeps a revenue target separate from an investment return.
- **Red flags:** "Neuro pays most, so grow Neuro"; stacking overlapping volume levers; leaving ~$5M as "rate increases and premium services" with no numbers; "shift patients to private insurers" without regard to access, ethics or regulation; judging marketing spend against a revenue growth rate.

---

## Case 19 — E-Commerce Platform: Cutting a 25% Return Rate
**Archetype:** Operations cost problem with a trend break → diagnose what changed, cost a return fully, Pareto the reasons, and prevent returns before optimising reverse logistics.

**Problem statement.** A large e-commerce platform's return rate (the share of delivered orders sent back) is 25%, up from 15% six months ago; peers run at 18–20%. It ships ~10M orders a month and wants to cut returns digitally without reducing assortment. Logistics cost is ~₹200 per return. Return reasons: size/fit 40%, product-quality mismatch 25%, changed mind 20%, delivery errors 5%, other 10%. About 10% of customers generate 40% of returns.

### Opening structure (issue tree)
```
Reduce returns (25% → ?)
├── What changed in six months? (15% → 25%)  ← ask this first
│   ├── Category mix (more apparel/footwear?)
│   ├── Policy (longer windows, free returns, instant refunds?)
│   ├── Supply (new sellers, catalogue quality, sizing standards?)
│   └── Demand (sale events, new customer cohorts?)
├── Why do returns happen? (reason-code Pareto)
│   ├── Pre-purchase expectation mismatch: size/fit, quality vs listing
│   ├── Fulfilment: wrong item, damage, delay
│   └── Behaviour/policy: bracketing (ordering multiple sizes), changed mind, abuse
└── What does a return cost? (full cost, not reverse shipping alone)
    → Prevent first, then make the remaining returns cheaper
```

### The quantified spine
```
Returns          = 10M × 25%                           = 2.5M/month
Logistics cost   = 2.5M × ₹200                         = ₹500M/month (₹6B/yr)
Full cost/return = ₹200 reverse + ₹80 wasted forward shipping
                   + ₹30 handling + ₹120 write-down/refurbishment = ₹430 [ILLUSTRATIVE]
Full cost        = 2.5M × ₹430                         ≈ ₹1.08B/month (₹12.9B/yr), 2.15× the logistics-only view
```

**Error fixed:** sizing the prize only as "reach the peer 20%: 0.5M × ₹200 = ₹100M/month" → that is the smallest version of the prize. Returning to the client's **own 15%** avoids 1.0M returns: ₹200M/month at logistics cost, or **₹430M/month (₹5.16B/yr)** at full cost. Even the peer level is worth ₹215M/month at full cost.

**Diagnose the jump with a mix test [ILLUSTRATIVE rates]:** suppose apparel returns at 40% and everything else at 8%. A blended 15% then implies apparel was ~22% of orders; a blended 25% would need apparel at ~53%. A 31-point category shift in six months is implausible without a major sale or category push, so mix alone probably does not explain the jump. Check within-category rates, policy changes and new sellers next.

**Reason-code Pareto and lever sizing (per month) [ILLUSTRATIVE lever effects]:**

| Reason | Share | Returns | Lever | Cut | Returns avoided | Saving at ₹200 |
|---|---|---|---|---|---|---|
| Size/fit | 40% | 1.0M | Fit recommendations, brand-level size charts | 25% | 250K | ₹50M |
| Quality mismatch | 25% | 625K | 360° imagery, seller catalogue standards, reviews | 20% | 125K | ₹25M |
| Changed mind | 20% | 500K | Exchange-first flows; fee on non-defect returns for heavy returners | 15% | 75K | ₹15M |
| Delivery errors | 5% | 125K | Pick/pack verification | 50% | 62.5K | ₹12.5M |
| Other | 10% | 250K | Investigate | — | — | — |
| **Total** | | **2.5M** | | | **512.5K** | **₹102.5M** |

These levers take the rate to (2.5M − 0.51M) ÷ 10M ≈ **19.9%**, the peer level, and save ~₹220M/month at full cost. Getting back to 15% requires diagnosing the jump; the Pareto alone will not get there.

**Error fixed:** treating "size/fit (40%) + quality (25%) + heavy returners (significant)" as additive drivers → they overlap. Heavy returners who order several sizes show up under the size/fit code, so much of the 40% of returns from heavy returners and the 40% coded size/fit are the same returns. Size the levers along one axis only.

**Heavy-returner concentration:** 10% of customers generate 40% of returns (1.0M/month), so a heavy returner returns 4.0 ÷ 0.67 = **6×** as often as other customers. Before tightening their policy, check net contribution per customer: many heavy returners are also heavy buyers.

**Prevent before you optimise:** a prevented return saves the full ~₹430. Better routing and faster restocking might save ~₹30 per return, or ~₹60M/month on the ~2.0M returns that remain at the peer level. Both are worth doing, but prevention is worth far more per return.

**Structure note:** wrong items and transit damage are fulfilment issues, not expectation mismatch. The 65% pre-purchase mismatch is fit plus quality only.

### Recommendation
1. **Diagnose the 15% → 25% jump** by category, seller cohort, policy change and campaign before building solutions; the fix for the extra 10 points lies in whatever changed.
2. **Prevent expectation-mismatch returns** (65% of volume): fit recommendations and brand-level size charts, richer imagery, seller catalogue standards and better use of reviews.
3. **Manage behaviour selectively:** identify heavy returners with analytics, then apply exchange-first flows, store credit and tailored return terms to unprofitable customers only.
4. **Then optimise reverse logistics:** nearest-node routing, faster inspection and restocking, and direct resale channels for returned stock.
5. **Measure the full cost per return** so business cases use ₹430, not ₹200.

### Coaching notes
- **What good looks like:** asks what changed before explaining the level; costs a return fully; sizes the prize against both the peer level and the client's own baseline; sizes levers by reason code without double counting; weighs heavy-returner policy against customer value.
- **Red flags:** jumping to reverse-logistics fixes first; adding overlapping drivers; costing returns at logistics cost only; putting fulfilment errors in the expectation-mismatch bucket; ignoring the 20% "changed mind" code; no category split (fashion vs electronics).

---

## How Claude should use this file
1. **As interviewer:** pick a case, reveal data only when the candidate asks for the right node, grade against the coaching notes.
2. **As coach:** compare a candidate's structure to the issue tree, push toward the quantified spine.
3. **On a real problem:** pattern-match (BP device = influencer-economics in a channel; drone = cost-floor-vs-value-ceiling; pharma = idiosyncratic decline vs growing market; PE = returns-math discipline; packaged snacks = demand→capacity via service level; foam-mattress = regulatory shift as demand-migration lever; gym = underserved-segment wedge + standardise-vs-speed; confectionery = value-chain isolation to the last metre; cross-border e-commerce = year-1 break-even gated by the partner choice; battery-pack entry = GWh→$ conversion done right, stock vs flow of installed capacity; in-flight Wi-Fi = break-even take rate on net revenue at realistic load factor; once-a-year drug = cost-recovery floor, then affordability and tiered access; mulch film = cost floor → competitor reference → EVC ceiling; smartphone carve-out = financeability and dis-synergies before synergy; beverage = test the premise with price-volume-mix; surgery-centre chain = prioritise by margin per OR-hour, not % lift; returns = diagnose the change, not the level, and cost a return fully).
4. Tag any number you add as **[ILLUSTRATIVE]**; show the math explicitly; sanity-check order of magnitude.
