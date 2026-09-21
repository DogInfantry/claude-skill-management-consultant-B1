# Functional Deep Dives — Supply Chain, Procurement, IT & HR Transformation

Each of these functions is a consulting discipline in its own right. This reference gives you the analytical frameworks, diagnostic tools, key metrics, and transformation playbooks to work credibly across all four.

## Table of Contents
1. [Supply Chain Strategy & Transformation](#supply-chain-strategy--transformation)
2. [Procurement Excellence](#procurement-excellence)
3. [IT Strategy & Transformation](#it-strategy--transformation)
4. [HR & Talent Transformation](#hr--talent-transformation)

---

## Supply Chain Strategy & Transformation

### What Supply Chain Consulting Actually Covers
Supply chain is end-to-end: from raw material sourcing through to delivery to the end customer. It includes:
- **Planning**: Demand forecasting, supply planning, inventory policy, S&OP
- **Sourcing**: Supplier selection, contracts, risk management
- **Manufacturing / Operations**: Production planning, capacity management, quality
- **Logistics**: Warehousing, transportation, last-mile, returns
- **Technology**: ERP, WMS, TMS, demand sensing, control tower

### Key Metrics

| Metric | Formula | World-Class Benchmark |
|--------|---------|----------------------|
| Perfect Order Rate | Orders with no errors / Total orders | >98% |
| On-Time In-Full (OTIF) | Orders delivered on time + full quantity / Total | >95% |
| Inventory Days (DIO) | (Inventory / COGS) × 365 | Industry-specific; ~15-30 days for FMCG |
| Cash-to-Cash Cycle | DSO + DIO − DPO | Minimize; best-in-class have negative cycles |
| Fill Rate | Units shipped / Units ordered | >99% |
| Forecast Accuracy | 1 − MAPE (mean absolute % error) | >80% at SKU/week level |
| Logistics Cost as % of Revenue | Freight + warehouse / Revenue | 5-10% for B2C; 2-5% for B2B |
| Supply Chain Cost as % of Revenue | Total SC cost / Revenue | 4-8% for manufacturing |

### The Supply Chain Diagnostic

**Step 1: Segment the portfolio**
Not all SKUs, customers, and flows are equal. Segment by:
- Volume / value (ABC analysis: A = top 80% of volume, B = next 15%, C = bottom 5%)
- Demand variability (high vs. low coefficient of variation)
- Criticality (what happens if this is out of stock?)
→ High-value/high-variability products need different treatment than low-value/predictable ones.

**Step 2: Map the value stream**
Draw the end-to-end flow for your top 3-5 product families. For each step, record:
- Cycle time (how long does this step take?)
- Lead time (how long does the customer wait for this step?)
- Inventory days at this stage
- Key pain points / failure modes

**Step 3: Benchmark**
Compare to best-in-class on the key metrics above. Quantify the "prize" — if fill rate improved from 94% to 99%, what is the revenue protection value? If DIO improved from 45 to 30 days, what cash is released?

**Step 4: Root cause the gaps**
Common root causes by problem type:

| Problem | Common Root Causes |
|---------|-------------------|
| Poor forecast accuracy | Siloed planning (S&OP doesn't work), poor data quality, no statistical forecasting |
| High inventory / stockouts | Batch-driven ordering, poor ABC segmentation, inaccurate lead times, no safety stock logic |
| High logistics cost | Mode suboptimization, poor network design, carrier fragmentation, no freight audit |
| OTIF failures | Upstream supplier variability, production planning failures, transportation unreliability |
| Long cash-to-cash cycle | High DSO (credit policies), high inventory, low DPO (not using full payment terms) |

### Supply Chain Transformation Levers

**Network Design**: Where should you manufacture, warehouse, and distribute? Network optimization (using linear programming tools) can reduce logistics cost 10-20% while improving service.

**S&OP / IBP (Integrated Business Planning)**: The process that aligns demand, supply, and financial planning. A world-class S&OP process significantly reduces inventory while improving service. Most companies have the process on paper; few have it working well.

**Supplier Segmentation & Dual Sourcing**: Categorize suppliers by strategic importance and supply risk. Critical single-source suppliers are existential vulnerabilities. Build redundancy into the top 10-20 critical categories.

**Digital / Control Tower**: Real-time visibility across the end-to-end supply chain. When you can see everything, you can act before problems become crises.

**Nearshoring / Reshoring**: Post-COVID and in the context of geopolitical risk, many companies are moving supply closer to demand. The analysis: logistics cost savings + resilience value vs. higher unit manufacturing cost.

---

## Procurement Excellence

### The Procurement Maturity Curve

**Level 1 — Transactional**: Procurement is order processing. No strategy, no leverage, no market intelligence.

**Level 2 — Commercial**: Negotiation is active. Some category management. Vendor consolidation underway.

**Level 3 — Strategic Sourcing**: Category strategies, supplier development, total cost of ownership, demand management.

**Level 4 — Value Chain Integration**: Joint innovation with suppliers, supply chain financing, should-cost modeling, ESG-linked contracts.

Most companies are at Level 2. World-class is Level 3-4.

### The Strategic Sourcing Process

1. **Spend Analysis**: Cleanse and categorize all spend. Who are we buying from? How much? For what? (This alone often reveals 15-20% of spend is duplicated or unmanaged.)

2. **Category Segmentation** (Kraljic Matrix):
   - **Strategic** (high spend, high supply risk): Manage relationship closely; develop suppliers; don't over-rely
   - **Leverage** (high spend, low supply risk): Drive hard on price; competitive bidding; consolidate to fewer suppliers
   - **Bottleneck** (low spend, high supply risk): Ensure supply security; accept higher cost for reliability
   - **Non-Critical** (low spend, low risk): Simplify and automate; e-procurement; reduce transaction cost

3. **Should-Cost Modeling**: Build a model of what the product/service should cost based on raw material costs, labor, overhead, and margin. Gives you a fact-based anchor for negotiation.

4. **RFP / Competitive Sourcing**: Issue to 3-5 suppliers. Evaluate on: price, quality, service, capability, financial stability, ESG profile.

5. **Negotiation**: Use the frameworks in `references/negotiations.md`.

6. **Supplier Management**: Post-contract, manage performance against SLAs. Annual business reviews. Relationship investment proportional to strategic importance.

### Procurement Savings Categories & Typical Ranges

| Lever | Typical Savings |
|-------|----------------|
| Competitive resourcing / RFP | 8-15% on addressable spend |
| Volume consolidation | 5-12% |
| Specification rationalization | 5-20% (depending on over-specification) |
| Demand management | 5-30% (do we need this at all? At this quantity?) |
| Payment term extension | Cash flow benefit: 1-3% of spend value |
| Supplier-led innovation | Highly variable; can reduce cost + improve quality |
| Make vs. buy shift | Highly variable |

### The Procurement Business Case
Total savings opportunity = Addressable spend × Average savings rate

- Addressable spend ≠ total spend (some spend is locked in contracts, regulatory requirements, or sole-source)
- Typical addressable spend: 50-70% of total indirect; 30-60% of total direct

---

## IT Strategy & Transformation

### The IT Consulting Agenda

IT consulting spans four domains:
1. **IT Strategy**: What should IT do, prioritize, and invest in?
2. **Application Rationalization / Modernization**: Legacy systems → modern architecture
3. **Cloud Migration**: Moving infrastructure and applications to the cloud
4. **Digital / Data Platforms**: Building the technology foundation for digital transformation

### IT Assessment Framework

**Demand side** (What does the business need from IT?):
- What are the top business priorities in the next 3 years?
- Which business capabilities are bottlenecked by technology?
- What's the digital ambition? (Automate? Transform? Disrupt?)

**Supply side** (What can IT actually deliver?):
- Application portfolio: How many apps? What % are legacy / end-of-life?
- Technical debt: How much of IT budget goes to "keeping the lights on" vs. new development?
- Talent: In-house vs. outsourced; skill gaps?
- Architecture: Monolithic vs. microservices? Cloud % vs. on-premise?

**Gap analysis**: Where demand exceeds supply → investment priorities.

### Key IT Metrics

| Metric | Benchmark |
|--------|-----------|
| IT spend as % of revenue | 2-5% (manufacturing), 5-10% (financial services), 8-15% (tech) |
| % of IT budget on "run" vs. "change" | Best-in-class: 50/50; typical: 70% run, 30% change |
| Application rationalization target | Reduce portfolio by 20-40% over 3-5 years |
| Cloud adoption | >60% of workloads in cloud is the 2025+ target |
| Mean Time to Recover (MTTR) | <4 hours for critical systems |
| IT project on-time/on-budget rate | Industry average: 30%; best-in-class: 70%+ |

### The Application Rationalization Playbook

Large organizations often have 500-2,000+ applications. Most are duplicative, outdated, or both.

**Step 1: Inventory** — List every application with: business owner, user count, annual cost (license + support + hosting), age, and criticality.

**Step 2: Rationalization options for each app:**
- **Retain**: Modern, strategic, worth keeping
- **Retire**: No longer used or needed; shut down
- **Replace**: Replace with modern SaaS equivalent
- **Rehost** (Lift & Shift): Move to cloud as-is (quick; limited benefit)
- **Replatform**: Move to cloud with minor modifications
- **Refactor / Re-architect**: Rebuild for cloud-native (expensive; high benefit for core systems)
- **Consolidate**: Merge 3 apps doing the same thing into 1

**Step 3: Sequence** — By dependency, business criticality, and ease.

**Typical value**: 30-40% reduction in application portfolio → 20-30% reduction in IT operating cost + significantly faster delivery speed.

### Cloud Strategy

The cloud decision isn't binary. Most enterprises adopt a hybrid multi-cloud model.

**Why cloud?**
- Elasticity: Scale up and down without capex
- Speed: Deploy in days vs. months
- Capability: Access to AI/ML, analytics, security tools from cloud providers
- Cost (usually): Operational vs. capital; pay-for-what-you-use

**Cloud providers comparison:**
- **AWS**: Market leader, broadest service portfolio, strongest for data/ML (S3, EC2, SageMaker)
- **Azure**: Strong enterprise integration (Active Directory, Office 365), strong in regulated industries
- **GCP**: Data and AI/ML leadership (BigQuery, Vertex AI), strong for analytics-heavy workloads

**Total Cost of Ownership (TCO) for cloud migration:**
Don't just compare infrastructure cost. Include:
- Migration cost (one-time)
- Application re-architecture cost
- Staff retraining
- Ongoing cloud management and optimization
- License cost changes (some on-prem licenses don't transfer to cloud)

---

## HR & Talent Transformation

### The HR Transformation Agenda

HR consulting covers three layers:
1. **Workforce Strategy**: What talent does the organization need? Where? When?
2. **Talent Processes**: How does the organization attract, develop, manage, and retain talent?
3. **HR Function Transformation**: How should the HR function itself be organized and what technology does it need?

### Workforce Planning Framework

**Step 1: Demand** — What talent does the future strategy require?
- What capabilities are needed in 3-5 years?
- Which roles will grow, stay flat, or decline?
- What new roles don't exist today?

**Step 2: Supply** — What talent do we have?
- Current headcount and skills inventory
- Attrition projections by role/level
- Internal mobility potential (who can be reskilled?)

**Step 3: Gap** — Demand minus Supply
- Quantify the gap by role category and skill
- Distinguish: Shortage (not enough people) vs. Obsolescence (wrong skills)

**Step 4: Strategy** — How to close the gap?
- **Buy**: External hiring
- **Build**: Reskill/upskill existing employees
- **Borrow**: Contingent labor, outsourcing, partnerships
- **Bot**: Automate roles that are disappearing

### Talent Acquisition Diagnostics

| Metric | Benchmark |
|--------|-----------|
| Time to fill (days) | 30-45 days (good), >60 days (problem) |
| Offer acceptance rate | >90% |
| New hire 90-day retention | >95% |
| Source of hire | Referrals should be 30-40% (highest quality, lowest cost) |
| Cost per hire | Varies widely; $5K-$30K for professional roles |
| Quality of hire (1-year performance rating) | Track and optimize toward sources with highest quality |

**Hiring-funnel template.** Applicants → screened → interviewed → offered → accepted → joined. Report two ratios separately rather than one blend: **offer acceptance** = accepted ÷ offers (declines are driven by pay gap, decision speed and employer brand) and **join ratio** = joined ÷ accepted (back-outs are driven by the offer-to-join gap and counter-offers). Offers needed = hiring plan ÷ (acceptance × join ratio); interview load = offers needed × interviews per offer. Price the leak with cost of vacancy per working day ≈ value of the role (e.g., 2× CTC) ÷ 240 working days. Example [ILLUSTRATIVE]: 55% acceptance × 73% join ratio = 40% offer-to-join, so 200 hires need 500 offers; at 85% × 90% = 76.5%, they need about 261. Worked drills: `references/case-bank-unconventional.md` (U1, U2).

### Talent Retention & Engagement

**The Great Retention Question**: Why do people leave? The most common reasons:
1. Better pay/total comp elsewhere (especially in tight labor markets)
2. Limited growth / career development opportunities
3. Poor manager relationship
4. Lack of meaning/purpose
5. Work-life balance / flexibility
6. Company culture / values misalignment

**Attrition cost**: Typically 50-200% of annual salary per departing employee (recruiting + onboarding + productivity loss + knowledge transfer + team disruption).

**Retention lever priority:**
- Manager quality is the #1 lever. People leave managers, not companies. Fix this first.
- Career pathing and transparent promotion criteria — ambiguity about how to advance drives exits
- Compensation market-pricing — should be done annually; falling behind 10-15% triggers departure consideration
- Flexibility — the post-COVID expectation; removing it without strong rationale drives attrition

### HR Function Transformation

**The Ulrich Model** (the standard HR operating model):
- **HR Business Partners (HRBPs)**: Embedded in business units; strategic advisors to business leaders
- **Centers of Excellence (CoEs)**: Deep expertise in specific domains (talent acquisition, L&D, compensation, culture)
- **Shared Services**: Transactional HR processes (payroll, onboarding, benefits admin) — candidates for automation/outsourcing

**HR Technology Stack:**
- **HRIS (Core HR)**: System of record for employee data (Workday, SAP SuccessFactors, Oracle HCM)
- **ATS (Applicant Tracking System)**: Recruiting workflow (Greenhouse, Lever, Workday Recruiting)
- **LMS (Learning Management System)**: Training delivery and tracking (Cornerstone, LinkedIn Learning)
- **Performance Management**: Goal-setting, reviews, continuous feedback (Lattice, Betterworks)
- **Workforce Analytics**: People analytics platform (Visier, Workday Prism)

**HR Transformation Cost / Benefit:**
Typical HR transformation reduces HR cost as % of revenue from 1.5-2.5% to 0.8-1.2% through:
- Shared services consolidation (30-50% admin cost reduction)
- HR technology automation (reduce manual processing)
- Outsourcing transactional processes to BPO providers

### Diversity, Equity & Inclusion (DEI)

DEI is both a values imperative and a business imperative (diverse teams outperform on innovation and problem-solving).

**Diagnostic dimensions:**
- Representation (by level, function, geography) vs. external benchmarks
- Equity (pay equity analysis — same job, same performance, same pay?)
- Inclusion (belonging scores in engagement surveys; difference in engagement by demographic group)
- Pipeline (representation at entry level vs. senior level — where does the funnel narrow?)

**Key interventions:**
- Structured interviews and standardized evaluation criteria (reduces bias in hiring)
- Blind resume screening for initial screening
- Sponsorship programs (not just mentorship — active advocacy by senior leaders for high-potential diverse talent)
- Promotion process audit (are criteria objective? Are evaluators trained on bias?)
- Pay equity analysis and remediation (run annually; remediate proactively)
