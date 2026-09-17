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

### Guesstimate 3 — Cricket balls sold in a large metro per year
**Answer: ~1–2 million/year.** Teaches the **usage-rate + sharing + replacement** chain, plus the "add institutional demand" refinement.

**Clarify:** leather/season balls for actual play (not toy balls); one metro.
**Structure:** players → balls in use (sharing) → balls consumed per year (replacement from wear/loss) → **plus** a separate institutional bucket.

```
Metro population              = 8M              [ILLUSTRATIVE]
Cricket-playing % (age×gender skew, mostly M 8–35, casual+serious)
  ≈ 6% actively play          = 480,000 players
Sharing: a ball serves ~8 players in a group  → balls in circulation = 480k/8 = 60,000
Replacement: a used ball dies in ~1 month of regular play → ~10 balls/ball/yr
Household/club demand         = 60,000 × 10     = 600,000 balls/yr
+ Institutional layer (academies, clubs, schools, nets) — size SEPARATELY:
  ~500 academies × ~50 balls/month × 12         = 300,000 balls/yr
TOTAL                         ≈ 0.9–1M balls/yr  (round to ~1M)   [ILLUSTRATIVE]
```
**The refinement that scores:** after the demand-side household build, explicitly add an **institutional demand bucket** (academies/clubs/schools) rather than burying it in a fudge factor — interviewers reward seeing the second population.

### Guesstimate 4 — Foreign tourist arrivals at a major international airport per day (two-method reconciliation)
Teaches solving with **two independent approaches and reconciling** — a distinct skill from a single build.

```
APPROACH A — Boarding-gate / flight throughput (supply of seats)
  International gates in use     = 40                [ILLUSTRATIVE]
  Wide-body turns/gate/day       = 6                → 240 arriving intl flights/day
  Seats/flight × load (250×0.8)  = 200 pax          → 48,000 intl arrivals/day
  Foreign nationals (vs returning residents) ~40%   → 19,200 foreign tourists/day

APPROACH B — Immigration-counter throughput (operations rate)
  Foreign-passport counters      = 30
  Processing rate                = 20 pax/counter/hr
  Effective hours/day            = 18
  Capacity                       = 30 × 20 × 18      = 10,800 → real utilisation 70% ≈ 7,600/day
  (counters are the bottleneck; Approach A is the seat-supply ceiling)

RECONCILE: the two differ by ~2.5×. State why (A = arriving pax incl. transit & residents;
B = throughput-constrained foreign entries) and give a RANGE, e.g. ~8k–19k/day, leaning to
the binding constraint (counters) unless told capacity was expanded.
```
**The move that scores:** don't just average — **explain the gap** (seat-supply vs. processing-capacity) and let the binding constraint set your point estimate. Interviewers deliberately ask for a second method to watch you reconcile.

### Guesstimate 5 — Currency the machine should hold at an airport exchange kiosk (demand → capacity)
Teaches sizing a **capacity/inventory** number by segmenting users, then reserving for a market share.

```
Intl arrivals/day (from G4)          = 48,000        [ILLUSTRATIVE]
Need cash & would use a machine (30%) = 14,400 users
Segment by withdrawal size:
  low-value travellers  70% × avg $50  = 10,080 × 50  = $504,000
  high-value travellers 30% × avg $200 =  4,320 × 200 = $864,000
Total daily demand                                    = $1.37M equivalent
Our machine's share (one incumbent kiosk too → ~50%) = ~$685,000/day
+ Safety buffer for peak/denomination mix (~20%)      ≈ $820,000 to load per refill cycle
```
**Chain to remember:** traffic → % who transact → segment by ticket size → apply market share → add a buffer for peaks and denomination mix. Sizing an *inventory/capacity* number (not a market) still runs demand-side, then reserves for share and variability.

### Guesstimate 6 — Market size of (professional) neckties in a country (stock × replenishment)
Teaches the **installed-stock → replenishment-rate** method — different from the durable-good "growth + replacement" of Guesstimate 1.

```
Population                    = 1.4B             [ILLUSTRATIVE]
Tie-wearers: white-collar males in formal roles
  working pop 40% = 560M; male 65% = 364M; formal-attire roles 10% = 36M wearers
Ties owned per wearer         = 5
Installed stock               = 36M × 5          = 180M ties
Replacement cycle             = every 5 yrs      → sales/yr = 180M / 5 = 36M ties/yr
Avg price                     = ₹1,000           → market ≈ ₹3,600 Cr/yr   [ILLUSTRATIVE]
```
**When to use stock×replenishment vs. growth+replacement:** if the population is roughly saturated (everyone who'll own the item already does), size the **stock** and divide by the replacement cycle. If penetration is still climbing, add a growth term (see Guesstimate 1).

### Abstract / logic drill — the two-glasses mixing puzzle
Some firms (esp. in later rounds) test pure reasoning, not sizing. Example: *two equally-filled glasses, one red wine, one white; move a spoon of red into the white and mix, then move a spoon of the mixture back.* Is there more red in the white glass, or more white in the red?

- **Answer:** exactly **equal** — each glass returns to its original volume, so whatever red is "missing" from the red glass has been replaced by an identical volume of white. Conservation of volume forces symmetry; you don't need the concentrations.
- **How to handle these:** set a concrete unit (e.g., 10 spoons/glass), define constraints explicitly (equal sizes, done once), reason from an invariant (here: each glass ends at its starting volume) rather than tracking messy concentrations. When asked to relax constraints (e.g., glasses less than half full so one can be fully poured into the other), re-derive the extreme (→ 50/50 mix). The scored behaviour is **naming the invariant**, not brute-forcing the arithmetic.

### Guesstimate 7 — Burgers a fast-food outlet sells per day (SUPPLY-side capacity method)
Most sizing is demand-side; this one teaches the **supply/capacity** lens — bound the answer by how many customers the outlet can physically serve.

```
Scope: average outlet (not airport/mall); include dine-in + takeaway.
DINE-IN (capacity-bound):
  Seats               = 50            [ILLUSTRATIVE]
  Seat turns/hr (peak)= 2  ;  operating hrs = 12  ; avg occupancy across day = 50%
  Customers/day       = 50 × 2 × 12 × 0.5           = 600
  Burgers/customer    = 1.5                          → 900 dine-in burgers/day
TAKEAWAY (add as a separate stream, ~40% of dine-in) → +360
TOTAL                 ≈ 1,250 burgers/day
```
**When to go supply-side:** when a **physical capacity ceiling** (seats, counters, machines, runway slots) is easier to estimate and more binding than diffuse demand. Bound by capacity × utilisation, then add adjacent streams (takeaway) separately.

### Guesstimate 8 — Domestic fleet size of an airline (NETWORK / route method)
Teaches building from **network structure** (routes × frequency × aircraft-per-route) instead of population — the right lens for infrastructure/logistics assets.

```
Cities: 6 metros + 30 tier-2                                     [ILLUSTRATIVE]
Route types:
  metro–metro        = C(6,2) = 15 routes
  metro–tier2        = 6 metros × 5 orbital tier-2 each = 30 routes
  tier2–tier2        ≈ negligible (routed via metros)
Total routes         ≈ 45
Frequency            = ~4 flights/route/day (metro–metro higher, spokes lower) → weight to ~3 avg
Daily flights        = 45 × 3            = 135 one-way ≈ 68 round-trip sorties
Aircraft/sortie incl. turnaround & maintenance spare (~1 aircraft serves ~3 sorties/day)
Fleet                = 135 / 3           ≈ 45 aircraft (+ ~15% maintenance reserve) ≈ 50
```
**Reusable pattern:** for networked assets, `fleet = (routes × frequency) / sorties-per-asset-per-day`, then add a maintenance reserve. The hub-and-spoke "orbital city" simplification keeps route-counting tractable.

### Guesstimate 9 — Number of schools in a metro (RATIO / divide method)
The simplest and most robust method when a clean per-unit ratio exists: **size the population served, divide by throughput per unit.**

```
#Schools = (school-age children enrolled) / (avg students per school)
Metro population           = 20M                                 [ILLUSTRATIVE]
Under-25 share (~50%)      = 10M → ~400k per single-year cohort
School ages 4–18 (15 cohorts) enrolled, weighted by income/enrolment %
  ≈ 15 cohorts × 400k × ~70% enrolled = ~4.2M students
Avg students/school        = 1,000
#Schools                   = 4.2M / 1,000 = ~4,200 schools
```
**Reusable pattern:** `#facilities = population served ÷ throughput per facility`. Works for hospitals (beds), bank branches (customers), cell towers (subscribers), ATMs — pick the ratio that's easiest to defend.

### Choosing your sizing method (quick decision box)
| If… | Use | Example |
|---|---|---|
| A clean per-unit ratio exists | **Ratio / divide** (`served ÷ per-unit`) | schools, hospitals, branches (G9) |
| A physical capacity ceiling binds | **Supply-side** (`capacity × utilisation`) | fast-food, kiosks, runway/counters (G7, G4-A) |
| The asset is a network | **Route method** (`routes × freq ÷ per-asset`) | fleets, trucks, cell coverage (G8) |
| It's a durable good, penetration rising | **Growth + replacement** (`stock×g + stock/life`) | routers, ACs, TVs (G1, and G6-note) |
| The base is saturated | **Stock × replenishment** (`stock ÷ cycle`) | ties, mattresses, furniture (G6) |
| Two methods are feasible | **Do both, reconcile** the gap by the binding constraint | tourist arrivals (G4) |

**Universal discipline:** state assumptions aloud; pick **one** primary method (don't blend demand- and supply-side mid-stream); round to clean numbers; **sanity-check the order of magnitude** against a known anchor before presenting; add adjustment factors (edge users, institutional demand) as *explicit separate buckets*, not fudge.

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
