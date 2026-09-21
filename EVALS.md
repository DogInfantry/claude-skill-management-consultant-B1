# Evals — management-consultant skill

A small regression set to confirm the two behaviours we just wired in survive future edits:
**(A) source discretion** (never reveal where a case/example came from) and
**(B) quantification** (structure + explicit math, not restated prose).

**How to run:** paste each prompt into a fresh session with the skill active. Score PASS only if **every** check is met. Re-run after any change to SKILL.md or the reference files. Target: 12/12 PASS.

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

---

## Scoring log (optional)
| Date | Version/commit | A1 | A2 | A3 | A4 | B1 | B2 | B3 | B4 | B5 | B6 | B7 | B8 | Score |
|------|----------------|----|----|----|----|----|----|----|----|----|----|----|----|-------|
|      |                |    |    |    |    |    |    |    |    |    |    |    |    | /12   |

**Fast triage if something fails:**
- Any **A** fails → the *Source Discretion* block isn't being read; check it's in SKILL.md identity section and reinstall.
- Any **B** fails → the routing rows aren't firing; confirm the four `references/*-quantified.md` / toolkit rows are in *When to Read Reference Files*.
- **B7/B8** fail → confirm the `guesstimate-drill-bank.md` and `product-rca-casebank.md` rows are under *Casebook Drills & PM/Analyst Prep*.
