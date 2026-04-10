# Zero-Based Organization Design

This file covers the clean-sheet approach to organizational design — starting from first principles rather than incrementally restructuring what currently exists. It is distinct from the gap analysis, benchmarking, and structural framework content in `references/org-design-workforce.md` (which covers incremental org redesign diagnostics), and from the decision rights content in `references/decision-rights-architecture.md` (which covers the governance layer of an operating model). This file covers the methodology for designing an organization from scratch — or as close to scratch as the political and operational constraints of the client allow.

Zero-based org design (ZBOD) is used in three principal contexts: greenfield entity design (joint ventures, spin-offs, new market entries), major transformation programs where the existing structure is fundamentally unsuited to the future strategy, and post-merger integration where neither legacy structure should be preserved as the template for the combined entity.

---

## The Fundamental Premise: Structure Follows Strategy — But Most Structures Don't

The Chandler principle — that organizational structure should follow strategy — is universally accepted and universally violated in practice. The reason: organizations accumulate structural complexity over time as the result of individual decisions made for individual reasons (an acquisition, a leader's preference, a historical regulatory requirement, a political accommodation) that were never reviewed as a system. The cumulative result is an organization shaped by its history rather than its strategy.

**The incremental redesign failure mode:** When organizations attempt to redesign by modifying the existing structure, they start with the wrong foundation. They eliminate some roles, consolidate some reporting lines, and add some new functions — but the underlying logic of the structure (why these units exist at all, why this authority is at this level, why these decisions are made in this part of the organization) is never examined. The result: a redesigned structure that has the same misalignments as the original, only with fewer headcount and slightly different names.

Zero-based design avoids this failure mode by starting the design process with the question "what structure would we build if we were starting today?" rather than "how do we improve what we have?"

---

## When to Use Zero-Based Design vs. Incremental Redesign

Zero-based design is more expensive, politically harder, and takes longer than incremental redesign. It is warranted when:

| Condition | Implication |
|-----------|-------------|
| The strategy has changed fundamentally, not marginally | The old structure was built for a different business model; modification cannot address the mismatch |
| Post-merger: two legacy structures, neither ideal | Neither legacy structure should be the template; a combined structure should be purpose-designed |
| Spin-off or carve-out: new entity | No legacy structure exists by definition; design from clean sheet |
| The organization has layer accumulation of 10+ years without systematic review | Structural drift has accumulated beyond what incremental correction can address |
| The existing structure is politically frozen (change is impossible without a clean break) | A zero-based process can be positioned as "everyone redesigns from scratch" rather than "some people's jobs are being restructured" |
| Transformation at scale (>30% headcount change anticipated) | Changes of this magnitude cannot be managed as marginal modifications |

Incremental redesign is appropriate when the strategy change is moderate, the existing structure has only specific misalignments, and the organization has the organizational health to implement targeted change without a full reset.

---

## The Zero-Based Design Process: Six Stages

### Stage 1: Strategy Translation (2–3 Weeks)

The design process begins not with the organization but with the strategy. The question is: "What must this organization be able to do, at what level of performance, to execute this strategy?"

**Step 1: Identify the value drivers.** What creates value in this business? For a consumer products company, it may be brand management and retailer relationships. For a B2B software company, it may be product development and customer success. For a professional services firm, it may be talent development and client relationship management. The organizational design should concentrate resources and authority around the value drivers.

**Step 2: Define the required capabilities.** Translate the value drivers into organizational capabilities — the things the organization must be able to do, not just the functions it must have. The distinction matters: "we need a marketing function" is not a capability; "we need to be able to launch new products in 90 days and achieve 40% market penetration within 12 months" is a capability.

**Capability specification format:**
```
Capability: [What the organization must be able to do]
Performance standard: [At what speed, quality, or cost]
Current state: [Can we do this today, and at what level?]
Capability gap: [Gap between required and current performance]
Build / buy / partner: [How will this capability be developed?]
```

**Step 3: Identify the critical decisions.** What are the 10–15 most consequential decisions this organization makes repeatedly? (See `references/decision-rights-architecture.md` for Decision Harvesting methodology.) The organizational structure should place authority for these decisions at the right level — neither too high (creating bottlenecks) nor too low (creating risk).

**Output of Stage 1:** A capability specification — the list of what the new organization must be able to do, at what performance standard, and which capabilities are currently present vs. absent.

---

### Stage 2: Design Principles (1–2 Weeks)

Before drawing any boxes or lines, establish the design principles — the constraints and values that will govern every structural decision in the design. Design principles prevent the design from becoming an exercise in preference ("I think we should have a COO" or "I prefer flat structures") and ensure it remains an exercise in logic ("structures that do not put customer P&L accountability at the BU level will not work for our strategy").

**How to develop design principles:**

Run a working session with the leadership team (typically 4–8 executives) to answer: "For each of our most important strategic imperatives, what does that imply about how the organization should be structured?"

Example outputs from a typical session:

*Strategic imperative: Grow enterprise market segment from 20% to 50% of revenue*
→ Design principle: Enterprise go-to-market must be a dedicated segment with its own sales, customer success, and product alignment — not a sub-function within a generalist commercial organization.

*Strategic imperative: Achieve 25% faster product release cycles*
→ Design principle: Product and engineering must be co-located organizationally (same reporting line or tight governance mechanism) — siloed reporting destroys release velocity.

*Strategic imperative: Expand into five new geographies in three years*
→ Design principle: Geographic general management capability must be embedded in the structure — not operated from headquarters by functional leaders who do not own P&L for the territory.

**Typical design principles set (4–8 principles):**
- Accountability for the customer relationship and P&L must be concentrated in a single role
- Cross-functional collaboration on [specific activity] requires shared governance, not sequential handoffs
- Strategic planning and execution oversight must not be co-located in the same role (separation of planning from operations)
- The structure must support [culture principle] — for example, "The structure must not create more than two layers of management between a frontline employee and a business unit P&L owner"

**The test:** At the end of Stage 2, any proposed structural element should be testable against the design principles. If a proposed unit or reporting line cannot be justified by at least one design principle, it should not exist in the design.

---

### Stage 3: Clean-Sheet Structural Design (2–4 Weeks)

With capabilities specified and design principles established, the structural design can begin. The sequence follows a defined logic:

**Level 1: The governing design choice — how is value aggregated?**

The first structural question is: at what level does the organization aggregate its primary business logic?

- **Customer-facing aggregation:** Organize around customer segments (Enterprise, SMB, Consumer) if the primary driver of business performance is customer relationship depth and cross-sell breadth.
- **Product aggregation:** Organize around product lines if the primary driver is product capability depth and development velocity.
- **Geographic aggregation:** Organize around geographies if the primary driver is local market presence, regulatory compliance, and cultural adaptation.
- **Functional aggregation:** Organize around functions (Sales, Operations, Technology, Finance) if the primary driver is scale efficiency in each functional domain.

Most large organizations combine these — for example, a matrix of geography and function, or a divisional structure by product line with shared functional services. The clean-sheet question is: which aggregation logic serves the strategy best, without the constraints of what already exists?

**Level 2: P&L structure**

Where does P&L accountability sit in the design? This is the single most consequential structural decision because it determines where resource allocation decisions are made, where performance accountability rests, and where career-defining leadership roles exist.

In a zero-based design, the P&L structure is designed before the reporting structure — not derived from it. The question is: "At what level of the organization does a manager have the complete accountability for revenue generation, cost management, and capital deployment that constitutes genuine P&L ownership?" Design the P&L units first. The reporting structure follows.

**Level 3: Functional design**

For each major functional domain (Finance, HR, Technology, Legal, Marketing, Operations, etc.), the clean-sheet question is: "Which of these activities must be embedded in the business units for proximity to the customer and speed? Which must be centralized for scale, standardization, and risk management? Which can be outsourced without capability loss?"

The answer produces the shared services vs. embedded function allocation — a critical design parameter for efficiency and cost.

**Clean-sheet heuristics:**
- Functions that require real-time customer knowledge → embed in business units
- Functions that benefit from standardization and scale → centralize in shared services
- Functions with high compliance or risk management requirements → centralize with clear reporting to board or C-suite
- Functions whose primary output is a commodity → consider outsourcing

**Level 4: Spans and layers**

Once the structural units are defined, set the target spans of control and layer count before drawing reporting lines. Designing spans and layers before reporting lines prevents the most common structural error: designing a logical structure and then discovering it creates a 12-layer hierarchy that violates every benchmark.

**Target spans by level (for a professionally managed organization):**
- CEO: 5–8 direct reports
- C-suite to senior VP: 4–8 direct reports
- VP to Director: 6–10 direct reports
- Director to Manager: 6–10 direct reports
- Manager to Individual Contributor: 8–15 direct reports

**Target layers by organization size:**
- <200 employees: 3–4 layers (CEO to individual contributor)
- 200–1,000 employees: 4–5 layers
- 1,000–5,000 employees: 5–7 layers
- 5,000+ employees: 7–9 layers (rarely more than 9 for any global business)

If the designed structure requires more layers than the target to accommodate the required P&L units and management roles, the structure is too complex — revisit the unit design.

---

### Stage 4: Role Design (2–3 Weeks)

Structural design defines the units. Role design defines the individual jobs within those units. In zero-based design, roles are defined before people are placed into them.

**The zero-based role design principle:** Start with a blank job description for every role in the new structure. Do not start with existing role descriptions and modify them — this anchors the design in the legacy role configuration rather than the new structural logic.

**For each role, specify:**

| Element | Specification |
|---------|--------------|
| Role purpose | One sentence: why does this role exist? What would fail if it did not? |
| Accountabilities | 4–6 outcomes the role is accountable for, not activities |
| Decision rights | What can this role decide unilaterally? What requires escalation? |
| Required capabilities | The skills, knowledge, and experience the role requires to succeed |
| Key relationships | Internal (peers, superiors, reports) and external (customers, partners, regulators) |
| Performance metrics | 3–5 metrics by which the role's success is measured |

**The role design test:** For each proposed role, ask: "If we hired the best possible person for this role, would they be able to create the value this role is designed to deliver? Or does the role design create structural barriers to that value creation?" If the answer is the latter, redesign the role.

**Eliminating role duplication:**
In a zero-based design, every role must have a distinct accountability set. If two roles have materially overlapping accountabilities, one of them should not exist, or the accountability boundary should be redrawn to eliminate the overlap.

---

### Stage 5: Transition Design (2–4 Weeks)

The gap between the clean-sheet design and the current state is the transition design challenge. Zero-based org design does not mean ignoring what currently exists — it means designing the destination state independently of the current state, and then designing the path from here to there.

**The transition assessment:**

For each proposed role in the new design, assess:
1. **Existing fit:** Is there a current employee who could fill this role without material development?
2. **Potential fit:** Is there a current employee who could fill this role with targeted development over 6–12 months?
3. **External hire required:** Does the role require capabilities not available internally?
4. **No match:** This role's responsibilities were previously handled differently; specific attention to the transition is needed.

**Transition sequencing:**
Not all structural changes can happen simultaneously. Design the transition in waves:

- **Wave 1 (Day 1–90):** Structural changes required for legal, regulatory, or operational continuity. Leadership appointments. Customer-facing structure finalized.
- **Wave 2 (Month 3–9):** Internal functional reorganization. Shared services consolidation. Process redesign to support new structure.
- **Wave 3 (Month 9–18):** Capability building for roles that are new or substantially different. Culture and behavior change to support new operating model.

**People process design:**
Zero-based design requires a rigorous and transparent people process:
- Communication: every affected employee understands what is changing, by when, and what their role is in the new design
- Selection process: where existing roles map to new roles, the selection criteria and process must be defined and applied consistently
- Severance and support: for roles that do not exist in the new design, a support process (outplacement, internal redeployment, severance terms) must be designed before the structure is announced

Announcing a structural design without a clear people process creates prolonged uncertainty that degrades organizational performance — often for 6–12 months.

---

### Stage 6: Operating Model Completion (Concurrent with Stages 4–5)

Organizational structure is one component of an operating model. A zero-based design is complete only when the five remaining components are also designed:

| Component | Design Question |
|-----------|----------------|
| **Structure** | What units exist, how do they relate, who reports to whom? (Stages 1–4) |
| **Processes** | How does work flow across the new structure? Which processes must be redesigned for the new structural logic? |
| **Governance** | How are decisions made? (See `references/decision-rights-architecture.md`) |
| **People and culture** | What behaviors, capabilities, and norms must the new structure develop and reinforce? |
| **Technology and data** | What systems, data flows, and digital tools support the new operating model? |
| **Performance management** | How is performance measured and incentivized in the new structure? |

The most common zero-based design failure is treating structure as the complete deliverable. A new org chart with unchanged processes, unchanged governance, and unchanged performance management produces minimal value change.

---

## Preserving What Works: The Cultural Heritage Inventory

Zero-based does not mean zero-respect for what the current organization does well. Before designing the new structure, conduct a cultural heritage inventory — a deliberate effort to identify the organizational capabilities, culture elements, and informal practices that have created value and should be preserved.

**The heritage inventory process:**
- Interview 20–40 people at various levels: "What is this organization uniquely good at? What would we be foolish to change?"
- Identify the informal practices that produce outcomes the formal structure does not explain (e.g., a weekly informal lunch between the engineering and commercial leads that resolves misalignment before it becomes conflict)
- Identify the cultural values that are differentiating and authentic (not aspiration, but the values employees actually observe being modeled)

**Incorporating heritage into the design:** For each heritage element identified, design an explicit mechanism in the new structure that preserves it. If the informal engineering-commercial lunch is valuable, create a formal version of the touchpoint in the governance design. If the culture of customer obsession is differentiating, design performance metrics and incentives in the new structure that reward customer-obsessed behavior at every level.

The cultural heritage inventory is both analytically valuable and politically important — it signals to the organization that the zero-based process is not a demolition of what they have built, but a design that honors what works and changes what does not.

---

## Common Failure Modes

**Starting with the org chart before the strategy.** Drawing boxes before establishing what the organization must be able to do produces a structure that looks organized but serves no analytical purpose. Strategy → capabilities → design principles → structure is the only correct sequence.

**Designing for today's organization size, not tomorrow's.** A zero-based design for a 500-person organization that must grow to 2,000 in three years will be obsolete before it is fully implemented. Design with explicit assumptions about what the organization must be able to accommodate as it scales.

**Failing to complete the operating model.** Announcing a new org chart as the deliverable, without redesigning the processes, governance, incentives, and technology that make the structure work, produces an expensive reorganization with minimal performance improvement. Structure without operating model completion is reorganization theater.

**Under-investing in the people process.** The people process — selection, communication, development, severance — is not a downstream HR activity. It is a core design element that must be specified before the structural announcement. Organizations that announce structures without clear people processes lose their best talent (who immediately start interviewing elsewhere) and demoralize the rest.

**The political compromise structure.** In most real organizations, zero-based design produces a structure that reduces the number of executive roles or changes their scope. Political negotiations often result in the creation of "new" executive roles that are really the old roles renamed, to accommodate executives who would otherwise exit. The result is a structure that looks zero-based and functions like the old one. The remedy is to conduct the design process with genuine leadership commitment to the clean-sheet logic, and to manage the political consequences as a separate workstream rather than solving them by corrupting the design.

**Declaring victory at go-live.** Organizational designs require 12–24 months of operation before they are either confirmed as working or revealed as needing adjustment. Go-live is not the end of the engagement — it is the beginning of the operating phase. Build in a 90-day and 12-month design review as standard deliverables.
