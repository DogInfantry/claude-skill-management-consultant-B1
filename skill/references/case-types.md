# Case Type Playbooks

Every consulting case falls into a handful of archetypes. This reference gives you the playbook for each: the standard structure, key questions, common traps, and what "great" looks like.

## Table of Contents
1. [Profitability / Turnaround](#profitability--turnaround)
2. [Market Entry](#market-entry)
3. [Growth Strategy](#growth-strategy)
4. [M&A and Due Diligence](#ma-and-due-diligence)
5. [Pricing](#pricing)
6. [Operations / Cost Reduction](#operations--cost-reduction)
7. [Digital Transformation](#digital-transformation)
8. [Org Design & Change Management](#org-design--change-management)
9. [New Product / Go-to-Market](#new-product--go-to-market)

---

## Profitability / Turnaround

**The question**: "Why is our profitability declining and how do we fix it?"

### Standard Structure
```
Profit Decline
├── Revenue Issues
│   ├── Volume decline
│   │   ├── Market shrinking? (external)
│   │   ├── Losing share? (competitive)
│   │   └── Channel / distribution issues?
│   └── Price decline
│       ├── Competitive pressure?
│       ├── Mix shift (lower-value products)?
│       └── Discounting / promotions?
└── Cost Issues
    ├── COGS increasing
    │   ├── Input costs?
    │   ├── Manufacturing inefficiency?
    │   └── Scale loss (volume decline → higher unit costs)?
    └── SGA / Overhead increasing
        ├── Headcount growth outpacing revenue?
        ├── Marketing spend efficiency declining?
        └── One-time costs?
```

### Driver Split: Internal vs External, Plus a One-Off Bucket
The standard tree tells you *where* profit went. Splitting every revenue driver into **internal** (inside management's control) and **external** (market, regulation, competitors) tells you *whether the client can fix it*, which is what the recommendation depends on. It also answers the clarifier "industry-wide or just us?" driver by driver instead of once for the whole case.

```
Profit = Revenue − Cost
├── Revenue = Σ (Price × Volume) across the product mix
│   ├── Volume (units sold)
│   │   ├── Internal: the 4A access lens (Awareness, Accessibility, Availability, Affordability)
│   │   └── External: economic cycle, regulation, competitor moves, industry trends, geography
│   ├── Price per unit
│   │   ├── Internal: pass-through of our own cost increases, discount policy, transfer pricing
│   │   └── External: price wars, regulated channel margins, price caps, customer sentiment, supply–demand balance
│   └── Mix: shift towards lower-margin products, channels or regions
└── Cost
    ├── Fixed: depreciation, salaries, rent, insurance
    ├── Variable: raw material, fuel, freight, packaging, sales commissions
    ├── Semi-variable: utilities, maintenance (a fixed base plus a usage-driven part)
    └── One-off / non-operating: write-offs, impairments, restructuring charges, litigation settlements
```

- **Normalise before you diagnose.** Strip the one-off bucket first. [ILLUSTRATIVE] Margin falls from 12% to 7% on revenue of Rs 1,000 crore, and the year includes a Rs 30 crore inventory write-off. Normalised profit = 70 + 30 = Rs 100 crore, a 10% margin. The one-off explains 3pp of the 5pp drop; only **2pp** is operating decline, and that is the part the tree has to explain.
- **Transfer pricing moves profit between group entities; it does not create it.** It changes one segment's reported margin but not the consolidated total, so confirm which P&L the question is about before you chase it.
- The 4A lens and where it sits in each case type are in `references/case-type-cheat-sheets.md` ("The 4A customer-access lens"). Card 1 there is the one-page profitability version of this playbook.
- **Error fixed:** filing "standard costs" under one-off costs → standard costing is a budgeting and inventory-valuation method, and variances from standard are operating costs that belong in the fixed or variable buckets (only genuinely non-recurring items go in the one-off bucket).
- **Trap:** reading a reported margin drop as operating decline without checking the one-off bucket. Recommending cost cuts against a write-off is the classic wasted recommendation.

### Cost Checklist: Value-Chain Lens and P&L-Line Lens
When the fixed/variable split is not MECE (utilities and maintenance straddle it), or the question is *where* costs sit, walk the value chain end to end. When the data arrives as a P&L, use the line-item lens. Pick one per branch; don't mix them in the same level of the tree.

**Value-chain lens (7 stages)**

| Stage | Cost lines to check | Typical lever |
|---|---|---|
| **Planning** | Forecasting error (excess stock, expediting), technology and equipment plan, capex phasing | Better forecasting, phased capex |
| **Raw material / procurement** | Price per unit, contract terms, supplier concentration, specifications | Bulk contracts, alternative suppliers, specification changes |
| **Processing** | Machine uptime, labour productivity, capacity utilisation, yield and scrap, packaging | Utilisation, automation, scrap reduction, pack redesign |
| **Storage** | Warehousing footprint, holding cost, obsolescence | Fewer, better-placed warehouses; lower safety stock |
| **Transportation** | Inbound and outbound logistics, network design, mode (road, rail, sea), load factor | Network redesign, mode shift, fuller loads |
| **Distribution / sales** | Channel margins, sales-force cost and productivity, go-to-market model, marketing technology, training | Channel mix, sales-force productivity |
| **Customer service** | Returns, warranty replacements, annual maintenance contracts, spares | Quality fixes upstream, spares pricing |

**P&L-line lens**
- **Cost of goods sold (COGS)** = opening inventory + purchases − closing inventory. [ILLUSTRATIVE] Opening stock Rs 20 crore, purchases Rs 100 crore, closing stock Rs 30 crore → COGS = **Rs 90 crore**. The Rs 10 crore gap between purchases and COGS is a stock build (30 − 20), which is a working-capital problem, not a margin problem.
- **SG&A:** selling, general and administrative costs, i.e. everything not directly tied to producing the goods or service.
- **R&D:** developing and testing new products.
- **Marketing:** promotion spend. It usually sits inside SG&A; break it out only if SG&A is then defined to exclude it.
- **Interest, tax and other:** below the operating line. They are financing and tax questions, not operating ones.

- **Error fixed:** treating purchases as the cost of sales ("cost = Rs 100 crore") → COGS = 20 + 100 − 30 = Rs 90 crore (the extra Rs 10 crore went into inventory; calling it cost overstates the margin problem and hides the cash tied up in stock).
- **Error fixed:** listing marketing as its own line *and* inside SG&A → count it once (the double count inflates overheads and sends the diagnosis to the wrong branch).
- **Trap:** counting the cost of finance twice, once under Planning and again under Interest. Also, an inventory-valuation change (FIFO to weighted average) moves reported COGS but not cash cost; LIFO is not permitted under IFRS or Ind AS.

### Key Questions
- Is this a company-specific problem or an industry-wide trend?
- When did the decline start? What changed?
- Which products/segments/geographies are affected most?
- Revenue problem, cost problem, or both?

### What Great Looks Like
- Quickly identifies whether it's revenue or cost driven (don't boil the ocean)
- Disaggregates to find the specific driver (not just "costs are up" but "freight costs in the Southeast region increased 30% due to carrier consolidation")
- Quantifies the gap: "Margin declined 8pp; 5pp from input costs, 3pp from mix shift"
- Recommends specific, prioritized actions with financial impact estimates

---

## Market Entry

**The question**: "Should we enter market X, and if so, how?"

### Standard Structure
```
Market Entry Decision
├── Market Attractiveness
│   ├── Size and growth (TAM/SAM/SOM)
│   ├── Profitability (industry margins, competitive intensity)
│   ├── Trends and tailwinds
│   └── Regulatory / barriers
├── Competitive Landscape
│   ├── Who are the incumbents?
│   ├── What's their positioning?
│   ├── Are there gaps / underserved segments?
│   └── How would they respond to our entry?
├── Company Fit
│   ├── Do we have relevant capabilities?
│   ├── Can we leverage existing assets (brand, distribution, tech)?
│   ├── What capabilities would we need to build?
│   └── Strategic fit with overall portfolio
└── Entry Strategy (if go)
    ├── Organic build vs. Acquisition vs. Partnership
    ├── Target segment and positioning
    ├── Go-to-market approach
    ├── Investment required and expected returns
    └── Timeline and milestones
```

### Key Questions
- Why this market? Why now?
- What's our right to win? (What gives us an advantage over incumbents?)
- What's the minimum viable entry — can we test before committing fully?
- What would make us walk away? (Define kill criteria upfront)

### What Great Looks Like
- Doesn't just say "the market is attractive" — quantifies and compares to alternatives
- Has a clear articulation of competitive advantage (not just "we're a good company")
- Models the economics: investment required, time to breakeven, 5-year NPV
- Considers competitive response: "When we enter, Competitor A will likely do X"

---

## Growth Strategy

**The question**: "How do we grow revenue/profit by X% over Y years?"

### Standard Structure
Use the Ansoff Matrix as the top level:
```
Growth Strategy
├── Grow Core (existing products × existing markets)
│   ├── Increase share of wallet / cross-sell
│   ├── Improve retention / reduce churn
│   ├── Optimize pricing
│   └── Improve sales effectiveness
├── Expand Markets (existing products × new markets)
│   ├── New geographies
│   ├── New customer segments
│   └── New channels
├── Expand Products (new products × existing markets)
│   ├── Adjacent products/services
│   ├── Product line extensions
│   └── Value-added services
└── Transform (new products × new markets)
    ├── New business models
    ├── Platform / ecosystem plays
    └── M&A for capabilities
```

### Key Questions
- What's the growth gap? (Target minus organic baseline)
- Which levers have the highest impact-to-effort ratio?
- Do we have the capabilities for each growth vector?
- How much investment is required, and what's the expected return for each?

---

## M&A and Due Diligence

**The question**: "Should we acquire Company X? What is it worth? What are the risks?"

### Standard Structure
```
M&A Evaluation
├── Strategic Rationale
│   ├── Why this target?
│   ├── Strategic fit and synergies
│   ├── Revenue synergies (cross-sell, new markets, pricing power)
│   └── Cost synergies (duplicative functions, scale economies, procurement)
├── Standalone Valuation
│   ├── DCF analysis
│   ├── Comparable company analysis (trading multiples)
│   ├── Precedent transactions
│   └── Synergy-adjusted valuation
├── Due Diligence Risks
│   ├── Financial (quality of earnings, working capital, off-balance sheet)
│   ├── Commercial (customer concentration, competitive position, market trends)
│   ├── Operational (integration complexity, key person risk, IT systems)
│   ├── Legal / regulatory (antitrust, litigation, compliance)
│   └── Cultural (integration risk, retention of key talent)
└── Integration Plan
    ├── Day 1 readiness
    ├── First 100 days priorities
    ├── Synergy capture timeline
    └── Integration governance
```

### Choosing the Lens: Deal Lifecycle vs Environment
Two structures cover M&A cases. Pick by what the case centres on.

**Deal-lifecycle lens.** Use it when the case is about screening, diligence, integration or exit.
```
Overall deal
├── Transaction
│   ├── Internal need analysis: why acquire; quantify the goal (revenue, capability, share)
│   ├── Target screening: market understanding, target performance, shortlist
│   ├── Valuation: standalone value, synergy PV, walk-away price (run alongside diligence)
│   ├── Due diligence: financial, commercial, operational, legal; management; lessons from past deals
│   └── Deal execution: price and structure (cash vs stock, earn-outs), funding, timeline
└── Beyond the transaction
    ├── Post-deal integration: set-up and consolidation, governance, technology, operating model
    └── Exit (financial buyers only): stake sale to a strategic, secondary sale to another fund, listing
```

**Environment lens.** Use it when M&A is one option inside a bigger question (a growth or entry case where "acquire" competes with "build" or "partner").
- **Acquirer:** financial position, growth, capabilities, management, culture.
- **Target:** the same attributes, tested for quality and sustainability.
- **Market:** size, growth, profitability, competition.
- **Synergies:** revenue, cost and financial; business overlap is where they come from.
- **Risk:** integration risk, regulatory limits, key-talent retention.
- Cross-cutting considerations: deal rationale, financing, structure.

**Combine them.** Use the environment lens for the go/no-go, then open the lifecycle branch the interviewer steers you towards. `references/case-type-cheat-sheets.md` (Card 5) has the one-page version with the clarifier bank.

### The Walk-Away Inequality
The deal creates value only if:

`Standalone value + PV(synergies) − Integration cost > Price paid`

The left-hand side is the **walk-away price**, a ceiling, not a bid. [ILLUSTRATIVE, Rs crore] Standalone value 1,000. Run-rate synergies of 60 a year, capitalised at 10%, are worth 600 at run rate, but they arrive after a two-year ramp, so PV = 600 / 1.1² ≈ **496**. Integration cost 100.
- Walk-away price ≈ 1,000 + 496 − 100 ≈ **1,400** (1,396).
- A bid of 1,200 keeps about **196** of value for the acquirer. A bid of 1,400 hands every synergy rupee to the seller.
- **Error fixed:** adding run-rate synergies undiscounted (1,000 + 600 − 100 = 1,500) → discount for time-to-capture: 1,000 + 496 − 100 ≈ 1,400 (counting synergies as if captured on day 1 overstates the ceiling by about 100).
- **Trap:** recommending the deal without price guidance. Always close with the walk-away price and a target bid below it.

### Exit Strategy: A Branch for Financial Buyers Only
A strategic buyer holds the asset and values synergies. A financial buyer values the return, so the exit is a full branch of the tree: route (stake sale to a strategic, secondary sale to another fund, listing), timing, and exit value = exit EBITDA × exit multiple. Don't assume the multiple expands.
- [ILLUSTRATIVE] In at Rs 1,000 crore, out at Rs 2,000 crore after 5 years: money multiple 2.0×, IRR = 2^(1/5) − 1 ≈ **14.9%**. Against a 20% hurdle the deal fails. Clearing it needs 1.2⁵ ≈ 2.49×, i.e. an exit near Rs 2,490 crore.
- **Error fixed:** "2× over 5 years is 20% a year" (100% ÷ 5) → the compound IRR is 14.9% (a simple average ignores compounding and overstates the return).

### Key Questions
- What's the strategic rationale beyond "it's a good company"?
- Are synergies realistic and achievable? (Most acquirers overestimate synergies by 25-40%)
- What's the maximum price we should pay? (Walk-away price)
- What are the integration deal-breakers?

### What Great Looks Like
- Separates "nice to have" synergies from "will actually happen" synergies
- Has a realistic integration plan (not just "we'll figure it out")
- Models scenarios: base case, upside, downside
- Identifies the 2-3 things that must be true for this deal to create value

---

## Pricing

**The question**: "How should we price our product/service?"

### Standard Structure
```
Pricing Strategy
├── Cost-Based Floor
│   ├── Variable cost per unit
│   ├── Allocated fixed costs
│   └── Minimum acceptable margin
├── Value-Based Ceiling
│   ├── Customer willingness to pay
│   ├── Value delivered vs. next best alternative
│   └── Price sensitivity / elasticity
├── Competitive Reference
│   ├── Competitor pricing
│   ├── Market price expectations
│   └── Price positioning (premium, parity, value)
└── Pricing Architecture
    ├── Pricing model (per unit, subscription, freemium, tiered)
    ├── Price discrimination / segmentation
    ├── Bundling strategy
    └── Promotional / discount policy
```

### Key Questions
- What value do we create for the customer? Can we quantify it?
- What's the customer's next best alternative and what does it cost?
- How price-sensitive is demand? (Elasticity)
- Are there opportunities for price discrimination (different prices for different segments)?

---

## Operations / Cost Reduction

**The question**: "How do we reduce costs by X% without hurting quality/growth?"

### Standard Structure
```
Cost Reduction
├── Cost Baseline
│   ├── Total cost structure (fixed vs. variable breakdown)
│   ├── Cost by category (labor, materials, overhead, etc.)
│   └── Benchmarking vs. best-in-class
├── Efficiency Levers
│   ├── Process optimization (lean, automation)
│   ├── Procurement savings (consolidation, renegotiation, specification changes)
│   ├── Footprint optimization (facility consolidation, near/offshoring)
│   └── Organizational simplification (delayering, shared services)
├── Strategic Cost Choices
│   ├── Make vs. buy decisions
│   ├── Product/service rationalization (kill unprofitable lines)
│   └── Scope reduction (what should we stop doing?)
└── Implementation
    ├── Quick wins (0-6 months)
    ├── Medium-term initiatives (6-18 months)
    ├── Structural changes (18+ months)
    └── Tracking and governance
```

---

## Digital Transformation

**The question**: "How should we use technology/digital to transform our business?"

### Standard Structure
```
Digital Transformation
├── Customer-Facing
│   ├── Digital channels (e-commerce, mobile, self-service)
│   ├── Personalization and CX
│   ├── Digital marketing and acquisition
│   └── Omnichannel integration
├── Operations
│   ├── Process automation (RPA, AI)
│   ├── Data and analytics capabilities
│   ├── Supply chain digitization
│   └── IoT and connected products
├── Business Model
│   ├── Platform / marketplace opportunities
│   ├── As-a-service models
│   ├── Data monetization
│   └── Ecosystem partnerships
└── Enablers
    ├── Technology infrastructure and architecture
    ├── Data strategy and governance
    ├── Talent and skills
    ├── Agile ways of working
    └── Change management
```

---

## Org Design & Change Management

**The question**: "How should we organize to execute our strategy?"

### Standard Structure
```
Organization Design
├── Strategic Requirements
│   ├── What does the strategy demand from the organization?
│   ├── Key capabilities needed
│   └── Decision-making speed requirements
├── Structure Options
│   ├── Functional, divisional, matrix, or hybrid?
│   ├── Centralize vs. decentralize decisions
│   ├── Spans and layers
│   └── Shared services vs. embedded
├── Operating Model
│   ├── Governance and decision rights
│   ├── Key processes and handoffs
│   ├── Performance management
│   └── Talent and capability building
└── Change Plan
    ├── Stakeholder mapping and engagement
    ├── Communication strategy
    ├── Transition plan and timeline
    └── Quick wins to build momentum
```

---

## New Product / Go-to-Market

**The question**: "How should we launch this new product/service?"

### Standard Structure
```
Go-to-Market Strategy
├── Product-Market Fit
│   ├── Target customer and need
│   ├── Value proposition
│   ├── Competitive differentiation
│   └── Pricing
├── Channel Strategy
│   ├── Direct vs. indirect
│   ├── Online vs. offline
│   ├── Partnership / distribution
│   └── Channel economics
├── Demand Generation
│   ├── Awareness building
│   ├── Lead generation
│   ├── Sales process and conversion
│   └── Customer success and expansion
└── Launch Plan
    ├── Pilot / beta strategy
    ├── Geographic / segment sequencing
    ├── Resource requirements
    └── Success metrics and pivot criteria
```

### Key Questions
- Do we have product-market fit, or are we still searching?
- What's the sales motion? (Self-serve, inside sales, field sales, partner-led?)
- What's the unit economics story? (CAC, LTV, payback)
- What would cause us to kill this product?
