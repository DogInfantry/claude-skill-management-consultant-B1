# Due Diligence Deep Dive: M&A & Investment Analysis

## 1. Commercial Due Diligence (CDD) Framework

### Definition & Scope

Commercial Due Diligence assesses the commercial attractiveness and viability of a target business. It answers: "Is this business worth what we think it's worth, and what are the revenue and margin risks?"

CDD focuses on **top-line** sustainability and growth:
- Market size and growth trends
- Customer concentration and retention
- Competitive positioning and barriers to entry
- Pricing power and margin sustainability
- Sales funnel health and pipeline quality
- Product-market fit and go-to-market efficiency

### Market & Customer Analysis

**Market Assessment:**
- Total Addressable Market (TAM): Top-down (industry research) and bottom-up (customer counts × average contract value)
- Serviceable Addressable Market (SAM): Realistic addressable portion within 3-5 years
- Market Growth Rate: CAGR from credible sources (IDC, Gartner, PitchBook for private companies)
- Competitive Intensity: Number and scale of competitors; market consolidation trends
- Barriers to Entry: Switching costs, network effects, regulatory moats, brand value

**Customer Due Diligence:**
- **Customer Concentration:** % revenue from top 10 customers (red flag if >40%)
- **Customer Retention:** Churn rate, customer lifetime value (LTV), repeat purchase rates
- **Customer Concentration by Segment:** Industrial customers vs. consumer; enterprise vs. SMB
- **Contract Terms:** Average contract length, renewal rates, gross retention, net retention (expansion revenue)
- **Net Revenue Retention (NRR):** For SaaS, the gold standard metric: (Beginning ARR + Expansion - Churn) / Beginning ARR. >100% is very strong; <90% signals risk

### Sales & Marketing Analysis

**Go-to-Market Efficiency:**
- Customer Acquisition Cost (CAC): Fully loaded marketing + sales expense per new customer
- CAC Payback Period: Months to recover CAC from gross profit; <12 months is strong for B2B
- Sales Force Productivity: Revenue per sales rep; benchmark against peer group
- Pricing Strategy: List price vs. effective price; discounting trends; pricing power vs. competitors
- Marketing Mix: Direct sales vs. channel vs. self-serve; cost by channel

**Sales Pipeline Health:**
- Pipeline visibility: Forecast accuracy (compare past projections to actuals)
- Win rates by customer segment and competitor
- Sales cycle length: Days from lead to close; trends over time (lengthening suggests deal quality risk)

### Pricing & Margin Analysis

**Pricing Power:**
- Historical price increases (absolute and %)
- Price elasticity: How do customers respond to price moves?
- Competitive pricing: How does target pricing vs. incumbents?
- Switching costs: Low switching costs = low pricing power

**Margin Sustainability:**
- Gross margin trends: 3-5 year history; benchmark vs. peers
- Variable cost drivers: COGS as % of revenue; inflation exposure (labor, materials, freight)
- Fixed cost structure: Can margins expand with operating leverage, or are they fixed?
- Gross margin by customer segment: Identify unprofitable segments
- Contribution margin by product line: Identify which products drive profitability

---

## 2. Operational Due Diligence (ODD)

### Operations & Processes

**Process Maturity:**
- Documented standard operating procedures (SOPs) for critical functions
- Process automation and manual steps; % automation
- Inventory management: Days inventory outstanding (DIO); inventory turnover; obsolescence risk
- Supply chain resilience: Single-source suppliers; geographic concentration; inflation hedging
- Supplier concentration: % spend with top 5 suppliers (red flag if >50%)

**Operational Efficiency Benchmarks:**
- Operating expense ratio (OpEx as % of revenue) vs. peers
- Headcount productivity: Revenue per employee; trend over time
- Capacity utilization: Operating at full capacity or spare capacity? Growth headroom without capex
- Capex intensity: Annual capex as % of revenue; capex/depreciation ratio (signals growth investment)

### Quality & Compliance

**Quality Management:**
- Defect rates, warranty costs, product returns as % of revenue
- Quality certifications (ISO 9001, etc.)
- Customer satisfaction metrics: NPS, CSAT trends
- Product safety and liability claims (current and historical)

**Regulatory Compliance:**
- Licenses and permits: Current status; renewal requirements
- Regulatory inspections: Historical findings; corrective actions
- Environmental compliance: Emissions, waste, water management; cap-ex for compliance
- Health & Safety: OSHA recordable incidents; safety certifications
- Trade compliance: Export controls, sanctions, import regulations

### Outsourcing & Vendor Management

**Third-Party Risk:**
- Critical outsourced functions: Manufacturing, call center, R&D, back-office
- Vendor concentration: Single-source vendors; switching feasibility
- Contract terms: Pricing escalation clauses; termination rights; SLA compliance
- Business continuity: Vendor financial stability; redundancy plans

---

## 3. Financial Due Diligence (FDD)

### Historical Financials & Quality of Earnings

**Financial Statement Analysis:**
- 3-5 year historical financials (P&L, balance sheet, cash flow)
- Quality of earnings assessment: Non-recurring items, accounting policy changes, revenue recognition timing
- EBITDA adjustments: Add-backs for owner compensation, consulting fees, one-time costs; justify each
- Working capital: Days sales outstanding (DSO), DIO, days payable outstanding (DPO); seasonal effects
- Cash conversion: Operating cash flow vs. net income; identify working capital swings or capex lumps

**Key Financial Metrics:**
- Revenue growth rate (YoY %)
- EBITDA margin trend (improving or deteriorating?)
- Free cash flow (EBITDA - capex - change in NWC)
- Return on Invested Capital (ROIC) = EBIT × (1 - tax rate) / (debt + equity)
- Debt/EBITDA ratio; interest coverage (EBIT / interest expense)

### Balance Sheet Health

**Liquidity & Solvency:**
- Current ratio and quick ratio (current assets / current liabilities)
- Cash position and burn rate (if pre-revenue)
- Contingent liabilities: Pending litigation, regulatory fines, environmental cleanup
- Off-balance-sheet obligations: Operating leases, pension liabilities, guarantees

**Asset Quality:**
- Goodwill and intangible assets: Impairment risk? (Red flag if >40% of equity)
- Accounts receivable aging: % over 60/90 days past due
- Inventory obsolescence: Slow-moving and excess inventory; write-down risk
- Fixed assets: Condition, useful lives, depreciation policy; capex required to maintain

### Debt & Covenant Analysis

**Debt Structure:**
- Total debt outstanding; maturity schedule (near-term refinancing risk?)
- Interest rates and terms: Fixed vs. floating; swap costs
- Covenants: Leverage, interest coverage, minimum cash; covenant headroom
- Related-party loans: Terms, subordination, forgiveness risk
- Earn-outs and contingent consideration: Future cash impact

---

## 4. Technology Due Diligence (TDD)

### Product & Technology Architecture

**Technology Stack:**
- Core technology: Proprietary vs. third-party; technical debt assessment
- Architecture: Scalable? Cloud-native or legacy monolithic system?
- Hosting: AWS, Azure, on-premise; security posture
- Technical debt: Code quality assessments; refactoring requirements
- Product roadmap: Feature velocity; alignment with market needs

**Intellectual Property (IP):**
- Patents: Issued patents, applications in process; claims and breadth
- Trade secrets: Source code protection, non-compete agreements
- Licenses: Third-party code; GPL or other open-source compliance risk
- IP litigation: Pending claims; freedom to operate assessment
- IP value: "Use" value (enables product) vs. "sell" value (licensing potential)

### Cybersecurity & Data Privacy

**Security Posture:**
- Penetration testing results; vulnerability management process
- Security certifications: SOC 2, ISO 27001, FedRAMP (if applicable)
- Incident history: Data breaches, ransomware, downtime; response time and impact
- Access controls: MFA, privileged access management (PAM), least-privilege design
- Encryption: Data at rest and in transit; key management

**Data Privacy & Compliance:**
- GDPR compliance (if EU customers): Data processing agreements, DPIA, consent mechanisms
- CCPA compliance (US): Data sale opt-out processes
- Industry-specific: HIPAA (healthcare), PCI DSS (payment cards), FINRA (financial)
- Data residency: Where is customer data stored? Cross-border data transfer mechanisms
- Vendor data access: Which third parties have access to customer data?

### Development & Support Operations

**Development Velocity:**
- Time to market: Months from concept to launch
- Release cadence: Weekly, monthly, quarterly?
- QA process: Test coverage; automated testing ratio
- Uptime/SLA: Historical uptime; SLA commitments to customers

**Technical Support:**
- Support organization: In-house vs. outsourced; support languages
- Support costs: As % of revenue (benchmark: 5-10% for SaaS)
- Customer-reported issues and resolution time

---

## 5. ESG Due Diligence

### Environmental Factors

**Emissions & Climate Risk:**
- Scope 1 emissions (direct): Manufacturing, fleet, facility operations
- Scope 2 emissions (indirect): Energy consumption from grid
- Scope 3 emissions (value chain): Supplier and customer emissions; hardest to quantify
- Carbon intensity: Emissions per $1M revenue; trend and peer comparison
- Climate scenario risk: Physical risks (flooding, supply chain disruption); transition risk (carbon pricing, regulation)

**Resource Management:**
- Water consumption and stress: High-risk geographies (California, Middle East, South Asia)
- Waste generation: % recycled, landfill, incineration; hazardous waste
- Pollution: Air and water discharge; regulatory violations
- Circular economy: Product recyclability; packaging waste reduction

**Supply Chain Environmental Risk:**
- Supplier environmental compliance: Audit findings; corrective actions
- Raw material sourcing: Conflict minerals, deforestation (palm oil, timber), mining practices
- Logistics emissions: Carrier selection; supply chain optimization

### Social Factors

**Labor & Working Conditions:**
- Union status and labor relations: Strike history; pending negotiations
- Workforce diversity: Gender, ethnicity, age; pay equity analysis
- Employee turnover: By level (entry, manager, executive); replacement cost
- Workplace safety: OSHA recordable rate; serious injury frequency (SIF); near-misses
- Training & development: Investment in employee upskilling; internal promotion rates
- Compensation: Market competitiveness; benefits; equity vesting

**Community & Human Rights:**
- Community engagement: Local hiring, investment in communities
- Human rights practices: Child labor, forced labor; supplier audits in high-risk geographies
- Customer privacy: Data breaches; customer lawsuits; regulatory action
- Product safety: Recalls, liability claims, customer harm incidents
- Regulatory violations: Labor law, discrimination, wages & hours

**Diversity, Equity & Inclusion (DEI):**
- Board diversity: Gender, ethnicity, independence
- Executive team diversity: C-suite gender/ethnicity representation
- Pay gap analysis: Gender and ethnicity wage gaps
- Women in leadership: % managers, directors, C-suite who are women
- Supplier diversity: % spend with diverse-owned suppliers

### Governance Factors

**Board & Management:**
- Board size, composition, independence
- Board committees: Audit, compensation, nominating & governance
- Executive tenure and turnover: High turnover red flag
- Related-party transactions: Fairness of terms; disclosure and approval
- Insider trading and stock pledges: Confidence signals; liquidity constraints

**Financial Reporting & Controls:**
- Internal control environment: Material weaknesses or significant deficiencies?
- Audit findings: Management letters; SEC comment letters (if public)
- Financial restatements: Magnitude and frequency; investor confidence
- Disclosure quality: SEC filing completeness (if applicable)

**Executive Compensation:**
- CEO pay ratio: CEO vs. median employee pay (if required to disclose)
- Performance-based compensation: % tied to ESG metrics
- Clawback provisions: Recoupment of compensation for restatements or misconduct
- Equity awards: Vesting schedules; alignment with long-term strategy

---

## 5.5 Legal, Regulatory & Consents Due Diligence (LDD)

The workstream most often under-scoped by commercially-minded teams — and the one that most often *stops a deal from closing*. CDD/FDD/ODD tell you whether the target is worth buying; LDD tells you whether you can actually acquire it, on what timeline, and what liabilities and consents travel with it. For the full execution mechanics behind this workstream, read `references/cross-border-ma-execution.md`; for the risk-allocation terms it feeds, read `references/spa-deal-terms-benchmarking.md`.

### Definition & Scope

LDD verifies **title, authority, and transferability**, and maps the **regulatory and consent gauntlet** between signing and closing. It runs in parallel with the other workstreams and directly shapes deal structure (share vs. asset vs. merger), the conditions precedent, the indemnity package, and the timeline.

### Corporate, Title & Structure

- **Title chain:** Does the seller actually own what it is selling — clean title to the shares/quotas, no undisclosed pledges, options, or pre-emption rights?
- **Constitutional documents:** Charter/by-law transfer restrictions, pre-emption, drag/tag, consent thresholds, and any director-appointment or bond requirements that gate the mechanics.
- **Capitalisation:** Cap table accuracy, unpaid/uncalled capital, convertibles, warrants, and option pools that dilute or create claims.
- **Structure fit:** Whether the intended acquisition method (share/asset/statutory merger) is available and optimal given where value and liability sit.

### Regulatory & Approvals Exposure (the gating items)

- **Foreign-investment / national-security screening:** Does the target operate in a sensitive sector (defence, critical infrastructure, advanced tech/semiconductors, sensitive data, telecoms, energy) in *any* jurisdiction? Is the buyer's ownership sensitive? Is filing **mandatory with a standstill**, or **voluntary with call-in risk**? This can be a *kill* item, not a checklist item — see the Broadcom–Qualcomm case (`case-studies/ma-broadcom-qualcomm-national-security-block.md`).
- **Merger control / antitrust:** In which jurisdictions are filing thresholds (turnover/asset/transaction-value) met? Where is the substantive competitive overlap? Which authority is the long pole on timing? What remedy risk (divestiture/behavioural) exists?
- **Sector regulators:** Change-of-control approvals for banking, insurance, financial services, telecoms, energy, healthcare, aviation — independent of antitrust.
- **Exchange control / repatriation:** Any central-bank approval or investment-registration gating consideration flow across borders.

### Contracts, Consents & Continuity

- **Change-of-control / anti-assignment clauses** in crown-jewel customer, supplier, financing, lease, franchise, IP-licence, and JV agreements — diligence the *top contracts by value first*; a single anchor-customer consent can be the real critical path.
- **Financing consents and cross-default triggers** that a change of control may trip.
- **Permits and licences** that may not survive an asset transfer or may require regulator consent even in a share deal.

### People & Liabilities That Don't Move Cleanly

- **Automatic-transfer employment regimes** and **works-council / union consultation** obligations that gate signing/closing and carry redundancy/harmonisation cost.
- **Pension and benefit** deficits and unfunded liabilities (classic hidden liability — price it explicitly).
- **Litigation, disputes, and contingent liabilities**; tax exposures (transfer pricing, withholding, historical positions); environmental legacy.
- **Survival:** which liabilities (tax, employment, environmental, litigation) outlive close, and how they should be secured (escrow, W&I insurance, or specific indemnity) — this is the direct bridge to `spa-deal-terms-benchmarking.md`.

### Typical LDD Work Plan (parallel to CDD/FDD, ~4–8 weeks)

1. **Week 1:** Corporate/title and constitutional review; map the acquisition structure; open the regulatory-exposure assessment (FDI + merger control in every operating country).
2. **Weeks 2–4:** Contract review for change-of-control/assignment triggers on top-value agreements; employment/pension/benefit review; litigation and contingent-liability review.
3. **Weeks 3–6:** Confirm filing requirements and timelines; draft the clearance/consent critical path; identify specific-indemnity candidates from findings.
4. **Weeks 5–8:** Feed findings into structure, conditions precedent, the indemnity/W&I package, and the integration/consents plan.

---

## 6. Red Flags by Category

### Financial Red Flags

- **Revenue Concentration:** >50% from single customer; >80% from top 5
- **Margin Deterioration:** Gross margin declining >200 bps YoY
- **Cash Flow Mismatch:** High net income but negative/weak operating cash flow (accounting quality)
- **Working Capital Deterioration:** DSO or DIO increasing; suggests operational stress
- **Inventory Obsolescence:** Old inventory, slow-moving SKUs, write-downs
- **Excess Debt:** Net Debt / EBITDA >4x; covenant violations imminent
- **Contingent Liabilities:** Unresolved litigation, environmental remediation, product recalls
- **Related-Party Transactions:** Unfavorable terms; lack of transparency
- **Frequent Restatements:** Financial reporting reliability concerns
- **Weak Internal Controls:** Material weakness in financial reporting

### Operational Red Flags

- **High Capex Intensity:** >15% of revenue required to maintain; strains cash flow
- **Supplier Concentration:** >50% cost from single supplier; switching risk
- **Quality Issues:** High defect rate, product recalls, warranty costs >5% of revenue
- **Regulatory Non-Compliance:** Outstanding citations, fines, license at risk
- **Outdated Infrastructure:** Legacy systems; significant technical debt
- **High Employee Turnover:** >20% annual turnover in stable businesses; key person dependencies
- **Capacity Constraints:** Running at >95% capacity with long lead times
- **Operational Inefficiency:** Headcount/revenue ratio significantly above peer group

### Technology Red Flags

- **Obsolete Technology Stack:** Legacy systems; difficult to attract talent; expensive maintenance
- **Technical Debt:** Code quality issues; difficult to implement features
- **Security Vulnerabilities:** History of breaches; poor incident response
- **IP Risk:** Patent litigation; ambiguous ownership; infringement exposure
- **Poor Uptime:** <99% availability; SLA breaches
- **Lack of Scalability:** Architecture can't handle projected growth
- **Data Privacy Violations:** GDPR or CCPA violations; regulatory fines
- **Vendor Lock-In:** Single-vendor dependencies; switching cost prohibitive
- **Development Velocity Stalled:** Slow feature releases; missing roadmap milestones

### ESG Red Flags

- **Environmental Non-Compliance:** Regulatory violations; environmental remediation needed
- **Labor Law Violations:** Wage & hour violations; discrimination lawsuits; union disputes
- **High Carbon Footprint:** Far above peer group; regulatory/market risk
- **Human Rights Issues:** Supplier violations in conflict zones; forced labor allegations
- **Governance Weakness:** Weak board independence; CEO/chair dual role with no compensation committee
- **Pay Equity Gaps:** Significant gender/ethnicity wage gaps; pay discrimination litigation
- **Executive Misconduct:** Criminal convictions, fraud, sexual harassment allegations
- **Community Conflict:** Significant community opposition; license to operate at risk
- **Supply Chain Risk:** Heavy exposure to high-ESG-risk geographies; climate-vulnerable suppliers

### Governance & Fraud Red Flags

- **Unverified Cash:** Bank/cash balances confirmed only via management-provided statements, never independently with the bank itself — the single most under-verified "hard" number on a balance sheet
- **Asset-Liability Duration Mismatch:** Short-term wholesale funding backing long-tenor assets inside a lender, NBFC, or leasing counterparty — invisible from the credit rating alone
- **Heavy Promoter/Founder Share Pledging:** Above ~30-40% of holding pledged signals personal leverage against company stock — a common precursor to forced selling or governance pressure
- **Related-Party Webs:** Lending, leasing, or services transactions between the target and founder-controlled entities that aren't arm's-length priced
- **Use-of-Proceeds Drift:** Loan or capital-raise proceeds not traceable to their stated purpose — the exact fact pattern regulators later classify as willful default or fund diversion
- **Unexplained Entity-Count Growth:** Dozens of subsidiaries/JVs/SPVs with unclear commercial rationale — complexity that primarily obscures cross-obligations rather than serving genuine business need
- **Rubber-Stamp Audit Signals:** Long auditor tenure without rotation, combined with an opinion that never queries a rapidly growing cash balance or margin profile that's smoother than peers'; an unqualified opinion is evidence of an audit process, not independent verification
- **Evergreening:** A lender restructuring or extending credit repeatedly without a credible, independently validated turnaround plan — delays loss recognition rather than preventing the loss
- **Trading-Pattern Correlation:** Personal or connected-party trades that consistently precede an institution's own large orders — the signature pattern of front-running, now detectable via real-time surveillance rather than only after the fact

Worked end-to-end with real figures and regulatory outcomes in `case-studies/gov-satyam-accounting-fraud.md`, `case-studies/gov-ilfs-shadow-bank-collapse.md`, `case-studies/gov-kingfisher-willful-default.md`, and `case-studies/gov-insider-trading-and-front-running-india.md`.

---

## 7. PE vs. Strategic Acquirer Due Diligence

### Private Equity (PE) Approach

**Financial Engineering Focus:**
- Deeply analyze EBITDA adjustments: Every add-back is scrutinized; will it survive LBO scrutiny?
- Leverage capacity: How much debt can this business support? Model 6-8 leverage, debt paydown schedule
- Exit multiples: At what multiple will we exit? 5-7 year hold period
- Cash-on-cash returns: Target 20-30% IRR; model multiple exit scenarios

**Operational Value Creation:**
- Identify 100-150 bps of EBITDA margin expansion: SG&A rationalization, procurement optimization, pricing actions
- Benchmark operations against best-in-class: Can we drive efficiency to peer levels?
- Management alignment: Will sellers/management stay? Rollover equity to align incentives
- Add-on acquisition targets: Can we bolt on complementary businesses to drive revenue growth?

**Key PE Red Flags:**
- Unsustainable EBITDA: Dependent on owner's unpaid labor or one-time events
- Debt service risk: Operating leverage too high; negative working capital
- Customer concentration: Can't support leverage with concentrated customer base
- Management risk: Key person dependencies; management staying only for retention bonus

### Strategic Acquirer Approach

**Strategic Fit Analysis:**
- Synergy identification: Revenue synergies (cross-sell, market access), cost synergies (procurement, manufacturing footprint, G&A)
- Quantify synergies: Model revenue uplift, integration cost savings, capex reductions
- Cost of integration: Time, resources, disruption to both companies
- Risk of integration: Customer/employee churn, cultural clash, execution risk

**Competitive & Market Positioning:**
- Competitive advantage: Does acquisition strengthen market position vs. competitors?
- Market share impact: Combined market share post-acquisition; regulatory clearance risk (FTC)
- Synergy capture: Can we actually realize cost synergies without losing revenue?
- Speed to market: Does acquisition accelerate product roadmap or market entry vs. organic development?

**Key Strategic Red Flags:**
- Modest synergies relative to purchase price: Overpay risk
- Integration complexity: Different systems, cultures, customer bases; high implementation risk
- Regulatory risk: Antitrust concerns; deal approval uncertain
- Seller retention: Key customers prefer old management; revenue at risk

### Financial Model Differences

| Aspect | PE | Strategic |
|---|---|---|
| **Valuation Floor** | Debt capacity (EBITDA / target leverage) | Synergies + standalone DCF |
| **Return Target** | 20-30% IRR | Revenue/strategic value + cost savings |
| **Working Capital** | Optimize (lower DPO = less cash) | Manage per integration plan |
| **Leverage** | Maximize (use debt for returns) | Moderate (financial flexibility) |
| **Exit** | Trade sale or IPO in 5-7 years | Integrate and hold indefinitely |

---

## 8. Vendor Due Diligence (VDD)

### Vendor Risk Assessment

**Financial Health:**
- Credit rating and payment history: Any late payments or defaults?
- Financial statements: Revenue, profitability, cash flow; assess viability
- Concentration: Dependent on single customer? (Red flag if >50% revenue from one customer)
- Industry trends: Is vendor's industry in decline? (E.g., print manufacturing)

**Operational Capability:**
- Certifications: ISO 9001, ISO 14001, industry-specific (UL, CE, FCC, etc.)
- Capacity: Current utilization; can vendor scale for your growth?
- Quality systems: SPC (Statistical Process Control), inspections, traceability
- Lead times: Historical on-time delivery; ability to meet your timeline
- Disaster recovery: What if vendor's facility is disrupted?

**Financial Terms & Risk:**
- Payment terms: Net 30/60/90; early payment discounts
- Price escalation: How are inflation/commodity price changes passed through?
- Minimum order quantities (MOQ): Lock-in risk?
- Termination rights: Can you exit contract? Termination costs?
- Liability & insurance: Adequate coverage? Indemnification provisions?

### Vendor Management Post-Close

**Contract Governance:**
- Service Level Agreements (SLAs): Uptime, response time, resolution time; financial penalties
- Escrow arrangements: Source code escrow for critical software vendors
- Key Person provisions: Named resources; replacement SLAs if turnover
- Auditing rights: Ability to audit vendor operations; security compliance

**Ongoing Monitoring:**
- Scorecard: Monthly/quarterly metrics (on-time delivery, quality, responsiveness)
- Escalation process: Issues tracked; resolution SLAs
- Regular business reviews: Quarterly/annual check-ins
- Diversity audits: Are vendors maintaining commitment to diversity/inclusion?

---

## 9. Due Diligence Work Plans & Implementation

### Typical CDD Work Plan (8 weeks)

**Week 1-2: Discovery & Data Gathering**
- Kick-off with target management; data request list issued
- Desktop research: Industry reports, competitive intelligence, customer research
- Customer & market interviews: Design questionnaire; 20-30 customer calls

**Week 3-4: Market & Customer Analysis**
- Analyze customer data: Concentration, retention, NRR, churn
- Market sizing: TAM/SAM bottom-up and top-down
- Competitive mapping: Competitive pricing, positioning, win/loss analysis
- Sales funnel: Pipeline quality, forecast accuracy, pipeline velocity

**Week 5-6: Pricing & Financial Modeling**
- Price elasticity analysis: Historical pricing changes and volume response
- Margin sustainability: Gross margin drivers; benchmarking vs. peers
- Revenue forecasting: Build financial model with scenarios (base/bull/bear)
- Perform sensitivity: Impact on valuation of key assumptions

**Week 7-8: Red Flag Investigation & Writeup**
- Deep-dive on identified issues: Customer concentration, product concentration, margins at risk
- Competitor interviews: Confirm market positioning and pricing power
- Final report: Summary findings, valuation sensitivities, deal recommendation

### Typical ODD Work Plan (6 weeks)

**Week 1-2: Operations Assessment**
- Factory/facility tours: Assess condition, automation, capacity
- Process documentation: Understand critical operations
- Supply chain mapping: Identify vendors, concentration, contract terms
- Management interviews: Operations strategy, challenges, investments needed

**Week 3-4: Quality & Compliance Deep-Dive**
- Quality metrics: Defect rates, warranty costs, NPS trend
- Compliance documentation: Licenses, certifications, regulatory inspections
- Environmental assessment: Emissions, waste, pollution; remediation costs
- Safety record: OSHA recordable incidents, corrective actions

**Week 5-6: Benchmarking & Recommendations**
- Operational efficiency: Benchmark metrics vs. peers (OpEx ratio, capex intensity, headcount per $M revenue)
- Identify quick wins: Procure optimization, headcount reductions, process improvements
- Capex requirements: Infrastructure upgrades, equipment replacement
- Integration plan: How will we operate post-acquisition?

### Typical FDD Work Plan (8 weeks)

**Week 1-2: Historical Analysis**
- Gather financials: 3-5 years P&L, balance sheet, cash flow
- Identify non-recurring items: Quantify add-backs and adjustments
- Quality of earnings: Investigate revenue recognition, accounting policy changes
- Working capital analysis: DSO, DIO, DPO; seasonal effects

**Week 3-4: Deep-Dive**
- Accounts receivable aging: % over 60/90 days; allowance for doubtful accounts
- Inventory analysis: Obsolescence, slow-moving SKUs, write-down risk
- Fixed assets: Condition, useful lives; capex required to maintain
- Debt analysis: Terms, covenants, refinancing risk; contingent liabilities

**Week 5-6: Tax & Compliance**
- Tax compliance: Federal, state, local; audit history
- Transfer pricing: If multinational, are transfer prices arm's length?
- Tax contingencies: Uncertain tax positions; valuation allowances
- Regulatory compliance: Environmental, labor, trade; pending violations

**Week 7-8: Valuation & Recommendations**
- Build 3-statement model: Base case; sensitivity to key assumptions
- Calculate enterprise value: DCF with multiple scenarios
- Identify value drivers: Which assumptions most influence valuation?
- Writeup: Key findings, risks, financial model documentation

### Typical TDD Work Plan (6-8 weeks)

**Week 1-2: Technology Stack & Architecture**
- Codebase review: Architecture assessment; technical debt evaluation
- Hosting & infrastructure: Cloud vs. on-premise; security posture
- Development environment: CI/CD pipeline, testing automation, deployment process
- Technology roadmap: Alignment with market needs; velocity assessment

**Week 3-4: Security & Compliance**
- Penetration test: Conduct or commission third-party assessment
- Security audit: Access controls, encryption, incident response, vendor management
- Data privacy: GDPR, CCPA, HIPAA compliance; data processing agreements
- IP audit: Patents, trademarks, trade secrets; third-party licensing

**Week 5-6: Development & Operations**
- Code quality: Static analysis tools; refactoring requirements
- Test coverage: % automated tests; QA process maturity
- Uptime/SLA: Historical availability; SLA compliance vs. customer commitments
- Customer support: Support model, costs, satisfaction metrics

**Week 7-8: Findings & Recommendations**
- Technical debt assessment: Refactoring effort and cost
- Scalability review: Can infrastructure handle projected growth?
- Integration considerations: How will target integrate with acquirer's tech stack?
- Roadmap: 12-month post-close priorities

### Team Composition (CDD Example, $200M acquisition)

| Role | Experience | FTE | Responsibility |
|---|---|---|---|
| **CDD Lead** | Principal-level | 1.0 | Overall coordination, client relationship, senior customer interviews |
| **Senior Analyst** | 5-8 years | 1.0 | Market research, customer interviews, competitive analysis |
| **Analyst** | 2-4 years | 1.0 | Data aggregation, customer analytics, model building |
| **Finance Support** | MBA/CPA | 0.5 | Financial model, valuation sensitivity, benchmarking |

**Total: ~3.5 FTE; 8-week engagement = ~280 consultant hours**

---

## 10. Due Diligence Costs & Benchmarks

### Typical CDD Costs

| Deal Size | Cost Range | As % of Deal Value | Duration |
|---|---|---|---|
| $50M–$100M | $75k–$150k | 0.1–0.3% | 6–8 weeks |
| $100M–$500M | $150k–$400k | 0.15–0.4% | 8–10 weeks |
| $500M–$1B | $400k–$800k | 0.08–0.16% | 10–12 weeks |
| $1B+ | $800k–$1.5M | 0.08–0.15% | 12–16 weeks |

**Note:** Larger deals are lower % because much work is fixed (market research, initial customer calls) and incremental work scales with deal complexity, not deal size.

### Financial Due Diligence Costs

| Deal Size | Cost Range | Duration |
|---|---|---|
| $50M–$100M | $100k–$200k | 8 weeks |
| $100M–$500M | $200k–$500k | 10 weeks |
| $500M–$1B | $500k–$1M | 12 weeks |
| $1B+ | $1M–$2M+ | 14–16 weeks |

Includes financial analysis, working capital review, tax analysis, and valuation modeling.

### Technology Due Diligence Costs

| Deal Size | Cost Range | Duration |
|---|---|---|
| $50M–$100M | $80k–$150k | 6–8 weeks |
| $100M–$500M | $150k–$350k | 8–10 weeks |
| $500M–$1B | $350k–$700k | 10–12 weeks |

Higher if penetration test or third-party security assessment required; add $50k–$100k for specialized tech vendor assessments.

### Multi-Workstream Bundling

Most large acquisitions run CDD + FDD + TDD + ODD in parallel:

**$250M Mid-Market Deal (Parallel Workstreams):**
- CDD: $200k, 10 weeks
- FDD: $250k, 10 weeks
- TDD: $150k, 8 weeks
- ODD: $120k, 8 weeks
- **Total: ~$720k, 10-week critical path**

**Benchmarking:** CDD typically 25–30% of total, FDD 30–35%, TDD 15–20%, ODD 12–18%.

### Red Flag Detection Rates

Historical data from advisor engagements:

| Red Flag Category | Detection Rate | Typical Impact |
|---|---|---|
| **Significant Revenue Concentration** | 35–45% | 10–20% valuation discount |
| **Margin Deterioration/Sustainability Risk** | 40–50% | 15–30% valuation discount |
| **Working Capital Surprise** | 25–35% | $5M–$25M+ cash impact post-close |
| **Technical Debt/IP Risk** | 30–45% | Capex requirement of $1M–$10M+ over 2 years |
| **Customer Retention/Churn Risk** | 50–60% | 10–15% revenue decline post-close (if not integrated well) |
| **Supply Chain/Operational Inefficiency** | 40–55% | 2–5% margin improvement opportunity |
| **Regulatory/Compliance Issues** | 20–30% | $2M–$20M+ remediation cost |

---

## Key Takeaways for Practitioners

1. **CDD is valuation intelligence:** Every $1 of risk identified can inform $5–$10 of valuation adjustment.
2. **Red flag investigation beats checkboxes:** Deep-dive on top 3–5 risks; confirm with primary research.
3. **NRR and CAC payback are gold standards:** For B2B software, NRR >100% and CAC payback <12 months indicate quality.
4. **Quality of earnings matters more than headline EBITDA:** Scrutinize every add-back; conservative FDD saves money later.
5. **Tech DD increasingly material:** Software/IP now core to valuation for most acquirers; allocate accordingly.
6. **ESG red flags are real:** Regulatory fines, litigation, supply chain risk are quantifiable and growing.
7. **PE vs. Strategic due diligence is fundamentally different:** Align workplan scope to buyer type and deal thesis.
8. **Vendor DD extends beyond deal close:** Ongoing contract management and monitoring reduce operational surprises.
9. **Parallel workstreams compress timeline:** 10–12 week due diligence cycles standard for $100M–$500M deals.
10. **Integration planning starts in due diligence:** Best acquirers use DD to inform post-close 100-day plans and synergy realization.
