# India Guesstimates, Benchmarks & Case Drills

Companion to `references/guesstimates-and-frameworks-quantified.md` and `references/case-bank-worked.md`, tuned to the **Indian market**: worked guesstimates drawn as segment trees, a benchmark-numbers cheat sheet, compact sector snapshots, and a few case drills. Every figure here is an **approximate, directional benchmark** for structuring — label anything you compute on top as `[ILLUSTRATIVE]` and sanity-check the arithmetic before presenting.

---

## India benchmark numbers (memorize the spine)

The estimation "starter kit." Round aggressively — precision is not the point; a defensible structure is.

| Quantity | Working number | Notes |
|---|---|---|
| Population | ~1.4 billion | ~1,400 million |
| Urban : rural | ~35% : 65% | urbanizing ~1%/yr |
| Persons / household | ~4–5 | urban ~4, rural ~5 |
| Households | ~300 million | population ÷ ~4.6 |
| Income mix (rule-of-thumb) | ~10% high / ~40% middle / ~50% low | segment ownership rates off this |
| Working-age share | ~65% | the "demographic dividend" |
| Median age | ~28–29 years | young population |
| Smartphone users | ~700–750 million | ~half the population |
| Two-wheelers : cars (new sales) | ~5 : 1 | 2W dominate personal mobility |
| Metro-city population | Delhi/Mumbai ~20M+ each | tier-1 cluster for demand sizing |
| City-proper populations (2011 census base, growing ~2%/yr) | Mumbai ~12M · Delhi ~11M · Bengaluru ~8.5M · Hyderabad ~7M · Ahmedabad ~5.5M · Chennai / Kolkata / Surat ~4.5M each · Pune ~3M | Clarify **city-proper vs. metro region** before sizing; the two differ by up to 2× |
| Household size, split | rural ~5.2 · urban ~4.0 | Use the split when the tree has an urban/rural branch |
| Alternative income split | urban ~30% upper-middle / 30% middle / 40% lower-middle; rural ~10% upper-middle / 40% middle / 30% lower-middle / 20% below poverty line | A finer cut than 10/40/50 when urban vs. rural behaviour differs |
| Spend of income | food ~35% · discretionary ~25% · housing ~10% · transport ~10% · travel ~10% · education ~5% · health ~5% | Consumption ~70% of income, savings ~30% (varies sharply by income) |
| Age spread (approx.) | 0–14 ~25% · 15–24 ~18% · 25–34 ~17% · 35–44 ~15% · 45–54 ~11% · 55+ ~14% | Check your own age buckets sum to 100% and don't overlap |
| GDP vs. workforce by sector | agriculture ~18% of GDP / ~45% of workers · industry ~29% / ~25% · services ~53% / ~30% | Explains the rural-income and productivity gap in any rural-demand case |

**Income-segmentation move** (the most reused pattern): split any population into 10/40/50 high/middle/low, then apply a different ownership or consumption rate to each tier. It appears in almost every ownership guesstimate below.

---

## Worked guesstimate 1 — vehicle license plates in a large state

*Prompt: estimate the number of license plates in a state of ~120M people (personal vehicles only).*

```
                     State population (120M)
                              │  ÷ ~4 persons/household
                     Households (30M)
             ┌───────────────┼────────────────┐
        High income      Middle income      Low income
         (10% = 3M)       (40% = 12M)        (50% = 15M)
        veh. own 90%      veh. own 50%       veh. own 30%
         = 2.7M            = 6M               = 4.5M
        × 2 veh/HH        × 1.5 veh/HH        × 1 veh/HH
         = 5.4M            = 9M               = 4.5M
             └───────────────┼────────────────┘
                     Vehicles ≈ 18.9M
                              │  × 2 plates per vehicle
                     License plates ≈ 37.8M
```

**Coaching notes:** clarify scope first (personal vs. commercial — here, personal only). The segment tree + differentiated ownership rates is the reusable engine. Close by naming where you'd refine (commercial fleets, multi-vehicle skew at the top).

## Worked guesstimate 2 — an everyday-object stock (dinner plates)

*Prompt: estimate the number of dinner plates in a state of ~100M people.*

```
        State population (100M)
   ┌──────────┼───────────┐
 High(10%)  Middle(40%)  Low(50%)
   10M         40M          50M
 own 100%    own 80%      own 60%
   10M         32M          30M
  ×8 plates   ×5 plates    ×3 plates   ← per person, by income
   80M         160M         90M
   └──────────┼───────────┘
     Households ≈ 330M plates
   (+ specify, don't compute: restaurants & offices as a separate add-on)
```

**Coaching notes:** a "stock" estimate (things that exist) vs. a "flow" estimate (things per period). State your assumption for plates-per-person and flag the non-household channels (restaurants, canteens) as an approach rather than grinding every branch — interviewers often only want the method there.

## Worked guesstimate 3 — an annual flow (new two-wheeler sales)

*Prompt: estimate annual new two-wheeler sales in India.* `[ILLUSTRATIVE]`

```
  Population 1,400M ÷ ~4.6 → households ~300M
  2W-owning households ~40% → ~120M own at least one 2W
  Installed base of 2Ws ~180M (some HHs own >1)
        │  replacement + new-adoption flow
  Avg 2W life ~10 yrs → replacement ≈ 180M / 10 = 18M/yr
  + net new adoption ≈ 2–3M/yr
        └─ Annual 2W sales ≈ ~20M   (reconcile vs. reported ~18–20M ✓)
```

**Coaching notes:** the **installed-base ÷ life + net-adds** pattern is the go-to for durable-goods flows (phones, TVs, cars, appliances). Always reconcile against a known reported figure if you have one — a two-method cross-check builds credibility.

## Worked guesstimate 4 — a daily flow via capacity/route logic (metro ridership)

*Prompt: estimate daily passenger journeys on a large city's metro.* `[ILLUSTRATIVE]`

```
  SUPPLY-SIDE (capacity) view          DEMAND-SIDE (population) view
  ─────────────────────────           ────────────────────────────
  Lines ~12, trains/line/hr ~15        City pop ~20M
  Cars/train ~8, cap/car ~300          Metro-catchment & affordability ~30% → 6M
  → train capacity ~2,400              Ride metro on a given day ~40% → 2.4M
  Peak-hr occupancy ~70% → 1,680       Avg journeys/rider/day ~2 (there + back)
  Operating hrs ~18, avg occ ~45%      → ~4.8M journeys
  → per-line-day ≈ 15×18×2400×0.45
    ≈ 290k ; ×12 lines ≈ ~3.5M           RECONCILE the two: ~3.5–5M/day ✓
```

**Coaching notes:** two independent methods (supply capacity vs. demand population) that you **reconcile** is the strongest guesstimate move — it signals rigor and self-checks your assumptions. Route/capacity logic also fits airlines, toll roads, and stadiums.

## Worked guesstimate 5 — a consumption total (monthly residential electricity)

*Prompt: estimate monthly residential electricity consumption in India.* `[ILLUSTRATIVE]`

```
  Households ~300M
   ┌──────────────┼───────────────┐
  High(10%=30M)  Middle(40%=120M) Low(50%=150M)
  ~300 kWh/mo    ~120 kWh/mo      ~30 kWh/mo
   = 9.0B kWh     = 14.4B kWh      = 4.5B kWh
   └──────────────┼───────────────┘
        ≈ 28 billion kWh / month (residential only)
   (state approach: exclude commercial & industrial; specify, don't grind)
```

**Coaching notes:** the income-tiered **units × per-unit consumption** pattern covers most "total consumption" prompts (water, fuel, data, groceries). Tie the per-tier rate to appliance ownership (AC vs. fan) to justify the spread.

## Worked guesstimate 6 — a decision tree (expected value, not a count)

*Prompt: should a studio green-light a film? Estimate expected profit.* `[ILLUSTRATIVE]`

```
                     Release film (cost ₹50cr)
              ┌───────────────┼───────────────┐
           Hit (25%)       Average (50%)      Flop (25%)
          net +₹200cr       net +₹20cr        net −₹40cr
              │                │                  │
   EV = 0.25(200) + 0.50(20) + 0.25(−40) = 50 + 10 − 10 = +₹50cr
```

**Coaching notes:** some "guesstimates" are really **expected-value decision trees** — assign probabilities to outcomes, value each branch, sum. State that a positive EV still hides downside risk (the 25% flop), so pair EV with a risk view before recommending. See `references/decision-making-under-uncertainty.md`.

---

## India sector snapshots (competitive structure at a glance)

Directional market-structure notes for fast orientation. For the **deep version** — market size, value chain, KPIs, regulators, and case tension per sector — read `references/india-sector-primers.md`; pair with `references/india-corporate-houses.md` (who the incumbents are) and `references/industry-heuristics.md` (global sector economics).

| Sector | Structure & who leads | The recurring case tension |
|---|---|---|
| Automobile | 2W (Hero, Honda, TVS, Bajaj) >> cars (Maruti Suzuki dominant, then Hyundai, Tata, Mahindra) | ICE→EV transition; rural demand cyclicality |
| Aviation | Consolidated: IndiGo dominant, Air India (Tata) #2; LCC-led | Fuel + lease costs vs. yield; route economics |
| Cement | Regional, freight-bound; UltraTech (ABG) #1, then Adani (ACC/Ambuja), Shree | Utilization, freight radius, consolidation |
| E-commerce | Flipkart (Walmart) vs. Amazon; Meesho on value tier; quick-commerce surging | Growth vs. contribution margin; logistics cost |
| FMCG | HUL, ITC, Nestlé, Britannia; deep rural distribution | Rural vs. urban, premiumization, D2C disruption |
| Financial services | Private banks (HDFC, ICICI, Axis) + NBFCs (Bajaj Finance) + fintech | Credit cost, NIM, digital acquisition |
| Steel | JSW, Tata Steel, SAIL, AM/NS, Vedanta | Global price cycle, input (coking coal) costs |
| IT / ITES | TCS, Infosys, Wipro, HCLTech; export-led | Wage inflation, discretionary spend, GenAI shift |
| Oil & gas | Reliance + PSUs (IOC, BPCL, ONGC) | Refining margins; energy-transition capex |
| Telecom | 3-player: Jio, Airtel, Vodafone Idea | ARPU repair, spectrum/5G capex, market repair |
| Pharma | Sun, Dr. Reddy's, Cipla; generics-export + domestic | US pricing pressure; complex generics, CDMO |
| Power | Generation (NTPC, Adani, Tata, JSW) + discom stress | Renewables shift, discom receivables |

---

## Case drills (compact worked patterns)

Rewritten as reusable patterns, not transcripts. Each: setup → structure → quantified spine → the "aha" → the trap.

### Drill A — Market entry: edible-oil manufacturer eyeing a new region
- **Structure (3C + entry lens):** market attractiveness (size, growth, margins) · competitive intensity (fragmented local vs. branded) · our right-to-win (sourcing, distribution, brand) · entry mode (build/buy/partner).
- **Quantified spine:** size the target region's consumption = population × per-capita edible-oil kg/yr × price; segment branded vs. loose; estimate reachable share × contribution margin vs. entry capex → payback.
- **Aha:** in edible oil the battle is **distribution reach and input-cost (imported palm/soy) pass-through**, not product — a fragmented "loose oil" base is the real share pool to convert.
- **Trap:** anchoring on brand marketing while ignoring that raw material is 70%+ of cost and swings margins more than any pricing move.

### Drill B — Profitability: a kirana (neighborhood) store under pressure
- **Structure:** Profit = Revenue − Cost. Revenue = footfall × conversion × basket × frequency. Cost = COGS + rent + labor + shrinkage/wastage.
- **Quantified spine:** disaggregate the decline — is footfall down (quick-commerce/e-grocery stealing trips?), basket down (trading down?), or margin down (input costs, credit given to customers)?
- **Aha:** the modern kirana threat is **quick-commerce eroding high-frequency, low-basket trips**; the defense is convenience (home delivery, digital payments/UPI, credit relationships) and category focus, not price war.
- **Trap:** treating it as a pure pricing problem when the driver is trip-frequency loss to a new channel.

### Drill C — Growth: a marketplace deciding where to expand
- **Structure:** grow existing (deepen wallet: frequency, cross-sell, AOV) vs. adjacent (new categories/geos) vs. new (new business model). Score each on market size × right-to-win × investment.
- **Quantified spine:** for each option, Δrevenue = incremental users × conversion × AOV × frequency, netted against CAC and contribution margin.
- **Aha:** the highest-ROI growth is usually **deepening monetization of the existing base** (raise frequency/AOV) before the costlier land-grab into new geos.
- **Trap:** confusing GMV growth with profit growth — India marketplace cases live or die on **contribution margin per order**, not top-line.

### Drill D — Pricing: a new toll expressway (or a first-of-its-kind product)
- **Structure (the three pricing lenses):** cost-plus floor (recover build + O&M + return over concession years) · value-based ceiling (willingness-to-pay = time + fuel saved vs. the old route) · competitive/alternative anchor (the free highway, rail, or air).
- **Quantified spine:** WTP ≈ (hours saved × value of time) + fuel saved; set the toll below that ceiling and above the cost floor; multiply by projected traffic × ramp-up to test concession-period payback.
- **Aha:** where there's no comparable, **anchor on value delivered (time/fuel saved), not cost** — the customer pays for the saving, not your construction bill. Segment by vehicle class (car vs. truck WTP differ sharply).
- **Trap:** cost-plus pricing that ignores WTP leaves money on the table (or kills volume) — and forgetting demand elasticity: too high a toll pushes traffic back to the free road.

### Drill E — Public-sector: a transport ministry cutting road-accident deaths
- **Structure (objective is social, not profit).** Frame outcome = f(exposure, behavior, infrastructure, enforcement, post-crash response). Build the tree: engineering (road/vehicle design) · education (driver behavior) · enforcement (rules, penalties) · emergency response (trauma care) — the "4 E's."
- **Quantified spine:** decompose fatalities = vehicle-km × crash rate per km × fatality rate per crash; attack the biggest multiplier (e.g., two-wheeler head injuries → helmet compliance; black-spot junctions → engineering fixes).
- **Aha:** public-sector cases optimize a **social outcome under a budget constraint**, not profit — success metrics are lives saved per rupee, adoption/compliance rates, and equity of access. Cost-benefit and stakeholder buy-in replace ROI.
- **Trap:** importing a private-sector "maximize profit" frame; ignoring implementation feasibility (enforcement capacity, political economy) that makes or breaks public programs. See `references/public-sector-government-defense.md`.

### Drill F — Profitability turnaround: a loss-making hospital chain (or thermal plant)
- **Structure:** Profit = Revenue − Cost. Revenue = beds × occupancy × ALOS-adjusted throughput × revenue/bed-day × payer mix. Cost = clinical staff + consumables + fixed (facility, equipment depreciation).
- **Quantified spine:** find the leak — is it low occupancy (demand/referrals), low realization (payer mix, discounting), or high cost (staff ratios, consumable leakage, high fixed-cost underutilization)? Benchmark occupancy and cost/bed against peers.
- **Aha:** capacity-heavy, high-fixed-cost businesses (hospitals, power plants, hotels, airlines) turn on **utilization × yield** — a few points of occupancy or realization swing the whole P&L because incremental volume is near-pure margin.
- **Trap:** cutting clinical quality/staff to hit short-term cost targets, damaging the reputation that drives referrals — the second-order effect that deepens the hole. Read `references/cost-restructuring-anatomy.md` for the disciplined cost build.

### Drill G — Profitability: food-delivery orders falling. Which discount maximises *what*?
- **Setup.** A food-delivery platform with ~1M users has a company-specific drop in orders (the industry is fine). Customers say price and deals decide which app they open. The interviewer supplies a discount curve.

  | Discount | AOV paid | Orders/user/month | Paid GMV/user |
  |---|---|---|---|
  | 0% | ₹200 | 5 | ₹1,000 |
  | 10% | ₹180 | 10 | ₹1,800 |
  | 20% | ₹160 | 15 | ₹2,400 |
  | 30% | ₹140 | 20 | ₹2,800 |
  | 40% | ₹120 | 30 | ₹3,600 |
  | 50% | ₹100 | 35 | ₹3,500 |

- **The tempting answer.** "40% maximises revenue, so pilot 40%." That optimises GMV, not profit.
- **Quantified spine.** `[ILLUSTRATIVE]` Assume the platform earns a 20% commission on the ₹200 list basket (₹40), loses ₹10 net on delivery (fee minus rider cost), and **funds the discount itself** (₹200 × d).
  - Contribution per order = 30 − 200d.
  - Per user per month, that gives: 0% → **+₹150** · 10% → +₹100 · 20% → −₹150 · 30% → −₹600 · 40% → **−₹1,500** · 50% → −₹2,450.
  - At 1M users, the "revenue-maximising" 40% burns ~₹150 cr a month.
- **Aha.** **State the objective before optimising.** Revenue-maximising and profit-maximising discounts are different numbers.
  - Also challenge the data: 30 orders per user per month is implausible for most users.
  - Better levers: target discounts only at price-sensitive or lapsed cohorts, add a free-delivery membership, and A/B test against **contribution** with a holdout that measures incrementality.
- **Trap.** Recommending the top of a revenue curve. Or diagnosing "lack of discounts" without first checking the price gap versus the competitor.

### Drill H — Profitability: food-delivery platform wants higher profit; revenue is flat, internal costs are up
- **Structure.** Revenue: commission, delivery fee, platform fee, ads. Cost: rider payouts, discounts, payment gateway, support/refunds, tech, admin. The interviewer rules out a revenue problem, macro inflation, salary hikes and marketing spikes.
- **Quantified spine: the per-order waterfall** `[ILLUSTRATIVE]`.
  - On an AOV of ₹400, revenue is ₹80 commission + ₹25 delivery fee + ₹5 platform fee + ₹10 ads = **₹120**.
  - Variable cost is ₹65 rider + ₹15 discounts + ₹8 gateway (2%) + ₹7 support/refunds = **₹95**.
  - **Contribution ≈ ₹25 per order.**
- **Aha: size the levers before choosing one.**
  - Batching 15% of orders at 30% rider savings adds ≈ ₹2.9 per order (+12% contribution).
  - A ₹5 platform-fee increase adds +20%.
  - Trimming "non-essential admin" is usually worth paise per order.
  - Rider cost per order, driven by **order density and batching**, is the biggest cost lever in delivery. Tech/cloud optimisation matters when internal fixed costs are the stated culprit.
- **Trap.** Stopping at "cut admin costs and use cheaper tech" without sizing either lever against the per-order economics.

### Drill I — Market entry: a household wind-energy device (~₹1 lakh price, ~₹700 cr investment)
- **Setup.** A US industrial-electronics maker wants to launch a household wind device in India.
  - Customer opex is ~20% of the price per year (fluids and consumables).
  - There are no government incentives today.
  - The market is nascent and fragmented.
- **Customer economics first** `[ILLUSTRATIVE]`.
  - Opex of ₹20,000/yr against a typical household bill of ₹24,000/yr leaves a net saving of ~₹4,000/yr.
  - **Payback ≈ 25 years**, so the value proposition fails before any market sizing.
- **Market sizing (the original tree, with a 10× slip fixed).**
  ```
  1.2B × 35% in consistently windy regions ÷ 4 per household = 105M households
   ├─ Can afford (3%)          = 3.15M  × 30% aware = 945k  × 10% interested = 94.5k
   └─ Could afford w/ subsidy (17%) = 17.85M × 15% aware = 2.68M × 5% interested = 134k
                                            (the original wrote 0.27M here: a 10× slip)
  Interested ≈ 94.5k (no subsidy) to 228k (with subsidy)
  × 20% buy within 5 years × 30% our share → ≈ 5.7k–13.7k units → ₹57–137 cr revenue
  Break-even at 30% contribution: ₹700 cr ÷ (₹1 lakh × 30%) ≈ 233k units → 17–40× short
  ```
- **Recommendation.** Don't enter.
  1. Customer payback is uneconomic.
  2. Most of the population lives outside viable wind zones.
  3. The case depends on incentives that don't exist.
  - Revisit if opex falls sharply or the device is sold as B2B/community-scale.
- **Trap.** Sizing the market before asking whether a buyer would ever earn the price back.

### Drill J — Market entry: an electric two-wheeler maker (successful in Asia and Europe) considering India
- **Setup.**
  - The client already makes e-buses in India, so battery supply and manufacturing can flex to two-wheelers (complete units).
  - The target is an economy model.
  - The brief claims "no current players". **Challenge that**: established two-wheeler makers and EV start-ups are active.
- **Error fixed.** The original sizing was a *stock*, and implausibly large:
  - 1.2B × 30% urban ÷ 4 = 90M households.
  - × (upper 10% × 40% + upper-middle 25% × 30% + lower-middle 25% × 10%) = **12.6M "E2W market"**.
  - As annual sales, that would be about two-thirds of *all* two-wheelers sold nationally (~18–20M/yr, *verify*).
- **Quantified spine (annual flow)** `[ILLUSTRATIVE]`.
  - 90M urban households × 50% owning a two-wheeler = 45M.
  - Replacement: 45M ÷ 8 years = 5.6M/yr, plus ~0.9M first-time buyers, gives **≈ 6.5M urban two-wheeler sales a year**.
  - × 10% EV share = **≈ 650k E2W a year**.
  - × 10% target share by year 3 = 65k units, × ₹1.1 lakh ≈ **₹720 cr revenue**.
  - Sanity: national E2W sales are on the order of ~1M+/yr (*verify*) ✓.
- **How to enter.**
  - Localise to qualify for demand incentives and avoid import duties on complete units.
  - Build the dealer and service network in the top urban clusters first.
  - Offer financing (EMI) partnerships.
  - Address charging and battery-swap access.
  - Price against petrol two-wheelers on **total cost of ownership per km**, not on sticker price.
- **Trap.** Treating the installed base as annual demand, and accepting a "first mover" premise without checking it.

### Drill K — Market entry / operations: launching ride-hailing in a new tier-2 city
- **Setup.** A fast-growing tier-2 city with decent digital adoption, weak organised transport, and only small local aggregators.
- **Structure.**
  1. **Market understanding with proxy data.** Transit use, density, smartphone penetration, commute patterns; driver supply via unions and RTO data; benchmarks from comparable tier-2 cities.
  2. **Phased launch.** Pilot in the densest 15–20% of zones (commercial and transit hubs), then expand to residential belts and add auto and bike categories.
  3. **Operating design.**
     - Zone-based incentives on 2–3 km clusters.
     - Trip chaining (assign the next ride before drop-off).
     - Heat-map repositioning.
     - Transparent fares, live ETAs and an SOS button.
  4. **Metrics.**
     - Business: revenue per driver-hour, week-1 rebooking.
     - Operations: fulfilment rate, ETA, cancellations.
     - Product: booking success, uptime, GPS accuracy.
- **Quantified spine: liquidity before breadth** `[ILLUSTRATIVE]`.
  - Pilot demand is 2,000 trips a day; 12% fall in the peak hour, so **240 trips/hr**.
  - A driver completes ~2 trips an hour, so **~120 drivers must be online at peak**.
  - With ~50% of onboarded drivers online at peak, **onboard ~240 before launch**.
  - Target ETA under 5 minutes.
- **Scenario playbook.**
  - Demand > supply: driver incentives, fast-track onboarding, mild surge.
  - Supply > demand: rider referrals, pooled rides, time-based driver guarantees.
  - Balanced: keep surge minimal to build trust.
- **Aha.** Marketplaces launch **dense, not wide**. Liquidity (short ETAs, high driver utilisation) in a few zones beats thin coverage citywide.
- **Trap.** A citywide launch with average-density math that hides empty zones.

### Drill L — Operations: the order-allocation system at a food-delivery platform is failing
- **Triage.**
  - **Scale:** regions, orders, riders.
  - **Nature:** temporary glitch or structural flaw (scaling limit, algorithm bug)?
  - **Time to fix.**
  - `[ILLUSTRATIVE]` At 1M orders a day with 10% misallocated, 100k orders are delayed; at ₹50 compensation each, that is **₹50 lakh a day**. That number sets the urgency.
- **Response in three layers.**
  1. **Interim.** A rule-based fallback allocation: nearest available rider, capped load; manual dispatch in the worst-hit zones.
  2. **Customers.** Proactive apology plus credits for affected orders. Keep the brand voice light, but don't joke while orders are still failing.
  3. **Permanent.** Root-cause the allocator with the tech team, load-test it, and add a kill-switch fallback and alerting on assignment latency.
- **Trap.** Jumping to a marketing campaign before the fallback is live.

### Drill M — Pricing: a star-led blockbuster at a 500-seat city-centre theatre in a tier-2 city (Sunday)
- **Setup.** City of 2M. The film is releasing only in theatres. The original sized the target as 50% middle/upper-class × 60% aged 18–50 = 600k people.
- **Error fixed.** 10–15% of 600k is **60–90k people**, not the 3–9k the original stated. More importantly, the original **never set a price**.
- **Quantified spine** `[ILLUSTRATIVE]`.
  - 600k × 12% watch in opening week = 72k.
  - × 8% share for our large screen = **~5,760 viewers in the week**.
  - Sunday takes 25% = 1,440 viewers across 4 shows (2,000 seats), i.e. **72% occupancy**.
  - Evening shows take 60% of Sunday demand: 864 viewers for 1,000 seats (86%). Morning shows take the other 576 for 1,000 seats (58%).
- **Price.**
  - Anchor on the local base (~₹180), then **time-differentiate**: evening ₹225 (+25%), morning ₹153 (−15%).
  - Revenue ≈ 864 × 225 + 576 × 153 = **₹2.83 lakh vs. ₹2.59 lakh at a flat price (+9%)**, before any morning volume lift.
  - Add premium seat tiers and F&B combos. Check any state caps on ticket prices.
- **Aha.** A price must come from **demand vs. capacity by time slot** plus willingness-to-pay. "Look at past data and competitors" is a method, not an answer.
- **Trap.** Ending the case without a number.

### Drill N — Operations (non-traditional): overcrowding outside a large cancer hospital, peaking 4–6 PM
- **Clarify.**
  - The crowd built gradually, then escalated within weeks.
  - It is mostly pedestrians at the reception entrance; patients arrive by car.
  - The hospital added lymphoma and melanoma care about 8 months ago, and **staff rose ~20%**.
  - Staffing is 3 shifts of 8 hours, with a **handover at 5 PM**.
  - **Staff check-in kiosks are only at reception**, and neither kiosks nor lifts were added.
- **Journey walk.** Staff exit path: workstation → stairs/lift → **kiosk queue** → parking → exit. The bottleneck is the kiosk queue.
- **Quantified spine: queueing** `[ILLUSTRATIVE]`.
  - Kiosks clear ~120 swipes a minute at the handover.
  - Before the expansion, the handover created ~100 swipes/min: **utilisation 83%**, and queues clear.
  - After +20% staff, demand is ~120/min: **utilisation ≈ 100%**. Queues grow without limit and spill into the patient path during the OPD peak.
- **Aha.** Queues are non-linear. A 20% demand increase near capacity turns "busy" into "gridlock". Look for **what changed on the supply side and what didn't**.
- **Recommendations.**
  - Add kiosks at a **separate staff entrance**.
  - Allow mobile or geofenced attendance.
  - Stagger handovers (clinical vs. administrative), and move handover off the 4–6 PM OPD peak.
  - Use dedicated staff lifts at shift change.
- **Trap.** Assuming more patients are the cause, from the new service line, without testing the staff flow.

**Method reminder:** every drill leads with structure, then puts an explicit quantified spine under it (a number, a ratio, a sensitivity), then states the "so what." That is the standard for every worked case in this skill — see `references/practice-cases-quantified.md` for the full method and `references/guesstimation.md` for the estimation techniques catalog.
