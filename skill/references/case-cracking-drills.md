# Case-Cracking Drills — Math, Exhibits & Structuring

The five reflexes that separate a clean case from a shaky one: **fast accurate math** (Part A), **reading an exhibit for the "so what" in seconds** (Part B), **structuring a novel prompt cold** (Part C), **catching a flawed number before it reaches the answer** (Part D), and **decomposing and reconciling a change** (Part E). This file is a drill ground for all five, in native, reusable form. Use it to *build reflexes* — not to memorise answers.

Pairs with: `guesstimation.md` and `guesstimates-and-frameworks-quantified.md` (market sizing), `quantitative-toolkit.md` (unit economics, price waterfall), `data-visualization.md` (building charts — the inverse skill), `case-bank-interview-classics.md` (full cases to apply these on), `case-facilitation-and-scoring.md` (how these are scored).

Parts D–E also pair with `guesstimate-drill-bank.md` (estimation error checklist), `synergy-modeling-validation.md` (turning revenue synergies into profit) and `india-sector-primers.md` (defining and dating market-size figures).

All numbers **[ILLUSTRATIVE]**.

---

## Part A — Case Math Drills

### The five habits that win the quant
1. **Structure before you compute.** Say the equation out loud first ("Profit = (price − unit cost) × volume, so I need three numbers…"). A clear approach with an arithmetic slip beats silent correct math — and usually the interviewer helps.
2. **Ask to round.** Confirm you can round, then do; rounding gets you an 80/20 answer fast. `223M × 21 ≈ 220M × 20 = 4,400M`.
3. **Accuracy over speed.** Written long division you trust beats mental math you don't. A wrong confident number costs more than ten extra seconds.
4. **Recover with poise.** Almost everyone slips once. Catch it, fix it calmly, move on — composure under a math error is itself being tested.
5. **Always end on the "so what."** A number is not an answer. "$40M of incremental profit — about 8% of today's total, enough to clear the hurdle" is the answer.

### Number-sense toolkit
- **Rounding + adjust.** Round to convenient figures, compute, then nudge. `1,030,850 / 33M ≈ 1/33 ≈ 3%`.
- **Distributive property.** Break a hard product into easy ones. `23 × 51 = (20×50) + (3×50) + 23 = 1,000 + 150 + 23 = 1,173`. And `3,756 / 33 = (3,300/33) + (456/33) = 100 + ~14 ≈ 114`.
- **Scientific notation** (kills zero-counting errors). `2,000 × 300 = (2×10³)(3×10²) = 6×10⁵ = 600,000`; `100,000,000 / 5,000 = (10×10⁷)/(5×10³) = 2×10⁴ = 20,000`.
- **Rule of 72** (doubling). Years to double ≈ 72 ÷ growth%. At 12% → 6 years; to double in 5 years needs 72/5 ≈ 14.4%.
- **Percentages via anchors.** 10% and 1% first, then combine. `17% of 450 = 45 + 45 − 4.5×... ` → easier: `10%=45, 5%=22.5, 2%=9 → 76.5`.
- **Growth over N years.** For small rates, ≈ `rate × N` as a first pass (5%/yr for 4y ≈ ~21% cumulative vs. exact 21.6%); flag that you've linear-approximated and can compound if it matters.
- **Fractions ↔ percentages** on sight: 1/3≈33%, 1/6≈17%, 1/8=12.5%, 1/7≈14%, 3/8≈37.5%.
- **Weighted average / blended margin.** `blended = w₁m₁ + w₂m₂`. Mix shifts move the blend even when each part is unchanged — a top trap.

### Drill set (structure the approach, then compute)
1. **Break-even.** Fixed cost $12M [ILL]; contribution/unit $30 on a $50 price. Units to break even? → `12,000,000 / 30 = 400,000 units`. So-what: at 500k current volume we clear it with ~20% headroom.
2. **Payback.** Build cost $90M [ILL]; annual free cash $12M. Simple payback? → `90/12 = 7.5 years`. So-what: fails a 5-year concession.
3. **Market size sanity.** Population 330M [ILL]; 40% are buyers; buy 2/yr at $6. Market? → `330M×0.4×2×$6 = $1.58B`. So-what: 5% share = ~$79M revenue.
4. **Margin bridge.** Revenue flat; volume −22% on one SKU while a 2-month plant outage (2/12 ≈ 17% capacity) hit. Is the drop supply or demand? → outage explains ~17 of 22 pts; it's mostly supply. So-what: fix the line, don't rebuild demand.
5. **Blended-margin trap.** 30 mature stores at 40% margin + 10 new at 15% during ramp. Blended? → `(30×40 + 10×15)/40 = (1,200+150)/40 = 33.75%`. So-what: a "−6pt" fall can be pure immature-store mix, not core erosion.
6. **ROI/hurdle.** Initiative costs $5M [ILL], returns $2M/yr for 5y. Simple ROI & payback? → payback 2.5y; 5-yr return $10M on $5M = 100% (ignoring discounting; flag NPV if stakes are high).

---

## Part B — Exhibit & Chart-Reading Drills

An exhibit lands mid-case. The skill is not describing it — it's **extracting the insight and tying it to the question** in ~20–30 seconds.

### The 6-step exhibit protocol
1. **Read the title and axes first.** Units, time frame, what's actually plotted. Half of exhibit mistakes are misread axes.
2. **State what the chart *shows*** in one sentence (the trend/comparison), before interpreting.
3. **Find the outlier / inflection / crossover** — the one feature the interviewer put there on purpose.
4. **Tie it to the case question** — "so this tells us…". An observation without a link to the objective scores nothing.
5. **Quantify the gap.** Don't say "much higher" — say "~2×, about $40M".
6. **State the implication / next step** — what you'd now test or recommend.

### Chart-type cheat sheet (what each is testing)
| Chart | Reads as | Watch for |
|---|---|---|
| **Bar / column** | Level comparison across categories | Truncated y-axis exaggerating gaps |
| **Line** | Trend over time | Inflection points, crossovers, changing slope |
| **Stacked bar** | Composition *and* total over groups | Mix shift hiding inside a flat total |
| **100% stacked / share** | Composition only (mix) | Share ≠ absolute — a rising share on a shrinking pie |
| **Waterfall** | Bridge from A to B via +/− drivers | Which one or two bars move the total (80/20) |
| **Clustered bar** | Two dimensions at once (e.g. segment × year) | Read *within* and *across* clusters |
| **Marimekko (Mekko)** | Segment size (width) × share/margin (height) | Big-width × high-height = the money box |
| **Scatter** | Correlation / positioning of many units | Clusters, the off-diagonal outliers |
| **Pie** | Composition, few slices | Hard to compare slices — convert to numbers |

### Drill set (say the insight, not the description)
1. **Line, crossover.** Our cost/unit and price/unit lines cross in year 3 [ILL]. Insight: we go contribution-negative in year 3 — the business breaks then, not gradually; fix must land before it.
2. **Waterfall, profit bridge.** Profit falls $100M→$70M [ILL] via bars: volume −5, price −20, cost −10, mix +5. Insight: **price** did ~⅔ of the damage — attack realised price/discounting first; volume is a sideshow.
3. **Stacked bar, hidden mix.** Total revenue flat 3 years, but the high-margin segment's slice shrinks from 40%→25% [ILL]. Insight: flat top line hides margin decay — profit is falling even though revenue isn't.
4. **Mekko.** One segment is wide (big revenue) but short (thin margin); a narrow segment is tall (fat margin). Insight: growth focus and margin focus point at *different* boxes — don't conflate size with profitability.
5. **Clustered bar, segment × year.** Two of five segments carry all the growth [ILL]. Insight: 80/20 the strategy onto those two; the rest are noise or drag.
6. **Truncated axis trap.** A bar chart with a y-axis starting at 90 makes a 2% gap look enormous. Insight: quantify the *real* gap (2%) before reacting — the visual is misleading.

---

## Part C — Structuring Drills

The hardest live skill: hearing a novel prompt and laying a **tailored, MECE** structure in 90 seconds. Drill it deliberately.

### How to drill
1. Read/hear only the **prompt**. Note the **clarifying questions** you'd ask out loud (objective, scope/geography, business model, success metric) — good clarifiers are half the score.
2. Time yourself building a structure: ~2 min starting out, ~90 sec with practice.
3. Compare to a **sample** structure — sample ≠ "the answer"; there are several good trees. Grade on: MECE, *tailored to this business* (not a template), prioritised, and hypothesis-ready.

### The four clarifier lenses (ask before you structure)
**Objective** (what does success look like — profit, share, cash, a decision?) · **Business** (what does the client actually sell / how does it make money?) · **Scope** (geography, segment, timeframe) · **Constraints** (budget, capabilities, no-go options). One sharp clarifier per lens beats ten scattershot questions.

### 90-second framework scaffolds (starting points, not templates)
Tailor every branch to the client's actual words. "Revenue from oil-barrel sales" always beats "revenue".

**Profitability.** `Profit = Revenue − Cost`. Revenue = Σ(price × volume) by segment/SKU/channel; Cost = fixed + variable, split by driver. Isolate *where* the change concentrates before explaining *why*. External overlay: is the industry moving too (structural) or just us (company-specific)?

**Growth / Revenue.** Market analysis (size, growth, drivers, competition) → **Organic** (existing products: price/elasticity, volume via S&M, new channels/segments; new products: extend mix, R&D, cannibalisation) → **Inorganic** (M&A: synergies, fit, cannibalisation). Prioritise by attractiveness × right-to-win.

**Market Entry.** Target market (size, growth, customer need, our capturable share) · Competition (incumbents, barriers, likely response) · Company (right to win, capabilities, economics) · **Entry mode** (build / buy / partner) → entry profitability vs. hurdle.

**M&A / Investment.** Rationale (why, strategic fit) · Target attractiveness (standalone market + economics) · Synergies (revenue cross-sell; cost; **dis-synergies**) · Deal (price, integration risk, alternatives) → NPV/IRR vs. price.

**Pricing.** Triangulate three anchors: **cost floor**, **competitive reference** (substitutes/standard of care), **value ceiling** (economic value to the customer) → choose position given objective, payer/willingness, and volume response.

**Design / "what should we do" (non-traditional).** Structure by the **client's own stated goals** (e.g. Access / Quality / Accountability), each split short-term quick wins vs. structural moves; then prioritise by impact × feasibility × cost. Don't diagnose — generate and sequence.

### Drill prompts (structure cold, then self-check against the scaffolds)
1. **Knight Perfumes.** A men's-fragrance brand's profit fell this year across all lines by volume; online/quick-commerce only. → profitability tree, but note *all SKUs down on volume* pushes you up a level to demand/channel, not per-SKU cost. (Full crack in `case-bank-interview-classics.md` #4.)
2. **Bank Co.** A Midwest retail bank (deposits, loans, insurance; 20 branches, decline uniform across branches) has falling profit. → uniform-across-branches ⇒ structural/industry, not a branch problem; revenue = fee + net interest + premium, each with its own driver (rates, spread, volume).
3. **Avalon Education Policy.** Design a 10-year national policy across access/quality/accountability with stated targets. → structure by the three goals × (quick win / structural). (Crack in `case-bank-interview-classics.md` #13.)
4. **Furry Zoo.** Should a zoo bring in cheetahs on loan from abroad? → investment-decision tree: incremental revenue (footfall uplift × ticket + ancillary) vs. incremental cost (transport, habitat, care, risk) vs. hurdle; plus feasibility/ethical/regulatory gate.

### What a strong vs. weak structure looks like
- **Strong:** tailored labels, MECE, 3–5 branches with sub-branches, a stated Day-1 hypothesis and the branch you'd test first, delivered out loud with signposting.
- **Weak:** a memorised framework bolted on regardless of fit, overlapping buckets, no prioritisation, no hypothesis, and reading it silently off the page. See `case-facilitation-and-scoring.md` for the full rubric.

---

## Part D — Error Hunt (find the flaw, then fix it)

Most blown case answers do not come from hard math. They come from a plausible-looking step that nobody checked: a stock added to a flow, a share applied to the wrong year, an interviewer's headline taken on trust. Each drill below shows a flawed calculation. Cover the **Fix**, find the flaw within 60 seconds, then say it out loud the way you would flag it live: *"Before I use this, the table implies 60%, not 50% — can we check which one is right?"* Catching the flaw earns credit. Building a recommendation on it costs the case.

All figures in Parts D and E are **[ILLUSTRATIVE]**.

### The error-hunt protocol (run it on every number before you use it)
| # | Check | Question to ask | Tell-tale sign | Drill |
|---|---|---|---|---|
| 1 | **Units** | Do the units cancel to the unit I want? | GWh × $/kWh; ₹ bn in a $ column; crore read as 100M | D2, D12 |
| 2 | **Base** | Is each % of the same base? Which year's base? | Netting "−10%" against "+15%"; a share target applied to next year's market | D6, D11 |
| 3 | **Stock vs flow** | Is this a count at a moment or a count per period? | Parc + annual sales added; riders on board called "riders per day" | D3, D8 |
| 4 | **Gross vs net** | Is this revenue before or after fees, margin or load factor? | 100% occupancy; vendor fee ignored; revenue added to cost savings | D4, D5 |
| 5 | **Double counting** | Is anything counted at both ends, or in two branches? | Airport footfall; a filter also built into a usage mix; capacity × venues | D7, D15, E4 |
| 6 | **Period labels** | How many compounding periods sit between the endpoints? | A CAGR that fits a different window | D1, E5 |
| 7 | **Capacity caps** | Can output exceed the stated bottleneck? | A multiplier above 1× on capacity | D9, E4 |
| 8 | **Weighted averages** | Did I weight by the right shares? Did I average rates or their inverses? | An "average" eyeballed; averaged headways | D10, D13 |
| 9 | **Reconciliation** | Does the prompt's number match the exhibit? | Headline 50% while the table implies 60% | D13, D14 |
| 10 | **The question** | Does the answer's unit and scope match what was asked? | Total given when the average was asked; ₹ when units were asked | D10, D16 |
| 11 | **Margin vs markup** | Is the % of price or of cost? | "Cost × 1.4" called a 40% margin (it is a 28.6% margin) | — |

### Drills

#### D1. The CAGR window is mislabelled
- **The work shown** [ILLUSTRATIVE]: A digital-payments value market doubles from $10T in 2026 to $20T in 2030. "Counting 2026, 2027, 2028, 2029 and 2030 gives five years, so CAGR = 2^(1/5) − 1 = 14.9%."
- **Find the flaw:** How many compounding periods sit between the two endpoints?
- **Fix:** Periods = 2030 − 2026 = 4, so CAGR = 2^(1/4) − 1 = **18.9%**. Rule-of-72 check: doubling in 4 years needs about 72 ÷ 4 = 18%. Reverse check: $10T × 1.149⁴ = $17.4T, not $20T. The same slide type often carries a rate that fits no window at all: $430B (2025) → $650B (2030) is **8.6%** a year, not a stated 14.8% (at 14.8% the end value would be ~$858B).
- **Error fixed:** five years counted in 2026–30 → four compounding periods and 18.9% (periods = end year − start year; counting calendar years adds one).
- **Lesson:** Count the gaps, not the years, then check the rate against the rule of 72.

#### D2. GWh to dollars, off by 10×
- **The work shown** [ILLUSTRATIVE]: A renewable developer sizes the storage-pack market. "Grid storage: 150 GW installed × 10% paired with 2-hour batteries = 30 GWh × $120/kWh = **$360M**. EV packs: 30M vehicles a year × 2% electric → 4.8 GWh (two/three-wheelers at 10 kWh) + 4.2 GWh (cars at 35 kWh) = 9 GWh × $120/kWh = $1,080M. Total: 39 GWh = **$4,680M**."
- **Find the flaw:** Do the line items add up to the total? Then look at what kind of quantity each line is.
- **Fix:** 30 GWh = 30,000,000 kWh, and × $120 = **$3.6B**. Shortcut: 1 GWh at $X/kWh = $X million. $360M + $1,080M = $1.44B, which contradicts the $4.68B total. The total is right only because it was computed from 39 GWh directly. Second flaw: the 30 GWh is sized on the **installed** renewable base (a stock), while the 9 GWh is **one year's** vehicle output (a flow). An annual market uses new capacity: 150 GW × 10% growth = 15 GW added × 10% paired × 2 h = 3 GWh, plus 9 GWh from vehicles = **12 GWh ≈ $1.44B a year**.
- **Error fixed:** 30 GWh × $120/kWh = $360M → $3.6B (a GWh is a million kWh), and 30 + 9 GWh → 3 + 9 GWh on an annual basis (never add an installed base to a year's sales).
- **Lesson:** When the line items do not sum to the total, one of them has a unit slip. Find it before quoting either number.

#### D3. A stock added to a flow
- **The work shown** [ILLUSTRATIVE]: SUV tyre market. "The SUV parc is 42M. With a 15-year vehicle life, 42M ÷ 15 = 2.8M new SUVs a year. SUVs this year = 42M + 2.8M = 44.8M; grow 10% → 49.3M. Each has 5 tyres (with spare) and tyres last 5 years, so the market = 49.3M × 5 ÷ 5 = **49.3M tyres a year**."
- **Find the flaw:** What is 42M, and what is 2.8M? Can they be added?
- **Fix:** New sales replace retiring vehicles; they are already inside the parc. The parc stays 42M. The tyre market is two **flows**. (a) OEM fitment: new SUV sales = replacements 2.8M + net fleet growth 10% × 42M = 4.2M → 7.0M × 5 tyres = **35M**. (b) Replacement: 42M × 4 tyres (spares are rarely replaced) ÷ 5 years = **33.6M**. Total ≈ **69M tyres a year**, ~40% above the flawed answer. Also note the "× 5 ÷ 5" in the flawed chain cancels out, so it just returns the vehicle count.
- **Error fixed:** 42M + 2.8M = 44.8M "SUVs" → parc 42M; OEM 35M + replacement 33.6M ≈ 69M tyres (a stock and a flow cannot be summed).
- **Lesson:** Label every number "at a moment" or "per period" before you add it to anything.

#### D4. Gross take rate at 100% load factor
- **The work shown** [ILLUSTRATIVE]: A low-cost carrier fits Wi-Fi to 90 aircraft at $250k each, with the airline paying 40% = **$9M**. The airline also pays the vendor a per-session fee. "Passengers over 2 years = 10 widebodies' 2,500 flights a year × 300 seats × 2 = 1.5M, plus 80 narrowbodies' 27,500 flights × 100 seats × 2 = 5.5M. So 7M passengers × take rate × $10 = $9M, and take rate = **12.9%**."
- **Find the flaw:** Are seats the same as passengers? Is $10 what the airline keeps?
- **Fix:** Seats × flights assumes 100% load factor. At 80%, passengers = 5.6M. The airline recovers capex from **net** revenue per session: at a $2 vendor fee, $8. Required take rate = capex ÷ (seats × load factor × (price − fee)) = 9M ÷ (5.6M × $8) = **20.1%**. Each correction alone gives 16.1%. Against observed paid take rates of 5–10%, the gap is 2–4×, not 1.3–2.6×. Also sanity-check the base: 27,500 flights ÷ 80 narrowbodies ≈ 344 a year, under one a day, when low-cost narrowbodies typically fly several sectors a day.
- **Error fixed:** 9M ÷ (7M × $10) = 12.9% → 9M ÷ (5.6M × $8) = 20.1% (seats are not passengers, and the fee comes off before payback).
- **Lesson:** A break-even rate must use net unit revenue and realised volume, never list price and capacity.

#### D5. A revenue synergy added straight to cost savings
- **The work shown** [ILLUSTRATIVE]: A full-service carrier absorbs a premium JV airline. Combined revenue is $6B. "A 5% revenue uplift = $300M. Costs are ~75% of revenue = $4.5B, and 3% savings = $135M. Total value = $300M + $135M = **$435M a year**." The closing summary then quotes "$180M of cost savings".
- **Find the flaw:** Can a revenue number sit beside a cost saving? Why do two cost-saving figures appear?
- **Fix:** Revenue must pass through a margin first. At the case's own implied 25% margin: $300M × 25% = $75M, + $135M = **$210M a year of profit impact**. If the uplift comes from filling seats that already fly, the incremental margin may be higher. State the rate you use. The $180M is 3% of $6B, which treats costs as 100% of revenue. Pick one cost base and use it everywhere. A 25% operating margin is also implausible for a full-service carrier, so test it. Then phase the run-rate synergy and deduct one-off costs before comparing it with any premium paid.
- **Error fixed:** $300M + $135M = $435M → $75M + $135M = $210M (top line and bottom line do not add).
- **Lesson:** Only profit adds to profit. Convert revenue synergies at an explicit incremental margin.

#### D6. Percentage changes on different bases
- **The work shown** [ILLUSTRATIVE]: An electronics maker's profit fell 12% after moving component sourcing offshore. "Procurement cost fell 10% and logistics cost rose 15%, so total cost rose. Logistics is the culprit."
- **Find the flaw:** A 10% change and a 15% change of what?
- **Fix:** Net cost change = −10% × procurement + 15% × logistics. Costs rise only if logistics spend exceeds 10/15 ≈ two-thirds of procurement spend. With procurement at 60% of total cost and logistics at 7%: −6.0 + 1.05 = **−4.95 points**. The move *saves* ~5% of cost on these two lines, so the 12% profit fall must come from lines not yet sized, such as inventory in transit and warranty claims from lower-quality parts. Variant: processing cost +15% against a price rise of +5%. The price rise needed is 15% × processing cost's share of price. At a 30% share that is **4.5%**, so a 5% rise more than covers it.
- **Error fixed:** "−10% and +15% means a net increase" → −4.95% of total cost at 60% and 7% weights (percentages must be weighted by their bases before they are netted).
- **Lesson:** Never net two percentages until both are expressed as shares of the same total.

#### D7. A filter applied twice
- **The work shown** [ILLUSTRATIVE]: Retail ketchup revenue in a ~750M-population high-income region. "Households = 750M ÷ 3 = 250M, and 80% buy sauce = 200M buying households. Usage mix: heavy 20% × 2 bottles a month + moderate 40% × 1 + light 20% × 0.5 + non-users 20% × 0 = 0.9, call it ~1 bottle per buying household. So 200M × 1 × 0.5 kg × 12 = 1,200M kg × €3/kg = **€3.6B**."
- **Find the flaw:** Who is inside the 0.9?
- **Fix:** The usage mix already includes the 20% of non-users, so 0.9 bottles is per **household**, not per buying household. The non-users were removed twice, and rounding 0.9 up to 1 partly hid it. Correct: 250M × 0.9 = 225M bottles a month (equivalently 200M buyers × 1.125) → × 0.5 kg × 12 = 1,350M kg × €3 = **€4.05B**. Without the lucky round-up, the flawed chain gives 200M × 0.9 → €3.24B, 20% low.
- **Error fixed:** 200M buying households × 0.9 (rounded to 1) → 250M households × 0.9 = 225M bottles a month and €4.05B (a filter must be applied once: in the base or in the mix, never both).
- **Lesson:** Before multiplying a segment mix, check whether its buckets include the people you have already filtered out.

#### D8. A snapshot reported as a daily flow
- **The work shown** [ILLUSTRATIVE]: Daily ridership of a capital city's metro. "Busiest line: 90 minutes end to end; trains every 2 minutes for 8 rush hours and every 5 minutes for 12 other hours, so average headway = (8×2 + 12×5) ÷ 20 = 3.8 min. Trains on the line = 90 ÷ 3.8 × 2 directions ≈ 47. Riders = 47 trains × 8 coaches × 150 per coach × 80% = **45,120 a day**. Ten lines → **~451k a day**."
- **Find the flaw:** What does 47 trains × their load actually count? Where do the 20 operating hours enter?
- **Fix:** 45,120 is the number of people on board **at one instant**, a snapshot. The operating hours never enter, which is the tell-tale sign. Daily riders = departures × load per departure × turnover per run. Departures: 8 × 30 + 12 × 12 = 384 per direction = **768 a day**. Load: 8 × 150 × 60% = 720 (the 80% quoted is a peak load, not an all-day average). Turnover: the average trip covers ~40% of the line, so each place is refilled ~2.5 times per run. 768 × 720 × 2.5 ≈ **1.4M a day on this line alone**, about 30× the flawed figure. Second slip: averaging headways understates trains. Average the **frequency** instead: (8 × 30 + 12 × 12) ÷ 20 = 19.2 trains an hour, an effective headway of 3.125 min, not 3.8.
- **Error fixed:** 47 × 960 = 45,120 "a day" → 768 runs × 720 × 2.5 ≈ 1.4M a day (a count at an instant needs a time dimension and turnover to become a flow).
- **Lesson:** If a stated duration (hours, days, life) is never used, the answer is probably a stock posing as a flow.

#### D9. A multiplier above capacity
- **The work shown** [ILLUSTRATIVE]: Cars a day over an 8-lane tolled sea bridge. The toll plaza is the stated bottleneck at 5 cars a minute per lane, so capacity = 8 × 5 × 60 = 2,400 an hour. "Low load 6 h × 0.5 × capacity = 7,200; medium 12 h × 1.0 = 28,800; high 6 h × **2.0** = 28,800. Total **64,800 a day**."
- **Find the flaw:** Can a bottleneck pass twice its capacity?
- **Fix:** Throughput = min(demand, capacity). A "2× capacity" peak is a queue, not flow, so cap it at 1.0: 6 h × 2,400 = 14,400. The hard ceiling is 7,200 + 28,800 + 14,400 = **50,400**. A realistic profile of 100% peak, 60% medium and 20% low utilisation gives 14,400 + 17,280 + 2,880 = **~34,600 crossings a day**. These are crossings, not unique cars: a commuter who goes and returns counts twice.
- **Error fixed:** high load at 2.0 × capacity = 28,800 → capped at 14,400, ceiling 50,400 (output cannot exceed the bottleneck the chain itself declared).
- **Lesson:** Once you name a bottleneck, every multiplier on it must be ≤ 1.

#### D10. The weighted-average slip
- **The work shown** [ILLUSTRATIVE]: The sports-shoe market in a 1.5B-population country. "Location filter ~80%, gender filter ~55%. Age: shares of 25/25/20/20/10% with buying rates of 40/80/60/40/2% → weighted average **~60%**. Relevant population = 1,500M × 0.8 × 0.55 × 0.6 = 396M. Average price = 60% × ₹500 + 30% × ₹1,200 + 10% × ₹3,000 = ₹960. Market = 396M × ₹960 = **₹380 bn**." The question asked for *the number of pairs sold a year*.
- **Find the flaw:** Recompute the age average. Then reread the question.
- **Fix:** 0.25 × 40 + 0.25 × 80 + 0.20 × 60 + 0.20 × 40 + 0.10 × 2 = **50.2%**. (Even the simple average is 44.4%, so 60% came from nowhere.) Relevant population = 1,500M × 0.8 × 0.55 × 0.502 = **331M** → × ₹960 = **₹318 bn**, 16% lower. Second flaw: the question asked for pairs. That needs a purchase frequency. At one pair every 1.5 years, that is ~**221M pairs a year**. Report ₹ only as a secondary figure.
- **Error fixed:** age-weighted average "~60%" → 50.2%, so 396M → 331M buyers and ₹380 bn → ₹318 bn (a weighted average must be computed, not eyeballed).
- **Lesson:** Write out every weighted average in full. Then check that the answer's unit is the one asked for.

#### D11. A share target applied to the wrong base
- **The work shown** [ILLUSTRATIVE]: A global e-commerce player entering a Southeast Asian market expects **20% share this year**. Incumbents earn $600M + $400M, so the market is $1,000M today and grows 40% next year. "Revenue = 20% × $1,400M = $280M. Variable cost at 80% = $224M, + $50M fixed = $274M < $280M, so we break even in year 1."
- **Find the flaw:** Which year does the 20% belong to? What kind of margin is the 20%?
- **Fix:** The share target is for this year, so revenue = 20% × $1,000M = **$200M**. Contribution at 20% = $40M, less $50M fixed = **−$10M**. There is no year-1 break-even. Break-even revenue = $50M ÷ 20% = $250M, a **25%** share of this year's market (17.9% of next year's), so the decision flips on the base. Also clarify the margin: if 20% is a *net* profit margin, the fixed cost already sits inside the 80% and the flawed chain counts it twice. The chain works only if 20% is a contribution margin.
- **Error fixed:** 20% × next year's $1,400M = $280M → 20% × this year's $1,000M = $200M and a $10M loss (a share applies to the market of the same period).
- **Lesson:** Tag every share, rate and market size with its year before multiplying them.

#### D12. Unit mismatches: ₹ bn as $ bn, crore as 100 million
- **The work shown** [ILLUSTRATIVE]: A sector slide ranks three hospital chains by market cap: "**$1,079B, $952B, $640B**". A market note says "insurers sold **290 million** new policies". The underlying filing reports 2.9 crore.
- **Find the flaw:** Would a hospital chain be worth about $1T? How many zeros are in a crore?
- **Fix:** A ~$1T hospital chain would outrank almost every listed healthcare company in the world, so these are **₹ billion**. At ₹85/$: **~$12.7B, $11.2B and $7.5B**. A crore is 10 million (100 lakh), so 2.9 crore = **29 million** policies, not 290 million. Conversion card: 1 lakh = 100,000; 1 crore = 10M; 1 lakh crore = ₹1 trillion ≈ $11.8B at ₹85.
- **Error fixed:** "$1,079B" → ≈ $12.7B (a ₹ figure in a $ column), and 2.9 crore = 290M → 29M (1 crore = 10M, not 100M).
- **Lesson:** Sanity-check any large figure against the biggest company or market you know. A 10× or 85× gap means a unit slip.

#### D13. The interviewer's headline does not reconcile with the exhibit
- **The work shown** [ILLUSTRATIVE]: Prompt: "A national bank's new internet-banking platform hit **97%** adoption at launch and has fallen to **50%**." Exhibit: by age band, 18–35 (20% of customers) 98% → 90%; 36–50 (20%) 95% → 78%; 50–65 (35%) 96% → 55%; 65+ (25%) 94% → 30%. The candidate sizes the recovery on a 47-point gap.
- **Find the flaw:** Weight the table. Does it give 97% and 50%?
- **Fix:** Initial = 0.20 × 98 + 0.20 × 95 + 0.35 × 96 + 0.25 × 94 = **95.7%**. Current = 0.20 × 90 + 0.20 × 78 + 0.35 × 55 + 0.25 × 30 = **60.4%**. The gap is **35.4 points**, not 47. The headline must use another metric (registered vs monthly active), another base (accounts vs customers) or another date. Say so, agree which figure to use, then size the recovery. Part E2 shows where the 35 points come from.
- **Error fixed:** a 97% → 50% headline taken as given → a 95.7% → 60.4% table-weighted gap of 35.4 points (the prompt and the exhibit must reconcile before you size anything).
- **Lesson:** Weight every segment table and compare it with the prompt. Raise any mismatch before building on it.

#### D14. A "revenue is falling" premise the data contradicts
- **The work shown** [ILLUSTRATIVE]: Prompt: "A leading beverage company's growth has dropped." Candidate: "Since revenue is falling, let's split it into price × volume," and goes straight to the soda brands. Exhibit (litres M, price ₹/L, cost ₹/L; last year → this year): soda 100 → 120 L at ₹30 → ₹24 (cost ₹15); water 30 → 33 L at ₹25 (cost ₹12); others 10 → 11 L at ₹50 → ₹55 (cost ₹30).
- **Find the flaw:** Is total revenue actually falling? What does the cost column say?
- **Fix:** Total revenue = ₹4,250M → ₹4,310M, **+1.4%**. Only soda revenue fell (₹3,000M → ₹2,880M, −4%), while water (₹750M → ₹825M) and others (₹500M → ₹605M) grew. The real drop is **profit**. Gross profit = ₹2,090M → ₹1,784M, **−14.6%**. Soda gross profit fell 28% (₹1,500M → ₹1,080M) and soda margin fell from 50% to 37.5%. The cost data was on the table and went unused. Restate the problem: "Revenue is up 1.4%, but gross profit is down 14.6%, driven by a collapse in soda price and mix." Then decompose it (E1).
- **Error fixed:** "revenue is falling" → revenue +1.4%, gross profit −14.6% (define which metric has dropped before you choose a tree).
- **Lesson:** Clarify which metric moved (revenue, profit, growth rate or margin) and use every column you are given.

#### D15. Airport footfall counts each trip twice
- **The work shown** [ILLUSTRATIVE]: "The country's airports handled ~380M passengers last year. Assume each flyer flies once a year, so ~380M people fly, over a quarter of the population."
- **Find the flaw:** What does one domestic flight add to the airport passenger count?
- **Fix:** Airport throughput counts a domestic passenger at both the departure and the arrival airport. Treating all traffic as domestic, 380M ÷ 2 = **190M one-way journeys**. A trip is usually a round trip: ÷ 2 = 95M round trips. Flyers average ~2.5 round trips a year: 95M ÷ 2.5 ≈ **38M unique flyers**, a tenth of the flawed answer. The same trap appears in toll crossings vs unique cars and metro entries vs unique riders.
- **Error fixed:** 380M airport passengers = 380M flyers → ~190M journeys and ~38M unique flyers (throughput counts each journey at both ends, and people repeat trips).
- **Lesson:** Ask what one event adds to the counter. Then convert events → journeys → trips → people.

#### D16. The answer does not answer the question
- **The work shown** [ILLUSTRATIVE]: "What is the **average** number of hours an air-conditioner runs in a year in a ~15M north-Indian city?" Work: "15M ÷ 5 = 3M households × 30% AC penetration = 0.9M ACs. Summer (Mar–Jul) 153 days × 7 h, monsoon (Aug–Oct) 91 days × 3 h, winter (Nov–Feb) 120 days × 0 h = 1,344 h per AC. Answer: 0.9M × 1,344 = **1,209M hours**."
- **Find the flaw:** Check the day count. Then check what was asked.
- **Fix:** Aug–Oct is 31 + 30 + 31 = **92** days, and the three seasons must sum to 365 (153 + 91 + 120 = 364). Hours per AC = 153 × 7 + 92 × 3 = **1,347 a year**, about 3.7 h a day averaged over the year. That is the answer to the question asked. The city-wide total (0.9M × 1,347 ≈ 1,212M hours) is a by-product. Also sanity-check the daily profile: a split that gives the hottest afternoon hours the least use is backwards.
- **Error fixed:** 91 days and a city total of 1,209M h → 92 days and an average of 1,347 h per AC (seasons must cover 365 days, and the unit must match the question).
- **Lesson:** Before you answer, restate the question's unit and scope, then check your final number matches it.

---

## Part E — Decomposition & Reconciliation Drills

Part D catches bad numbers. Part E builds the tools that explain a change and reconcile it to the whole. Use them whenever a case says "X fell" or "can we hit Y". Each drill gives the setup, the spine with the math, the aha and the trap. All figures are **[ILLUSTRATIVE]**.

### E1. Price-volume-mix (PVM) decomposition
**Setup.** Soda revenue fell ₹120M (₹3,000M → ₹2,880M) while soda volume rose 20%. Three brands:

```
Brand         Litres M (LY → TY)   ₹/L (LY → TY)   Revenue ₹M (LY → TY)
Premium A        50 → 30             36 → 36          1,800 → 1,080
Brand B          25 → 30             26 → 26            650 →   780
Value brand      25 → 60             22 → 17            550 → 1,020
Total           100 → 120      avg   30 → 24          3,000 → 2,880
```

**Spine: formulae, and the base each effect uses.**
```
Volume effect = (Q₁ − Q₀) × P̄₀                       total volume change at LY average price (LY mix, LY prices)
              = (120 − 100) × 30                     = +600
Mix effect    = Q₁ × (Σ s₁ᵢ·P₀ᵢ − P̄₀)                TY volume, TY mix shares s₁ᵢ, LY prices, vs LY average
              = 120 × (0.25×36 + 0.25×26 + 0.50×22 − 30)
              = 120 × (26.5 − 30)                    = −420
Price effect  = Σ Q₁ᵢ × (P₁ᵢ − P₀ᵢ)                    TY volumes × price change
              = 60 × (17 − 22)                       = −300
Check         = 600 − 420 − 300                      = −120 ✓
```
Cross-check via "TY volume at LY prices": 30×36 + 30×26 + 60×22 = ₹3,180M. Volume + mix = 3,180 − 3,000 = +180. Price = 2,880 − 3,180 = −300.

**Aha.** The 20% volume growth would have added ₹600M on its own. The loss comes from **mix** (−₹420M), as buyers traded down from premium A to the value brand, more than from the value brand's price cut (−₹300M). The value brand's volume grew 2.4× while its revenue grew only 1.85×. The real question is why A's buyers switched (cannibalisation by a cheaper sibling), not how to promote A to a new demographic. Carry it to profit: with cost at ₹15/L, the extra 20M litres cost ₹300M, so a ₹120M revenue dip becomes a **₹420M gross-profit drop** (₹1,500M → ₹1,080M).

**Trap.** Explaining the dip as "A lost volume and the value brand cut price" without isolating mix. Also, PVM is order-dependent: this convention puts the price × volume cross-term in the price effect by using this year's volumes. State your convention. The total never changes, but rupees can shift between effects.

### E2. Weighted contribution: who drives the decline?
**Setup.** Digital-banking usage fell (table in D13). Which customers cause the drop?

**Spine.** A segment's contribution to the change in the average is its weight × its own change. Its share of the decline is wᵢΔᵢ ÷ ΣwⱼΔⱼ.
```
Segment   Weight   Δ usage (pts)   w × Δ (pts)   Share of decline
18–35      20%        −8              −1.60            4.5%
36–50      20%       −17              −3.40            9.6%
50–65      35%       −41             −14.35           40.6%
65+        25%       −64             −16.00           45.3%
Total     100%                       −35.35          100%
```
Over-50s: 30.35 ÷ 35.35 = **~86% of the decline from 60% of customers.**

**Aha.** Prioritise the over-50 fix (assisted onboarding, simpler login, fraud reassurance). But a 17-point fall among 36–50s says something platform-wide changed too. Ask *when* the decline started, for example after a login or security change, before blaming age alone.

**Trap.** Comparing raw drops (−64 vs −8) without weights, or sizing on an unreconciled headline (D13). Also, complaint shares are percentages of *complainants*, not of all users, so they are not prevalence rates.

### E3. Market-share points → revenue in a growing market
**Setup.** A 500-store grocery chain's share fell from 30% to 22% over two years while the market grew. "Is revenue down, and how big is the problem?"

**Spine.**
```
R₁ / R₀ = (s₁ / s₀) × (M₁ / M₀)
Flat revenue needs M₁/M₀ = 30/22 = 1.364  → +36.4% market growth over 2 years (~16.8% a year)
Example: market ₹10,000 cr growing 12% a year → ₹12,544 cr
  Client revenue: ₹3,000 cr → 22% × 12,544 = ₹2,760 cr   (−8.0%, a ₹240 cr visible decline)
  Held-share counterfactual: 30% × 12,544 = ₹3,763 cr
  Share loss in value: 8 pts × ₹12,544 cr ≈ ₹1,000 cr        (~4× the visible decline)
```
**Aha.** An 8-point loss is a 26.7% relative loss. In a growing market it shows up as only a modest revenue dip. Size the prize against the **held-share counterfactual**, not last year's revenue. Because the loss is client-specific, industry-level tools (five forces) cannot explain it. Compare the client with the players who *gained* share on price, assortment, delivery and convenience.

**Trap.** Treating "share down" as "revenue down" (or the reverse), and never turning share points into money.

### E4. Revenue target vs physical capacity
**Setup.** A music company enters live theatre with a **$20M** year-1 revenue target. It has three 320-seat venues and **9 shows a week in total**, sells tickets at $14, expects 60% occupancy and plans $60M of capex.

**Spine.** Revenue = seats × occupancy × shows × (ticket + ancillary per head).
```
Filled seats per show   = 320 × 60%                  = 192
Weekly ticket revenue   = 192 × 9 × $14              = $24,192   → × 52 = $1.26M
Ancillary ($4/head)     = 192 × 9 × 52 × $4          = $0.36M    → total ≈ $1.62M
Sold-out ceiling        = 3 venues × 8 shows × 320 × 100% × ($14 + $4) × 52 = $7.19M
Shows needed at $14     = $20M ÷ ($14 × 192)         = 7,440 a year ≈ 143 a week
Price needed at 24/wk   = $20M ÷ (192 × 24 × 52)     = ~$83
```
**Error fixed:** 192 × 9 × $14 × 3 venues = $72,576 a week ($3.77M a year) → $24,192 a week ($1.26M) (the 9 shows are already the total across all venues, so multiplying by venues counts capacity three times).

**Aha.** The target is ~16× what the current plan produces (~12× with ancillary) and ~2.8× a sold-out, 24-show-a-week ceiling. No operating lever closes that gap. The answer is to reset the target or change the model (larger venues, touring, licensing the music IP). With $60M of capex against ~$1.6M of revenue, payback exceeds 37 years even at a 100% margin, so as structured this leans no-go. Note also that only $40M of the $60M is allocated ($25M venues + $15M staff and productions). Ask where the rest goes.

**Trap.** Softening the verdict to "proceed cautiously" when the capacity math says the target cannot be met. Compute the physical ceiling before discussing marketing.

### E5. CAGR sanity check with the rule of 72
**Setup.** A sector deck quotes growth rates. Test each one in 20 seconds.

**Spine.** Periods n = end year − start year. CAGR = (End ÷ Start)^(1/n) − 1. Rule of 72: doubling time ≈ 72 ÷ rate%. Anchor: 1.1⁷ ≈ 2. Reverse check: End = Start × (1 + r)ⁿ.
```
Claimed rate & window   Endpoints                    n   Implied CAGR   Verdict
14.9%, 2026–30          $10T → $20T                  4   18.9%          2× in 4 yrs ≈ 72/4 = 18%; 14.9% is a 5-yr doubling
14.8%, 2025–30          $430B → $650B                5   8.6%           only 1.5× in 5 yrs; 14.8% would give ~$858B
6.7%, 2026–31           $39B → $75B                  5   ~14%           near-doubling in 5 yrs; 6.7% doubles in ~11 yrs (→ ~$54B)
15%, 2024–30            $125B → $345B                6   18.4%          15% would give ~$289B
11.9%, "2024–30"        $16.5B (2026) → $29.0B (2031) 5  11.9%          rate right, label wrong: it is 2026–31
```
**Aha.** Two mental checks catch nearly every bad CAGR. First, how many doublings fit the ratio? Second, does 72 ÷ rate match the years? A rate right for the endpoints but wrong for the label is still an error, because anyone projecting forward will compound from the wrong year.

**Trap.** Computing n by counting calendar years (one too many), and trusting a market size whose metric (GMV vs revenue vs spend) and date are not stated.

### E6. Geometric-series break-even (growing subscriber base)
**Setup.** A game studio must recover **$180M** ($150M development + $30M marketing) within 3 years from a **$15/month** subscription. The subscriber base grows **20% a year** (stepwise, flat within each year). How many launch subscribers S are needed?

**Spine.**
```
Revenue = 12 × P × S × (1 + g + g² …)        → S = C ÷ (12 × P × F)
F = Σ (1+g)^t for t = 0..n−1 = ((1+g)^n − 1) ÷ (g) with 1+g = 1.2, n = 3
  = (1.728 − 1) ÷ 0.2 = 3.64                  (= 1 + 1.2 + 1.44)
S = $180M ÷ (12 × $15 × 3.64) = $180M ÷ 655.2 = 274,725 ≈ 275k
Check: Y1 $49.45M + Y2 $59.34M + Y3 $71.21M = $180M ✓
```
**Error fixed:** 12 × 15 × 3.64 = 654.72 → 655.2 (and $180M ÷ 654.72 = 274,927, which does not match the 274,725 quoted beside it; multiply the constants once, carefully).

**Aha.** F is the growth-series (annuity-style) factor, and it turns a growing stream into one division. The flat shortcut, $180M ÷ 36 months ÷ $15 = 333,333, is the *average* base, not the launch base.

**Trap.** Applying the factor to the wrong quantity: F multiplies the *launch* base, not the average one, and n counts periods, not year-labels. 275k is a gross-revenue floor, not a plan.

**Full business case:** `case-bank-unconventional.md` U8 carries this through platform fee, running costs, a live-ops team, churn and discounting.
