# Emerging Demand Archetypes — Pattern-First Project Mapping

## What This File Does

Most consulting briefs are underspecified at arrival. A client says "we need to think about AI" or "help us on supply chain" — and the undiscerning consultant treats it as a blank slate. The elite move is to pattern-match immediately: which of the five dominant demand archetypes does this map to? Each archetype has a known project shape, a standard cast of workstreams, common risks, and proven levers. Using this file, you should be able to walk into any brief and generate a credible Day 1 hypothesis about what the engagement will actually look like — before you've done a single interview.

These archetypes reflect where 80%+ of new consulting demand is clustering across industries as of 2025–2026. They are not mutually exclusive: a single engagement often combines two or three. But one archetype usually dominates and should govern your structuring instinct.

---

## Archetype 1: GenAI Operating-Model & Governance Builds

### Where it shows up
Every major industry — Financial Services, Healthcare, Industrials, Public Sector, Consumer/Retail. Most commonly triggered when a client has completed 3–15 AI pilots but is failing to scale, or is facing board/regulatory pressure to demonstrate responsible AI.

### What the project actually looks like
The client's problem is almost never the technology. It is the absence of an operating model around the technology. Typical workstreams:

- **AI Roadmap & Portfolio Governance**: Prioritizing use cases on a value/feasibility matrix, deciding build/buy/partner for each, establishing a portfolio review cadence. (Read `references/genai-enterprise-strategy.md` for the value-feasibility matrix and build/buy/partner framework.)
- **Operating Model Design**: Who owns AI centrally vs. in business units? Hub-and-spoke vs. federated vs. centralized? How does the AI center of excellence relate to IT, Risk, and Business? (Read `references/org-design-workforce.md` for structural design work.)
- **Guardrails & Explainability**: Model risk frameworks, bias audits, EU AI Act compliance, SR 11-7 or equivalent model validation standards, AI incident response protocols. Increasingly non-negotiable in FS and healthcare.
- **Change Management & Literacy**: AI literacy programs by level (executives vs. frontline), role redesign as AI absorbs tasks, change readiness assessment. (Read `references/change-management.md`.)
- **Ethical AI & Audit**: Fairness assessments, explainability documentation, AI ethics committee design, external audit readiness.

### Key hypotheses to test on Day 1
1. Is this a "pilot purgatory" problem (many pilots, no scale) or a governance-pressure problem (scale is happening but ungoverned)?
2. Is the client's AI team technically strong but organizationally orphaned — no clear home, no executive sponsor?
3. Does a specific regulatory trigger (EU AI Act, Basel model risk, FDA SaMD guidance) drive urgency, or is this primarily a competitive/efficiency play?

### Common risks & failure modes
- Over-indexing on technology architecture when the real constraint is organizational authority and change readiness.
- Governance frameworks that exist on paper but have no teeth — no actual decision rights or consequences.
- Underestimating the change management scope: AI transformations are workforce transformations first.

### Value levers
Quantify through: (a) cycle time reduction in high-frequency decisions; (b) reduction in manual review FTEs; (c) risk-adjusted value of audit-readiness and regulatory penalty avoidance; (d) speed-to-deployment improvement across the AI portfolio.

### Cross-references
`references/genai-enterprise-strategy.md` | `references/ai-orchestration.md` | `references/ai-ml-analytics.md` | `references/org-design-workforce.md` | `references/change-management.md` | `references/erm-quantitative-risk.md`

---

## Archetype 2: Sustainable Ops, Green Megaprojects & Supply Chains

### Where it shows up
Manufacturing, Energy & Utilities, Consumer/Retail/CPG, Infrastructure, Industrials. Triggered by CSRD reporting deadlines, Scope 3 emissions pressure from customers, IRA tax credit monetization opportunities, or major capital programs (green hydrogen, offshore wind, EV manufacturing) that need project delivery capability.

### What the project actually looks like
Two flavors that often run in parallel:

**Flavor A — Decarbonization & ESG Compliance:**
- Scope 1/2/3 inventory and hotspot analysis
- Science-Based Targets (SBTi) commitment and pathway design
- Marginal Abatement Cost (MAC) curve to prioritize interventions
- CSRD/SEC/TCFD disclosure architecture and data infrastructure
- Internal carbon pricing design to influence capex decisions
- Supply chain decarbonization: Scope 3 supplier engagement, green procurement criteria, logistics optimization using GenAI

**Flavor B — Green Megaproject Delivery:**
- Portfolio design: which green projects, in what sequence, with what risk profile?
- Project controls, governance, and PMO design for capital programs
- GenAI-enabled project monitoring: predictive delay models, cost forecasting, resource optimization
- Government incentive capture: IRA, EU Green Deal, Contracts for Difference
- Financing structures: green bonds, blended finance, PPP

### Key hypotheses to test on Day 1
1. Is the urgency regulatory (CSRD deadline) or commercial (customer/investor ESG requirements)?
2. Does the client have the internal project delivery capability for their green capex ambitions, or are they systematically under-resourced?
3. Is Scope 3 the dominant emissions source? If so, the real program is supplier transformation, not internal operations.

### Common risks & failure modes
- **Greenwashing exposure**: overstating progress, using unverified offsets, making claims that outrun the data. Surface this early and build authenticity checkpoints into the program design.
- MAC curves that look rigorous but rest on engineering assumptions that haven't been stress-tested against procurement reality.
- Green megaprojects replicating the dysfunctions of conventional megaprojects (cost overruns, schedule slippage) because the PMO was designed for steady-state operations, not capital transformation.

### Value levers
(a) CSRD/regulatory penalty avoidance; (b) IRA/green incentive capture (quantify $/tonne CO₂ and total program value); (c) Supply chain cost reduction from logistics and energy optimization; (d) Customer retention value from ESG credentialing; (e) Green premium improvement on financing cost.

### Cross-references
`references/esg-sustainability.md` | `references/climate-netzero-implementation.md` | `references/implementation-pmo.md` | `references/industrial-manufacturing.md` | `references/energy-resources-utilities.md` | `references/erm-quantitative-risk.md`

---

## Archetype 3: AI-Augmented Project & Portfolio Management

### Where it shows up
Cross-industry, concentrated where organizations run large project portfolios: infrastructure, IT transformation, pharma R&D, defense procurement, large-scale consumer rollouts. Triggered when PMOs are drowning in data but starved for foresight — or when executive leadership has lost confidence in project status reporting.

### What the project actually looks like
The client already has a PMO. The problem is that it runs on backward-looking reporting (RAG status, Gantt charts, meeting notes) while the portfolio is large enough that by the time a risk surfaces in a status update, it is already a crisis. The engagement installs an intelligence layer:

- **Predictive Risk & Delay Modeling**: ML models trained on project data to predict schedule and cost overruns 4–8 weeks before they materialize. Inputs: milestone completion rates, resource utilization, dependency chains, external signals.
- **Resource Forecasting & Capacity Planning**: AI-driven supply/demand matching across a portfolio — identifying over-allocation, skill gaps, and bench utilization. (Read `references/org-design-workforce.md` for workforce design work.)
- **Semi-Autonomous Scheduling & Estimation**: AI handles re-sequencing, critical path recalculation, and bottom-up re-estimation as conditions change — human PMs focus on stakeholder management and judgment calls.
- **Portfolio Prioritization**: Value/risk matrix for active and pipeline projects; GenAI-assisted scenario modeling for portfolio rebalancing decisions.
- **Governance Redesign**: Streamlining steering committees, automating status reporting, exception-based escalation so humans focus where judgment matters.

### Key hypotheses to test on Day 1
1. Is the PMO's core problem data quality (garbage in, garbage out) or analytics capability (data exists but isn't being used)?
2. Are project managers spending >40% of time on reporting and coordination vs. actual project management? If so, the ROI of automation is enormous.
3. Does the organization have a culture of surfacing bad news early, or does it suppress it? The latter makes predictive models less effective because the underlying data is sanitized.

### Common risks & failure modes
- Building a sophisticated analytics layer on top of bad underlying data — the AI amplifies noise, not signal.
- Change resistance from PMs who see AI as a threat to their jobs rather than a tool that liberates them from administrative burden.
- Governance designs that add process without removing it: the steering committee meets weekly AND gets AI dashboards, resulting in more work not less.

### Value levers
(a) Reduction in project overruns (% of portfolio budget at risk × historical overrun rate); (b) PM productivity recovered from reporting automation (FTE hours × hourly rate); (c) Faster escalation of risks (time-to-detect reduction × cost of late detection); (d) Portfolio rebalancing value from better prioritization of the right projects.

### Cross-references
`references/implementation-pmo.md` | `references/implementation-practitioner.md` | `references/ai-orchestration.md` | `references/genai-enterprise-strategy.md` | `references/decision-making-under-uncertainty.md` | `references/org-design-workforce.md`

---

## Archetype 4: Resilience & Risk Programs

### Where it shows up
Cross-industry with concentrations in: Financial Services (cyber, operational resilience, Basel), Healthcare (supply chain resilience post-COVID), Industrials (geopolitical supply chain), Consumer/Retail (inventory resilience, single-source dependency), Energy (grid resilience, climate physical risk). Triggered by a shock (cyberattack, supplier failure, regulatory exam finding) or by board/regulator demand to demonstrate crisis readiness.

### What the project actually looks like

**Sub-type A — Supply Chain Resilience:**
- Mapping and stress-testing multi-tier supply chain exposure (single-source, geographic concentration, geopolitical chokepoints)
- Supplier diversification strategy and dual-sourcing analysis
- Inventory buffering and safety stock optimization
- Nearshoring/reshoring economics — TCO model including labor, logistics, quality, and risk-adjusted cost of disruption
- Demand-supply scenario planning under shock conditions

**Sub-type B — Cyber & Operational Resilience:**
- Operational resilience frameworks (BOE PS21/3, DORA, FFIEC) — critical business services, impact tolerances, recovery testing
- Third-party/vendor risk management redesign
- Incident response and crisis management playbooks
- Business continuity planning with AI-enhanced scenario generation

**Sub-type C — GenAI Scenario Planning & Crisis Simulation:**
- Agent-based models to simulate cascading failures under geopolitical, climate, or regulatory shock scenarios
- War-gaming and Red Team exercises with AI-synthesized adversary behavior
- Board-level crisis simulation exercises
- Physical climate risk quantification under TCFD scenarios

### Key hypotheses to test on Day 1
1. Is this driven by a specific regulatory deadline or exam finding? If so, scope is largely defined and the question is speed and credibility of delivery.
2. Has the client mapped its critical dependencies, or is Day 1 literally unknown? (Most companies have a shockingly incomplete picture of their Tier 2 and Tier 3 supply chain.)
3. Is the resilience program genuinely cross-functional (Procurement, IT, Operations, Finance, Legal simultaneously), or siloed in one function? Siloed programs consistently fail to deliver lasting results.

### Common risks & failure modes
- Resilience plans that look good on paper but have never been tested — the first real crisis becomes the test.
- Overinvestment in tail-risk scenarios while ignoring higher-probability medium-disruption events that actually occur most often.
- Treating resilience as a compliance exercise rather than a competitive differentiator — firms that build genuine resilience advantage often outperform peers during disruption cycles.

### Value levers
(a) Expected value of avoided disruption (probability × magnitude × duration × cost/day of disruption); (b) Insurance premium reduction from improved risk posture; (c) Regulatory penalty avoidance; (d) Working capital improvement from optimized inventory buffers (opportunity cost of excess stock × WACC).

### Cross-references
`references/erm-quantitative-risk.md` | `references/scenario-planning.md` | `references/industrial-manufacturing.md` | `references/financial-services.md` | `references/decision-making-under-uncertainty.md` | `references/esg-sustainability.md`

---

## Archetype 5: Sector-Specific GenAI Transformations

### Where it shows up
Everywhere, but with sector-specific project patterns distinct enough to warrant separate treatment. The common thread: the client wants to move from generic AI experimentation to AI embedded in specific workflows that drive the core business model.

### Sector-specific project patterns

**Healthcare & Life Sciences**
- AI triage and clinical decision support: NLP/LLM tools for diagnostic workflows, prior authorization, clinical note summarization, patient routing. Key constraint: FDA SaMD pathways, HIPAA, and physician acceptance.
- Drug discovery acceleration: ML-assisted target identification, clinical trial design optimization, real-world evidence platforms.
- Revenue cycle and coding automation: AI-assisted ICD-10 coding, denial prediction, payer contract optimization.
- Read `references/healthcare-life-sciences.md` for sector economics and regulatory detail.

**Banking & Insurance (Financial Services)**
- Autonomous-agent analytics: AI agents that monitor portfolios, flag anomalies, and generate analyst-grade reports — replacing significant portions of junior analyst workflows.
- Underwriting and claims automation: LLM-assisted policy review, AI-driven claims triage, fraud detection.
- Regulatory compliance automation: AI-assisted CCAR/DFAST narrative generation, BSA/AML monitoring uplift, model documentation automation.
- Read `references/financial-services.md` for sector economics; `references/genai-enterprise-strategy.md` for build/buy/partner and governance frameworks.

**Technology, Media & Telecommunications (TMT)**
- GenAI-driven product innovation: AI-assisted product design, personalization engines, content generation at scale, developer co-pilot deployment.
- Platform monetization: embedding AI features into SaaS products to improve NRR/expansion revenue; pricing AI features as add-on vs. bundled.
- Cost structure transformation: AI-assisted customer support (deflection rate improvement), QA automation, code generation to improve developer productivity.
- Read `references/technology-media-telecommunications.md` for SaaS unit economics and platform dynamics.

**Consumer, Retail & CPG**
- AI-driven innovation and product design: consumer insight mining from unstructured data, AI-assisted concept testing, trend forecasting.
- Demand planning and inventory optimization: ML demand forecasting to reduce GMROI drag and stockout costs.
- Personalization and marketing efficiency: next-best-action models, GenAI content generation for campaigns, media mix optimization.
- Read `references/consumer-retail-cpg.md` for retail P&L dynamics.

**Cross-sector: AI Skills, Org Design & Workforce Transformation**
The people-and-org layer that sits underneath every sector-specific transformation: skills gap assessment, role redesign, AI-augmented job architecture, reskilling program design, and change management. Increasingly a standalone workstream — clients who have deployed AI tools but are failing to realize value because the workforce doesn't know how to use them. Read `references/org-design-workforce.md` for the workforce transformation methodology.

### Key hypotheses to test on Day 1 (any sector-specific GenAI engagement)
1. Is the bottleneck technology, data, people, or process? (Usually people and process — not technology — in 2025+.)
2. Does the client have a clear "north star" use case with measurable ROI, or is this still exploratory?
3. What is the regulatory exposure for this specific AI application in this sector? (FDA, OCC, HIPAA, EU AI Act — sector-specific rules vary enormously.)
4. Is there competitive urgency — is a competitor already deploying this capability at scale?

### Common risks & failure modes
- Sector-specific GenAI projects that are technically successful but organizationally inert: the clinician doesn't use the AI triage tool because it wasn't co-designed with them.
- Underestimating data readiness requirements: sector-specific GenAI often requires proprietary training data (claims data, transaction data, clinical records) that is messy and poorly governed.
- Regulatory surprises mid-project that require redesign (common in healthcare AI and FS model risk contexts).

### Value levers
Sector-dependent, but always anchor to: (a) labor hours redirected from manual to judgment work; (b) decision speed and quality improvement (error rate reduction, cycle time); (c) revenue impact (new product features, conversion improvement, retention); (d) regulatory cost avoidance.

### Cross-references
`references/genai-enterprise-strategy.md` | `references/ai-orchestration.md` | `references/healthcare-life-sciences.md` | `references/financial-services.md` | `references/technology-media-telecommunications.md` | `references/consumer-retail-cpg.md` | `references/org-design-workforce.md`

---

## How to Use These Archetypes in Practice

### The Pattern-Matching Protocol

When a user describes a client situation, run this sequence before reaching for any framework:

1. **Industry + trigger scan**: What sector? What triggered the engagement (regulatory, competitive, internal crisis, strategic ambition)?
2. **Archetype match**: Which of the five archetypes does this map to? Is there a dominant one or a hybrid?
3. **Project shape hypothesis**: Based on the archetype, what are the likely workstreams, team structure, and typical engagement length?
4. **Risk & failure mode pre-load**: What are the known failure modes for this archetype? Surface them early in structuring and pre-wiring.
5. **Value anchor**: What is the value creation story most likely to resonate for this archetype? Build the business case logic from that anchor.

### Common Archetype Combinations

- **1 + 5** (GenAI operating model + sector-specific transformation): Most frequent. Client wants to deploy AI in a specific sector context AND needs governance around it.
- **2 + 4** (Sustainable ops + resilience): Green supply chain programs almost always have a resilience component.
- **3 + 1** (AI-augmented PMO + GenAI governance): Common in large transformation programs.
- **4 + 2** (Resilience + sustainability): Physical climate risk programs sit naturally at this intersection.

### Rapid Archetype Diagnostic (for client conversations)

These five questions reveal the dominant archetype in 30 minutes:

- "What was the thing that made this a priority right now?" → Identifies trigger and archetype
- "Where are you on your AI journey — experimenting, scaling, or governing?" → Archetypes 1 vs. 5
- "What keeps you up at night from a supply chain or operational perspective?" → Archetype 4
- "What's your board asking you about ESG or climate?" → Archetype 2
- "How confident are you in your project portfolio — are your big programs on track?" → Archetype 3

The question that generates the most energy and specificity is usually the real archetype.
