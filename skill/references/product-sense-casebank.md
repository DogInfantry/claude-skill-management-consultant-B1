# Product-Sense Casebank — Design, Improve, Favourite Product, Unconventional, Deck Blueprint

Worked product-interview cases rewritten as reusable patterns. Each one follows the same shape: **prompt → who and what matters → prioritised solution → metric → the upgrade a strong candidate adds → trap**. The file also covers the **"favourite product"** question and a slide-by-slide **product case-competition deck blueprint**.

Companion to `references/product-management-toolkit.md` (frameworks), `references/india-pm-cases.md` (CIRCLES/HEART diagrams, teardowns) and `references/product-rca-casebank.md` (metric-drop diagnoses). Numbers are `[ILLUSTRATIVE]` unless marked *verify*.

**The six PM prompt types and what each rewards**

| Type | Sounds like | Rewards |
|---|---|---|
| Design | "Design X for Y" | Segment choice, needs → prioritised features, success metric |
| Improve | "Improve X / grow metric M" | Goal clarity, journey leak, RICE-ranked fix |
| Favourite product | "What's your favourite product and why?" | Product taste backed by a mechanism, not adjectives |
| Metrics | "How would you measure success of X?" | A metric *tree* with a North Star and guardrails |
| Experiment | "How would you test feature F?" | Hypothesis, unit of randomisation, sample size, guardrails |
| Strategy / unconventional | "Should X enter Y?" / "Build Z from scratch" | Where to play, right to win, sizing against the parent's base |

---

## Part A — Design prompts

### A1. School-commute experience on a ride-hailing app
- **Stakeholders.** Kids are the users; parents are the **buyers**; drivers are the supply; schools are a channel.
- **Pain points.**
  - Unvetted drivers and poorly maintained vehicles.
  - Overcrowded vans.
  - Irregular price hikes.
  - No visibility of where the child is.
  - No cover when a driver doesn't turn up.
- **Target segment.** Middle-income families, for two reasons: lower-income families use shared autos or buses on price, and higher-income families use a family car and driver.
- **Features, in priority order.**
  1. **Verified-driver pool** with background checks and driving tests.
  2. **Live tracking + milestone alerts**: started, 10 minutes away, dropped at the gate.
  3. **Guaranteed backup vehicle** at no extra cost.
  4. **Monthly subscription with fixed pricing.**
  5. School tie-ups for gate-side pickup.
  6. A free trial ride so parents can try it.
- **Upgrade: the unit economics.** The subscription only works if seats are pooled.

  `[ILLUSTRATIVE]` 4 children per car × 2 trips a day × 22 school days = 176 child-trips a month per car. At ₹2,500 per child per month, that is ₹10,000 per car per month for about 2 hours of peak driving. That must beat what the driver would otherwise earn in those peak hours, so **route density** (children per km) is the variable to design around.
- **Metric.**
  - North Star: children-weeks delivered on time.
  - Supporting: subscription renewal rate.
  - Guardrail: safety incidents, where the target is zero.
- **Trap.** Designing for the child's experience and forgetting that the parent pays and the driver must earn.

### A2. Headphones for a big-tech ecosystem, across age groups
- **Segments and core jobs.**

  | Segment | Core job | Features |
  |---|---|---|
  | Kids | Learn safely | Volume limiter, parental controls, durable build, interactive learning mode |
  | Professionals | Focus and switch devices | Adaptive noise cancelling, device fast-pairing, calendar-synced focus mode, live translation |
  | Seniors | Hear clearly and stay safe | Voice-first controls, large tactile buttons, speech-clarity amplification, fall/emergency alerts to the home hub |

- **Two architectures.** (a) Three editions with separate SKUs. (b) **One modular, adaptive device** that recognises the signed-in profile and switches mode: limits for kids, work sync for professionals, simplified voice mode for seniors.
- **Recommendation.** Lead with (b) where families share devices; keep a kids SKU for durability and price.
- **Upgrade.** Name the moat. The hardware is copyable; **account-level personalisation across the ecosystem** is not. Say what data the device uses and what privacy controls apply, especially for kids.
- **Metric.**
  - North Star: weekly active wearers per household.
  - Supporting: ecosystem attach rate.
  - Guardrail: returns and complaint rate.
- **Trap.** A feature list for three personas with no prioritisation and no business model.

### A3. Lift revenue on a horizontal e-commerce marketplace via interest communities
- **The idea.** Interest communities where like-minded buyers discuss products, share reviews and compare alternatives.
- **Supporting features.**
  - Interest profiling at onboarding.
  - Recommendations built from purchase history.
  - Gamified participation (challenges, badges, credits).
- **Upgrade.** Make the **revenue logic** explicit, because "community" alone isn't a revenue plan:

  > community content → trusted UGC on product pages → higher conversion and lower returns → revenue

  `[ILLUSTRATIVE]` If 10% of sessions touch community content and that lifts conversion from 3.0% to 3.3%, blended conversion rises ~1%. That is the size of prize to test.
- **Metric.**
  - North Star: GMV from sessions that touched community content (incremental, via a holdout).
  - Guardrails: return rate and moderation load.
- **Trap.** Proposing a search-partner integration (sharing users' external search history) without addressing privacy.

### A4. Serve the start-up ecosystem on a professional network
- **Stakeholders.** Founders and investors. **Prioritise founders**: investors have teams and dedicated services, while founders are resource-poor and engage more.
- **Founder journey and features.**

  | Stage | Needs | Features |
  |---|---|---|
  | Ideation | Validation | Crowd-feedback on prototypes from verified professionals |
  | Commitment | Team, MVP | Skills-gap analyser that maps the team's skills to learning content and to hires |
  | Traction | Funding, mentors | **Mentor connect** (verified domain experts with a badge); **investor marketplace** (pitch cards discoverable by investors) |

- **Prioritisation (RICE).** Mentor connect and the investor marketplace address the core needs and use the network's unique asset, the graph. The skills analyser is a later supporting feature.
- **Metric.**
  - North Star: founder–mentor/investor conversations started.
  - Guardrail: spam and cold-pitch reports from investors.
- **Trap.** Building an investor marketplace without friction controls. Investors leave if their inbox floods.

### A5. Abstract design: "You rule a medium-sized 19th-century empire. Design a product to enable territorial expansion."
- **Why interviewers ask it.** To test structure under absurdity. Treat it as a normal design prompt.
- **Clarify.** Continental, industrialising, with neighbours that are 60% small, 20% equal and 20% large.
- **Users and needs.**
  - The ruler needs information and legitimacy.
  - The army needs logistics.
  - Administrators need control at a distance.
  - Annexed populations need a reason to comply.
- **"Products" ranked by impact × feasibility.**
  1. A **telegraph + rail logistics network**: speed of information and troops.
  2. A **customs union / common currency offer**: economic pull on small neighbours.
  3. Standardised administration: a common code and census.
- **Strategy on top.** Integrate smaller neighbours first, through alliances or union, to gain the scale to negotiate with larger ones. Growing the economy and building diplomacy can beat conquest on cost.
- **Metric.** Territory integrated per unit cost; stability of annexed regions (revolts per year).
- **Trap.** Answering with pure military strategy and never naming a "product".

---

## Part B — Improvement prompts

### B1. The #2 e-commerce player wants to close the gap with the leader
- **Diagnose where the gap is.** The leader wins in tier-2 and tier-3 cities, helped by trust features such as **open-box delivery**. The #2 player is strong in tier-1 on fast delivery.
- **Pick one domain: fashion**, where the #2 player trails specialist fashion apps.
- **Leaks.**
  - Weak brand and offer visibility on the landing page.
  - Thin assortment in high-demand sub-categories.
  - No conversational discovery.
- **Fixes.**
  - A dynamic offer and brand hub.
  - Curated brand partnerships.
  - A GenAI stylist ("beach-ready white outfits").
  - **Differentiator:** a virtual try-on on a body-matched avatar.
- **Upgrade.** Be ready for "rivals already have a GenAI stylist, so what's your USP?"
  - The answer: combine try-on with **size-fit prediction**. Fashion returns are the P&L killer, so fewer wrong-size returns is the real prize.
  - Metric: return rate and conversion. `[ILLUSTRATIVE]` A 5-point cut in fashion return rate is worth more than a 5% lift in sessions.
- **Trap.** Quoting market-share numbers you can't source. Say "the leader is roughly 2× our share" and move on.

### B2. Raise checkout conversion from homepage recommendations (food delivery)
- **Goal.** More orders placed directly from homepage tiles, with fewer searches and scrolls.
- **Persona.** Prioritise the **time-poor professional**: high frequency, and they value speed and a reliable meal.
- **Ranking signals.**
  - Delivery ETA.
  - Past orders and time-of-day patterns.
  - Meal quality, using low refund/complaint rate as the proxy.
  - Price band.
- **New users (cold start).** Recommend by location first (fast, well-rated nearby places) plus quick filters for cuisine and diet.
- **Metrics.**
  - **North Star:** orders attributed to homepage recommendations ÷ homepage sessions.
  - **Supporting:** searches per order ↓, time to first add-to-cart ↓, scroll depth ↓.
  - **Guardrails:** order-level CSAT, restaurant concentration (don't starve long-tail partners).
- **Upgrade.** Total time in app is **ambiguous**: less time can mean faster success. Don't use it as a success metric.
- **Trap.** "Personalise for everyone" with no persona or ranking signals.

### B3. Monetise search on a social network beyond search ads
- **Start with the problem.** Search results aren't intent-aware, local or organised. They lose to a general search engine for "running shoes" or "car service near me".
- **The edge.** The **social graph**: people trust friends' experiences.
- **Feature.** Friend-powered travel and local discovery: a map of places friends have visited, with their photos and reviews, filterable by type. It links to **book / reserve** actions and prompts reviews after a visit, which keeps the loop fed.
- **Monetisation.** Transaction fees on bookings, sponsored listings, and pay-per-call-to-action.
- **Upgrade.** Sequence it: fix relevance, then earn intent, then monetise. Size the prize against the ad base (see D2 below), otherwise it's a feature, not a business.
- **Trap.** Jumping to monetisation before search is useful.

---

## Part C — "What's your favourite product?"

**Skeleton (≈ 2 minutes):**
```
1. WHAT & FOR WHOM   one line: what it is, who it serves, the job it does
2. WHY IT WINS       2–3 reasons, each a MECHANISM (not "clean UI"):
                     habit loop · network effect · friction removed · trust built
3. VS. THE OBVIOUS RIVAL   one crisp differentiator (expect "why not X?")
4. WHERE IT FALLS SHORT    1–2 real gaps, for a named segment
5. WHAT I'D BUILD          one prioritised bet + the metric that proves it
```
**Guardrails.**
- Check your "only they do X" claims. Competitors copy fast, and a false "only" costs credibility.
- Check whether your proposed feature **already exists**.
- Keep personal backstory to one sentence.

**Exemplar 1 — a UPI payments app (Google Pay).**
- **Why it wins.**
  - Repeat payments are near-frictionless: recent contacts, one tap.
  - Gamified rewards drive habit.
  - Bills and recharges add daily use.
- **Vs. a super-app.** It stays focused, while the super-app feels cluttered.
- **Stakeholder lens.** Users, banks (UPI rails), the network operator (NPCI) and merchants.
- **Gaps and fixes.**
  - First-time users need guided onboarding.
  - Bank-side failures at peak load call for success-rate monitoring and smart retry.
  - Merchants need faster payment confirmation and simpler integration.
- **Metric.** Payment success rate; monthly transacting users.

**Exemplar 2 — a beginner-friendly broking app (Groww).**
- **Why it wins.** Mobile-first simplicity for first-time investors, where incumbent bank-broker apps feel dated.
- **Vs. the power-trader platform.** Easier for novices; the rival serves experts.
- **Gaps and fixes.**
  - Active options traders need **bulk position exit**.
  - A missing asset class (commodities) blocks diversification.
  - There is no in-app market news.
- **Priority.** Bulk exit first: it is a risk-control need at the moment of highest stress.
- **Metric.** Order-failure and slippage complaints, and retention of active traders.
- **Watch-out.** Verify feature gaps before claiming them. Apps ship fast.

**Exemplar 3 — a music-streaming app (Spotify).**
- **Why it wins.** Library depth, taste-blending playlists, cross-device continuity.
- **The interviewer's twist.** "Premium conversion is X%. Raise it."
- **Diagnosis.** Price is higher than rivals, exclusive content is thin for this market, and ad-avoidance leaks free users to modified apps.
- **Fixes.**
  - Social listening: listen together with friends, with presence.
  - Premium-only high-quality offline downloads.
  - Regional pricing tiers.
- **Metric.** Free→paid conversion and paid churn.
- **Watch-out.** Some of these social features exist in some form, so say how you'd extend them.

**Exemplar 4 — a food-delivery app (Zomato).**
- **Why it wins.** Discovery and ratings that help decide *what and where* to eat; a strong three-sided network.
- **Gap.** It is great for occasional orders and poor for **daily meals**: choice fatigue, cost, health.
- **Fix.** A daily-meal vertical: a subscription plan, a small rotating menu, and verified home chefs and tiffin kitchens for supply.
- **Metric.** Weekly active subscribers; meals per subscriber per week.
- **Watch-out.** A version of this has been launched in the market. Acknowledge that and pitch the *next* iteration.

---

## Part D — Unconventional prompts

### D1. How would you test a "people you may know" module?
- **Goal.** Grow *meaningful* connections, not just requests.
- **Test candidates.**
  1. **Presentation.** Swap the "Name + 7 others" text link for thumbnails of mutual contacts.
  2. **Ranking for new users.** Prioritise imported contacts for users with a thin network.
  3. **Filters.** Mutual connections, company, school.
  4. **Information.** Add a "shared skills" line.
- **Priority.** Filters and shared skills first: low effort and high relevance.
- **Design each test properly.**
  - **Hypothesis.** H0: no change in accepted connections per viewer.
  - **Primary metric.** *Accepted* connections per exposed user (not clicks).
  - **Guardrails.** "I don't know this person" reports, invite ignore rate, block rate.
  - **Sample size.** Baseline connect rate 5%, detecting a +10% relative lift (0.5 pp). By the rule of thumb n ≈ 16·p(1−p)/δ², that is **≈ 30,400 users per arm**.
  - **Network interference.** Treated users' invites land on control users, which contaminates the control group. Randomise by cluster (e.g. geography or company), or measure the sender side only.
  - **Novelty effect.** Run for 2+ weekly cycles.
- **Trap.** Declaring a winner on click-through when the acceptance rate fell.

### D2. Should a large social network enter travel?
- **Map the value chain.** Inspiration/discovery → research/reviews → booking (OTAs, stays) → in-trip → sharing. Exclude corporate travel: poor fit with the network's mission.
- **Where to play.** Leisure **discovery**, where the social graph and creator content are genuinely advantaged.
- **Capability gaps.** Booking requires GDS connectivity, supplier contracts and servicing, none of which the network has today.
- **Sizing against the parent's base.**

  ```
  Users in target regions ~600M (verify) × 10% engage with travel discovery  = 60M
  Discovery ads: 60M × ~$8 incremental ad revenue/user/yr                   ≈ $0.5B/yr
  Booking (later): 60M × 5% book in-app × $1,500 trip × 15% commission      ≈ $0.7B/yr
  Parent ad base: >$100B/yr (verify) → each is well under 1% of revenue
  ```
- **Error fixed.** The original claimed ~$0.5B would add "~5% growth" to ad revenue. Against a base of over $100B it is **under 0.5%**.
- **Recommendation.**
  - Enter discovery through **partnerships** (affiliate links to OTAs), not a build. Justify it on engagement and data, not revenue.
  - Revisit booking only if discovery shows strong intent signals.
- **Aha.** Always size an opportunity *relative to the parent*. Big-looking numbers can be immaterial.

### D3. Reposition a legacy, bundled drawing app seen as "for kids"
- **Personas.**
  - Casual creator.
  - Nostalgic reviver.
  - Tech-savvy explorer.
  - Student.
  - Teacher.
  - Creative pro (a stretch goal).
- **Shared need.** Quick, simple creation with just enough power.
- **Goal.** Make it SMART. "6× users in 6 months" is not credible for a mature bundled app; propose **+50% MAU and 2× weekly creators in 6 months** `[ILLUSTRATIVE]`.
- **Prioritise with MoSCoW.**
  - **Must:** precise selection and masking, layers and non-destructive edits, a touch-friendly interface.
  - **Should:** AI image generation and fill.
  - **Could:** a simple animation / storyteller mode, live co-editing.
  - **Won't (now):** a pro-grade photo suite.
- **Go-to-market.**
  - Nostalgia-led marketing.
  - School and art-class partnerships.
  - Creator challenges.
- **Metrics.**
  - MAU and weekly creators.
  - Feature adoption.
  - Share rate of creations.
  - Guardrail: app performance on low-end devices.
- **Trap.** Chasing professionals, which means competing with pro suites, and alienating the casual core.

### D4. Build a racquet-sport venue business from scratch (30 venues × 5 courts, plus a fitness app)
- **Session types.**
  - Onboarding and training (skills).
  - Workout (fitness).
  - Open play.
- **User segments.**
  - Students: evenings and weekends.
  - Working professionals: after work, want personalised plans.
  - Adults 40–60: light play and fitness.
- **App.** Booking with live availability, coach assignment, progress tracking, diet and timetable plans, coach chat.
- **Upgrade: test the premise with unit economics** `[ILLUSTRATIVE]`.

  ```
  Court capacity: 5 courts × 16 h = 80 court-hours/day × 60% utilisation = 48
  × 4 players × ₹150 per player-hour = ₹28,800/day ≈ ₹8.6 lakh/month per venue
  Coaches as briefed: 27 × ₹25,000 = ₹6.75 lakh/month → ~78% of court revenue (before rent)
  Right-sized: ~1 coach per court per shift × 2 shifts ≈ 10–12 coaches ≈ ₹3 lakh/month
  + Coaching programmes: 150 enrolled × ₹3,000/month = ₹4.5 lakh/month per venue
  ```

  **The brief's staffing ratio breaks the P&L.** Challenge it, then add coaching subscriptions as the second revenue line.
- **Structure alternative.** Hub-and-spoke: ~5 large hubs with 10–15 courts for academies, plus smaller neighbourhood venues. Use a freemium app with paid personalised plans.
- **Metrics.**
  - Court utilisation by hour.
  - Revenue per court-hour.
  - Coaching retention.
  - App weekly active users.
- **Trap.** An operations plan with no revenue model and no check on the ratios the interviewer handed you.

---

## Part E — Success-metrics drill: "How would you measure a food-delivery app's success?"

Build a **tree**, not a list:
```
 NORTH STAR: orders delivered on time per week (captures value to all three sides)
   = monthly transacting users × orders per transactor × on-time share
 ├─ Acquisition   installs by channel, cost per install, CAC by channel (attribution!)
 ├─ Activation    install → first order within 7 days  (realistic: ~20–40%, not 85%)
 ├─ Retention     cohort curves (M1, M3, M6 repeat rate); reasons for lapse
 ├─ Engagement    DAU/MAU, sessions per week, browse → order conversion
 ├─ Reachability  push opt-in rate, notification CTR, email open rate
 └─ Health / guardrails  uninstalls per 1,000 installs (tie to crashes, load time),
                         checkout/payment drop-off, delivery time, refunds, rider & restaurant NPS
```
- **Error fixed.** The original set an 85% activation "benchmark", which is not credible for install→first order. It also listed inventory turnover as a primary metric, which matters only for owned-inventory quick-commerce, not a restaurant marketplace.
- **Aha.** Every metric needs an **action attached**. A spike in uninstalls should route to app performance and onboarding. A payment drop-off should route to gateway success rates (see `product-rca-casebank.md` Case 5).

---

## Part F — Product case-competition deck blueprint (6 slides)

Typical prompt: *"It's 2030. Identify a problem in that world and solve it with a product of the future."*

| Slide | Purpose | Must contain | Common failure |
|---|---|---|---|
| **1. Problem & market relevance** | Prove the problem is real, big and solvable *now* | A one-line problem statement with tight scope; data on severity; **why it wasn't solved before** (tech/cost/market) and what changed; public validation (survey, social proof); a guesstimated market size and business potential | A vague problem; no "why now" |
| **2. Users & pain points** | Make it human and prioritised | Two contrasting **user stories** with journey pain points; the **priority segment** chosen on an explicit metric (value, reach, frequency or retention) | Five personas, none prioritised |
| **3–4. Solution journey** | Show the product working | **2/3–1/3 layout**: wireframes along the user journey (two-thirds) plus concise text (one-third) on how each touchpoint resolves a pain, and one line on the broader shift it enables (behavioural or technological) | Feature lists without flow |
| **5. How it works & why these features** | Show technical competence and judgment | A simple **architecture** (data sources → models/services → app), optional but differentiating; a **prioritisation framework** (RICE / impact–effort) showing what made the MVP and why | Architecture jargon with no link to user value |
| **6. Success & risks** | Close like an owner | A **North Star** metric with activation, retention and business metrics beneath it, charted; **pitfalls and workarounds** (adoption, regulation, data/privacy, unit economics) | Metrics with no targets; risks with no mitigations |

**Deck hygiene.**
- Use action titles: each slide title is the takeaway.
- Keep one idea per slide.
- Keep numbers consistent across slides.
- Put detail in an appendix.

See `references/output-craft.md` and `references/storylining.md` for slide craft.
