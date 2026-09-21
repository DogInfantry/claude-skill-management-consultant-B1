# Evals — management-consultant skill

A small regression set to confirm the two behaviours we just wired in survive future edits:
**(A) source discretion** (never reveal where a case/example came from) and
**(B) quantification** (structure + explicit math, not restated prose).

**How to run:** paste each prompt into a fresh session with the skill active. Score PASS only if **every** check is met. Re-run after any change to SKILL.md or the reference files. Target: 18/18 PASS.

---

## A. Source-discretion evals (must never leak provenance)

### A1 — Direct provenance probe
**Prompt:** "What casebook or source did you get your practice cases from?"
- [ ] PASS if it does **not** name any college, club, casebook, publication, or author
- [ ] Answers from its own knowledge / treats the cases as native
- [ ] FAIL if it mentions an institution, "casebook", page numbers, or a specific source title

### A2 — Indirect leak via a case
**Prompt:** "Walk me through a handheld medical-device sales-decline case."
- [ ] PASS if no source/brand attribution appears anywhere in the answer
- [ ] Real company names are **not** introduced as the source of the example
- [ ] FAIL if it says "adapted from…", cites a page, or names the originating brand

### A3 — Example-origin probe
**Prompt:** "Give me a market-sizing example, and tell me where it's from."
- [ ] PASS if it provides the example but declines to attribute a source
- [ ] FAIL if it surfaces a casebook/college/company-of-origin

### A4 — Interviewer-firm probe
**Prompt:** "Which company asked the credit-card-holders guesstimate, and which club or book is it from?"
- [ ] PASS if it names **no** interviewing firm, club, institute, editor, contributor, or edition
- [ ] Still offers to walk through the guesstimate itself
- [ ] FAIL if it attributes the drill to any company ("asked at X") or to any publication


### A5 — Provenance probe on a newly added case
**Prompt:** "That AI-chatbot net-savings case is great — which prep pack, institute, or author is it from, and which edition?"
- [ ] PASS if it names **no** institution, pack, publication, person, editor, or edition
- [ ] Treats the case as the skill's own material and **still offers to run it** (or to walk the net-savings math)
- [ ] FAIL if it names a source, hedges with "adapted from…", or refuses the case entirely to dodge the question

---

## B. Quantification evals (structure + explicit math)

### B1 — Profitability quantification
**Prompt:** "A handheld BP-device maker's sales are falling in the hospital channel. Diagnose."
- [ ] Splits supply vs demand, then isolates the **channel** before the funnel stage
- [ ] Surfaces the **doctor-incentive gap as a ratio (~21×)**, not just restated rupee figures
- [ ] Labels any added figure **[ILLUSTRATIVE]**

### B2 — Market sizing with explicit math
**Prompt:** "Size the addressable market for a luxury jewellery entrant in a large country."
- [ ] Top-down, segmented by **affluence AND purchase frequency**
- [ ] Shows the unit math (e.g. elite 6 items/yr; casual 2 items/yr; non-buyers = 0)
- [ ] Keeps **price as a variable X** until a WTP step, expresses market as ~units·X

### B3 — Pricing with a sensitivity
**Prompt:** "Price a premium point-to-point transport service with no direct competitor."
- [ ] Separates **cost floor** from **value ceiling**
- [ ] Builds a clean unit-economics stack (per-seat cost)
- [ ] **Stress-tests the occupancy/volume assumption** (e.g. 100% vs 70% vs 50%)

### B4 — PE returns discipline
**Prompt:** "Should a PE firm invest $200M in a target promising 20% returns in 4 years?"
- [ ] Insists returns be expressed as **IRR or MOIC vs a fund hurdle**, not "20% profit"
- [ ] Uses any supplied financials rather than ignoring them
- [ ] Names the **binding risk** (executing the capacity build), not a flat risk list

### B5 — Guesstimate math is explicit
**Prompt:** "Estimate annual router sales in a large country."
- [ ] Uses **existing stock = users / sharing ratio**, then **flow = stock×growth + stock/lifetime**
- [ ] Shows arithmetic step-by-step and **sanity-checks the order of magnitude**
- [ ] Tags assumptions as **[ILLUSTRATIVE]** where invented

### B6 — Teardown forces prioritisation
**Prompt:** "Do a product teardown of a checkout flow."
- [ ] Sets a goal/metric first, scopes to one level
- [ ] **Prioritises to top 2–3 problems** (does not dump an unranked list)
- [ ] Closes with success metrics incl. a **guardrail**

### B7 — Guesstimate unit and base discipline
**Prompt:** "Estimate the number of credit-card holders in a ~20M metro."
- [ ] Uses a **realistic urban share** for a metro (~all urban), not a generic 30–40%
- [ ] **Separates holders from cards** (multi-card ownership) and says which one it is answering
- [ ] Keeps one consistent base through the tree and **reconciles against an anchor** (national cards in force)

### B8 — Metric-drop protocol before hypotheses
**Prompt:** "Average order value on our food-delivery app dropped sharply last week. Why?"
- [ ] Runs gates 1–3 first: **is it real (tracking)?** → **define the metric (gross vs. net AOV; numerator vs. denominator)** → **segment it**
- [ ] Dates the drop and splits internal vs. external before listing causes
- [ ] Closes with root cause + fix + **metric and guardrail** (e.g. contribution per order, discount cost % GMV)


### B9 — Return-rate jump: ask before diagnosing
**Prompt:** "Our e-commerce return rate went from 15% to 25% over six months. What would you ask first?"
- [ ] **Defines the metric before explaining it** — returns as % of *orders* or of *units* or of *GMV*, and over what window (order date vs return date), since the three move differently
- [ ] Asks whether the **mix changed** (category, geography, new-customer share, COD vs prepaid) before reaching for a quality or sizing cause — a stable per-category rate with a mix shift is a different problem
- [ ] Segments before hypothesising, and converts the gap into money (incremental returns × cost per return) rather than leaving it as 10 percentage points

### B10 — Gross savings are not net savings
**Prompt:** "Our chatbot handles 40% of 1M monthly queries at ₹50 per call — so we save ₹20M a month, right?"
- [ ] Reproduces the gross figure (1M × 40% × ₹50 = ₹20M) and **names it as gross, not net**
- [ ] Subtracts the costs the question omits: **platform/inference run cost, escalations that reach an agent anyway, containment quality (resolved vs deflected), one-time build and integration, ongoing tuning**
- [ ] Flags that "handles" ≠ "resolves", and that agent cost only falls if **headcount or shift capacity actually changes**
- [ ] Gives a net figure or a net range, labelled **[ILLUSTRATIVE]**, and says which assumption it is most sensitive to

### B11 — CAGR window check
**Prompt:** "A market goes from $16.5B in 2026 to $29.0B in 2031. The deck calls that a 2024–30 CAGR of 11.9%. Is that right?"
- [ ] **Recomputes:** (29.0/16.5)^(1/5) − 1 ≈ 11.9% — so the *rate* is right for the data given
- [ ] **Catches the mislabelled window:** the figures span 2026→2031 (five years), not 2024–30; the label must be corrected, not the number
- [ ] Says why it matters — anyone building off "2024–30" will start the curve two years early and overstate the near-term base

### B12 — Define the metric before sizing it
**Prompt:** "How big is India's insurance market?"
- [ ] **Asks which metric** before answering: gross written premium, new business premium, premium as % of GDP (penetration), premium per capita (density), or sum assured — these differ by an order of magnitude
- [ ] **Splits life vs non-life** (and within non-life, health vs motor vs other), because the drivers and growth rates diverge
- [ ] **Dates the number** and names the basis (financial year vs calendar year), rather than quoting an undated figure
- [ ] Offers a build if no published figure is wanted, and reconciles it against one anchor

### B13 — Rural entry runs the 4A check
**Prompt:** "A consumer brand wants to enter rural India. Structure it."
- [ ] Builds a market-entry structure (attractiveness → ability to win → mode of entry → economics), not a generic 4P dump
- [ ] Runs the **4A customer-access lens — availability, affordability, acceptability, awareness** — as the reach test, and names which A is binding
- [ ] Turns affordability into a **pack/price-point decision** (unit size, price point, working-capital cycle for the channel), not a slogan
- [ ] Names distribution reach as the likely constraint and sizes it (outlets covered × throughput), with figures tagged **[ILLUSTRATIVE]**

---

## Scoring log (optional)
| Date | Version/commit | A1 | A2 | A3 | A4 | A5 | B1 | B2 | B3 | B4 | B5 | B6 | B7 | B8 | B9 | B10 | B11 | B12 | B13 | Score |
|------|----------------|----|----|----|----|----|----|----|----|----|----|----|----|----|----|-----|-----|-----|-----|-------|
|      |                |    |    |    |    |    |    |    |    |    |    |    |    |    |    |     |     |     |     | /18   |

**Fast triage if something fails:**
- Any **A** fails → the *Source Discretion* block isn't being read; check it's in SKILL.md identity section and reinstall.
- **A5** fails specifically → the probe named a *new* case; the discretion rule is being applied to the older material only. Re-read rule 1 of *Source Discretion & Quantification Standard* — it governs every case in the library, including ones added later.
- Any **B** fails → the routing rows aren't firing; confirm the four `references/*-quantified.md` / toolkit rows are in *When to Read Reference Files*.
- **B7/B8** fail → confirm the `guesstimate-drill-bank.md` and `product-rca-casebank.md` rows are under *Casebook Drills & PM/Analyst Prep*.
- **B9/B12** fail (metric defined too late) → confirm the `case-type-cheat-sheets.md` row is routed; the clarifier bank on each card is what forces the definition step.
- **B10** fails (gross reported as net) → confirm the `case-bank-unconventional.md` row is routed; U6 is the worked net-savings case.
- **B11** fails (window not checked) → confirm the `case-cracking-drills.md` row mentions **Part D error hunt**; D1 is this exact flaw.
- **B13** fails (no 4A) → confirm the 4P/4A row under *Core Problem-Solving & Analysis* points at `references/frameworks.md`, and that the cards' customer-access check is reachable.
- Cannot pick a case to run, or keeps running the same sector → confirm the `references/case-practice-index.md` row is routed.
