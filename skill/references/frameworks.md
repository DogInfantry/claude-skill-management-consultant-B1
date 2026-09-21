# Consulting Frameworks — Complete Toolkit

This is the full inventory of frameworks available to you. Never apply a framework mechanically — adapt it to the specific problem. Frameworks are scaffolding for thinking, not substitutes for it.

## Table of Contents
1. [Structuring Frameworks](#structuring-frameworks)
2. [Strategy Frameworks](#strategy-frameworks)
3. [Market & Competitive Analysis](#market--competitive-analysis)
   - [4P / Marketing Mix](#4p--marketing-mix)
   - [4A (Customer Access)](#4a-customer-access)
4. [Operations & Execution](#operations--execution)
5. [Financial & Valuation](#financial--valuation)
6. [Organization & People](#organization--people)
7. [Digital & Technology](#digital--technology)
8. [Framework Selection Guide](#framework-selection-guide)

---

## Structuring Frameworks

### MECE (Mutually Exclusive, Collectively Exhaustive)
The foundational principle of all consulting thinking. Any decomposition of a problem must have:
- **Mutually Exclusive**: No overlaps between categories. Each item belongs in exactly one bucket.
- **Collectively Exhaustive**: Nothing is left out. All possibilities are covered.

How to test MECE:
- Can I place every item in exactly one category? (ME test)
- Is there anything that doesn't fit in any category? (CE test)
- Common MECE splits: Internal vs. External, Revenue vs. Cost, Supply vs. Demand, Organic vs. Inorganic, Short-term vs. Long-term
- **Rule of thumb:** give each level 2–5 branches, ideally 3–4. One branch is not a split, and more than five usually means two levels have been merged. Label the levels (L0 = the question, L1 = revenue / cost, L2 = their drivers) so you can say which level you are working on.
- **Check exhaustiveness against the real business.** "R&D, manufacturing, distribution, sales & marketing" looks like a complete cost chain but leaves out procurement, G&A/overheads and after-sales service. Walk the chain end to end before you call it collectively exhaustive.

### Issue Trees
A hierarchical decomposition of a problem into sub-questions. Two types:

**Diagnostic Issue Tree** (Why-based): Starts with "Why is X happening?" and branches into possible causes.
```
Why is profit declining?
├── Revenue declining?
│   ├── Volume declining?
│   │   ├── Fewer customers?
│   │   └── Lower purchase frequency?
│   └── Price declining?
│       ├── Competitive pressure?
│       └── Mix shift to lower-price products?
└── Costs increasing?
    ├── Variable costs up?
    │   ├── Raw materials?
    │   └── Labor?
    └── Fixed costs up?
        ├── Rent/facilities?
        └── Overhead?
```

**Solution Issue Tree** (How-based): Starts with "How can we achieve X?" and branches into options.
```
How can we grow revenue by 20%?
├── Grow existing customers
│   ├── Increase purchase frequency
│   ├── Increase basket size / cross-sell
│   └── Reduce churn
├── Acquire new customers
│   ├── New segments
│   ├── New channels
│   └── New geographies
└── New products/services
    ├── Adjacent offerings
    └── New business models
```

### Hypothesis-Driven Thinking
Don't "boil the ocean." Start with a hypothesis and test it.

1. **Form hypothesis**: "We believe profit is declining because of rising raw material costs in the SMB product line"
2. **Identify analyses needed**: What data would prove/disprove this?
3. **Gather evidence**: Run the analyses
4. **Confirm or pivot**: Does the evidence support the hypothesis? If not, what does it point to?

**The initial-hypothesis loop, run with 80/20.**
1. Build the MECE tree.
2. *Generate* two or three candidate hypotheses from it, then *state* the most likely one crisply. Generate first, then define, not the other way round.
3. *Test* it first on the branch most likely to hold most of the effect. The 80/20 (Pareto) rule says a minority of causes usually drives most of the result; for example, a small share of customers or SKUs often produces most of the profit.
4. If the test confirms the hypothesis, go one level deeper on that branch. If it disproves it, pivot. The test still narrowed the tree, so the next hypothesis starts better informed.

### 5W1H (Problem Definition)
A clarifying-question checklist that pins a problem down before you structure it:
- **What** is the problem, stated as a measurable fact?
- **Where** was it found (site, line, region, channel)?
- **When** did it start, and is it gradual or sudden, one-off or recurring?
- **Who** found it, and who is affected?
- **Why** does it matter (impact, e.g. downtime or lost orders)?
- **How** big or severe is it (₹, units, customers)?

*Example.* A shaft is found oversized on one machine of one assembly line. That stopped assembly for ~2 hours and puts a large order at risk. Once each W is answered, the root-cause search (5 Whys / fishbone) has a tight scope.

Use it for clarifying questions in cases, quality problems, process fixes, and scoping a product or market-entry question. It pairs with the metric-drop protocol in `references/product-rca-casebank.md`.

### The Pyramid Principle (Barbara Minto)
Structure all communication top-down:
- **Governing Thought**: The single most important message (the answer)
- **Key Line**: 2-4 supporting arguments (MECE)
- **Support**: Evidence and data under each argument

Rules:
- Ideas at any level must be summaries of the ideas below them
- Ideas within a group must be logically ordered (time, structure, importance)
- Ideas within a group must be MECE

---

## Strategy Frameworks

### Porter's Five Forces
Analyze industry attractiveness and competitive dynamics:

1. **Threat of New Entrants**: Barriers to entry (capital, regulation, brand, network effects, switching costs)
2. **Bargaining Power of Suppliers**: Concentration, switching costs, forward integration threat
3. **Bargaining Power of Buyers**: Concentration, price sensitivity, switching costs, backward integration
4. **Threat of Substitutes**: Functional alternatives, price-performance trade-off, switching costs
5. **Competitive Rivalry**: Number of competitors, industry growth, differentiation, exit barriers

Key insight: The stronger these forces, the lower the industry profitability. Strategy is about positioning where forces are weakest.

**What strengthens each force** (the drivers to test when you rate a force high or low):

| Force | It gets stronger (worse for incumbents' profits) when… |
|---|---|
| **Competitive rivalry** | There are many rivals of similar size; fixed costs are high, which pushes firms to fill capacity with price cuts; products are poorly differentiated; industry growth is slow; exit barriers are high (specialised assets, long leases, labour rules). |
| **Threat of substitutes** | Substitutes are easy to find; switching to them is cheap; they offer a better price-performance trade-off; buyers are willing to experiment. |
| **Threat of new entrants** | Entry barriers are **low**: little scale advantage, modest capital needs, weak brands, loose regulation, easy access to distribution, low customer switching costs. Barriers work the opposite way to the other drivers in this table: *higher* barriers mean a *weaker* threat. |
| **Buyer power** | There are few buyers and each buys a lot; switching suppliers costs them little; substitutes exist; the product is undifferentiated; buyers could make it themselves (backward integration); buyers are price-sensitive (high elasticity). |
| **Supplier power** | The input matters a lot to our quality or cost; changing suppliers is expensive for us; there are few suppliers; suppliers could credibly move into our business (forward integration). |

**Usage tip:** don't force Five Forces onto a case as the whole structure. Use the forces inside a broader frame, e.g. to test "market attractiveness" in a market-entry case or the "competition" bucket in a cost–benefit case, and rate only the forces that bear on the question.

### 3C's (Company, Customer, Competitor)
A simple but powerful strategic triangle:
- **Company**: What are our capabilities, resources, and competitive advantages?
- **Customer**: Who are they, what do they value, how do they decide?
- **Competitor**: Who are they, what's their strategy, where are they vulnerable?

The sweet spot is where your capabilities match customer needs and competitors can't follow.

### 3C + 1P (adds the Product)
3C's plus a **Product** lens. It is the default qualitative scan for market entry, new products, new businesses, position assessment, growth, and divest/turnaround questions. Checklist by bucket:
- **Product.** What it is and why someone buys it. Is it a commodity or differentiable (and can differentiation be raised)? What are its complements (can it ride their growth)? Its substitutes (indirect competitors)? Its lifecycle stage (new vs. near-obsolete)?
- **Customer.** Segments with size, growth and share; trend vs. prior years; needs vs. wants; willingness to pay, price points and elasticity; disposable income.
- **Company.** Capabilities and technical edge, distribution channels, cost structure, brand perception and loyalty, culture and organisation, financial capacity.
- **Competition.** Concentration (monopoly → fragmented), share distribution, entry barriers, competitor behaviour (targets, pricing, distribution), regulation, industry lifecycle.

### McKinsey 7S Framework
Assess organizational alignment across 7 elements:

**Hard S's** (easier to change):
- **Strategy**: The plan to build competitive advantage
- **Structure**: How the organization is organized
- **Systems**: Processes, IT systems, performance management

**Soft S's** (harder to change):
- **Shared Values**: Core beliefs and culture
- **Skills**: Distinctive capabilities
- **Style**: Leadership and management approach
- **Staff**: People, talent management, development

Key insight: All 7 elements must align. Changing strategy without changing structure, systems, and skills leads to failure.

### Ansoff Growth Matrix
Four growth strategies based on market/product novelty:

|  | Existing Products | New Products |
|--|------------------|--------------|
| **Existing Markets** | Market Penetration (lowest risk) | Product Development |
| **New Markets** | Market Development | Diversification (highest risk) |

The matrix's core message is that **risk rises with novelty**: each step away from existing products and existing markets adds execution risk, so the expected return has to rise with it.

| Quadrant | What it means | Actions | Example (generic) |
|---|---|---|---|
| **Market penetration** | Sell more of today's products to today's market. | Promotion, loyalty and retention, deeper distribution, pricing moves. A price cut must be paid back by extra volume (see the price–volume rule in `case-type-cheat-sheets.md`, Card 4). | A phone maker sells its new model to its existing customer base. |
| **Market development** | Take existing products to new customers. | New geographies (domestic or international), new segments, new channels. | The same phone launches in a country where the brand has never sold. |
| **Product development** | Sell new products to the existing market. | R&D, line extensions, co-development partnerships. | The phone maker launches a wearable for its existing phone owners. |
| **Diversification** | New products in new markets. | Related diversification (it reuses a capability or the customer base) or unrelated diversification (new capability and new customers; highest risk). | An electronics maker starts a video-streaming service. It reaches its installed device base, so it is arguably *related* diversification. |

**Action line:** first choose between a market strategy and a product strategy based on the client's priorities and capabilities, then pick the quadrant. Acquisition, JV and partnership are **entry modes**, not quadrants, and each can serve any quadrant. Decide the quadrant first and the mode second.

### BCG Growth-Share Matrix
Classify business units by market growth and relative market share:
- **Stars** (high growth, high share): Invest heavily, future cash cows
- **Cash Cows** (low growth, high share): Harvest cash, fund stars
- **Question Marks** (high growth, low share): Invest selectively or divest
- **Dogs** (low growth, low share): Divest or manage for cash

**Action lines per quadrant:**
- **Stars.** Invest, innovate and defend share. They often use as much cash as they generate. A Star is defined by high relative share in a high-growth market; being first to market or a monopoly does not make a product a Star.
- **Cash Cows.** Strengthen the position, harvest the cash, and use it to fund Stars and selected Question Marks. Don't starve them into decline.
- **Question Marks.** Decide quickly: invest heavily enough to make them Stars, or exit. Half-funding them is the usual failure.
- **Dogs.** Harvest a Dog while it still generates cash. Divest or exit once it drains cash. "Liquidate immediately" is too absolute.

**Generic example (consumer electronics):**
- A flagship phone line with high share in a mature, slow-growing market is a **Cash Cow**, not a Star.
- A wearable line that leads a fast-growing category is a **Star**.
- A streaming-device line with small share in a growing category is a **Question Mark**.
- A legacy portable media player in a shrinking category is a **Dog**.

**Action line:** use the matrix to decide where portfolio cash goes (invest, hold, harvest, exit). It is not a cost-analysis tool. Where two variables are too thin to decide, move to the GE-McKinsey or IE matrix below.

### Value Chain Analysis (Porter)
Identify where value is created and where costs accumulate:

**Primary Activities**: Inbound logistics → Operations → Outbound logistics → Marketing & Sales → Service

**Support Activities**: Firm infrastructure, HR, Technology development, Procurement

Use to identify: Where do margins pool? Where are we strong/weak vs. competitors? Where can we differentiate?

### Blue Ocean Strategy
Instead of competing in existing markets (red oceans), create uncontested market space:
- **Eliminate**: Which factors can you remove entirely?
- **Reduce**: Which factors can you reduce well below industry standard?
- **Raise**: Which factors can you raise well above industry standard?
- **Create**: Which factors can you introduce that the industry has never offered?

### GE-McKinsey 9-Box Matrix
Evaluate business portfolio using Industry Attractiveness (high/medium/low) × Competitive Strength (high/medium/low). More nuanced than BCG matrix.

### Internal–External (IE) Matrix
A 9-cell portfolio tool that plots each division by two scores:
- **Internal Factor Evaluation (IFE)** score on the x-axis: weighted strengths and weaknesses, 1–4.
- **External Factor Evaluation (EFE)** score on the y-axis: weighted opportunities and threats, 1–4.

Bubble size shows each division's revenue share; a slice shows its profit share. Each axis splits into low (1.0–1.99), medium (2.0–2.99) and high (3.0–4.0). The three diagonal zones prescribe:
- **Grow & build** (top-left cells): intensive and integrative strategies.
- **Hold & maintain** (the diagonal): penetration and product development.
- **Harvest or divest** (bottom-right cells).

Use it when BCG's two variables (share, growth) are too thin. The IE matrix lets you weight many internal and external factors per division, and compare against rivals' matrices.

### PESTEL Analysis
Macro-environmental scanning:
- **Political**: Government stability, trade policy, regulation
- **Economic**: GDP growth, interest rates, inflation, exchange rates
- **Social**: Demographics, cultural trends, health consciousness
- **Technological**: R&D, automation, digital disruption
- **Environmental**: Climate, sustainability, waste regulations
- **Legal**: Employment law, consumer protection, antitrust

---

## Market & Competitive Analysis

### Market Sizing (TAM/SAM/SOM)
- **TAM** (Total Addressable Market): Total demand for the product/service
- **SAM** (Serviceable Addressable Market): TAM you can actually reach (geography, channel, capability)
- **SOM** (Serviceable Obtainable Market): SAM you can realistically capture

### STP (Segmentation, Targeting, Positioning)
1. **Segment** the market by needs, behaviors, demographics, or value
2. **Target** the most attractive segments (size, growth, profitability, fit)
3. **Position** your offering distinctively in the target segment's mind

### 4P / Marketing Mix
The four levers a company controls when it takes a chosen offer to a chosen segment. Run STP first: 4P assumes the target customer has already been picked.

**Product**
- What it is and does: specifications, features, quality level.
- Range: SKUs, variants, pack sizes. Pack size is often the affordability lever.
- Packaging and design.
- Positioning and differentiation: head-on in a crowded space, uncontested space, or an unserved white space.
- Substitutes, and how they compare on price and performance.
- Brand equity, and the risk of diluting it with a cheaper or off-brand variant.
- Lifecycle stage: introduction, growth, maturity, decline.

**Price**
- **Price elasticity:** how much volume moves when price moves.
- **Willingness to pay (WTP):** the target customer's WTP and the value they perceive; what they spend today for the same utility.
- **Switching:** how likely customers are to switch, and how easy it is for them.
- **Reference points:** our historical prices, substitute prices, competitor price points.
- **Architecture:** tiers, bundles, discount policy, payment terms such as instalments or subscription.
- The floor/ceiling logic and the price–volume arithmetic are in `case-types.md` (Pricing) and `case-type-cheat-sheets.md` (Card 4).

**Place**
- Channel types: modern retail, general trade, wholesale, online, omnichannel.
- Fit between each channel and the company's strategy and capabilities.
- What each intermediary does in the value chain, and the margin it takes.
- How much control the company has over the channel (pricing, display, data).
- Reach and availability: numeric distribution, stock-outs, rural depth.

**Promotion**
- The objective and the message: what the customer should know, feel or do.
- **Pull vs push:** consumer demand creation (advertising, digital, sampling) versus trade push (channel margins, schemes, sales force).
- The media and channel mix, and the budget.
- Effectiveness metrics: reach, cost per acquisition, conversion, repeat rate, return on spend.
- Retention and loyalty programmes that turn first purchases into repeat ones.

**Services extension (7P).** For a service, add **People** (who delivers it, and their training), **Process** (how it is delivered: wait times, steps, consistency) and **Physical evidence** (the environment and the tangible cues that signal quality).

**When 4P beats 3C.**
- Use **3C** (or 3C + 1P) for *whether* and *where* questions: strategic position, the entry decision, competitive response.
- Use **4P** for *how to sell* questions: a launch plan, a go-to-market design, or a volume decline already traced to the marketing mix (the product is fine, but the price, channel or message is off).
- 4P looks inside-out at the company's own levers, so it misses competitor moves and market shifts. Pair it with a competition check.

### 4A (Customer Access)
Awareness, Accessibility, Affordability and Availability together form the customer-side check on volume: can customers who want the product actually get it? Use it as the internal volume driver in profitability cases and as the reach test in entry, launch, pricing and growth cases. `references/case-type-cheat-sheets.md` has the definitions, India examples (rural availability, small-SKU affordability) and where the lens sits in each case type.

### Competitive Positioning Map
Plot competitors on 2 key dimensions (e.g., price vs. quality, convenience vs. selection) to identify white space and positioning opportunities.

### Jobs to Be Done (JTBD)
Customers don't buy products — they hire them to do a job. Understand:
- **Functional job**: What task are they trying to accomplish?
- **Emotional job**: How do they want to feel?
- **Social job**: How do they want to be perceived?

---

## Operations & Execution

### Lean / Six Sigma Basics
- **Value Stream Mapping**: Map every step in a process, classify as value-add vs. waste
- **8 Wastes (DOWNTIME)**: Defects, Overproduction, Waiting, Non-utilized talent, Transport, Inventory, Motion, Extra-processing
- **DMAIC**: Define → Measure → Analyze → Improve → Control

### McKinsey's Three Horizons of Growth
- **Horizon 1**: Core business — optimize and defend (0-12 months)
- **Horizon 2**: Emerging opportunities — build and scale (12-36 months)
- **Horizon 3**: Transformational bets — explore and experiment (36-72 months)

### RACI Matrix
Clarify roles in any initiative:
- **Responsible**: Does the work
- **Accountable**: Owns the outcome (only one per task)
- **Consulted**: Provides input
- **Informed**: Kept in the loop

### Implementation Roadmap
For any recommendation, build:
1. **Quick Wins** (0-3 months): Low effort, visible impact — builds momentum
2. **Core Initiatives** (3-12 months): Main value drivers
3. **Structural Changes** (12-36 months): Foundational shifts (org, tech, culture)

---

## Financial & Valuation

### Profitability Framework
```
Profit = Revenue − Costs
Revenue = Price × Volume
Volume = # Customers × Purchase Frequency × Units per Purchase
Costs = Fixed Costs + Variable Costs
Variable Costs = Volume × Cost per Unit
```

Always disaggregate one level deeper than you think necessary.

### DuPont Analysis
ROE = Net Margin × Asset Turnover × Financial Leverage

Decomposes return on equity into profitability, efficiency, and leverage — shows where returns are coming from.

### Unit Economics
- **CAC** (Customer Acquisition Cost): Total sales & marketing spend / # new customers
- **LTV** (Lifetime Value): Average revenue per customer × Gross margin × Average lifespan
- **LTV:CAC ratio**: Should be >3:1 for healthy business; payback <12-18 months
- **Contribution margin**: Revenue per unit − Variable cost per unit

### DCF (Discounted Cash Flow) Basics
Enterprise Value = Σ (Free Cash Flow_t / (1 + WACC)^t) + Terminal Value / (1 + WACC)^n

Key inputs: Revenue growth, margins, capex, working capital, WACC, terminal growth rate.

### Cost–Benefit Analysis (CBA)
Compare the present value of all benefits with the present value of all costs, including indirect and intangible ones such as disruption, training time and risk.
- **NPV model:** NPV = PV(benefits) − PV(costs). Proceed if NPV > 0; among options, pick the highest NPV.
- **Benefit–cost ratio:** BCR = PV(benefits) ÷ PV(costs). Proceed if BCR > 1; the usual lens for public and social projects.
- **Use for:** project go/no-go, comparing investments, hires, change initiatives, policy appraisal, stakeholder impact.

Always add a sensitivity on the one or two assumptions that flip the decision. Worked examples, including when NPV, IRR and PI disagree: `references/stats-and-capital-budgeting-primer.md`.

---

## Organization & People

### Change Management (Kotter's 8 Steps)
1. Create urgency
2. Form a guiding coalition
3. Create a vision
4. Communicate the vision
5. Empower action
6. Create short-term wins
7. Build on the change
8. Anchor in culture

### Talent and Capability Assessment
Assess along two dimensions: Performance (current results) × Potential (future growth). Creates 9-box grid for talent decisions.

### Organizational Design Principles
- Structure follows strategy
- Span of control: 5-8 direct reports optimal
- Decision rights must be clear
- Minimize layers between customer and CEO

---

## Digital & Technology

### Digital Maturity Assessment
Evaluate across: Customer experience, Operations, Business model, Organization & culture, Technology infrastructure

### Build vs. Buy vs. Partner
Decision framework:
- **Build**: Core differentiator, high strategic importance, have the capability
- **Buy**: Commodity capability, speed matters, proven solutions exist
- **Partner**: Complementary strengths, shared risk, market access

### Platform / Ecosystem Thinking
- **Network effects**: Does value increase with more users?
- **Multi-sided platforms**: Who are the sides? Who subsidizes whom?
- **Winner-take-all dynamics**: High switching costs + network effects = power law outcomes

---

## Framework Selection Guide

| Problem Type | Primary Framework | Supporting Frameworks |
|-------------|-------------------|----------------------|
| "Why is profit declining?" | Profitability tree | DuPont, Value chain |
| "Should we enter market X?" | 3C's + Market sizing | Porter's 5, PESTEL, Ansoff |
| "How to grow revenue?" | Ansoff + Solution tree | STP, JTBD, Three Horizons |
| "Evaluate this acquisition" | 3C's + Synergy analysis | DCF, Value chain, 7S |
| "Optimize operations" | Lean / Value stream | DMAIC, 8 Wastes, Benchmarking |
| "Build a strategy" | Porter's 5 + 3C's | Blue Ocean, BCG matrix, PESTEL |
| "Organizational change" | 7S + Kotter | RACI, Talent 9-box |
| "Pricing strategy" | Value-based pricing | Price elasticity, Competitive positioning |
| "Digital transformation" | Digital maturity | Build/Buy/Partner, Three Horizons |
| "Should we launch/enter with this product?" | 3C + 1P | Market sizing, Porter's 5, Ansoff |
| "Which divisions to grow, hold or exit?" | IE matrix | BCG matrix, GE-McKinsey 9-box |
| "Is this project/policy worth it?" | Cost–benefit (NPV/BCR) | Sensitivity analysis, DCF |
| "Pin down a vague problem fast" | 5W1H | 5 Whys, Issue tree |
| "How should we take this product to market?" | STP → 4P | 4A, JTBD, Channel economics |
| "Volume is down but the market is growing" | Profitability tree (volume branch) | 4A, 4P |

Remember: the best consultants combine frameworks fluidly. A profitability case might require market sizing, competitive analysis, and operational diagnostics all in one engagement. Let the problem guide your toolkit, not the other way around.
