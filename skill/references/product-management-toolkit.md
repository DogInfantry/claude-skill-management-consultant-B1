# Product Management Toolkit — Teardowns, Frameworks, Interview Patterns

Operational toolkit for product cases and PM interview prep: an 8-step teardown method, the high-frequency PM frameworks as compact instructional entries, and the recurring interview-round patterns. Use alongside `product-thinking-digital.md` and `case-interview.md`.

---

## Part A — Product Teardown (8 steps)

A teardown is an analytical dissection of a product — *what it does, for whom, where it falls short, and what you'd change*. Run it in order; the skill being tested is **prioritisation**, not exhaustive listing.

1. **Set context & goals.** State the teardown's purpose and the metric it serves: revenue, engagement, retention, or user growth. Everything downstream aligns to this.
2. **Define scope.** Narrow to one level — feature (e.g. search), workflow (e.g. checkout end-to-end), or design (UI/UX, accessibility, hierarchy). Don't try to cover all three.
3. **Identify the users.** Break the audience into specific personas (e.g. a marketplace has buyers and sellers). For each: frustrations, motivations, context, use cases.
4. **Find the gaps & problems** *(the most important step)*. Build a user journey and find where the product's offering diverges from real user needs. Tools: **JTBD** (what is the user hiring this to do?) and **5 Whys** (symptom → root cause). Analyse four layers: functionality, usability, technical, business alignment.
5. **Prioritise.** Pick the 2–3 problems that matter most, aligned to the Step-1 goal. *Listing ten problems with no ranking is a red flag.*
6. **Solutions.** Generate multiple options per problem; weigh with **Impact vs Effort**. Impact must map to the Step-1 goal; if effort is high, scope it down to an experiment or MVP.
7. **Success metrics.** Define four types: **North Star** (main goal movement), **Awareness** (discovery check), **Adoption** (usability check), **Guardrail** (what must not get worse).
8. **Summarise.** One slide / one screen: the solution, how you got there, why it's better. Compression itself signals PM maturity.

---

## Part B — PM Frameworks (when to reach for each)

- **JTBD (Jobs To Be Done):** frame what users are really "hiring" the product to accomplish; use to find the underlying need behind a feature request.
- **CIRCLES (product design):** Comprehend situation → Identify customer → Report needs → Cut/prioritise → List solutions → Evaluate trade-offs → Summarise. The default scaffold for "design a product for X."
- **North Star Metric:** the single measure of delivered customer value that the whole team optimises. Pick one; everything else is an input or guardrail.
- **OKRs:** Objective (qualitative goal) + 3–5 measurable Key Results. Use for goal-setting and alignment, not task tracking.
- **Kano model:** classify features as Basic (expected), Performance (more = better), or Delighters. Use to decide what wins and what merely prevents dissatisfaction.
- **MoSCoW prioritisation:** Must / Should / Could / Won't. Fast scoping for a release.
- **RICE prioritisation:** score = (Reach × Impact × Confidence) / Effort. Use to rank a backlog quantitatively.
- **Product Life Cycle:** Introduction → Growth → Maturity → Decline; the stage dictates the strategy (acquire vs monetise vs defend vs harvest).
- **Hook model:** Trigger → Action → Variable Reward → Investment. Use to diagnose or design habit-forming engagement.
- **HEART:** Happiness, Engagement, Adoption, Retention, Task success — a UX metrics framework; pair each with a Goal-Signal-Metric.
- **AARRR (pirate metrics):** Acquisition, Activation, Retention, Referral, Revenue — the funnel for growth diagnosis; find the leakiest stage first.
- **Ansoff matrix:** Market Penetration / Product Development / Market Development / Diversification — growth-direction choices by new-vs-existing product and market.

**Choosing fast:** design prompt → CIRCLES; improve-a-metric → AARRR or HEART to locate the stage, then RICE to rank fixes; prioritise a backlog → RICE or MoSCoW; engagement problem → Hook + JTBD.

---

## Part C — Interview Round Patterns (what real processes look like)

Distilled, generic structure of non-tech / PM / analyst hiring rounds (company-agnostic):

- **Round 1 — Online aptitude / screening:** logical reasoning, quantitative aptitude, problem-solving; sometimes light data-science or coding (regression/classification) for analyst roles; occasionally a deck-submission on a given problem statement.
- **Round 2 — Offline interview (technical + CV/analytical):**
  - **CV deep-dive:** internships, projects, positions of responsibility — always tied to *measurable impact created*.
  - **RCA / guesstimate:** a root-cause or market-sizing question (use the guesstimate discipline file).
  - **Puzzles:** classic probability/logic puzzles (e.g. the coin-flip "split into two groups with equal tails," "golf balls in a bus").
  - **SQL:** common ask — list the join types and reason about which produces the most/fewest rows (often pen-and-paper).
  - **Product/analytical:** a metric-definition or product-improvement prompt.
- **Later rounds:** product/business case, behavioural (leadership, conflict, ownership), and sometimes a VP/leadership round on long-term vision.

**Prep implications:** measurable-impact CV bullets; fluency in guesstimates + RCA; a handful of standard puzzles; SQL joins cold; one clean product-improvement framework (CIRCLES) ready to deploy.

---

## Part D — Extensions: case types, metric hierarchy, lifecycle metrics, roadmaps

**The PM case universe (know which one you're in).**

| Type | Typical prompt | Worked examples |
|---|---|---|
| Design | "Design X for Y" | `product-sense-casebank.md` |
| Favourite product | "What's your favourite product and why?" | `product-sense-casebank.md` |
| Go-to-market | "How would you launch X to Y?" | `product-sense-casebank.md` |
| Market entry | "Should X enter Y?" | `product-sense-casebank.md` |
| Pricing | "How would you price X?" | `pricing-strategy.md` |
| Metric definition | "How would you measure X?" | `product-sense-casebank.md` |
| Metric drop / RCA | "DAU fell X% in 2 weeks" | `product-rca-casebank.md` |
| Technical | "How does the internet work?" / "Design a photo-sharing app" | — |
| Market trend | "What's the next big bet?" | — |
| Guesstimate | "Estimate the market for X" | `guesstimate-drill-bank.md` |

**Good metrics are the 3 A's:** *actionable* (they change a decision), *accessible* (the team can see and understand them) and *auditable* (the definition and data can be checked).

**The metric hierarchy.**
- **Focus metric (North Star).** One number tied to the business goal, e.g. weekly active users who complete the core action.
- **Level-1 drivers** move it directly, e.g. 7-day retention.
- **Level-2 diagnostics** explain the L1 drivers, e.g. session length or onboarding completion.
- Diagnose top-down; improve bottom-up.

**Metric families.**
- **Reach:** users touched in the period.
- **Activation:** time to first value.
- **Active usage:** DAU/WAU.
- **Engagement:** depth per session.
- **Retention:** D30 or cohort curves.

**Metrics by lifecycle stage.** The stage decides which number matters.

| Stage | Strategic intent | Metrics that matter |
|---|---|---|
| Introduction | Prove value | Activation rate, time to first value, early retention (D7), qualitative feedback |
| Growth | Acquire efficiently | Acquisition by channel, CAC, referral rate, retention cohorts, LTV/CAC |
| Maturity | Monetise and defend share | ARPU, margin, churn, NPS, share vs. rivals, price realisation |
| Decline | Harvest or reinvent | Contribution margin, cost-to-serve, migration to the successor product |

**Kano, complete.** The model has five categories:
- Must-be (basic)
- Performance
- Excitement (delighter)
- Indifferent: users don't care, so cut it.
- Reverse: some users actively dislike it, so make it optional.

Delighters **decay into must-haves** over time, so re-survey periodically.

**MoSCoW trade-offs.**
- *Strengths:* simple, controls scope creep, aligns stakeholders.
- *Weaknesses:* category boundaries blur, "Must" inflates under pressure, and it is rigid for continuous delivery. Re-prioritise every cycle or pair it with RICE.

**Scrum in one line ("3-3-5-5").**
- 3 roles: product owner, scrum master, developers.
- 3 artifacts: product backlog, sprint backlog, increment.
- 5 events: sprint, planning, daily scrum, review, retrospective.
- 5 values: commitment, courage, focus, openness, respect.

See `product-thinking-digital.md` for delivery at programme scale.

**Glossary deltas.**
- **MVP:** the smallest release that maximises *validated learning* per unit of effort.
- **A/B test:** a controlled comparison of variants on real behaviour. For the statistics, see `stats-and-capital-budgeting-primer.md`.
- **Go-to-market is product-led or sales-led.**
  - *Product-led:* the product itself acquires, converts and expands users (freemium, self-serve).
  - *Sales-led:* marketing generates leads and sales converts them (typical of enterprise and B2B).

**Roadmapping in three components.**
1. **Research:** user problems, market and competition, available funding and capacity.
2. **Strategic planning:** a priority hierarchy (themes → epics → features), the MVP cut, a resourced development plan.
3. **Organisational coordination:** align sales, support, services and marketing on the go-to-market.

A roadmap communicates **vision and sequence**, not a delivery-date contract. Keep near-term items specific and far-term items thematic.

---

## Usage rules for Claude
1. When running a teardown, **force prioritisation** (Steps 5–6) — penalise unranked problem dumps.
2. Match the framework to the prompt type; don't apply more than one scaffold at once.
3. For interview prep, coach the *pattern* (round → question type → what's being tested), not memorised answers.
