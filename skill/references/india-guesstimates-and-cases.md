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
| Telecom | 3-player: Jio, Airtel, Vo