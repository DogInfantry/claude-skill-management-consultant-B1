# Product Root-Cause Casebank — The Metric-Drop Protocol + 7 Worked Diagnoses

"Metric X dropped Y% — why?" is the most common product/analyst interview prompt and the most common real-world fire drill. This file gives a **repeatable 5-gate protocol** and **seven worked cases**. Each case is chosen to teach a different root-cause archetype: a promotion change, a payment-policy change, a UI plus incentive change, an environmental handover failure, a partner outage, a multi-cause slow decline, and a rights or content loss.

Companion to `references/india-pm-cases.md`, which holds the generic internal/external/measurement tree, and `references/product-management-toolkit.md`, which covers the AARRR/HEART metric frameworks. For experiment readouts after a fix, see `references/stats-and-capital-budgeting-primer.md`.

---

## The 5-gate metric-drop protocol

Run the gates **in order**. Most weak answers jump straight to gate 5 and list twenty causes.

```
  GATE 1  IS IT REAL?          tracking/tagging change? metric definition change? data pipeline lag?
     │                         → "Analytics events verified" is an answer you must ask for, not assume
  GATE 2  DEFINE THE METRIC     write the formula: AOV = GMV ÷ orders; viewership = users × watch-time
     │                         → a ratio can fall because the numerator fell OR the denominator rose
  GATE 3  SEGMENT IT            platform · OS/app version · geography · cohort · user type · category ·
     │                         funnel step · time of day → is the drop uniform or concentrated?
  GATE 4  DATE IT               sudden (hours/days → one event) vs. gradual (quarters → several causes);
     │                         line the inflection up with releases, policy/price changes, external events
  GATE 5  INTERNAL vs EXTERNAL  internal: product/UX change, algorithm, pricing/promo, policy, tech/partner
                                external: competitor, seasonality, regulation, macro, rights/content, infra
                                → ask "is the industry seeing it too?" to split the two in one question
```

**Then walk the funnel.** Walk only the segment that gate 3 isolated. For each step, name the metric that proves the step is healthy.

```
  Discover → Open app → Search/browse → View item → Add to cart → Checkout → Payment success → Fulfilment
  (impr.)    (DAU)      (search→result)  (CTR)       (ATC rate)    (checkout   (success rate by  (pickup/
                                                                   start)      instrument/bank)  delivery)
```

**Close every diagnosis with the same three things.** State the root cause with the evidence chain, the fix (immediate mitigation, then permanent fix), and the **metric plus guardrail** you'll watch to confirm recovery.

**Superficial cause vs. root cause.** If fixing it wouldn't stop the problem recurring, you haven't reached the root. Keep asking "why" until you reach something the team can act on.

---

## Case 1 — Average order value falling on a food-delivery app (promotion change)

**Prompt.** AOV on the food-delivery vertical has fallen sharply over the last week. Find the root cause.

**Gates 1–4.**
- *Real?* Tracking is verified.
- *Define:* AOV = order value ÷ orders.
- *Segment:* the food vertical only, nationwide, where there was a steep drop starting last week.
- *Date:* no algorithm, fee or UI change, and payments are completing normally.

**Gate 5.** No competitor move and no seasonality. Internally, a promotion that had run for three months, **₹50–60 off orders above ₹300**, ended last month once its acquisition target was met.

**Mechanism.** A threshold discount pulls baskets up to the threshold: people add a side or dessert to cross ₹300. Remove it and baskets relax back below ₹300, so **gross AOV falls**. `[ILLUSTRATIVE]` If 40% of orders had been topped up from ~₹250 to ~₹310, removing the incentive cuts AOV by ≈ 0.4 × 60 = ₹24.

**Aha.** Pin down *which* AOV before diagnosing. **Net** AOV (after discount) could actually **rise** when a discount ends. The original interviewer transcript said both "AOV is falling" and "AOV is increasing"; a strong candidate stops and resolves that contradiction first.

**Fix and metrics.**
- Test a cheaper basket-builder instead of a flat discount, such as free delivery above a threshold or a "complete your meal" add-on nudge.
- **Watch:** gross AOV, orders per user and contribution margin per order.
- **Guardrail:** discount cost as a % of GMV.

**Trap.** Recommending the discount be reinstated without checking whether the AOV lift ever paid for its cost.

## Case 2 — Movie-ticket bookings down 70% on a payments super-app (payment-policy change)

**Prompt.** Ticket bookings through the app's movie section fell 70%. Other ticketing platforms are unaffected.

**Diagnosis.**
1. Only our app is affected, so the cause is **internal**.
2. Daily app users are flat, so the drop is not in acquisition.
3. Clicks into the movie section are flat, so discovery is fine.

That localises the drop to **seat selection → payment**. The interviewer then confirms a change to terms and conditions that **removed some payment options** (and added fees), and conversion collapsed at the payment step.

**Aha.** A drop this large and sudden, confined to one app, with an intact top of funnel, is almost always a **single change at a single funnel step**. Walk the funnel with a metric at each step rather than brainstorming external causes such as OTT substitution, outbreaks or weak releases. Those causes would hit every platform.

**Fix.** Restore the high-share payment instruments, or offer a fee-free alternative, for ticketing. Measure payment-step conversion by instrument.

**Trap.** Spending the case on external factors after the interviewer has told you competitors are fine.

## Case 3 — "Hover activity" down 25% on a ride-hailing driver app (UI + incentive change, and is it even bad?)

**Prompt.** Driver in-app idle activity (session time and screens per session while not on a trip) dropped 25% two weeks ago.

**Evidence.**

| What you check | What you learn |
|---|---|
| Tracking | Verified |
| Scope | Driver app only |
| Where the drop is | Concentrated in tier-1 cities |
| Recent changes | A **dashboard redesign** that streamlined navigation shipped three weeks ago; a **streak/referral bonus programme** ended two weeks ago |
| Competitors | No competitor promotions |
| Outcomes | **Trips per driver are slightly up**; churn is unchanged |

**Root cause.** Drivers need fewer screens to do their jobs, because of the redesign, and have less reason to check the app for bonuses, because the programme ended. The tier-1 concentration matches where the bonus programme ran.

**Aha: gate 0, "is this drop bad?"** Idle engagement is an *input* metric. If the output metrics (trips per driver, acceptance, driver earnings, churn) are flat or up, the drop reflects **efficiency, not dissatisfaction**. Don't "fix" it.

**What to do.** Retire hover time as a success metric. If re-engagement matters for supply at peak, use targeted, time-bound nudges rather than blanket bonuses.

**Trap.** Treating every engagement decline as a problem to reverse.

## Case 4 — Airport-to-city pickups down 20% at one tier-2 airport (environmental handover failure)

**Prompt.** Over two months, airport→city pickups fell 20%, sharply at first and then gradually. City→airport trips are unchanged.

**Evidence.**
- No bugs, experiments, releases or pipeline anomalies.
- No regulatory access changes.
- **A competitor sees the same pattern**, so the cause is location-specific and industry-wide.
- The drop is uniform across demographics and platforms (Android and iOS).
- **Book→confirm conversion is normal**, and driver supply and allocation are healthy.
- But **confirmed bookings aren't turning into pickups**.

**Root cause.** Connectivity degrades when passengers walk out of the terminal and their phones hand over from airport Wi-Fi to the mobile network. Real-time coordination fails at the curb, and pickups are missed despite successful bookings.

**Aha.** Separate **booking** from **fulfilment**. A drop confined to one location, shared by competitors and platform-agnostic, points to the **physical or network environment**, not your code.

**Fix.**
- Offline-tolerant pickup flows: a pre-assigned pickup zone and PIN, SMS fallback, and cached driver details.
- A designated pickup bay.
- Coordination with the airport operator on coverage.

**Watch:** booking→pickup completion at that airport.

## Case 5 — Marketplace sales down 15% in 24 hours across all segments (partner outage)

**Prompt.** Total sales fell 15% in the last day across all user segments and all platforms. Top priority.

**Protocol.**
1. Say what you'd measure at each step, not just which steps exist. For example, *search tap→results rate*.
2. Rule out external factors: no strike, no competitor event, no seasonality.
3. Establish that the funnel is healthy up to checkout.
4. At payment, segment the **payment success rate** by instrument, bank or network, and device.

**Credit-card success has collapsed**, and error logs show intermittent failures on the card network's processing API.

**Fix, in order.**
1. **Mitigate now.** Route traffic to alternate gateways and surface UPI and other instruments first for affected users.
2. **Communicate.** Show failed-payment messaging with retry options.
3. **Fix permanently.** Work with the partner on a root-cause fix, add multi-gateway redundancy, and alert on success rate by instrument.

**Aha.** Sudden, platform-wide and segment-agnostic points to **shared infrastructure** (payments, auth, CDN, a third-party API). Go to the last common step every user passes through.

**Trap.** A slow step-by-step journey walk from registration onward while revenue bleeds. Triage from the shared dependencies first.

## Case 6 — Video-platform engagement sliding for several quarters (multi-cause structural decline)

**Prompt.** Watch time per session and DAU have both declined slowly over several quarters. The decline is concentrated in 18–25-year-olds across several large markets.

**Evidence chain, confirmed one by one:**
1. A recommendation change six months ago over-optimised for retention and watch time. Users see repetitive content and tire of it.
2. Short-form rivals are pulling young users, and the hand-off from short-form to long-form isn't working.
3. More unskippable ads, plus lag and buffering complaints on Android.
4. Uploads from small and mid-tier creators are down ~15% after stricter monetisation rules, which shrinks content variety.

**Synthesis.** Five reinforcing causes: repetition, competition, ad load, performance and creator supply.

**Aha.** **Slow and gradual means several structural causes; sudden means one event.** For a slow decline, build a driver tree and **size each branch** rather than hunting for a single culprit. `[ILLUSTRATIVE]` Attribute the watch-time loss with cohort analysis: short-form substitution in the 18–25 cohort vs. ad-load exposure vs. Android performance.

**Fix.** A portfolio of fixes:
- Diversity constraints in recommendations.
- A short→long-form bridge.
- An ad-load cap for new and young cohorts.
- An Android performance sprint.
- A creator-monetisation review.

**Guardrail:** ad revenue per user.

## Case 7 — Streaming viewership dropped steeply a few weeks ago (rights/content loss)

**Prompt.** Viewership (users × watch time) fell steeply a few weeks ago.

**Evidence.**
- Metric definitions are unchanged and the backend is stable.
- **Both** users and watch time fell.
- The drop **starts at app open**, not mid-journey.
- It is concentrated in casual and sports-focused mobile users.
- The timing coincides with the **premier T20 cricket league season**.
- The platform **lost the league's streaming rights to a rival** this year.

**Root cause.** Sports viewers migrated to the rights holder.

**Aha.**
- A drop at **app open** rules out UI or playback issues; people never arrived.
- A seasonal and event-timed drop, with a known rights change, is external.
- Decomposition helps: viewership = subscribers × % who open × watch time per opener. Here the "% who open" collapsed.

**Response by horizon.**
1. **Short term.** Retain non-sports users with personalised campaigns, watch streaks, trial extensions and a push on the global franchise library.
2. **Medium term.** Diversify content with regional originals and creator partnerships, plus telecom bundles to cut subscription friction.
3. **Long term.** Rebuild a live-content moat through other leagues, regional sports and e-sports.

**Metrics:** DAU, watch time per user, churn by cohort.

**Trap.** Recommending a UX overhaul for a problem that begins before the user sees any UX.

---

## Archetype cheat sheet

| Signature | Likely archetype | First question to ask |
|---|---|---|
| Sudden, one app only, top funnel intact | Internal change at one step | "What changed in pricing, policy or payments that day?" |
| Sudden, all users, all platforms | Shared infrastructure / partner outage | "What's the success rate at the last common step?" |
| One location, competitors hit too | Environment / infrastructure | "Do bookings convert but fulfilment fail?" |
| Gradual over quarters, one cohort | Several structural causes | "What else changed for this cohort: rivals, content, ads, performance?" |
| Starts at app open, event-timed | Content/rights/seasonality | "What did users come for, and do we still have it?" |
| Input metric down, outputs up | Efficiency, not a problem | "Are trips, earnings and churn affected?" |
| Ratio metric moved | Numerator vs. denominator | "Is it the value or the count that moved, and gross or net?" |
