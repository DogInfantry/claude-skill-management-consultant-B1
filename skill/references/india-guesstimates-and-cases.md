# India Guesstimates, Benchmarks & Case Drills

Companion to `references/guesstimates-and-frameworks-quantified.md` and `references/case-bank-worked.md`, tuned to the **Indian market**: worked guesstimates drawn as segment trees, a benchmark-numbers cheat sheet, compact sector snapshots, and case drills A–S (profitability, market entry, pricing, growth, operations and public sector). Every figure here is an **approximate, directional benchmark** for structuring — label anything you compute on top as `[ILLUSTRATIVE]` and sanity-check the arithmetic before presenting.

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
| Land area & density | India ~3.3M km² · ~430–460 people/km² | Recompute density from the population you chose (1.4 Bn ÷ 3.29M km² ≈ 426; 1.5 Bn ÷ 3.3M ≈ 455). Rounding up to ~500/km² overstates it by ~10–17% |
| City areas (municipal, approx.) `[ILLUSTRATIVE]` | Delhi (capital territory) ~1,500 km² · Bengaluru ~700–740 · Mumbai ~600 · Lucknow ~600–630 · Chennai ~425 · Kolkata ~200 | Pair a municipal area with a city-proper population: Mumbai ~12M ÷ 600 ≈ 20,000/km²; Kolkata ~4.5M ÷ 200 ≈ 22,500/km². A metro-region population over a municipal area (14M ÷ 200 = 70,000/km²) is a base mismatch |
| Land-use split (share of geographic area) `[ILLUSTRATIVE]` | ~90% land / ~10% water · within land: cropland (net sown) ~43% and forest ~22% of geographic area; the rest is built-up, pasture and barren | Forest and cropland are *subsets* of land. Never add "land 70% + water 10% + forest 20%" as if the three were exclusive |
| Population growth | ~0.8–0.9% a year | Older sets use ~1.25%; over a 5-year projection that overstates population by ~2 points |
| Life expectancy | ~70–72 years | Use for lifetime and replacement logic (insurance, pensions, lifetime value) |
| Sex ratio | ~52 : 48 male : female | Female-only segments are ~48% of the population, not 50% |
| Internet users `[ILLUSTRATIVE]` | ~55–65% of the population (~0.8–0.9 Bn) | Urban penetration sits well above rural. A blended rate must lie between the two: urban 55% and rural 45% at a 40:60 mix blend to 49%, not 40% |
| Mobile connections `[ILLUSTRATIVE]` | ~1.15 Bn wireless subscriptions (~80–85% teledensity; >90% prepaid) · urban ~130% · rural ~58% | Subscriptions ≠ people: dual SIMs push urban teledensity above 100% (490M × 1.3 + 910M × 0.58 ≈ 1.16 Bn). Unique mobile users are fewer |
| 5G adoption `[ILLUSTRATIVE]` | ~25–35% of mobile connections, rising fast | Verify before use. Apply it only to users with a 5G-capable handset |

**Income-segmentation move** (the most reused pattern): split any population into 10/40/50 high/middle/low, then apply a different ownership or consumption rate to each tier. It appears in almost every ownership guesstimate below.

**Pick one set and state it.** Two benchmark sets are in common use, and they disagree:

| Anchor | Set A (this file's default) | Set B (common alternative) |
|---|---|---|
| Population | ~1.4 Bn | ~1.5 Bn |
| Urban share | ~35% | ~40% |
| Persons per household | urban ~4.0, rural ~5.2 (~4.6 blended) | 5 flat |
| Households | ~300M | ~300M |
| Median age | ~28 | ~25 |
| Smartphone users | ~700–750M | ~1 Bn (quoted as ~71% "penetration") |
| Population growth | ~0.8–0.9% | ~1.25% |
| Income split | 10 / 40 / 50 high / middle / low | 1 / 15 / 30 / 25 / 29 high / upper-middle / lower-middle / low / below poverty line |

- **The rule.** At the start of an interview or engagement, say which set you are using ("I'll use 1.4 Bn, 35% urban and ~300M households"). Then apply it to every estimate in the session. If the interviewer supplies a number, adopt it everywhere, not just in the current branch.
- **Why it matters.** Mixing sets silently moves answers by ~7% (population) to ~40% (smartphone users), and two estimates in the same deck stop reconciling.
- **Where the choice bites.** Both sets land at ~300M households (1.4 Bn ÷ 4.6 ≈ 1.5 Bn ÷ 5), so household trees barely move. Per-capita, age and penetration branches move most.
- **Which is fresher.** Set A is closer to recent estimates of population (~1.45 Bn; 1.4 is the round working number), median age and growth. Set B's 29% below-poverty-line share reflects an old poverty line; recent estimates are far lower (*verify*).
- **Error fixed:** an age split of 30 / 20 / 15 / 10 / 10 / 10 → it sums to 95%, so rescale it or place the missing 5 points before use (every segment tree must close to 100%, or the total is understated by the gap).

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

## Worked guesstimate 7 — a venue-event consumption (cold drinks inside stadiums over a T20 season)

*Prompt: estimate cold-drink consumption inside stadiums across one franchise T20 league season.* `[ILLUSTRATIVE]`

**Clarify scope first:** drinks sold inside the venues only (not home viewers or bars), and all beverage sizes converted to litres.

```
  Season ~74 matches → 18 afternoon + 56 evening      Avg venue CAPACITY ~50,000
        ┌───────────────────────┴───────────────────────┐
  Afternoon: 65% occupancy                        Evening: 85% occupancy
  Attendance 0.65 × 18 × 50k = 585k               Attendance 0.85 × 56 × 50k = 2.38M
  × 80% buy a drink → 468k buyers                 × 80% buy a drink → 1.90M buyers
  × 0.5 L (heat) → 234k L                         × 0.3 L → 571k L
        └───────────────────────┬───────────────────────┘
             ≈ 805k litres ≈ 8 lakh litres per season
  Sanity: attendance 2.97M ÷ 74 ≈ 40k per match — in line with typical crowds ✓
```

**Coaching notes:**
- **The pattern:** events × capacity × occupancy × purchase rate × volume per buyer, **split by time slot**. The heat of an afternoon game raises litres per buyer, but the evening games carry ~70% of the volume because they are more numerous and fuller.
- **Supply check:** an evening game has 0.85 × 50k × 80% ≈ 34,000 buyers. If half of them buy in a 20-minute innings break, that is ~850 drinks a minute. Counter and vendor throughput, not thirst, caps real volume. This is the check that impresses.
- **Error fixed:** calling the 2.37M figure "total people attending" → it is drink **buyers** (the 80% filter is already applied). Attendance is ~2.97M. Also, "65% / 85%" are occupancy rates, not shares of matches; label them so the tree reads correctly.
- **Trap:** one average capacity hides a venue mix of roughly 30k to 100k+. If the interviewer pushes, weight by venue.

## Worked guesstimate 8 — a validity-period flow (visas approved per day at one consular post)

*Prompt: estimate the visitor-and-student visas that one foreign country's consular post in an eastern Indian metro approves per day.* `[ILLUSTRATIVE]`

```
  STOCK → FLOW via validity period
  1.4 Bn × 10% high-income × 1.25% travel to that country in a decade
        = ~1.75M people who hold or need its visa
  Visitor visas valid ~7 yrs → 1.75M ÷ 7 ≈ 250k applications/yr
        (stock ÷ validity already includes steady-state renewals)
  + Students & temporary workers (1–3 yr validity; own branch) ≈ 150k/yr
  = 400k first-pass applications
  + Refused applicants reapplying: 400k × 30% refused × 50% reapply ≈ 60k
  = ~460k applications/yr nationally
        │ × this post's share ~10% (range 8–12%)
  ~46k/yr ÷ 250 working days ≈ 184 interviews/day
        │ × ~70% approval
  ≈ 130 approvals/day   (range ~100–155 across the 8–12% post share)
```

**Coaching notes:**
- **The pattern:** for any renewable permit (visas, licences, passports, insurance policies), **annual flow = eligible stock ÷ validity period**, plus the categories whose validity is shorter.
- **Capacity cross-check:** assume ~6 interview windows × 6 hours × ~6 interviews an hour ≈ 216 slots a day. Demand of ~184 fills ~85% of that. If appointment waits run to months, capacity is the binding number and approvals ≈ 216 × 70% ≈ 150 a day, whatever the demand tree says.
- **Top-down anchor:** if the country publishes national issuance, national issuance × post share ÷ 250 is a second estimate. Reconcile the two before answering (*verify*: a large issuer's national figure can put this post several times higher).
- **Error fixed:** doubling "stock ÷ validity" to add renewals → stock ÷ validity *is* the steady-state renewal flow, so doubling double-counts it. Add only refused reapplicants and short-validity categories, each as its own branch. A related slip is an undefined "1.5 Bn × 4% × 3%" filter: name each filter (income-eligible × propensity to travel) so the interviewer can challenge it.
- **Trap:** applying the approval rate to renewals that skip the interview. If the post waives interviews for renewals, count them separately.

## Worked guesstimate 9 — a subscription market with an ARPU cross-check (prepaid mobile recharge)

*Prompt: estimate India's annual prepaid mobile recharge market.* `[ILLUSTRATIVE]`

```
  METHOD 1 — household tree (Set A: urban ~120M HH at 4.0, rural ~175M HH at 5.2)
  Segment (HH)            Active SIMs/HH   ₹/SIM/month   SIMs     ₹ Cr/month
  Urban upper   20% = 24M        7            280        168M       4,704
  Urban middle  40% = 48M        5.5          200        264M       5,280
  Urban lower   40% = 48M        4            160        192M       3,072
  Rural upper   10% = 17.5M      5            200        87.5M      1,750
  Rural middle  40% = 70M        3.5          160        245M       3,920
  Rural lower   50% = 87.5M      2            130        175M       2,275
                                                  ≈ 1.13 Bn SIMs  ≈ 21,000
  × 12 ≈ ₹2.52 lakh Cr (all SIMs) × ~90% prepaid ≈ ₹2.27 lakh Cr/yr
  Implied ARPU = ₹21,000 Cr ÷ 1.13 Bn ≈ ₹186/SIM/month

  METHOD 2 — subscribers × ARPU
  ~1.15 Bn wireless subscriptions × ~92% prepaid ≈ 1.06 Bn
  × ~₹180/month × 12 ≈ ₹2.29 lakh Cr/yr

  RECONCILE: ≈ ₹2.3 lakh Cr a year ✓
```

**Coaching notes:**
- **The pattern:** any subscription tree (telecom, OTT, broadband, insurance) must pass two checks. First, the **implied subscriber base** against the known one. Second, the **implied ARPU** against the reported one. The two segment splits here also imply a national mix of ~14 / 40 / 46 (high / middle / low), close to the 10 / 40 / 50 benchmark.
- **SIMs, not people:** dual SIMs put urban teledensity above 100%, so count active SIMs per household, not phones per person.
- **Error fixed:** a tree with 1 phone per low-income urban household, 0.5 per low-income rural household and ₹50–200 recharges → implies only ~455M connections at ~₹106 a month, and a market of ~₹57,700 Cr. That is ~2.5× too few connections against ~1.15 Bn subscriptions and ~4× too small overall, because it ignores dual SIMs and recent tariff rises (*verify* current ARPU). A related slip is writing "₹5,76,900 Mn", which mixes lakh-style grouping with millions: write ₹577 Bn or ₹57,690 Cr.
- **Trap:** stale per-unit prices. Tariffs move in steps, so re-anchor ARPU before sizing.

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
- **Split patient revenue before diagnosing.**
  - Surgical = surgeries × realisation per surgery (the package price, not its cost).
  - Medical (non-surgical inpatient) = beds × occupancy × days × ARPOB (average revenue per occupied bed-day). Average length of stay (ALOS) drives throughput inside occupancy; it is not a parallel branch.
  - Ancillary = pharmacy, diagnostics, food. Non-patient revenue (research, teaching) is usually small.
- **Worked leak: one of four hospitals, costs on plan, revenue falling after complaints about post-operative care** `[ILLUSTRATIVE]`.
  - Baseline per month: 300 surgeries × ₹2 lakh = ₹6.0 cr; 120 medical beds × 80% × 30 days = 2,880 bed-days × ₹25,000 = ₹7.2 cr; ancillary ₹2.0 cr. **Total ₹15.2 cr.**
  - Negative reviews spread by word of mouth. Surgeries fall 20% (−60 = −₹1.2 cr). Referrals then dry up, so medical occupancy drops 8 points (−288 bed-days = −₹0.72 cr). Ancillary falls 10% (−₹0.2 cr).
  - **Loss ≈ ₹2.12 cr a month (~14% of revenue).** With ~25% of revenue variable (consumables, implants), ~₹1.6 cr falls through. That is ~70% of a 15% EBITDA (₹2.28 cr → ~₹0.7 cr).
- **Test the rival causes before accepting "bad reviews".** Each has its own fingerprint:
  - Senior surgeons leaving → the drop is concentrated in one specialty.
  - Lost empanelment with an insurer or government scheme → the drop is concentrated in one payer.
  - A new competitor nearby → the drop is concentrated in one catchment.
  - Post-op quality → review trend, surgical-site infection and 30-day readmission rates worsen across specialties.
- **Fix in order:** clinical first (post-op nursing ratios, infection control, discharge follow-up calls, outcome audits), then publish outcomes, then market the improvement. Marketing a hospital that has not yet fixed the problem accelerates the word of mouth.
- **Error fixed:** writing "surgeries × cost per surgery" in a revenue tree → surgeries × realisation per surgery (cost belongs on the other side of the P&L). Listing occupancy and length of stay as parallel revenue branches double-counts, because occupancy already embeds length of stay.
- **Aha:** capacity-heavy, high-fixed-cost businesses (hospitals, power plants, hotels, airlines) turn on **utilization × yield** — a few points of occupancy or realization swing the whole P&L because incremental volume is near-pure margin. In healthcare, a quality failure in one service (post-op care) spreads by word of mouth into **both** surgical volume and bed occupancy, so the revenue loss is larger than the service line that failed.
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

### Drill O — Profitability: a grocery chain losing share to quick commerce
- **Setup.** A 500-store grocery chain (urban and semi-urban, strongest in two regions, ~70% middle-income shoppers) has seen its share fall from 30% to 22% in two years.
  - National chains compete on price and online ordering. Regional players compete on local assortment. Quick-commerce apps have entered.
  - The client is store-only.
- **Define the market first.** 30% of *all* grocery is implausible for one chain, because organised retail is a small slice of Indian grocery. The base must be something like "modern-trade grocery in its regions". Every share figure depends on that definition.
- **Turn share points into rupees** `[ILLUSTRATIVE]`.
  - Losing 8 points from 30 is a **26.7% relative** loss of share.
  - Client revenue = (22 ÷ 30) × (1 + market growth). Revenue is flat only if the market grew 36.4% over two years (~17% a year).
  - If the market grew 20% over the two years, revenue is 0.733 × 1.20 = 0.88, i.e. **−12%**.
  - With a 22% gross margin and store costs (rent, staff) fixed at 16% of the old revenue, EBITDA falls from 6% to 0.22 × 0.88 − 0.16 = 3.4% of old revenue: **−44% on a −12% revenue drop.** Operating leverage turns a share problem into a profit problem.
- **Diagnose by shopping mission, against the winners.**
  - Split revenue per store into footfall × conversion × basket, separately for top-up trips (milk, bread, fruit, snacks) and monthly stock-up trips.
  - Quick commerce usually takes the high-frequency, small-basket top-up trips, so footfall falls faster than revenue.
  - Compare the client with the chains that *gained* share, for the same customer: price gap, assortment, delivery promise, app experience.
- **Recommendations.**
  - Get online fast and capital-light: list on delivery platforms first, then run ship-from-store in the densest catchments.
  - Defend the stock-up mission, where stores win on range and price: private label for margin, loyalty for data and repeat visits.
  - Only then consider dark stores, and only where order density justifies them.
- **Aha.** Industry forces act on every player equally. They cannot explain why *this* chain lost share while rivals gained it. Ask what the winners do differently for the same shopper.
- **Error fixed:** "we lost 8 points, so sales fell 8%" → the chain lost 26.7% of its share, and the revenue effect depends on market growth (flat only at +36% market growth). Share points are not percent of sales.
- **Trap.** Running Porter's Five Forces on a company-specific share loss, and never converting share points into revenue and profit.

### Drill P — Market entry: a home-services marketplace in tier-3 towns
- **Setup.** A home-services platform (repairs, installation, cleaning) that works in metros asks whether its aggregator model can work in tier-3 towns, and how to enter.
- **Structure.**
  - **Demand:** how often households need each service, willingness to pay for convenience, smartphone use. Today they hire through word of mouth and local contacts.
  - **Supply:** enough skilled providers, but fragmented, with low digital literacy and resistance to commissions.
  - **Model:** commission, customer subscription, provider-paid lead subscription, or employed/franchised branded technicians. Costs are acquisition, onboarding, quality control and support.
- **Quantified spine: contribution against acquisition cost, with leakage** `[ILLUSTRATIVE]`.
  - Order value ₹400 × 20% take = ₹80, less ~₹20 for payments and support = **₹60 contribution per order**.
  - Customer acquisition cost (CAC) ₹300 → **5 on-platform orders to pay back**.
  - A household needs ~4 jobs a year, so ~8 over two years. After the first job, the customer can simply phone the technician. Call the share of repeat jobs that stay on the platform *r*.
  - At r = 30%: 1 + 7 × 0.3 = 3.1 orders = ₹186 in two years. **CAC is never recovered.**
  - At r = 80%: 1 + 7 × 0.8 = 6.6 orders = ₹396, **1.3× CAC**.
  - Leakage, not the take rate, decides feasibility.
- **Make staying on the platform worth it for both sides.**
  - Customers: a service warranty and payment protection that apply only to platform bookings; verified, rated technicians; booking by phone and chat apps as well as the app.
  - Technicians: steady lead flow, accident insurance, tool finance and faster payouts. Consider a flat monthly lead fee instead of a commission, which removes the incentive to take jobs off the platform.
- **Where to start.** Appliance repair and installation (air conditioners, water purifiers) is the frequent need, and it is seasonal. Paid cleaning is weak where domestic help is cheap. Expand cluster by cluster so each town has dense supply before the next one opens.
- **Aha.** In small towns trust sits with the individual technician, not the brand. A marketplace survives only if both sides keep transacting through it after the first job.
- **Error fixed:** payback = CAC ÷ contribution = 5 orders, assuming every repeat job stays on the platform → with leakage, a customer must generate 1 + 4 ÷ r jobs to yield 5 platform orders. At r = 30% that is ~14 jobs, or ~3.6 years of demand.
- **Trap.** Copying the metro model, and never computing contribution per order against CAC and repeat rate.

### Drill Q — Public sector: girls' school dropout in a state (cohort flow)
- **Setup.** A state government wants to cut girls' school dropout. Dropout is higher in rural areas and among poorer, more conservative households.
- **Structure: follow one cohort, then segment.**
  - Track 100 girls who enter Grade 1 through Grade 10, grade by grade.
  - Split each transition by rural/urban × income × district.
  - Organise causes by barrier, so each appears once: **access** (distance, transport, safety), **cost** (fees, uniforms, books, and the opportunity cost of chores or wages), **value** (teaching quality, female teachers, relevance), **norms** (early marriage, son preference), **facilities** (toilets, menstrual hygiene).
- **Quantified spine: the cohort flow** `[ILLUSTRATIVE]`.
  ```
  100 enter Grade 1
   │ Grades 1→5 at 98% a year        → 92.2 reach Grade 5   (lost 7.8)
   │ Grade 5→6 at 85% (new, more distant upper-primary school)
   │                                 → 78.4 reach Grade 6   (lost 13.8)
   │ Grades 6→9 at 97% a year        → 71.5 reach Grade 9   (lost 6.9)
   │ Grade 9→10 at 85% (secondary school, puberty, marriage pressure)
   │                                 → 60.8 reach Grade 10  (lost 10.7)
   Two transitions carry 24.5 of 39.2 girls lost (~62%)
  ```
- **Cost per additional girl retained** `[ILLUSTRATIVE]`, per 1,000 eligible girls. Divide spend by the girls *who would otherwise have left*, not by all recipients.

  | Intervention | Cost | Lift | Extra girls retained | Cost per extra girl |
  |---|---|---|---|---|
  | Bicycles at Grade 9 entry (₹4,000 each) | ₹40 lakh | 9→10 transition 85% → 90% | 50 | ₹80,000 |
  | Cash transfer of ₹5,000 at Grade 9 entry, conditional on attendance | ₹50 lakh | +4 points | 40 | ₹1.25 lakh |
  | Girls' toilets in 5 schools (₹2 lakh each, ₹20,000 a year upkeep, 10-year life) | ₹20 lakh over 10 years | +2 points a year | ~200 over 10 years | ~₹10,000 |

  - Most of the cash transfer is deadweight: 850 of the 1,000 girls (₹42.5 lakh) would have stayed anyway.
  - Capital works that serve many cohorts are often the cheapest per girl, but only where the facility is actually missing.
- **Recommendations, tied to the two transitions.**
  - Put upper-primary and secondary places, transport and safety measures into the rural blocks with the worst 5→6 and 9→10 rates.
  - Fix toilets and hire female teachers where they are missing.
  - Target cash support at the transition years.
  - Enforce against child marriage and work with village councils.
  - Review existing schemes before adding new ones.
- **Metrics.** Transition rates at 5→6 and 9→10 by block, gross and net enrolment ratios, attendance of girls after puberty, learning outcomes, and child-marriage incidence. Link inputs to outcomes with a logic model (see `references/public-sector-government-defense.md`).
- **Aha.** Dropout concentrates at transition points. That is when a girl must reach a new, often distant school, just as the household's opportunity cost of keeping her in school jumps. Target the transitions, not the whole system evenly.
- **Error fixed:** averaging the loss (39 of 100 over nine transitions ≈ 4 a year) → ~62% of the loss sits at two transitions. A flat average spreads the budget evenly and misses the peaks. A related slip is listing safety and distance under both "social" and "infrastructure", which breaks MECE.
- **Trap.** Listing generic causes without segmenting where and when dropout happens, and ending with no metric or cost per outcome.

### Drill R — Growth: a dining-out and events platform in tier-2 cities (incentive math)
- **Setup.** A dining-out and events booking app has stalled at 200k monthly active users (MAU) with 20% repeat use in tier-2 cities.
  - 60% of people who download it never book.
  - Users say the venue list is limited and not trendy.
  - Competitors offer cashback and exclusive events.
  - Target: 500k MAU in six months (+240k from new users, +60k from better activation and retention) and repeat use from 20% to 40%.
- **Diagnose the funnel before buying users.** Use funnel data, app-store reviews and a competitor venue audit. The binding problems are **activation and supply relevance**. Paid acquisition before fixing them pours users into a leaky funnel.
- **Quantified spine** `[ILLUSTRATIVE]`.
  - **MAU bridge.** 240k *active* new users ÷ (40% activation × 45% month-2 retention) ≈ **1.33M installs**. At ~₹40 per install that is ~₹5.3 cr, before any incentive.
  - **Incentive budget.** A capped ₹20 lakh pilot. Cashback is 10% on a user's first two bookings, half co-funded by restaurants, so the platform pays 5%. That funds ₹20 lakh ÷ 5% = ₹4 cr of bookings, ~26.7k bookings at a ₹1,500 bill.
  - **Contribution.** An 8% commission on ₹1,500 = ₹120 per booking; after the ₹75 of cashback, ₹45 is left. On a commission-free trial venue, the same booking loses ₹75.
  - **Referral.** A ₹200 + ₹200 two-sided referral costs ₹400 per referred booking, so the pilot funds only 5,000 of them. Treat repeat rate *p* as the chance a booker books again. Lifetime value = ₹120 ÷ (1 − p) = ₹150 at 20% repeat and ₹200 at 40%, only **0.4–0.5× the ₹400 cost**. Meeting an LTV:CAC ≥ 3 guardrail needs acquisition cost ≤ ~₹67 at 40% repeat, or 90% repeat at ₹400.
- **Plan.**
  - Month 1: a "trending in your city" section and onboarding by city and taste, showing 5–10 personalised venues.
  - Month 2: sign ~50 trendy venues per city on a time-limited, costed trial.
  - Month 3: a tapered loyalty programme (points instead of cash after the first bookings) and two exclusive events per city.
  - A/B test cashback against points on contribution per booking. Track cost per install, booking conversion and repeat rate.
- **Aha.** Incentives must be sized from contribution per booking and the LTV:CAC guardrail, not by matching competitors. Taper them, co-fund them and cap them.
- **Error fixed:** treating "+240k new users" as +240k MAU → with 60% never booking and weak retention, it takes ~1.3M installs. A related slip is setting repeat use at 40% in the objective and 30% in the success criterion: pick one target.
- **Trap.** Setting MAU targets the funnel cannot deliver, and buying growth with subsidies before the unit economics work.

### Drill S — Market entry: an Indian two-wheeler maker entering a West African market (rider earnings and TCO)
- **Setup.** An Indian two-wheeler maker is entering a West African market where low-cost imported brands win on price, which the client cannot match. The goal is a profitable, lasting position.
  - Most bikes are used commercially, as motorcycle taxis.
  - **Check the premise:** established brands, including other Indian makers, may already hold a large share of the commercial segment (*verify*).
- **Structure.** The buyer is a rider earning a living, so the product is the rider's **daily profit**.
  - Rider profit = working days × (hours × trips per hour × fare − fuel − maintenance) − financing cost.
  - Trips per day is hours × trips per hour, so do not list "trips per day" and "hours in use" as separate levers.
- **Quantified spine: total cost of ownership (TCO) in US$** `[ILLUSTRATIVE]`.
  - Revenue: 10 hours × 2.5 trips an hour × $0.80 = **$20 a day**. The rider covers 120 km a day, with fuel at $0.90 a litre.

  | | Rival bike | Our bike |
  |---|---|---|
  | Fuel efficiency | 40 km/L → $2.70 a day | 45 km/L (+12.5%) → $2.40 a day |
  | Maintenance | $1.20 a day | $0.80 a day |
  | Net per working day | $16.10 | $16.80 |
  | Working days a month (26 less breakdowns) | 22 | 24 |
  | **Monthly profit** | **$354** | **$403** |

  - The advantage is **~$49 a month**. A $200 price premium pays back in ~4 months, and over a 3-year life the advantage is ~$1,760, ~9× the premium.
  - Riders buy on credit. Financing the $200 premium over 18 months at 30% a year adds ~$14 a month, so the rider is **~$35 a month better off from the first month**. Sell that number, not the sticker price.
- **How to win.**
  - Financing first: hire-purchase through microfinance lenders and fleet owners, repaid daily or weekly.
  - After-sales service next: spare-parts availability and quick-repair points on taxi routes, because uptime is the product.
  - Durability and passenger comfort, pay-per-use insurance, and local assembly to hedge currency swings that inflate imported prices.
- **Test the risks.**
  - Several large cities in the region restrict or ban commercial motorcycle taxis in parts of town (*verify*). Map where taxis are legal, and diversify into delivery and logistics fleets.
  - Currency devaluation hits affordability and the cost of imported parts.
- **Aha.** When the buyer uses the product to earn a living, differentiate on uptime, fuel cost and financing. A higher price can still be the cheaper bike.
- **Error fixed:** proposing "ride pooling" as an earnings lever → a motorcycle carries one pillion passenger, so pooling is physically and often legally limited. Grow earnings through uptime and trips per hour instead.
- **Trap.** Competing on sticker price, and ignoring city-level bans on bike taxis. For currency, regulatory and distribution context, see `references/emerging-markets.md`.

**Method reminder:** every drill leads with structure, then puts an explicit quantified spine under it (a number, a ratio, a sensitivity), then states the "so what." That is the standard for every worked case in this skill — see `references/practice-cases-quantified.md` for the full method and `references/guesstimation.md` for the estimation techniques catalog.
