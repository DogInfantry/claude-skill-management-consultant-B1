# Product Management Cases — Frameworks, Teardowns & Interview Flows

Companion to `references/product-management-toolkit.md`, focused on the **product interview** and **product-sense** conversation, with framework diagrams you can reproduce and worked case flows drawn from Indian digital products. Use when running or coaching a PM/APM interview, doing a product teardown, answering a design or root-cause prompt, or bringing product thinking into a strategy engagement.

The four canonical PM prompt types and the tool each rewards:

```
  PROMPT TYPE            "Sounds like…"                        Reach for
  ------------------     ----------------------------------    -----------------------
  Product design         "Design X for segment Y"              CIRCLES
  Improvement            "Improve metric/experience of X"      user-journey + RICE
  Root cause             "Metric M dropped Z% — why?"          root-cause tree
  Estimation             "How many / how big is X"             segment-tree guesstimate
  Strategy               "Should X do Y / enter Z"             market entry / growth tree
```

---

## Design prompts — CIRCLES

The workhorse for "design a product/feature for a user." It keeps you user-first and stops you jumping to solutions.

```
C  Comprehend the situation   → clarify goal, platform, constraints
I  Identify the customer       → pick 1–2 segments (persona + context)
R  Report customer needs       → jobs-to-be-done, pain points per segment
C  Cut through prioritization  → pick the needs that matter most (impact × reach)
L  List solutions              → 3+ ideas per prioritized need
E  Evaluate trade-offs         → effort vs. impact vs. risk
S  Summarize the recommendation→ what to build, why, and the success metric
```

**Delivery tip:** spend real time on *Identify* and *Report*. Weak candidates design for "everyone"; strong ones pick a segment, articulate its job-to-be-done, then design. Always close with the **metric you'd watch** — design without a success metric is incomplete.

*Worked pattern — "Design [a food-delivery app] for senior citizens."* Comprehend (goal = accessibility + independence, mobile); Identify (tech-hesitant seniors living alone vs. with family); Report needs (large-type/voice UI, trust, help placing orders, dietary needs, human fallback); Cut (trust + ease-of-ordering dominate); List (voice ordering, one-tap "usual," assisted ordering via a support agent or family-linked account, curated senior-friendly/health menus); Evaluate (assisted-ordering = high impact, moderate effort); Summarize (ship voice + assisted ordering; metric = repeat order rate among the 60+ cohort). Rewrite the segment and you have any "design X for Y" answer.

## Improvement prompts — journey + prioritization

"Improve X's experience / reviews / retention." Don't brainstorm features — **map the user journey**, find where value leaks, then prioritize fixes.

```
  Awareness → Acquisition → Onboarding → Core use → Retention → Advocacy
      │            │             │            │           │          │
      └── at each stage: what's the friction? what metric proves it? ──┘
                          then RICE the fixes
```

**RICE** to choose what to build: **R**each × **I**mpact × **C**onfidence ÷ **E**ffort. It converts opinion into a rankable score and is the fastest way to defend "why this first."

*Worked pattern — "Improve [a marketplace's] product reviews."* First clarify the goal (more reviews? more *trustworthy* reviews? higher conversion from reviews?). Establish what reviews are *for* (reduce purchase risk → conversion) and the current layout. Diagnose leaks (low review volume, low helpfulness, fake-review distrust). Solutions: incentivize reviews (store credit/points), structured prompts (rate specific attributes: fit, quality), verified-purchase badges, surface most-helpful reviews first, photo/video reviews. RICE them; recommend the highest-scoring one with a success metric (reviews-per-order, review-influenced conversion).

## Root-cause prompts — the diagnostic tree

"Engagement dropped 10%." Resist listing causes. Build a **MECE root-cause tree**, then ask which branch the data implicates.

```
                 Metric drop (e.g. −10% engagement)
                          │
        ┌─────────────────┼──────────────────┐
     INTERNAL          EXTERNAL            MEASUREMENT
   (our change)      (market/seasonal)    (is it real?)
        │                 │                    │
  ┌─────┴─────┐      ┌─────┴─────┐        tracking bug?
 product   pricing  competitor  seasonality  definition change?
 change    /policy   launch      /holiday
        │
  which segment / platform / geography / cohort?
        │
  when did it start? (correlate to a release date)
```

**The three first moves:** (1) *Is it real?* — rule out a tracking/definition change. (2) *Segment it* — is the drop uniform or concentrated (a platform, region, cohort, or funnel step)? (3) *When did it start?* — correlate the inflection to a release, price change, or external event. Isolating *where* and *when* usually reveals *why*. Then quantify and recommend.

## Product metrics — HEART & the North Star

To judge "is this feature working," define metrics before you build. **HEART** structures UX metrics; for each dimension set Goals → Signals → Metrics.

```
  H  Happiness    satisfaction, NPS, ratings
  E  Engagement   frequency, depth, DAU/MAU
  A  Adoption     new users taking up the feature
  R  Retention    users who come back (D1/D7/D30)
  T  Task success completion rate, time-to-complete, error rate

  For each:  GOAL (what good looks like) → SIGNAL (observable behavior) → METRIC (the number)
```

Pair this with the **AARRR pirate funnel** (Acquisition, Activation, Retention, Revenue, Referral) for growth diagnostics, and always name **one North Star metric** that captures delivered user value (e.g., successful orders, minutes of content watched) rather than a vanity count.

## Product teardown skeleton

A teardown shows product sense. Same skeleton for any app:

```
1. What is it & who's it for   (mission, target user, JTBD)
2. Business model              (how it makes money; unit economics)
3. Core user journey           (the 3–5 steps that deliver value)
4. What's great / what's weak  (2–3 each, with the "why")
5. Competitive position        (substitutes, moat, network effects)
6. What you'd build next       (1–2 prioritized bets + success metric)
```

**India digital-product angles worth holding** (as reasoning references, not scripts):
- **Food delivery (Zomato / Swiggy).** Two-sided marketplace (eaters ↔ restaurants ↔ riders); economics turn on order density, AOV, delivery cost per order, and take rate; expansion into quick-commerce (Blinkit/Instamart) and dining/loyalty. Teardown tension: growth vs. contribution margin.
- **E-commerce (Flipkart / Meesho).** Buyer-seller marketplace; levers are selection, trust (reviews/returns), and logistics cost; Meesho's wedge is zero-commission + social/reseller distribution into price-sensitive tiers.
- **Investing (Groww / Zerodha).** Low-cost broking + mutual funds for first-time retail investors; growth via UX simplicity and trust; monetization via broking, margin, and distribution. Teardown tension: engagement vs. investor protection.
- **Ride-hailing (Uber / Ola / Rapido).** Marketplace liquidity, surge pricing, driver supply economics; Rapido's bike-taxi wedge on affordability and congestion.
- **Payments/credit (Paytm / PhonePe / CRED).** UPI's zero-MDR reshaped payment economics; the real business is the cross-sell to lending, insurance, and commerce on top of a payments funnel.

## PM interview round patterns

- **Structure the same way you'd run a case:** clarify → pick a framework out loud → segment → prioritize → recommend with a metric. Interviewers reward visible structure over clever features.
- **Clarify before diving.** Confirm goal, platform, and target user. "Improve X" is ambiguous until you know *for whom* and *toward what metric.*
- **Always land a metric.** Every design or improvement answer ends with how you'd measure success. This single habit separates strong candidates.
- **Trade-offs, out loud.** Name what you're *not* doing and why (effort, risk, focus). Product judgment is shown in the cuts, not the list.
- **Engineering-undergrad depth is welcome.** Technical feasibility ("moderate if it integrates with maps/UPI") strengthens the answer — bring it where relevant without drowning the product logic.

For the underlying toolkit (JTBD, CIRCLES long-form, RICE/HEART/AARRR mechanics, SQL for PM questions) see `references/product-management-toolkit.md` and `references/sql-for-pm-analysts.md`. For estimation prompts, see `references/india-guesstimates-and-cases.md`.
