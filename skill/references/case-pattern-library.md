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
