# Case Pattern Library — Canonical Archetypes and Solution Logic

This file provides a pattern library of consulting case archetypes — not a list of frameworks, but a map of *what actually drives the answer* in each case type. Use it to shortcut to the right analysis, anticipate the "aha" insight, and coach candidates away from common failure modes.

This file complements `references/case-interview.md` (which covers the candidate playbook, scoring rubrics, and interview formats) and `references/case-types.md` (which covers framework selection). This file goes one level deeper: for each major case type, it provides archetypal sub-patterns with their diagnosis logic, critical analysis paths, and the insight that closes the case.

---

## How to Use This File

**When simulating a case as interviewer:** Use the archetype descriptions to pre-select which pattern you're running. The "information to reveal" sequencing is intentional — release it when the candidate asks for the right data, not before.

**When coaching a candidate:** After they present their structure, compare it to the archetype's "critical analyses." If they're missing the key driver, prompt them toward it without giving it away.

**When solving a real client problem:** Use the archetypes as a rapid diagnostic. A pattern-match in the first 10 minutes gives you a working hypothesis before you've run any analysis.

---

## Archetype 1: Profitability Decline

The most common case type. Three sub-patterns drive ~90% of profitability cases.

### Pattern 1A: Revenue Mix Shift (The "Invisible Volume Problem")

**Signature:** Total revenue is flat or growing, but profits are falling. Management is confused because "we're selling more."

**What's actually happening:** The growth is in lower-margin products, channels, or customer segments — while higher-margin business is eroding or being cannibalized.

**Critical analyses:**
1. Segment revenue by product/channel/customer and margin per segment
2. Calculate contribution margin by segment, not just revenue
3. Identify where the mix has shifted over the analysis period (% of revenue vs. % of margin)
4. Quantify: how much of the margin drop is mix vs. volume vs. price vs. cost?

**The "aha" insight:** The company has been optimizing for volume metrics while inadvertently destroying margin structure. Fix: reprice low-margin segments or redirect sales effort toward high-margin business.

**Common failure modes:**
- Candidate splits revenue vs. costs but doesn't segment within revenue
- Candidate identifies "volume is up, so revenue is fine" without looking at mix
- Candidate jumps to cost-cutting before diagnosing whether this is a revenue problem

**Probe questions to plant:**
- "You said revenue grew — but what happened to the product mix within that revenue growth?"
- "If I told you gross margin per unit fell while total volume rose, what would you want to know?"

---

### Pattern 1B: Cost Inflation Mismatch (The "Pricing Lag")

**Signature:** Input costs (labor, materials, energy) rose sharply, but pricing was not adjusted proportionally. Margin compression is real and quantifiable.

**What's actually happening:** The company under-reacted to cost inflation — either because of competitive fear, long-term contracts, or management inertia — while costs reset at a higher level.

**Critical analyses:**
1. Decompose COGS into labor, materials, overhead — identify which component rose
2. Compare cost escalation rate to pricing escalation rate over the same period
3. Benchmark: did competitors raise prices more? (If yes, there's pricing power being left on the table)
4. Calculate the pricing catch-up required to restore target margin at current cost base
5. Model timeline to recovery: is this a one-time reset or a recurring structural issue?

**The "aha" insight:** The margin gap is a known, quantifiable number. It requires a specific pricing action of X% to close — not a cost-cutting program. The company has been absorbing costs it didn't have to absorb.

**Common failure modes:**
- Candidate recommends cost reduction without first testing whether pricing is the lever
- Candidate misses the competitive benchmarking step (which reveals available pricing room)
- Candidate identifies the gap but doesn't quantify the pricing action required

**Probe questions to plant:**
- "Your analysis suggests costs drove the margin decline. Before recommending cost cuts — do you know what competitors charged for the same product over the same period?"
- "If I told you competitors raised prices 14% and the client only raised 6%, what does that change?"

---

### Pattern 1C: Fixed Cost Deleverage (The "Volume Shortfall")

**Signature:** Revenue fell, but costs fell less — because a significant portion of the cost base is fixed. The business has operating leverage that works against it on the downside.

**What's actually happening:** The business was sized for a volume that no longer exists. Variable costs scaled down, but fixed costs (rent, depreciation, core headcount) did not. Each unit of lost revenue carries more fixed cost than anticipated.

**Critical analyses:**
1. Split costs into fixed vs. variable components
2. Calculate contribution margin (revenue minus variable costs only)
3. Compare fixed cost base to breakeven volume — how far below breakeven is the business?
4. Identify which fixed costs are truly fixed (lease, D&A) vs. "sticky fixed" (management headcount, discretionary spend)
5. Model scenarios: what volume recovery is needed vs. what restructuring is possible?

**The "aha" insight:** The fix is not operational efficiency — it's either volume recovery or a structural cost reset (rightsizing the fixed base to a new volume reality). Which path is correct depends on whether the volume decline is temporary or structural.

**Common failure modes:**
- Candidate treats all costs as equally variable and misses the leverage math
- Candidate recommends efficiency improvements without addressing fixed cost structure
- Candidate doesn't distinguish temporary volume decline (fix: demand stimulation) from structural (fix: restructure)

### The Cross-Cutting Move: Isolate Along the Value Chain Before Theorising

Across all three profitability patterns, the technique that most reliably converges the case is to **isolate the problem along the value chain before running a Customer/Competitor/Company scan.** The conventional path — find the broken metric, then immediately scan the whole business for "why" — explores the entire world of causes before narrowing *where* the cause lives. Insert one step in between.

Once you know (say) *volume* is the broken metric, a volume decline can only come from three structurally distinct places:

1. **Production issue** — we can't make or ship as much as before.
2. **Distribution-push issue** — the product reaches fewer shelves or is pushed less by the trade (thinner margins vs. competitors, worse visibility/packaging, fewer outlets). *"Reaches the shop" is not the same as "reaches the customer."*
3. **Customer-pull issue** — end demand or preference has genuinely shifted.

Combine this with two other early isolators: **which segment** (geography / product / channel) carries the drop, and **is the fall company-specific or industry-wide** (market-wide → substitutes or demand shock; company-specific → share loss to rivals). Each answer *kills whole branches* of the tree, so the eventual Customer/Competitor/Company analysis is aimed at one node, not the whole business. The reward is that the answer often sits somewhere unglamorous a "customers and competitors" scan never reaches (see `references/practice-cases-quantified.md` Case 10 — a packaging change that throttled the retailer's ability to dispense a commodity toffee).

Two discipline points that make this move work:

- **Ask what *changed*, not what *exists*.** An outcome that moved must trace to a driver that moved. Decide how you'll *use* a segmentation before requesting it — that's what reminds you to ask "…and *has* this channel's mix or margin *changed* over the period?" rather than merely cataloguing what channels exist.
- **Narrate the hypothesis, don't just hold it.** "Be hypothesis-driven" usually means *communicate* the logic, not that your thinking is wrong. Say the decomposition, name the branch you expect and *why*, then ask for the data that confirms or kills it — instead of firing scattered questions or asking the right questions silently.

---

## Archetype 2: Market Entry

Three sub-patterns dominate market entry cases.

### Pattern 2A: New Geography Entry

**Signature:** A company wants to expand from its home market into a new country or region.

**Critical analyses:**
1. **Market attractiveness:** Size, growth rate, profitability of local players, regulatory environment
2. **Right to win:** Does the company's competitive advantage (brand, cost, technology, relationships) transfer to this geography? What local players already serve this need?
3. **Entry mode:** Organic build, acquisition, JV/partnership, licensing — and what the economics of each look like
4. **Sequencing:** Which geography first? What's the beachhead strategy?
5. **Risk: market-specific downside** — currency, regulation, political risk, cultural barriers to the value proposition

**The "aha" insight:** Market attractiveness is often not the binding constraint — right to win is. A large, growing market where the entrant has no competitive advantage is a value-destruction trap. The most common case resolution: enter a smaller but more defensible niche first, prove the model, then expand.

**The kill criteria:** Always define upfront what would make you NOT enter. A recommendation without kill criteria is incomplete.

**Common failure modes:**
- Candidate only assesses market size without right to win
- Candidate recommends organic build without modeling cost and timeline vs. acquisition
- Candidate misses the "what does success look like" question (i.e., what's the return threshold?)

---

### Pattern 2B: New Segment or Customer Entry

**Signature:** The company is established in one segment but wants to enter an adjacent one (e.g., moving from SMB to enterprise, or from B2C to B2B).

**Critical analyses:**
1. **Is this segment contiguous?** Does the company's current product/service require meaningful adaptation?
2. **Segment economics:** What are the margins, sales cycles, and unit economics in the target segment?
3. **Distribution and GTM:** How does the company reach this new segment — same channels or new?
4. **Cannibalization risk:** Will moving upmarket/downmarket undermine the core business?
5. **Capability gap:** What new capabilities are required (enterprise sales team, compliance, customization)?

**The "aha" insight:** The economics in the adjacent segment often look better on paper (higher ACV, lower churn) but require a fundamentally different operating model. The question is not whether to enter, but whether the company can actually operate in the new segment without losing focus on the core.

---

### Pattern 2C: New Product or Category Launch

**Signature:** The company is entering an adjacent product category, not just a new geography or customer segment.

**Critical analyses:**
1. **Build vs. buy vs. partner:** Is this an area where speed matters (acquire or partner) or where the company has a genuine capability advantage (build)?
2. **Time to market:** How long does each option take, and does timing matter competitively?
3. **Cannibalization:** Does the new product displace existing revenue?
4. **Unit economics:** What is the margin profile of the new product, and when does it reach contribution breakeven?
5. **The customer:** Is this same buyer or a new buyer? If new, how does the company acquire them?

---

## Archetype 3: Growth Strategy

### Pattern 3A: Organic Growth Stall

**Signature:** The company has been growing but growth has slowed or plateaued. Leadership wants to reignite it.

**Critical analyses:**
1. **Diagnose the stall:** Is growth slowing because the market is slowing, or because the company is losing share?
2. **Segment the growth:** Which customer segments, geographies, or products are growing vs. declining? Where is the mix shifting?
3. **Funnel analysis:** Where in the acquisition/retention/expansion funnel is the growth breaking down?
4. **Competitive dynamics:** Have competitors changed pricing, product, or go-to-market in a way that explains the stall?
5. **Ansoff matrix as a hypothesis tool:** Core (same product, same customer), adjacent (new segment or geography), transformational (new product or business model)

**The "aha" insight:** Most growth stalls are not market stalls — they are share stalls. The company stopped winning relative to competitors. The fix is usually in go-to-market, not in product or cost.

---

### Pattern 3B: Unlocking a Latent Revenue Pool

**Signature:** The company has significant existing assets (customers, data, distribution, brand) that are underleveraged. The growth question is how to monetize what you already have.

**Critical analyses:**
1. **Customer lifetime value audit:** What percentage of available wallet share are we capturing?
2. **Cross-sell/upsell analysis:** Which customers are candidates, and what is the attach rate?
3. **Pricing power:** Is the current pricing below what customers would pay?
4. **Adjacency mapping:** What related products or services would the existing customer base buy from this company?

**The "aha" insight:** The fastest growth path is often not acquisition of new customers but deeper penetration of existing ones. Retention and expansion economics are almost always better than acquisition economics.

---

## Archetype 4: M&A / Acquisition Assessment

### Pattern 4A: Strategic Rationale + Synergy Sizing

**Signature:** Should the company acquire Target X? What is it worth, and does the deal create value?

**Critical analyses:**
1. **Strategic rationale:** Why does this acquisition make sense? (Capability, market position, geography, technology, talent)
2. **Standalone value:** What is the target worth as a standalone business? (Comparable company analysis, DCF)
3. **Synergy analysis:** Revenue synergies (cross-sell, market access, pricing power) + cost synergies (overlap elimination) − dis-synergies (management distraction, integration costs)
4. **Value of synergies vs. premium paid:** Is the premium justified by the net present value of achievable synergies?
5. **Integration risk:** What is the probability synergies are actually captured? What are the top integration failure modes?

**The "aha" insight:** Most acquisitions destroy value because the synergies assumed in the deal model are not realized. The critical discipline is distinguishing "guaranteed" synergies (known cost overlaps) from "dependent" synergies (require behavior change) from "aspirational" synergies (require market conditions outside your control). Only the first category should support the premium.

**Synergy benchmarks (use as anchors, adjust for context):**
- Cost synergies: typically 3–5% of combined revenue for horizontal deals
- Revenue synergies: typically take 3× longer to achieve than cost synergies
- Integration costs: typically 1–2× the annual synergy run-rate in Year 1

---

### Pattern 4B: PE / Investment Thesis (CDD)

**Signature:** A PE firm is evaluating an acquisition. The question is: is this a good investment at this price?

**Critical analyses:**
1. **Market analysis:** Is the market growing, stable, or declining? What structural tailwinds/headwinds exist?
2. **Competitive position:** Does the company have durable competitive advantage? Is it a market leader, follower, or nicher?
3. **Management quality:** Can the current team execute the value creation plan?
4. **Value creation levers:** Revenue growth (organic + M&A), margin expansion (cost efficiency + pricing), multiple expansion (positioning for exit to strategic)
5. **Exit optionality:** Who is the likely buyer in 4–6 years, and at what multiple?

**The "aha" insight:** PE value creation almost always comes from one of three places: paying the right price, improving operations faster than planned, or exiting at a higher multiple. The case resolution is identifying which lever is most controllable and what the downside case looks like if the primary lever doesn't materialize.

---

## Archetype 5: Pricing

### Pattern 5A: Underpriced Product / Pricing Power Capture

**Signature:** The company has been pricing at or below the market, leaving value on the table.

**Critical analyses:**
1. **Willingness to pay:** What do customers actually value, and what would they pay? (Van Westendorp, conjoint, competitive benchmarking)
2. **Price-volume tradeoff:** What is the elasticity? At what price increase does volume fall off, and by how much?
3. **Competitor anchoring:** Where are competitors priced, and what is the implied price gap?
4. **Segment-level differentiation:** Are all customers equally price-sensitive, or is there a segment that can absorb higher prices?
5. **Pricing architecture:** Is the current structure (flat fee, per-seat, usage-based, value-based) optimal for capturing the value delivered?

**The "aha" insight:** Price increases in B2B markets are almost always more achievable than management believes, because churn is lower than feared and value delivered exceeds what customers articulate. The risk is usually in the wrong segment, not across the board.

---

### Pattern 5B: Price War Response

**Signature:** A competitor has cut prices aggressively. The company is losing share and facing pressure to respond.

**Critical analyses:**
1. **Is the competitor's pricing sustainable?** What are their unit economics, and can they fund this price level long-term?
2. **How much share have we actually lost?** Is the loss in volume or in price (some customers may be paying the competitor's price to renegotiate with us)?
3. **Respond or differentiate?** Is matching prices the only option, or is there a non-price response (value-add, service level, switching cost) that breaks the price comparison?
4. **Segment-level response:** Are all segments equally price-sensitive? Protect premium segments with differentiated value; compete on price in commodity segments only if economically rational.

---

## Archetype 6: Operations and Cost Transformation

### Pattern 6A: Structural Cost Reduction

**Signature:** The company needs to take out significant cost — not incrementally, but at scale.

**Critical analyses:**
1. **Cost base decomposition:** What are the major cost buckets? Where is the spend concentrated?
2. **Benchmarking:** How does each cost bucket compare to peers? Where is the company above the benchmark?
3. **Controllable vs. structural costs:** Which costs can be reduced without changing the business model, and which require structural change (e.g., outsourcing, asset-light model, process redesign)?
4. **Zero-based budgeting lens:** Start from zero — what is the minimum cost to deliver the current service level?
5. **Speed vs. depth tradeoff:** Quick wins (overhead reduction, procurement) vs. structural changes (footprint, outsourcing, org redesign). Sequence matters.

**The "aha" insight:** Most cost transformation programs fail because they cut incrementally from the existing base rather than asking "what is the right cost structure for this business?" The sustainable fix requires a model for what the cost base *should* be, not just what it currently is.

---

## Archetype 7: People and Talent Funnel

People cases look "soft" but crack on the same logic as a sales funnel: find the stage that leaks, split blended ratios into their separate failures, then price the leak against the cost of the fix.

### Pattern 7A: Leaky Hiring Funnel ("Offers Made, Joiners Missing")

**Signature:** Applications and interview pass rates look healthy, but "conversion has fallen": offers go out and too few people join. Management's instinct is to raise pay.

**What's actually happening:** One blended conversion number hides two failures with different causes. **Declines** (the candidate says no) are driven by decision speed and the pay gap against rivals. **Back-outs** (the candidate accepts, then never turns up) are driven by a long offer-to-join gap and counter-offers. Employer brand and candidate experience act on every stage; they are cross-cutting drivers, not a separate stage.

**Critical analyses:**
1. Rebuild the funnel stage by stage (applicants → interviewed → offered → accepted → joined) and compute every ratio, not only end-to-end
2. Split "not joining" into offer acceptance (accepted ÷ offers) and join ratio (joined ÷ accepted)
3. Ask what *changed* when conversion fell: a rival's pay reset, an added interview round, longer notice periods in the talent pool
4. Collect decline and back-out reasons (a short survey of every decliner) before recommending fixes
5. Price the leak: cost of vacancy per working day, and interviewer hours burnt on every extra offer the leak forces

**The number that cracks it:** with 40 offers → 22 accepted → 16 joined [ILLUSTRATIVE], acceptance is 55% and the join ratio 73%, so only 40% of offers become joiners. Lifting that to 85% acceptance × 90% join = 76.5% cuts the offers needed for 200 hires a year from 500 to about 261.

**The "aha" insight:** Declines and back-outs need different fixes. Decision speed and targeted pay benchmarking fix declines; a shorter, actively managed join gap (notice-period buy-outs, pre-joining engagement, a named buddy) fixes back-outs. The leaky funnel also burns interviewer capacity, which is a cost the business feels directly.

**Common failure modes:**
- Reading joined ÷ offers as the "acceptance rate", so one blended number is treated as one problem
- Assuming pay is the only lever
- Cutting interview rounds without protecting hire quality (merge rounds rather than delete assessment content; track 90-day retention and first-year performance)

**Probe questions to plant:**
- "Of the people who didn't join, how many said no, and how many said yes and then didn't turn up?"
- "What changed in the process or the market when conversion started falling?"

---

### Pattern 7B: Attrition Spike in One Pocket

**Signature:** Attrition is far above peers, but only in one level, site or shift pattern. The rest of the organisation is fine.

**What's actually happening:** A local and often cheap-to-fix condition (commute, shift roster, one manager, a rival's amenity) is pushing people out, and a recent trigger has turned a long-standing condition into a problem.

**Critical analyses:**
1. Pin the metric: annualised leavers ÷ average headcount, for the affected cohort only
2. Segment who leaves (level, tenure, shift, commute distance, hired-from location), where they go, and why (exit-interview Pareto)
3. Separate push factors (commute, shifts, manager, career path) from pull factors (rival pay, amenities)
4. Find the trigger: what changed when the problem started
5. Build the business case: excess leavers × cost per leaver (typically 50–200% of annual salary) against the annual cost of the fix, and compute the break-even reduction

**The number that cracks it:** 120 junior engineers at 50% attrition against a 15% peer norm means 42 excess leavers a year [ILLUSTRATIVE]. At ₹7 lakh per leaver that excess costs ₹2.94 crore a year, while shuttles plus leased housing cost about ₹1.3 crore, so the fix breaks even at about 18.5 fewer leavers (attrition from 50% to about 35%).

**The "aha" insight:** When attrition clusters in shift-working junior staff at a remote site, and nearby employers offer transport, the cause is a basic-needs gap rather than pay or careers. The business case closes the argument, because the fix only has to move attrition about 15 points to pay for itself.

**Common failure modes:**
- Explaining a three-year-old problem with a condition that has not changed (the site has always been remote) without finding the trigger
- Recommending amenities without costing them against the attrition bill
- Assuming pay is the cause without exit data

**Probe questions to plant:**
- "The plant has always been remote. Why did attrition jump three years ago?"
- "How far would attrition have to fall for your fix to pay for itself?"

Worked drills with full math: `references/case-bank-unconventional.md` (U1 hiring funnel, U2 attrition). Benchmarks: `references/functional-deep-dives.md` (Talent Acquisition Diagnostics; Talent Retention & Engagement).

---

## Archetype 8: Social-Sector Outcome

### Pattern 8A: Outcome Gap in a Public Programme

**Signature:** A government, foundation or NGO wants to move a social outcome (reduce girls' school dropout, raise take-up of a scheme, cut road deaths), usually with a fixed budget and a favoured intervention already in mind.

**What's actually happening:** Losses cluster at a few points in the system, typically **transition points** where a person must change institution, travel further or pass a test. Meanwhile the favoured intervention is judged on beneficiaries reached (outputs), not on outcomes added over what would have happened anyway (the counterfactual).

**Critical analyses:**
1. Define the outcome metric precisely (e.g., girls enrolled in Grade 10 per 100 who enter Grade 1) and the counterfactual
2. **Cohort flow:** follow 100 entrants through the system and locate where they leak
3. MECE causes: supply (a school at the next level within reach, teachers, toilets), demand (household cost, household labour, social norms), access and safety (distance, transport, harassment), learning (foundational gaps that end in exam failure). Each cause sits in one branch only
4. **Logic model:** inputs → activities → outputs → outcomes → impact, with the assumption at each link written down
5. Rank interventions on **cost per additional outcome**, spreading durable assets across the cohorts they serve
6. Pilot with a comparison group before scaling, and design for the implementing agency's delivery capacity

**The number that cracks it:** in an illustrative cohort, 47.7 of every 100 girls are lost by Grade 10, and the two school-change transitions account for 28.0 of them (about 59%). Bicycles for all 8,600 Grade 9 entrants that lift the transition from 80% to 86% cost about ₹57,000 per *additional* girl enrolled, because 93% of recipients would have enrolled anyway; girls' toilets cost about ₹15,000 per additional girl once spread over a 10-year life [ILLUSTRATIVE].

**The "aha" insight:** The unit of value is the additional outcome over the counterfactual, not the beneficiary. Most recipients of a universal handout would have reached the outcome anyway, so targeted or durable interventions at the leak points usually win.

**Common failure modes:**
- Counting outputs (bicycles delivered, camps held) as outcomes
- Overlapping causes (distance listed under both supply and access)
- Comparing interventions on cost per beneficiary instead of cost per additional outcome
- Recommending a state-wide scale-up with no pilot, no comparison group and no delivery plan
- Ignoring stakeholder constraints and the capacity of the last-mile implementing staff

**Probe questions to plant:**
- "Of the girls who received a bicycle, how many would have stayed in school anyway?"
- "Across the twelve school years, where do most girls leave?"

Worked material: `references/case-bank-unconventional.md` (Part D — Social Sector & Public Outcomes); `references/india-guesstimates-and-cases.md` (Drill Q, girls' school dropout); `references/public-sector-government-defense.md` (Logic Model / Theory of Change; Program Evaluation).

---

## Archetype 9: Technology / AI Business Case

### Pattern 9A: "Should We Deploy This?" (Chatbot, Automation, Platform)

**Signature:** The client wants to deploy a chatbot, an automation tool or a new platform, and the business case quotes a large gross saving: volume × automation rate × unit cost.

**What's actually happening:** The gross figure overstates the value. Only fully contained work saves money; escalated work still incurs the technology cost on top of the human cost; the platform carries a fixed monthly cost; adoption ramps; and savings become cash only when capacity is actually released. Risks (wrong answers, security, regulation) are a design constraint, not an appendix.

**Critical analyses:**
1. Pin the primary objective (cost, experience or engagement), because it sets the success metric
2. Net business case: volume × containment × (human unit cost − technology unit cost) − technology cost on escalated items − fixed platform cost
3. Adoption ramp and one-off build cost → year-1 net and payback month
4. Cash conversion: how many FTE or outsourced seats are released, and how (attrition without backfill, fewer vendor seats)
5. Risk heat map (likelihood × severity) with guardrail metrics for the top risks
6. Phased roll-out: lowest-risk, highest-volume use cases first

**The number that cracks it:** 1 million queries a month × 40% handled × ₹50 = ₹24 crore a year *gross*. At 75% true containment, ₹5 per bot interaction and ₹30 lakh a month of fixed platform cost, the net run-rate is about ₹12 crore a year, half the gross, and year 1 delivers only about ₹7.6 crore before a ₹5 crore build because adoption ramps [ILLUSTRATIVE].

**The "aha" insight:** The saving is net, not gross, and it is real only when capacity is released. The north-star metric is cost per *resolved* outcome at equal or better quality, protected by guardrail metrics (repeat-contact rate, audited wrong-answer rate, complaints, human-vs-bot satisfaction).

**Common failure modes:**
- Counting every touched transaction as a fully avoided cost
- Ignoring the fixed platform cost and the ramp, so there is no payback month
- An unranked risk list that omits hallucination and prompt injection
- Optimising containment by trapping customers who need a human

**Probe questions to plant:**
- "Of the queries the bot touches, how many never reach a human within a week?"
- "Which agent seats actually go away, and when?"

Worked drill: `references/case-bank-unconventional.md` (U6). Cost structures and governance: `references/genai-enterprise-strategy.md` (ROI Modeling and Cost Structures; Governance and Risk Architecture).

---

## Sector Profit-Tree Mini-Library

A generic "revenue − cost" tree wastes the first five minutes of a sector case. Start from the sector's own economic identity, find the one ratio that moved, and size it. All figures below are **[ILLUSTRATIVE]**.

**Airport — aero vs non-aero, then the retail funnel.** Profit = aeronautical revenue (landing, aircraft parking, passenger-service and security fees, usually regulated) + non-aeronautical revenue (retail, F&B, advertising, car parking, real-estate leases, lounges) − opex. Retail revenue to the airport = departing passengers × store penetration (driven by **airside dwell time**, the minutes left after security) × spend per shopper × concession share. At 20M departing passengers × 40% penetration × ₹800 × 25% share, retail earns the airport ₹160 crore; if check-in and security queues cut dwell time enough to lose 5 points of penetration, the airport loses ₹20 crore. *Aha:* queues are a commercial problem, not only an operations problem. *Trap:* treating a retail decline as a merchandising problem, and never asking whether concessions pay a revenue share or a fixed rent with a minimum guarantee (under fixed rent, weaker shop sales do not hit airport revenue until the leases reset).

**Bank — NII, fees, opex, provisions.** PBT = NII (average earning assets × NIM) + fees and commissions + treasury income − opex (cost-to-income ratio) − provisions (regulatory/specific + management overlay; together, credit cost × loans). On a ₹1 lakh crore book, every 10 basis points of NIM or credit cost moves PBT by ₹100 crore. *Aha:* split each line that moved into client-specific and industry-wide parts, and split provisions into regulatory and discretionary overlay. *Trap:* listing interest expense as a generic cost beside opex instead of netting it into NII. Full exemplar: `references/case-bank-interview-classics.md` (#16 Provision Squeeze).

**Hospital — surgical vs medical, ARPOB.** Inpatient revenue = beds × occupancy × 365 × ARPOB (average revenue per occupied bed-day); split it into surgical (surgeries × revenue per surgery) and medical (admissions × average length of stay × revenue per bed-day), plus outpatient, pharmacy and diagnostics. A 300-bed hospital at 70% occupancy has 76,650 occupied bed-days; at ₹50,000 ARPOB that is about ₹383 crore, and each 5 points of occupancy is about ₹27 crore. *Aha:* a quality failure in one service (post-operative care) spreads by word of mouth into surgical volume and bed occupancy at the same time. Test the Indian-specific causes too: senior surgeons leaving, loss of insurer or government-scheme empanelment, a new competing hospital nearby. *Trap:* writing "cost per surgery" in a revenue tree.
**Error fixed:** treating occupancy and length of stay as parallel revenue branches → occupancy already contains length of stay; use beds × occupancy × 365 × ARPOB, and let ALOS explain throughput (admissions = occupied bed-days ÷ ALOS).

**Hotel — RevPAR, then revenue per capex rupee.** Room revenue = rooms × 365 × RevPAR, where RevPAR = ADR × occupancy; add F&B and events. For a location choice, rank cities on return per rupee of capex, not on revenue. A 200-room hotel at ₹10,000 ADR, using each city's *market* occupancy as the base:

| City | Market occupancy | Room revenue | Capex | Revenue ÷ capex | Payback at 35% EBITDA margin |
|---|---|---|---|---|---|
| A (capital region, next to existing hotels) | 70% | ₹51.1 cr | ₹150 cr | 34% | 8.4 years |
| B (western metro) | 65% | ₹47.5 cr | ₹100 cr | 47% | 6.0 years |
| C (southern metro) | under 60% | ₹43.8 cr at most | ₹120 cr | 37% at most | 7.8 years or longer |

City B wins on capital efficiency; City A also risks cannibalising the client's existing hotels. Before deciding, replace the common ₹10,000 ADR with each city's own luxury rate (compare RevPAR).
**Error fixed:** giving the new hotel the *highest* occupancy in the city whose existing hotels fill the fewest rooms → low market occupancy signals oversupply or weak demand, not headroom; high market occupancy is what signals unmet demand.

**Theatre / live venue — capacity first.** Revenue = seats × occupancy × shows × ticket price + ancillary (F&B, merchandise, sponsorship). Three 320-seat halls at 60% occupancy fill 192 seats a show; at a $14 ticket and 9 shows a week *across all three halls*, revenue is $24,192 a week, about $1.26M a year. Against a $20M year-1 target that is roughly 16× short; even at full use — 8 shows per hall, 24 a week, every seat sold — revenue is about $5.6M, still more than 3× short. Hitting $20M at $14 needs about 143 shows a week, or a ticket of about $83 at 24 shows a week on the same 60% occupancy. *Aha:* test the target against physical capacity before debating strategy; the show count is the first lever, and ancillary income cannot close a gap of 3.6–16× capacity. With $60M of capex against $1–6M of revenue, the case as structured points to no-go or a rescoped entry.
**Error fixed:** multiplying by 3 halls when "9 shows a week" is already the total → that triple-counts capacity ($72,576 a week, $3.77M a year, instead of $24,192 and $1.26M).

---

## Cross-Archetype Failure Modes (Coach These)

These mistakes appear across case types and signal underdeveloped consulting instincts:

| Failure Mode | What It Looks Like | What It Signals | The Coaching Point |
|---|---|---|---|
| Framework fetishism | "I'll use Porter's Five Forces to structure this" | Reliance on memorized tools instead of thinking | "Build the structure from the problem, not the textbook. What are the 2–3 questions that actually drive the answer here?" |
| No hypothesis | Dives into analysis without a point of view | Comfort with process over conviction | "Before you analyze, what's your best guess right now? Hypothesis-first." |
| Boiling the ocean | Analyzes every branch of the issue tree | Poor prioritization | "Where is 80% of the answer? Start there." |
| Summary not synthesis | "Revenue went down and costs went up" | Doesn't know the difference between data and insight | "What does that *mean*? What should the client *do*?" |
| Generic recommendation | "Improve operations" / "invest in marketing" | Hasn't solved the specific problem | "Specifically, which operations? By how much? By when? Who owns it?" |
| Missing the killer assumption | Builds a logical structure on a wrong foundation | Hasn't pressure-tested the key lever | "What's the single assumption that, if wrong, breaks your recommendation? Have you tested it?" |
