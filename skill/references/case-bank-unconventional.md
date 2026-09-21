# Case Bank — Unconventional Cases (People, Operations, Technology, Social)

A drill bank for the cases that do **not** fit a profitability, market-entry, pricing or M&A template: hiring and attrition, plant capacity with every obvious lever banned, IT integration of an acquired site, digitisation on a fixed budget, an AI service business case, location choice, a subscription break-even, and public or social outcomes. Same compact format as `case-bank-worked.md` (**Setup / Structure / Spine / Aha / Trap**), plus an **Error fixed** callout wherever a common calculation or logic slip needs correcting, and a **Pairs with** line pointing to the deeper reference.

## What makes a case "unconventional", and why candidates fail it

An unconventional case is one where the question is about an **outcome other than profit** (joiners, uptime, retention, girls in school) or where the client **rules out the standard levers** ("no capex, no automation, no extra headcount"). Candidates fail these cases for three predictable reasons:

1. **No framework to lean on.** With no memorised tree to fall back on, they produce an unranked list of ideas ("hackathons, better pay, faster interviews...") with no numbers attached.
2. **They never define the outcome metric.** "Improve retention" stays vague, so the gap cannot be sized and the levers cannot be ranked.
3. **They quote a gross number as the answer.** Savings before bot costs, capacity before the bottleneck, beneficiaries before the counterfactual.

## The universal move (use it on every drill below)

1. **Define the outcome metric** precisely: numerator, denominator, period, segment (e.g., annualised leavers ÷ average headcount, L1–L2 engineers only).
2. **Build the funnel or flow** that produces the outcome (applicants → offers → joins; planned hours → running hours → good batches; queries → handled → contained → capacity released; Grade 5 → Grade 6 transition).
3. **Quantify the gap** at each stage against a benchmark or the client's own history, and find the stage where most of the loss sits.
4. **Prioritise levers** by value per rupee (or per bottleneck hour, or per additional outcome), not by how interesting they sound.
5. **Name the guardrails**: the metric that must not get worse while you push the main one (hire quality, safety, wrong-answer rate, learning levels).

| Case family | Outcome metric | Flow to build | Guardrail |
|---|---|---|---|
| Hiring conversion | Joiners per offer; days from offer to join | Applicants → interviews → offers → accepts → joins | 90-day retention, first-year performance of hires |
| Attrition | Annualised leavers ÷ average headcount, by level | Hire → tenure cohort → exit (by reason) | Cost per leaver vs cost of the fix |
| No-capex capacity | Good output per year at the bottleneck | Planned hours × A × P × Q ÷ ideal cycle | Safety, product quality |
| Acquired-site IT/OT | Day-1 continuity; TSA exit date | Inventory → stabilise → secure → integrate | Downtime hours, cyber incidents |
| Digitisation on a budget | Annual benefit per rupee invested | Value pool → initiative → adoption | Adoption and usage KPIs |
| AI service channel | Net cost per resolved query | Queries → handled → contained → capacity released | Wrong-answer, complaint and repeat-contact rates |
| Location choice | Weighted score, robust to weight changes | Criteria → weights → scores → sensitivity | Attrition, ramp-up time, data risk |
| Subscription break-even | Starting subscribers needed | Base × net price × growth, less churn and running cost | Churn, acquisition cost |
| Social outcome | Additional outcomes per rupee | Cohort flow → transition points → counterfactual | Equity across groups, learning levels |

**How to use as an interviewer/coach:** give only the setup. Reward the candidate who asks for the outcome metric and its baseline before structuring. Release the funnel numbers only when they ask for the right stage. Push for the number in the **Spine**, ask "so what?" after each figure, and coach the **Trap**. Score with the rubric in `case-facilitation-and-scoring.md`. All figures tagged **[ILLUSTRATIVE]** are for practice; swap in the client's data.

---

## Part A — People & Talent

### U1. Hiring funnel — offers made, joiners missing
**Setup.** A fast-growing technology company gets strong applications and good interview results for backend-developer roles, but hiring "conversion has declined": many candidates who receive offers never join. Facts released on request: pay is slightly below large tech firms and well-funded start-ups; five interview rounds with a 3–4 week cycle; 6–8 weeks from offer to joining; strong enterprise brand but low visibility among developers; candidates hold multiple offers.
**Structure.** First split "not joining" into its **two separate failures**: (1) **declines** (the candidate says no to the offer) and (2) **back-outs** (the candidate accepts, then does not turn up). Then walk the funnel stage by stage: sourcing → interview process → offer (pay, speed) → offer-to-join gap. Treat employer brand and candidate experience as **cross-cutting drivers** that act on several stages, not as a separate stage. Ask **what changed** when conversion started falling (a rival's pay reset, an added interview round, a longer notice period in the target talent pool).
**Spine.**
```
Funnel [ILLUSTRATIVE]: 1,000 applicants → 150 interviewed → 40 offers → 22 accepted → 16 joined
  Offer acceptance = 22 / 40 = 55%     (declines: 18 = 45% of offers)
  Join ratio       = 16 / 22 = 73%     (back-outs: 6 = 27% of accepts)
  Offer-to-join    = 16 / 40 = 40% ;  end-to-end = 16 / 1,000 = 1.6%
  Benchmark: offer acceptance >90%; target here 85% acceptance × 90% join = 76.5%

Scale to a plan of 200 joiners/yr:
  Offers needed now    = 200 / 0.40  = 500  → 1,875 interviewed (3.75 interviewed per offer)
  Offers at target     = 200 / 0.765 ≈ 261  → ~980 interviewed
  Interviewees saved   ≈ 895 × 10 engineer-hours (5 rounds × 2 panellists × 1 h) ≈ 8,950 h ≈ 5 FTE-years

Cost of vacancy [ILLUSTRATIVE]: CTC ₹24 lakh; value of a developer ≈ 2× CTC
  Per working day      = 2 × ₹24 lakh / 240 = ₹20,000
  Each back-out        ≈ 40 extra vacant working days = ₹8 lakh
  Back-outs now        = 500 × 55% − 200 = 75 → 75 × ₹8 lakh = ₹6.0 crore/yr
  Back-outs at target  = 261 × 85% − 200 ≈ 22 → ≈ ₹1.8 crore/yr  (≈ ₹4.2 crore/yr recovered)

Notice-period buy-out: pay 1 month (₹2 lakh) to cut the join gap by 30 days (~21 working days)
  Vacancy avoided = 21 × ₹20,000 = ₹4.2 lakh → 2.1× return before counting fewer back-outs
Speed: 5 rounds × ~4 working days each ≈ 4 weeks; 3 rounds in one interview day + a 48-hour decision ≈ 1 week
```
**Aha.** The two failures have **different causes and different fixes**. Slow decisions (a four-week cycle against rivals who decide in a week) and the pay gap drive **declines**; the long offer-to-join gap drives **back-outs** to counter-offers. So the priority fixes are speed of decision and a shorter, actively managed join gap (buy-outs, pre-joining engagement, a named buddy), with pay benchmarking for the roles where the gap is real. The leaky funnel also burns **about five engineers' worth of interview time a year**, which is a cost the business feels directly.
**Trap.** Assuming pay is the only lever; working without funnel numbers; cutting rounds from five to three **without protecting hire quality**. Merge rounds rather than delete assessment content, use structured scorecards, and track 90-day retention and first-year performance of hires before and after the change. Also: recommending fixes before collecting decline and back-out reasons (a short survey of every decliner).
**Error fixed:** reading 16 joiners ÷ 40 offers = 40% as the "offer acceptance rate" → acceptance is 22 ÷ 40 = 55% and the join ratio is 16 ÷ 22 = 73% (one blended number hides two failures that need different fixes).
**Pairs with:** `functional-deep-dives.md` (Talent Acquisition Diagnostics benchmarks), `case-bank-interview-classics.md` (#12 heavy attrition), `genai-enterprise-strategy.md` (AI-assisted scheduling to cut time-to-hire).

### U2. Remote-plant engineer attrition — the business case for fixing it
**Setup.** A B2B chemical manufacturer has had about 50% annual attrition among L1–L2 engineers (the two junior levels of a seven-level ladder) for three years; peers do not have the problem. L1–L2 staff work rotating shifts. The plant is ~35 km from a large western-Indian metro; the nearest residential area is ~20 km away. The company offers no transport or housing; some smaller nearby employers do, and some leavers join them. Other benefits are at industry norms.
**Structure.** Pin the metric first (annualised leavers ÷ average headcount, L1–L2 only). Then segment: **who** leaves (level, shift pattern, tenure, commute distance, hired-from location), **where to** (exit destinations), **why** (exit-interview Pareto). Test pull factors (rival amenities, pay), push factors (commute, shifts, manager, career path) and **what changed three years ago**. Close with a **business case**: cost of attrition vs cost of the fix.
**Spine.**
```
Headcount L1–L2 [ILLUSTRATIVE] = 120 ; attrition 50% → 60 leavers/yr ; peer benchmark 15% → 18
Excess leavers           = 42
Cost per leaver          ≈ 100% of a ₹7 lakh CTC = ₹7 lakh  (typical range 50–200% of salary:
                           recruiting + training + months of ramp-up + overtime cover)
Attrition cost           = 60 × ₹7 lakh = ₹4.2 crore/yr   (excess vs peers: 42 × ₹7 lakh = ₹2.94 crore/yr)

Fix [ILLUSTRATIVE]:
  Shuttle: 4 contracted buses × ₹1.5 lakh/month × 12       = ₹72 lakh/yr  (routes timed to all 3 shift changes)
  Housing: 60 leased rooms near the plant × ₹8,000/month × 12 = ₹57.6 lakh/yr
  Total                                                    = ₹1.30 crore/yr
Break-even: ₹1.296 crore / ₹7 lakh = 18.5 leavers avoided → attrition must fall from 50% to ~35%
If attrition falls to 25% (30 leavers): saving ₹2.1 crore − ₹1.3 crore = ~₹0.8 crore/yr net (1.6× the spend)
```
**Aha.** Attrition concentrated in **shift-working junior staff at a remote site**, while nearby employers offer transport, points to a **commute and amenity gap**: a cheap, fixable basic need, not a pay or career-path problem. The business case closes the argument: the fix only needs to cut attrition by about 15 points to pay for itself.
**Trap.** Assuming pay is the cause; accepting one hypothesis without exit-interview or attrition-by-distance data; recommending shuttles and housing without costing them against the attrition bill. Longer-term levers (hiring from local colleges and vocational institutes, shift-roster redesign, a satellite unit nearer the talent pool) should be ranked by the same cost-per-leaver-avoided logic.
**Error fixed:** "the plant is remote and has no transport, so that explains three years of high attrition" → a condition that has not changed cannot, on its own, explain a problem that started three years ago; find the trigger (a rival adding shuttles, a new rotating-shift roster, a closed hostel, a shift to hiring from the metro) and treat remoteness as the amplifier.
**Pairs with:** `functional-deep-dives.md` (Talent Retention & Engagement: attrition cost 50–200% of salary), `case-bank-interview-classics.md` (#12 heavy attrition), `industrial-manufacturing.md` (shift-based plant operations).

---

## Part B — Operations & Technology

### U3. No-capex debottleneck — more batches from the same plant (OEE)
**Setup.** A batch-process manufacturer is at full capacity and demand keeps rising. The client rules out a new plant, automation and extra headcount. How do you meet more demand with the existing assets?
**Structure.** Capacity = number of units of equipment × effective output per unit. With equipment fixed, work on output per unit, **at the bottleneck only**: find the step with the lowest good batches per year, then decompose its losses with **OEE = Availability × Performance × Quality**. Availability = running time ÷ planned time (breakdowns, unplanned stops). Performance = ideal cycle ÷ actual cycle (slow running, long cycles). Quality = good batches ÷ total batches (off-spec, rework). Then add **commercial levers** the constraints do not ban: product mix by contribution per bottleneck hour, toll manufacturing, building stock in the low season, a shorter annual shutdown.
**Spine.**
```
Bottleneck = the reactor (every other step has ≥20% slack) [ILLUSTRATIVE]
  Planned time   = 8,760 h − 760 h annual shutdown = 8,000 h
  Availability   = 0.85  → running time 6,800 h
  Performance    = ideal 16 h ÷ actual 20 h cycle = 0.80
  Quality        = 0.95
  OEE            = 0.85 × 0.80 × 0.95 = 64.6%
  Good batches   = 6,800 h ÷ 20 h × 0.95 = 323      (check: 323 × 16 h ÷ 8,000 h = 64.6%)

Batches = available hours ÷ cycle time; output uplift = new OEE ÷ old OEE − 1
Levers:
  Cycle 20 → 17.8 h: SMED on inter-batch cleaning (3.0 → 1.5 h: pre-staged kits, parallel tasks)
                     + preheated feed (heat-up −0.7 h)          → P ≈ 16/17.8 = 0.90 → +12.4%
  Availability 0.85 → 0.90 (preventive maintenance on pumps/agitator)  → +5.9%
  Quality 0.95 → 0.97 (tighter charging tolerances, error-proofing)    → +2.1%
  Combined OEE = 0.90 × 0.90 × 0.97 = 78.5% → 78.5 / 64.6 − 1 = +21.5%
  Good batches = 8,000 × 0.90 ÷ 17.8 × 0.97 ≈ 392 → +69 batches/yr
Value: 69 batches × 10 t × ₹40,000 contribution/t ≈ ₹2.8 crore/yr, with no capex

Mix at the bottleneck: SKU X (10 t, 20 h, ₹40,000/t) = ₹20,000 per reactor-hour
                       SKU Y (10 t, 30 h, ₹50,000/t) = ₹16,700 per reactor-hour → favour X
```
**Aha.** With capex, automation and headcount all blocked, the only source of capacity is **lost time at the binding constraint**. In batch plants the reaction time is usually fixed by chemistry, so attack the **non-reaction time** (charging, heat-up, discharge, cleaning, waiting) and unplanned stops at the bottleneck. An hour saved at any other step adds nothing. Rank products by **contribution per bottleneck hour**, not per tonne.
**Trap.** Improving steps that are not the bottleneck; muddling the OEE components (batch cycle time is a **performance** loss under this convention; error-proofing is a **quality** lever); counting the same lost hour twice (decide once whether inter-batch cleaning sits inside the cycle or in downtime); listing automation or extra manpower when the prompt excluded them; forgetting that "no extra manpower" still allows roster changes and a shorter shutdown.
**Error fixed:** "cutting the cycle 20% (20 → 16 h) lifts output 20%" → output scales with 1 ÷ cycle time, so 6,800 h ÷ 16 h = 425 vs 340 batches, **+25%**; likewise, raising Performance from 80% to 90% is +12.5% output, not +10% (0.90 ÷ 0.80 − 1).
**Pairs with:** `industrial-manufacturing.md` (OEE, SMED, Theory of Constraints, TPM), `practice-cases-quantified.md` (Case 6, capacity expansion), `quantitative-toolkit.md` (sensitivity).

### U4. Acquired-plant IT/OT integration
**Setup.** A food-and-beverage manufacturer is buying a single manufacturing plant from another company. From an IT perspective, how do you make the acquisition smooth?
**Structure.** Two cuts, used together. **Timing:** pre-close (diligence and Day-1 plan) → Day 1 → Day 100 → Year 1. **Layer:** office **IT** (ERP, email, identity, network, finance) vs plant-floor **OT** (PLCs, SCADA, MES, historians, quality/lab systems, lot traceability). Sequence the work as **stabilise → secure → integrate**.
- *Pre-close:* inventory every system with a retain / migrate / retire decision; confirm which services the seller will keep providing under a **transition services agreement (TSA)**, at what price and with what exit criteria; run a cyber assessment (patch levels, remote-access vendors, flat networks); find out whether the plant has its own IT staff at all.
- *Day 1:* the plant runs, people can log in, orders and invoices flow, and **recall and traceability work** (a food-safety must).
- *Day 100:* segment the plant network from corporate IT before connecting them; single sign-on; plan the ERP/MES cutover.
- *Year 1:* cut over in a planned shutdown with a parallel run; exit the TSA; retire duplicate applications; settle people decisions.
**Spine.**
```
Downtime is the dominant risk [ILLUSTRATIVE]:
  Plant revenue ₹600 crore/yr over 8,000 h = ₹7.5 lakh/h ; contribution 30% = ₹2.25 lakh/h
  A botched 72-h cutover = 72 × ₹2.25 lakh = ₹1.62 crore contribution lost (plus spoiled stock)
TSA dependency:
  Seller runs ERP + network at ₹40 lakh/month → 12 months = ₹4.8 crore
  Exit 3 months early saves ₹1.2 crore; a 6-month extension at a 20% step-up costs ₹2.88 crore
People (redundancy math):
  Site IT staff 18 = 8 plant-floor OT (site-specific, keep) + 10 office IT
  Office IT after consolidation: 4 → 6 roles redundant
  Run-rate saving 6 × ₹12 lakh = ₹72 lakh/yr ; one-time severance 6 × ₹6 lakh = ₹36 lakh → payback 6 months
Licences: 5 duplicated applications × ₹20 lakh = ₹1 crore/yr
Perspective: one 72-h outage (₹1.62 crore) wipes out 2.25 years of the IT headcount saving
```
**Aha.** For a single-plant purchase, the critical path is **keeping the line running and traceable on Day 1**, not merging IT teams. The value sits in avoided downtime, an early TSA exit and retired licences; the IT headcount saving is small, and the plant-floor OT engineers are **not** redundant, because their knowledge of that site's control systems is what keeps it running.
**Trap.** A generic IT checklist with no sequencing, budget or Day-1 priorities; connecting the acquired plant network straight to corporate IT on Day 1 (a flat network lets ransomware jump between them); assuming the plant comes with its own IT team; cutting local OT staff to hit a synergy number; benchmarking "software performance against competitors", which is not an integration test.
**Error fixed:** booking the ₹72 lakh/yr redundancy saving as the year-1 benefit → net of ₹36 lakh one-time severance, year-1 benefit is at most ₹36 lakh, and only if exits happen on Day 1 (in practice they follow the TSA exit, so less).
**Pairs with:** `post-merger-integration.md` (IT Integration; Day 1 Readiness; Carve-Outs and Transition Services Agreements), `industrial-manufacturing.md` (SCADA, MES, and ERP Integration), `functional-deep-dives.md` (IT Strategy & Transformation).

### U5. Outbound logistics and field-sales digitisation on a fixed budget
**Setup.** An Indian generics manufacturer (OTC products plus prescription drugs in cardiology, neurology and anti-infectives; SKUs priced ₹50–500; exports to South-East Asia and Africa) has automated its plants, but distribution and field sales still run on paper. It will spend about ₹30 crore (~1% of annual revenue) over 24 months on digitising **outbound logistics** and **sales & marketing**. Where should the money go?
**Structure.** Scope to the two functions asked (leave inbound logistics and manufacturing out). Build **value pools** first, then match initiatives to them, then rank by **annual benefit per rupee**, with mandatory compliance funded first.
- *Outbound logistics:* secondary-sales and inventory visibility at distributors and chemists, first-expiry-first-out allocation, near-expiry liquidation, returns processing, track-and-trace/serialised packs (verify current export-market and domestic rules at time of use).
- *Field sales:* sales-force automation for medical representatives: call planning and routing, visit logging, doctor segmentation, prescription-trend analytics.
- *Order-to-cash:* distributor ordering, e-invoicing, collections.
**Spine.**
```
Implied revenue = ₹30 crore / 1% = ₹3,000 crore
Value pools [ILLUSTRATIVE]:
  Expiry + returns write-offs 3% of sales = ₹90 crore/yr ; −1 point = ₹30 crore/yr
  Reps: 2,000 ; prescription sales 70% = ₹2,100 crore → ₹8.75 lakh per rep per month
        SFA lifts prescription sales 3% = ₹63 crore × 40% contribution = ₹25.2 crore/yr
  Order-to-cash: DSO −5 days = ₹3,000 crore / 365 × 5 ≈ ₹41 crore one-time cash release
        → recurring value = carrying cost at 10% ≈ ₹4.1 crore/yr
Budget split (₹ crore): track-and-trace compliance 3 | expiry/returns visibility 10 | SFA 12 | order-to-cash 5 = 30
Benefit per rupee per year: expiry 30/10 = 3.0 | SFA 25.2/12 = 2.1 | order-to-cash 4.1/5 = 0.8 (plus the cash)
Risk-adjusted at 50% realisation: 15 + 12.6 + 2.05 ≈ ₹29.7 crore/yr → ~1-year payback once adopted
Adoption KPIs: % of distributors reporting secondary sales weekly; rep app daily-active %; calls/day; near-expiry stock %
```
**Aha.** With a fixed budget, pick initiatives by **payback**, not by novelty. Cutting expiry and returns by one point of sales is worth about ₹30 crore a year, which alone repays the entire budget; rep productivity is the second pool. Both depend on **adoption** by distributors and reps, so change management belongs inside the budget, not after it.
**Trap.** Listing digital tools with no value case, budget split or phasing; proposing a B2C online-pharmacy channel without flagging **channel conflict** with distributors and chemists and an unsettled regulatory position; a manufacturer-run telemedicine service (conflict-of-interest and drug-promotion concerns); calling hospital supply a "hotel-restaurant-café-style" channel when it is **institutional or tender sales**; over-weighting cold chain for a mostly-tablet portfolio; confusing sales-force automation with demand planning.
**Error fixed:** adding the ₹41 crore DSO release to the annual savings → it is a **one-time** cash release (a stock); the recurring P&L benefit is only its carrying cost, about ₹4 crore a year (a flow).
**Pairs with:** `sales-force-effectiveness.md` (coverage, workload sizing), `functional-deep-dives.md` (Supply Chain Transformation Levers), `problem-playbooks.md` (§7 Digital Transformation), `healthcare-life-sciences.md`.

### U6. AI customer-service chatbot — net savings, not gross
**Setup.** A large retail bank will launch an AI chatbot for balance enquiries, transaction support, loan information and card issues. Goals: better customer experience, lower service cost, more digital engagement. What are the risks, what should be measured, and what will it save? Data on request: 1 million queries a month; ₹50 to service a call; the bot is expected to handle 40%.
**Structure.** Pin the primary objective first (cost, experience or engagement; each changes the success metric). Then three blocks: **(1) risks, prioritised** by likelihood × severity; **(2) a metric tree** (customer experience: CSAT, NPS, resolution, response time; operations: contained share, cost per resolved query, call volume, handle time; AI quality: intent accuracy, wrong-answer rate, escalation and completion rates); **(3) a net business case** with an adoption ramp.
**Spine.**
```
Gross (the tempting answer): 1M × 40% × ₹50 = ₹2 crore/month (₹20M) → ₹24 crore/yr (₹240M)

Net [ILLUSTRATIVE]:
  Handled 400K/month ; truly contained (no human contact within 7 days) 75% = 300K ; escalated 100K
  Saving per contained query = ₹50 human − ₹5 bot = ₹45 → 300K × ₹45 = ₹1.35 crore
  Escalated queries still incur the bot cost: 100K × ₹5 = −₹5 lakh
  Fixed platform (licences, cloud, model/content-ops team) = −₹30 lakh/month
  Net run-rate = ₹1.35 crore − ₹0.05 crore − ₹0.30 crore = ₹1.0 crore/month ≈ ₹12 crore/yr (half of gross)
  Per handled query: net = 1M × h × (0.75 × ₹45 − 0.25 × ₹5) − ₹30 lakh = 1M × h × ₹32.5 − ₹30 lakh
  Break-even handled share = ₹30 lakh / ₹3.25 crore ≈ 9%

Is it cash? ₹50 = 5-min handle time × (₹65,000/month agent cost ÷ 120 productive h) + ~₹5 telephony
  300K × 5 min = 25,000 h/month ≈ 208 agent FTE → savings are real only if ~208 FTE are released
  (attrition without backfill, fewer outsourced seats)

Ramp: handled 10% (months 1–3) → 25% (4–6) → 40% (7–12)
  Monthly net ≈ ₹2.5 lakh → ₹51 lakh → ₹1.0 crore ; year 1 ≈ ₹7.6 crore
  After a ₹5 crore build: year-1 net ≈ ₹2.6 crore ; payback in month 10

Risk heat map (likelihood × severity, 1–5):
  Wrong-but-confident answer on fees, rates, eligibility (hallucination)  4 × 4 = 16
  Prompt injection / jailbreak (bot leaks data or takes an action)         3 × 4 = 12
  Customer trapped, poor handoff to a human                                4 × 3 = 12
  Account data shown to the wrong person (weak authentication)             2 × 5 = 10
  Regulatory: mis-selling, unfair treatment, data residency, outsourcing   2 × 5 = 10
  Legacy integration (stale balances)                                      3 × 3 =  9
  Model drift, vendor lock-in                                              3 × 2 =  6
```
**Aha.** "Handled × cost per call" overstates the value. Real savings = **contained** queries × (human cost − bot cost) − fixed platform cost, and they turn into cash **only if agent capacity is actually released**. Launch in phases: informational intents first, answers grounded only in approved content, step-up authentication before any account-specific answer, no actions without authorisation, and a "talk to a human" route that always works and passes on the conversation.
**Trap.** Counting every bot-touched query as a saving; ignoring escalations, repeat contacts and the semi-fixed contact-centre cost; pricing every query as a voice call when some already arrive by cheaper digital channels; an unranked risk list that omits hallucination and prompt injection. **Guardrail metrics:** repeat-contact rate within 7 days, audited wrong-answer rate on regulated intents, complaints per 10,000 chats, bot vs human CSAT, and zero tolerance for authentication failures. North-star: cost per **resolved** query at equal or better CSAT.
**Error fixed:** "₹24 crore a year saved" (1M × 40% × ₹50 × 12) → that is gross; net of 75% containment, a ₹5 bot cost per query and ₹30 lakh a month of fixed cost, run-rate is ~₹12 crore a year, and year 1 is ~₹7.6 crore before the build cost because adoption ramps (gross counts every touched query as a fully avoided call).
**Pairs with:** `genai-enterprise-strategy.md` (ROI Modeling and Cost Structures; Governance and Risk Architecture; contact-centre benchmarks of 20–35% Tier-1 deflection).

---

## Part C — Location & Business-Model Math

### U7. Offshore delivery-centre location — weighted decision matrix
**Setup.** A multinational technology company will open a 500-person delivery centre (software development, technical support, analytics) and must choose among four hubs: **Hub A** (large South Asian engineering talent pool, lowest cost), **Hub B** (South-East Asian, strong English voice-support base), **Hub C** (Central European nearshore, EU data regime, close time zone to European clients), **Hub D** (emerging South-East Asian engineering base).
**Structure.** Four lenses: **operational feasibility** (talent depth and seniority, infrastructure, scalability, language and time-zone fit), **financial viability** (fully loaded cost, set-up cost, payback), **country risk** (macro and currency stability, attrition and wage inflation, competition for talent from existing capability centres) and **regulation** (foreign-ownership rules, incentives, data-protection and cross-border transfer rules). Turn them into a **weighted matrix**, fill it in, then **test how sensitive the winner is to the weights**. Also consider a tier-2 city inside the chosen country and a pilot before full scale.
**Spine.**
```
Is cost decisive? [ILLUSTRATIVE] Fully loaded cost per FTE, same role mix: onshore $120k | A $30k | C $60k
  Savings vs onshore: A 500 × $90k = $45M/yr ; C 500 × $60k = $30M/yr
  Set-up $5M → payback A ≈ 1.3 months, C = 2 months → every hub clears the bar; the A–C gap is $15M/yr

Weighted matrix (scores 1–5):
  Criterion (weight)              A   B   C   D
  Talent depth & quality (30%)    5   3   4   3
  Fully loaded cost (25%)         5   4   2   5
  Time-zone / language fit (15%)  3   4   5   2
  Country & attrition risk (15%)  3   3   4   3
  Regulation & data (15%)         3   3   5   3
  Weighted score                4.10 3.40 3.80 3.35   → A leads

Sensitivity:
  European-client weights (talent 25, cost 10, fit 25, risk 15, regulation 25):
    A 3.70 | B 3.35 | C 4.30 | D 2.95                  → C wins
  Break-even shift: moving 6 points from cost to time-zone fit (cost 19%, fit 21%) ties A and C at 3.98
```
**Aha.** When every option pays back its set-up cost within months, cost alone cannot pick the winner; **talent depth, attrition, time-zone fit and data risk** decide. And because a six-point change in the weights flips the answer, the weights **are** the recommendation: agree them with the client first. That is also why a two-hub footprint (A for scale, C for European nearshore work) is often the robust answer.
**Trap.** Ranking hubs on salary alone; proposing a decision matrix and never filling in weights and scores; using "lines of code per developer" as a quality proxy (use attrition, defect escape rate, on-time delivery and senior-talent depth instead); scoring incentives from memory, since tax-holiday schemes in several hubs have closed to new units and data-protection regimes keep changing, so verify both at time of use.
**Error fixed:** comparing an entry-level offshore salary ($10k) with an unspecified onshore "$60k+" (500 × $50k = $25M saving, 2.4-month payback) → compare **fully loaded cost for the same role mix** (salary, benefits, facilities, management overhead, attrition and transition cost); the like-for-unlike version misstates both the saving and the gap between hubs.
**Pairs with:** `case-bank-worked.md` (E5, weighted objectives), `quantitative-toolkit.md` (§6 sensitivity and scenario modelling), `case-types.md`.

### U8. Subscription break-even with a growing subscriber base
**Setup.** A renowned studio known for immersive role-playing games is building an open-world title on a single $15/month subscription tier. It wants critical acclaim and to recover its costs within three years. Development costs $150M and marketing $30M. Subscribers are expected to grow 20% a year. How many subscribers does it need at launch?
**Structure.** Define success on both axes (acclaim: review scores; commercial: cost recovered within 36 months of launch, so confirm when the clock starts). Build the revenue line: starting base × price × 12 × growth factor per year. Then extend the model the way a real business case would: **platform fee, running costs, churn, time value of money**. Close with the plan that makes the number reachable (a proven lead designer, a launch campaign with beta and creator partnerships, and a live-operations roadmap of monthly patches, quarterly events and annual expansions to hold churn down).
**Spine.**
```
Costs = $150M + $30M = $180M
Flat base:  $180M / 36 months = $5M/month ÷ $15 = 333,333 subscribers

Growing base (20%/yr, base held constant within each year):
  Revenue = S × 12 × $15 × (1 + 1.2 + 1.44) = S × 180 × 3.64 = S × 655.2
  S = $180M / 655.2 = 274,725 at launch (~18% below the flat requirement)
  Check: yr1 $49.45M + yr2 $59.34M + yr3 $71.21M = $180.0M
  General form: S = C / [12 × P × ((1+g)^n − 1)/g] ; ((1.2^3 − 1)/0.2 = 3.64)

Break-even is on contribution, not revenue [ILLUSTRATIVE]:
  30% platform fee → net $10.50        → S = $180M / (12 × 10.5 × 3.64) ≈ 392K
  Servers + support $2/sub/month       → net $8.50 → S ≈ 485K
  Live-ops team $10M/yr (+$30M costs)  → S = $210M / (12 × 8.5 × 3.64) ≈ 566K  (≈ 2× the naive answer)

Churn (5%/month) turns net growth into gross sign-ups:
  Year 1: replace 0.05 × 12 × 274,725 ≈ 164.8K lapsed + add 54.9K net = ~220K gross sign-ups
  → 4 gross sign-ups for every net subscriber added (each one carries an acquisition cost)
Time value (10%, year-end revenue): discount factor 1/1.1 + 1.2/1.21 + 1.44/1.331 = 2.98
  → S = $180M / (180 × 2.98) ≈ 335K (~22% higher)
```
**Aha.** Growth lets the studio start about 18% below the flat requirement, but the honest requirement is set by **contribution**: once the platform fee, running costs and a live-ops team are included, the launch base roughly doubles to ~570K, and churn means every net subscriber costs four sign-ups. Benchmark that number against comparable subscription titles before calling it feasible, and test alternatives (a box price plus subscription, or a platform-subscription deal).
**Trap.** Treating revenue as break-even; ignoring platform fees, running costs, churn and discounting; never asking when the three-year clock starts; tagging the case as manufacturing when it is a media/gaming business model.
**Error fixed:** "S × 654.72 = $180M, so S ≈ 274,725" → 12 × 15 × 3.64 = **655.2**, which gives S = 274,725 (dividing by 654.72 would give ~274,927; the multiplier and the answer must match).
**Pairs with:** `case-bank-worked.md` (B3 break-even, E3 success defined as acclaim plus break-even), `case-cracking-drills.md` (Part E, E6 geometric-series break-even), `quantitative-toolkit.md` (§2 unit economics).

---

## Part D — Social Sector & Public Outcomes

Social and public-sector cases (school dropout, road deaths, hospital crowding, scheme take-up) reward the same universal move, with three tools that differ from commercial cases.

**1. Logic model / theory of change.** Lay out inputs → activities → outputs → outcomes → impact, and **write down the assumptions** linking each step (e.g., "a bicycle removes the distance barrier" assumes distance, not household labour, is the binding reason). Outputs (bicycles delivered) are not outcomes (girls still enrolled in Grade 10).

**2. Cohort-flow math.** Follow 100 entrants through the system and find **where** they leak. Losses usually cluster at **transition points**, where a child must change school, travel further or pass a board exam.
```
Girls' cohort [ILLUSTRATIVE]: 100 enter Grade 1
  Survive to Grade 5          90.0   (loss 10.0)
  Transition 5 → 6 at 85%     76.5   (loss 13.5)
  Survive 6 → 8 at 95%        72.7   (loss  3.8)
  Transition 8 → 9 at 80%     58.1   (loss 14.5)
  Survive 9 → 10 at 90%       52.3   (loss  5.8)
Total loss 47.7; the two transitions account for 28.0 (~59%) → target the transitions first
```
Structure causes MECE: **supply** (a school at the next level within reach, teachers, girls' toilets), **demand** (household cost, household labour, early-marriage norms), **access and safety** (distance, transport, harassment), **learning** (foundational gaps that lead to exam failure and exit). Keep each cause in one branch; "distance" belongs to access, not also to supply.

**3. Cost per additional outcome (not per beneficiary).** Compare interventions on the outcomes they add **over the counterfactual**, and spread durable assets across the cohorts they serve.
```
Bicycles for Grade 9 entrants [ILLUSTRATIVE]: cohort 10,000; transition 80% → 86% = +600 girls
  Cost 8,600 × ₹4,000 = ₹3.44 crore → ₹57,333 per additional girl (93% of recipients would have enrolled anyway)
Girls' toilets in 50 schools: ₹2 lakh each = ₹1 crore; 2,000 girls per cohort; transition +5 pts = +100/yr
  One cohort: ₹1 lakh per additional girl
  Over a 10-year life with ₹10,000/school/yr upkeep: (₹1 crore + ₹50 lakh) / 1,000 = ₹15,000 per additional girl
```
The durable asset wins once it is spread over its life, even though it looks worse on a single cohort. Test either result before scaling with a pilot and a comparison group (randomised roll-out or difference-in-differences).

For a full worked dropout drill, see `references/india-guesstimates-and-cases.md` (Drill Q, girls' school dropout). For programme design, evaluation methods and government delivery constraints, see `references/public-sector-government-defense.md` (Logic Model / Theory of Change; Program Evaluation).

---

## Coaching cross-reference
- **U1 hiring funnel, U2 attrition:** `functional-deep-dives.md` (Talent Acquisition Diagnostics; Talent Retention & Engagement) for benchmarks; `case-bank-interview-classics.md` #12 for a qualitative attrition exemplar. Coach the split between declines and back-outs, and the "what changed?" question.
- **U3 no-capex debottleneck:** `industrial-manufacturing.md` (OEE, SMED, Theory of Constraints, TPM); `practice-cases-quantified.md` Case 6 for the capex version of the same question.
- **U4 IT/OT integration:** `post-merger-integration.md` (IT Integration; Day 1 Readiness; TSAs); `industrial-manufacturing.md` (SCADA, MES, and ERP Integration).
- **U5 digitisation on a budget:** `functional-deep-dives.md` (Supply Chain Transformation Levers; IT Strategy); `sales-force-effectiveness.md`; `problem-playbooks.md` §7.
- **U6 AI chatbot:** `genai-enterprise-strategy.md` (ROI Modeling and Cost Structures; Governance and Risk Architecture; use-case benchmarks).
- **U7 location matrix, U8 subscription break-even:** `case-bank-worked.md` (E5, B3, E3); `quantitative-toolkit.md`; `case-cracking-drills.md` for the math habits (state the approach, then compute, then "so what").
- **Case-type framing:** `case-type-cheat-sheets.md` for the standard case cards these drills deliberately step outside; `case-types.md` for framework selection.
- **Running and scoring any drill here:** `case-facilitation-and-scoring.md` (rubric and common-mistakes catalogue). Watch especially for gross-vs-net answers, unranked lists, and a missing outcome metric.
- Tag any figure you add as **[ILLUSTRATIVE]**, show the math, keep stock and flow apart, and sanity-check magnitude before presenting.
