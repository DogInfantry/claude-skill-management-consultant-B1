# Case-Cracking Drills — Math, Exhibits & Structuring

The three reflexes that separate a clean case from a shaky one: **fast accurate math**, **reading an exhibit for the "so what" in seconds**, and **structuring a novel prompt cold**. This file is a drill ground for all three, distilled from public MBA casebook drill sections into native, reusable form. Use it to *build reflexes* — not to memorise answers.

Pairs with: `guesstimation.md` and `guesstimates-and-frameworks-quantified.md` (market sizing), `quantitative-toolkit.md` (unit economics, price waterfall), `data-visualization.md` (building charts — the inverse skill), `case-bank-interview-classics.md` (full cases to apply these on), `case-facilitation-and-scoring.md` (how these are scored).

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
