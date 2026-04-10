# Cost Restructuring Anatomy

This file covers the design and delivery of large-scale cost restructuring programs — how to identify cost reduction opportunities with precision, size them credibly, sequence them for delivery, and manage the human and organizational dimensions that determine whether savings are captured or evaporate. It is distinct from `references/process-improvement.md` (which covers process-level efficiency), `references/zero-based-org-design.md` (which covers organizational structure as a cost lever), and `references/synergy-modeling-validation.md` (which covers the cost synergy component of M&A). This file covers cost restructuring as a standalone engagement type — the standalone cost program, the performance improvement program, and the cost response to a profit recovery situation.

The operating reality: cost reduction programs routinely underdeliver. The studies that track realized vs. announced savings consistently show 30–50% shortfalls. The causes are not mysterious — they are structural: savings are identified at the initiative level but tracked at the P&L level where attribution is difficult, one-time savings are conflated with sustainable run-rate savings, cost reductions are reversed by volume growth that absorbs the savings, and organizational resistance converts paper savings into workarounds rather than genuine elimination. This file is organized around avoiding these failure modes.

---

## The Cost Anatomy: Seven Cost Categories

Before identifying savings opportunities, understand the cost structure completely. Most cost analyses stop at the functional or departmental level; the value-creating diagnostic goes deeper to the cost driver level.

| Category | What It Is | Primary Savings Levers | Typical Realization Risk |
|---|---|---|---|
| **Direct labor** | People cost directly attributable to producing the product or service | Productivity improvement; work design; automation; offshore/nearshore | Medium — labor savings require headcount reduction or redeployment, which has human and organizational costs |
| **Indirect labor** | People cost in support and overhead functions (finance, HR, IT, legal, procurement) | Spans and layers; shared services; outsourcing; process automation | Medium — often political; support functions protect their headcount |
| **Cost of goods sold (COGS)** | Direct material and supplier costs | Procurement leverage; specification redesign; supplier rationalization; should-cost modeling | Low-medium — procurement savings are generally well-tracked and well-managed |
| **External spend** | Consulting, professional services, marketing, IT spend | Category management; vendor rationalization; demand management; make vs. buy | Low — quick wins available through demand management; harder to sustain |
| **Technology and infrastructure** | Systems, hardware, cloud, data center | Application rationalization; infrastructure consolidation; cloud migration; vendor renegotiation | Medium — technology savings often require upfront investment; realization is delayed |
| **Footprint** | Real estate, facilities, logistics network | Location optimization; remote work policy; network design | Low — real estate savings are real and trackable; logistics network savings require capital investment |
| **Waste and complexity** | Costs of doing things wrong, doing unnecessary things, or doing right things inefficiently | Defect and rework elimination; product/SKU rationalization; process simplification | High — waste savings are notoriously difficult to track and sustain |

The category with the highest realization risk is waste and complexity — because the savings are dispersed across many processes and functions, the baseline is often not well-defined, and the savings are frequently re-absorbed by activity growth rather than falling to the bottom line.

---

## The Cost Diagnostic: From P&L to Cost Driver

### Level 1: The P&L Benchmarking

Start with the top-level cost structure and benchmark against comparable organizations. The purpose is to identify the cost categories where the client is materially above peer benchmarks — these are the priority diagnostic areas, not necessarily the priority savings areas.

**Benchmarking sources by cost category:**
- Labor cost as % of revenue: published industry benchmarking (Hackett Group for support functions; sector-specific benchmarks from consulting data); competitor disclosure analysis
- SG&A as % of revenue: public company filing analysis; industry trade data
- COGS as % of revenue: public company data; industry cost structure analysis
- External spend intensity: less commonly published; triangulate from procurement maturity assessments and management commentary in earnings calls

**The benchmarking interpretation caveat:** A cost that is above the benchmark is a hypothesis for investigation, not a confirmed saving. The client may have a strategic reason for the higher cost (premium quality, proprietary capability, regulatory requirement), or the benchmark may be an inappropriate comparator. The diagnostic must explain the gap, not just identify it.

### Level 2: The Cost Driver Analysis

For each cost category identified as a priority, decompose the cost to its economic drivers. Cost driver analysis asks: what causes this cost to be the level it is?

**Labor cost driver decomposition:**
- Headcount × average fully-loaded cost per FTE
- Headcount = volume of work ÷ productivity (output per FTE)
- Fully-loaded cost = base salary × benefits multiple × overhead allocation

The driver decomposition reveals which lever is the opportunity: Is the cost high because of high headcount per unit of volume (productivity issue)? Or because of high cost per FTE (compensation and benefits issue)? Or because of high overhead allocation (cost allocation issue rather than a real cost difference)?

**External spend driver decomposition:**
- Number of suppliers × average spend per supplier × average price per unit
- Driver analysis asks: is the spend high because of too many suppliers (rationalization opportunity), too high volume (demand management opportunity), or too high price (procurement leverage opportunity)?

### Level 3: The Activity-Based View

For labor costs specifically, the most actionable diagnostic moves below the headcount level to the activity level: what are these people actually doing, and which activities are candidates for elimination, reduction, automation, or offshoring?

**The activity census protocol:**
1. Identify the population of roles in the focus area
2. For each role, document the activities performed and the estimated time allocation across activities
3. Sort activities into four categories: value-adding (contributes directly to customer value or regulatory requirement), value-enabling (necessary to perform value-adding activities), non-value-adding but required (compliance, governance, audit), non-value-adding and not required (rework, duplicative checking, excessive reporting)
4. The non-value-adding and not required category is the immediate savings opportunity; the non-value-adding but required category is the process and governance redesign opportunity

**The warning:** Activity census data is highly subject to respondent bias. People systematically overstate time on value-adding activities and understate time on non-value-adding activities. Apply a correction factor: validate survey responses against observed behavior (time-in-motion studies, system log analysis) for a random sample of the population.

---

## Savings Identification: The Bottom-Up Build

The most credible savings identification process is a bottom-up build — initiative by initiative, with a specific savings calculation for each initiative rather than a top-down percentage target allocated to each function.

### The Initiative Template

For each savings initiative:

| Field | Content |
|---|---|
| **Initiative name** | Specific, descriptive (not "HR efficiency" — "Consolidate HRBP function from 1 per 150 employees to 1 per 200") |
| **Cost category** | Which of the seven categories does this address? |
| **Gross savings** | Total cost eliminated before one-time costs and implementation costs |
| **One-time costs** | Severance, technology, transition costs required to achieve the saving |
| **Net savings (run-rate)** | Gross savings minus one-time cost amortized over 3 years, or as specified by client |
| **Confidence level** | High (>80% confidence), Medium (50–80%), Low (<50%) |
| **Timing** | Month in which savings begins to flow; month in which full run-rate is achieved |
| **Dependency** | What other initiatives or decisions does this depend on? |
| **Owner** | Who in the client organization is accountable for delivery? |
| **Risk** | Primary risk to realization; mitigation |

### The Confidence Tiering Discipline

Confidence tiering prevents the most common savings identification error — presenting all savings as equally certain when they manifestly are not.

**High confidence savings (apply 90% realization factor):**
- Savings that require only a management decision and have no significant implementation complexity
- Savings where the cost driver is fully understood and the lever is fully in management's control
- Savings that have been achieved by comparable organizations in comparable timeframes

**Medium confidence savings (apply 65% realization factor):**
- Savings that require significant implementation effort or change management
- Savings that depend on external parties (supplier renegotiation, regulatory approval)
- Savings where the baseline measurement is uncertain

**Low confidence savings (apply 35% realization factor):**
- Savings that depend on technology delivery on schedule
- Savings in categories with high historical realization shortfalls (complexity reduction, waste elimination)
- Savings where a similar initiative has been attempted previously and underdelivered

The total expected savings is the sum of savings × confidence factor for each initiative, not the gross total of all identified savings. Present both numbers: gross identified savings (the full potential) and risk-adjusted expected savings (the credible forecast).

---

## The Sequencing Logic: Phasing for Maximum Credibility and Minimum Disruption

Cost restructuring programs fail when sequenced incorrectly — either because quick wins are deferred while complex structural changes are pursued, or because structural changes are attempted before organizational readiness exists.

### The Phasing Framework

**Phase 1 (Months 1–6): Immediate actions and demand management**
Focuses on: external spend demand management, discretionary spend freeze, procurement leverage on existing contracts, process stops (eliminating activities that consume cost without creating value).
Characteristics: minimal implementation risk; no restructuring required; savings begin in weeks, not months. Purpose: generate early credibility for the program and fund the investment required for later phases.

**Phase 2 (Months 4–18): Organizational and process redesign**
Focuses on: spans and layers optimization, shared services consolidation, process automation where systems are available, footprint rationalization.
Characteristics: requires organizational change management; some headcount reduction; implementation risk is medium. Purpose: the structural cost reduction that creates sustainable savings.

**Phase 3 (Months 12–36): Transformational and technology-enabled**
Focuses on: major technology-enabled process redesign, operating model transformation, major supplier or business model restructuring.
Characteristics: high implementation complexity; long realization timeline; dependent on technology delivery. Purpose: the step-change in cost efficiency that Phase 1 and 2 cannot achieve.

**The overlap principle:** Phases should overlap — Phase 2 activities begin before Phase 1 is fully complete, and Phase 3 design begins during Phase 2 implementation. Sequential phasing with clean handoffs produces programs that stall between phases and lose momentum.

---

## The One-Time Cost Estimate

One-time costs are routinely underestimated in cost restructuring programs. The consequence: the savings case looks better than it is, and CFOs discover mid-program that the net economics are significantly worse than presented.

**One-time cost components:**

**Severance:** Typically 3–6 months of salary per affected employee in developed markets (varies significantly by jurisdiction, collective bargaining agreements, and contract terms). The common error: applying a single severance estimate across all affected roles without accounting for tenure distribution, contractual obligations, or geographic variation.

**Transition costs:** The cost of running the old and new operating model simultaneously during the changeover period. Typically 10–20% of annual savings for a 6-month transition period. This is a budget line item that most cost cases omit.

**Technology:** System changes required to support the new operating model. Technology costs are systematically underestimated — apply a 1.5× contingency to any technology estimate provided by IT at the initiative identification stage.

**Change management and training:** Communication, training, and behavioral change support. Typically 3–5% of total program cost. Frequently cut from the program budget to improve the savings case, which then increases realization risk.

**The one-time cost rule of thumb:** Total one-time costs for a comprehensive cost restructuring program typically run at 0.5–1.5× first-year gross savings. If the one-time cost estimate is below 0.5× first-year gross savings, it is likely underestimated.

---

## Tracking and Governance: Closing the Realization Gap

The realization gap — the difference between identified savings and actually captured savings — is primarily a governance problem, not an analytical problem. The savings identification was correct; the tracking and accountability failed.

### The Three Realization Failure Modes

**The absorption problem:** The savings are realized at the activity level (headcount reduced, contract cancelled) but re-absorbed at the P&L level because volume grows into the freed capacity. A finance team that is reduced from 50 to 40 people does not produce a saving if the 40 people are subsequently running at 120% utilization because transaction volume increased. Prevention: track savings at the activity level (capacity removed) and separately track whether removed capacity is being re-created.

**The stranding problem:** Costs are reduced in one part of the organization, but the supporting costs in other parts of the organization are not reduced proportionally. A headcount reduction in a business unit that is served by a shared service center does not reduce shared service center costs unless the business unit's service demand is also reduced. Prevention: require cross-functional savings cases that trace the full cost chain.

**The reversal problem:** Savings that were achieved are subsequently reversed — rehires to backfill reduced headcount, contract reinstatements, discretionary spending that resumes after an initial freeze. Prevention: savings should be locked in the budget baseline immediately upon realization, making them structurally impossible to reverse without an explicit budget decision.

### The Savings Tracker

The governance mechanism that prevents realization failure is a savings tracker maintained at the initiative level — not the P&L level.

**Savings tracker columns:**
- Initiative name and ID
- Planned savings (from the business case)
- Timing: planned month of first saving; planned month of full run-rate
- Current status (on track / at risk / delayed / cancelled)
- Savings realized to date (actuals, from finance)
- Variance (planned vs. actual) and explanation
- Actions required to close variance
- Owner and next review date

The savings tracker is reviewed at every program steering committee. Initiatives that are at risk require a specific action plan with an owner and a deadline. Initiatives that are cancelled require a replacement — the total expected savings should not decline without an explicit decision to accept a lower target.

---

## Common Failure Modes

**The top-down target problem.** The CFO announces a 15% cost reduction target and then allocates it to functions as a quota. Each function finds 15% somewhere, often by cutting the easiest things rather than the most structural things. The result: headcount in cost-of-living-low locations is cut while structural complexity in high-cost locations is maintained; discretionary spend is frozen for 6 months and then returns to prior levels. Prevention: build savings bottom-up from specific initiatives; test the total against the top-down target; redesign the target if the bottom-up analysis does not support it.

**The savings case that double-counts.** Two initiatives both claim credit for the same $5M saving — one from a headcount reduction and one from a process redesign that enables the headcount reduction. The total savings case overstates by $5M. Prevention: explicit initiative dependency mapping; rule that no dollar of saving can be counted in more than one initiative.

**The missing P&L owner.** Every savings initiative needs a budget owner — someone whose budget will visibly decline by the amount of the saving when the initiative is delivered. Without a budget owner, savings are identified but never locked in. Prevention: at initiative identification, require the budget owner to sign off on the saving before it is included in the program total.

**The communication failure that triggers attrition.** Cost restructuring programs require careful communication management — not to hide the program (that never works and makes the outcome worse) but to sequence communications so that clarity about what is changing and for whom comes as quickly as possible. The most damaging pattern: prolonged uncertainty during which high-performers (who have the most options) leave before the program is complete, and the organization loses the talent it most needs to deliver the transformation.
