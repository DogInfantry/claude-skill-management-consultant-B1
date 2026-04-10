# Pricing Architecture for Consulting Clients

This file covers how to analyze, diagnose, and redesign a client's pricing model as a consulting engagement — the methodologies for understanding price realization, identifying structural pricing problems, designing pricing architecture changes, and managing the implementation of pricing strategy shifts. It is distinct from `references/commercial-dd-market-sizing-shortcuts.md` (which covers market sizing in a due diligence context) and `references/consulting-negotiation-fee-anchoring.md` (which covers the fee negotiation of the consulting engagement itself). This file covers pricing as a client deliverable — the substantive consulting work of helping a client improve how they price their own products and services.

The operating reality: pricing is the single highest-leverage P&L lever available to most businesses. A 1% improvement in price realization typically produces a 6–8% improvement in operating profit for a typical industrial or consumer goods business — more than a comparable improvement in volume or cost. Despite this, most organizations underinvest in pricing capability relative to other P&L levers, and most pricing engagement work is shallower than the strategic importance of the topic warrants.

---

## The Pricing Diagnostic: Five Diagnostic Lenses

A pricing engagement begins with diagnosis. Before recommending any change to pricing strategy or architecture, understand the current state across five lenses.

### Lens 1: Price Realization Analysis

Price realization is the most diagnostic starting point. The "price waterfall" — the decomposition of list price to actual net price — reveals where pricing value is being destroyed and why.

**The price waterfall structure:**

List price → less: functional discounts (distribution tier, volume, payment terms) → less: promotional discounts (temporary promotional offers, seasonal pricing) → less: channel support costs (trade spending, co-op advertising, slotting fees) → less: customer-specific allowances (off-invoice allowances, price exceptions) → **= Net invoice price** → less: post-invoice allowances (rebates, chargebacks, returns) → **= Net-net price (pocket price)**

**What the waterfall reveals:**
- Discount structure: Are discounts structured around value (volume tiers that reflect lower service cost at scale) or around negotiating pressure (exceptions granted without economic logic)?
- Pocket price variance: What is the range of net-net prices realized for the same product across different customers? High variance indicates that price is being set by negotiating strength rather than by a consistent pricing architecture.
- Below-the-line leakage: What share of list price is being given away in post-invoice adjustments that are invisible to front-line sales at the point of pricing? High below-the-line leakage suggests that the incentive structure is misaligned — sales people are pricing against invoice price, not pocket price.

**The target:** Characterize the average pocket price as a percentage of list price (typical range: 60–85% in B2B industrial; 80–95% in consumer categories with less trade complexity). Benchmark against industry norms. Identify the three largest waterfall elements and assess whether each is justified by economic logic or represents value destruction without corresponding value creation.

### Lens 2: Customer Segmentation Analysis

Price realization analysis tells you where discounts are going. Customer segmentation analysis tells you whether they are going to the right customers.

**The customer profitability analysis:**
Rank customers by pocket price realization (not revenue). The distribution typically reveals a "whale curve" — a small number of customers receiving above-average net pricing who are highly profitable, and a long tail of customers receiving below-average pricing who consume disproportionate service cost and generate minimal profit.

**Key questions:**
- What is the correlation between customer size (revenue) and price realization? (In well-structured pricing, larger customers receive modest volume discounts; in poorly structured pricing, the largest customers often receive the steepest discounts precisely because their size gives them negotiating leverage — which is economically backwards)
- What is the correlation between customer service cost (complexity of orders, customization requirements, payment terms) and price realization? (High-service-cost customers should receive lower discounts, not higher ones)
- Are there customer segments that are systematically under- or over-priced relative to the value they receive?

### Lens 3: Product and Segment Pricing Architecture

Examine the pricing architecture — how products are priced relative to each other and relative to competitive alternatives.

**Architecture questions:**
- Is the pricing architecture value-based or cost-plus? Value-based pricing sets prices based on the value the product creates for the customer; cost-plus pricing sets prices based on production cost plus a margin target. Cost-plus architectures systematically underprice high-value products and overprice low-value ones.
- Is there a coherent "good-better-best" product and pricing tier structure? If not, customers default to the cheapest option because there is no architecture that guides them toward higher-value choices.
- What is the price gap to the nearest competitor at each product tier? Is the gap justified by the value differential, or is there an opportunity to narrow or widen it?
- Are there products or services that are priced as line items but bundled in practice? (Unbundled pricing often reveals that add-on services are being given away for free in practice)

### Lens 4: Sales and Pricing Behavior

The most carefully designed pricing architecture is undermined by a sales force that discounts freely. Understanding sales pricing behavior — who discounts, how much, under what circumstances — is critical to diagnosing the root cause of price leakage.

**Sales behavior diagnostic:**
- What is the distribution of discounts across the sales force? Is price leakage concentrated in a small number of high-discounting salespeople, or is it a system-wide pattern? (Concentrated pattern suggests a training or accountability issue; system-wide pattern suggests a structural pricing or incentive issue)
- What triggers discounts? Are discounts primarily given in competitive situations (where they may be economically rational), or routinely to avoid a difficult conversation (where they represent pure value destruction)?
- What is the authority structure for discounts? Who can approve what level of discount? Is the authority structure being followed? (Many organizations have formal discount approval processes that are routinely bypassed)
- What is the incentive structure for pricing? Are salespeople compensated on revenue (which incentivizes volume at any price) or on margin-adjusted revenue or pocket price (which incentivizes pricing discipline)?

### Lens 5: Competitive Pricing Intelligence

Pricing does not exist in a vacuum — it is set against the competitive reference frame that customers use to evaluate value.

**Competitive pricing intelligence methods:**
- Price point benchmarking: Systematic collection of competitor list prices and published rates (available for most B2C categories; requires reverse-engineering for B2B)
- Win/loss analysis: What proportion of competitive losses are price-related? (If less than 15–20% of losses are price-related, the company has significant pricing power it may not be fully exercising; if more than 40–50% are price-related, price may be the primary competitive issue)
- Customer surveys: Direct evidence of how customers perceive the price-value relationship relative to alternatives
- Distributor and channel intelligence: Distribution partners typically have direct visibility into competitor pricing and can provide intelligence that is not available from public sources

---

## The Pricing Architecture Design: Five Design Decisions

After the diagnostic, the pricing architecture redesign requires explicit choices on five design dimensions.

### Decision 1: Value Metric

The value metric is the unit that pricing is attached to. It is the most fundamental pricing architecture decision and the one most frequently chosen by default rather than by design.

**Example value metrics by business type:**
- Seat / user (software, professional services)
- Unit of output (manufacturing)
- Outcome achieved (consulting success fees, insurance)
- Time (professional services hourly billing)
- Subscription / access (media, SaaS)
- Usage (cloud computing, utilities)

**The value metric design question:** What metric best tracks the value the customer receives? A customer who uses your software more intensively receives more value — seat-based pricing does not capture this; usage-based pricing does. A customer who achieves better outcomes from your professional services receives more value — time-based billing does not capture this; outcome-based fees do.

Most businesses use the value metric that was adopted at founding because it was conventional, not because it optimally aligns price with value creation. The most significant pricing architecture gains often come from reconsidering the value metric.

### Decision 2: Tier Structure

The tier structure determines how price scales with value delivered. The most common tier architectures:

**Flat pricing:** Same price for all customers or usage levels. Simple to administer; does not capture value variation across customers. Appropriate only when customer value homogeneity is genuinely high.

**Volume tiers:** Price decreases with volume. The economic rationale is lower service cost at scale. The pricing design question: do the tier thresholds and discounts reflect actual service cost differentials, or are they arbitrary?

**Good-better-best:** Three product tiers at different price points, targeting three distinct customer segments or use cases. The design principle: the "good" tier should be genuinely good (not a stripped-down version designed to push customers to "better"), the "best" tier should be clearly differentiated on features that specific customers value, and the price gaps should reflect the value differential.

**Outcome or success-based tiers:** Price varies with the outcome achieved. Requires outcome measurement and attribution methodology — the central implementation challenge.

### Decision 3: Discount Authority and Policy

Discount authority design determines who can approve what level of discount and under what circumstances. The design should be anchored in three principles:

1. **Discounts require justification, not just approval.** The approval workflow should require the salesperson to document the specific business reason for the discount — competitive situation, strategic customer value, unusual service commitment. Generic approvals without justification should not be possible.

2. **Authority scales with economics.** Discounts up to X% require manager approval; discounts up to Y% require regional director approval; discounts above Z% require headquarters approval. The escalation thresholds should reflect the economics of the discount — the total economic impact of the discount, not just the percentage.

3. **Below-the-line allowances require the same governance as above-the-line discounts.** The most common governance failure: rigorous approval processes for invoice discounts, but no governance for the post-invoice allowances (rebates, chargebacks, co-op spending) that destroy equivalent value invisibly.

### Decision 4: Value Communication Architecture

Pricing architecture cannot succeed if salespeople cannot articulate the value of the product relative to the price. Value communication architecture is the set of tools, training, and supporting evidence that enables the sales force to hold the price.

**Components:**
- Value ROI calculators: customer-specific tools that quantify the value of the product in the customer's economic language
- Competitive differentiation evidence: specific, quantified claims about the performance advantages relative to named competitors
- Reference customer stories: customer-specific evidence of value delivered, with numbers
- Price anchoring tools: framing techniques that position the price in the context of the value (see `references/consulting-negotiation-fee-anchoring.md` for the general anchoring techniques; apply the same logic to client product pricing)

### Decision 5: Pricing Governance and Rhythm

Pricing should not be a set-and-forget exercise. A pricing governance model specifies when prices are reviewed, how market changes are incorporated, and who has authority to make pricing changes.

**Minimum viable pricing governance:**
- Annual pricing review: systematic assessment of list prices across all products against cost changes, value changes, and competitive position changes
- Event-triggered reviews: protocols for when pricing is reviewed outside the annual cycle (major cost input change, significant competitive move, product launch)
- Price change authority: who can change what prices without escalation; what requires executive approval

---

## Implementation: The Transition Management Challenge

Pricing architecture changes are among the most operationally complex changes to implement because they require simultaneous changes to systems, sales behavior, and customer agreements — often for large, active customer portfolios.

### The Implementation Sequencing

**Step 1: Lock the baseline.** Before any pricing change, document the current pocket price for every customer in the portfolio. This is the baseline against which realization improvement will be measured.

**Step 2: Segment the portfolio for transition.** Not all customers should transition simultaneously. Segment by: transition difficulty (customers with contractual pricing constraints that prevent immediate change), strategic importance (customers where pricing tension has the highest relationship risk), and upside potential (customers with the largest gap between current pocket price and target architecture).

**Step 3: New business first.** Price new business at the new architecture immediately. Never quote new customers at the old architecture — even temporarily. New business at the new price sets the market reference point.

**Step 4: Renewal events as transition triggers.** Use contract renewals and annual repricing events as the mechanism for transitioning existing customers. This is the least disruptive approach — the customer expects a pricing conversation at renewal and has time to adapt.

**Step 5: Proactive migration for high-priority accounts.** For customers where the gap between current and target pricing is large and the transition cannot wait for a natural renewal event, manage a proactive repricing conversation. Prepare the sales team with value evidence and the customer-specific ROI calculation. Set expectations internally that some customers will object; the objective is to retain the customer at the new price, not to avoid the conversation.

---

## Common Failure Modes

**The list price obsession.** The pricing analysis and redesign focuses entirely on list prices without addressing the discount structure and below-the-line leakage. A 5% list price increase that is accompanied by 5% more discounting produces no realization improvement. The pocket price is the only metric that matters.

**The pilot that never scales.** The new pricing architecture is tested in a pilot market or segment, produces encouraging results, and then sits in pilot indefinitely because the organizational change required to scale it is too difficult to manage. Prevention: design the scale-up plan at the same time as the pilot, not after it concludes.

**The sales force abandonment.** The pricing redesign is created by finance and strategy teams and handed to the sales force to implement without adequate training, tools, or incentive realignment. Sales people who lack the tools to hold the price will discount; sales people whose compensation does not change will optimize for the old metric. Prevention: sales enablement and incentive redesign must be part of the pricing program scope.

**The value communication gap.** The new pricing architecture reflects higher prices, but the value proposition has not been refreshed to support the higher price. Customers who pushed back on the old price at the old level will push back harder at the new level if the value communication has not changed. Prevention: value communication development must precede or accompany the pricing transition.

**The one-time capture.** The pricing program produces a realization improvement in Year 1 that is not sustained in Years 2–3 because the governance mechanism was not implemented. Without ongoing pricing governance, discount creep resumes, the sales force returns to old behaviors, and the realization gains are gradually eroded. Prevention: the governance and measurement system must be in place before the initial transition is complete.
