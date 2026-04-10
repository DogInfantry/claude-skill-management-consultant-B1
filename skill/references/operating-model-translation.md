# Operating Model Translation

This file covers the six-component operating model as a coherent consulting deliverable — how to diagnose it, design it, and communicate it as an integrated system rather than a collection of disconnected workstreams. It is distinct from `references/zero-based-org-design.md` (which covers organizational structure specifically, from a clean-sheet design perspective), `references/decision-rights-architecture.md` (which covers the governance component in detail), and `references/process-improvement.md` (which covers process analysis and redesign methodology). This file covers the operating model as a whole — the six interdependent components, the diagnostic approach for identifying which components are misaligned, the design principles for building them as a coherent system, and the communication approach for making the operating model visible and actionable to a leadership team.

The operating reality: "operating model" is one of the most overused and under-defined terms in consulting. It is used to mean everything from an org chart to a complete business system design. The result is that clients receive operating model deliverables that address one or two components (typically structure and maybe process) while leaving four components unchanged — and then are surprised when the transformation does not produce the expected performance improvement. A genuine operating model design addresses all six components as an interdependent system.

---

## The Six-Component Operating Model

Every organization's operating model has six components. All six must be designed and aligned for the operating model to function as intended. Misalignment in any one component degrades performance in all.

| Component | The Design Question | Misalignment Symptoms |
|-----------|--------------------|-----------------------|
| **Structure** | How is work grouped and accountability allocated? | Decision latency; unclear ownership; duplicated effort |
| **Process** | How does work flow to produce outcomes? | Handoff failures; rework; cycle time overruns |
| **Governance** | How are decisions made and escalated? | Bottlenecks at senior levels; accountability diffusion; inconsistent standards |
| **People and Culture** | What behaviors, capabilities, and norms are required? | Performance gaps in critical roles; culture-strategy misalignment; resistance to change |
| **Technology and Data** | What systems, information flows, and tools enable the model? | Manual workarounds; data quality issues; system fragmentation |
| **Performance Management** | How is performance measured, rewarded, and corrected? | Misaligned incentives; lagging indicators only; performance issues unaddressed |

The operating model design principle: **no component is independently effective if the others are misaligned.** A redesigned structure with unchanged processes is a new org chart with the same workflows. A new technology platform with unchanged culture is an expensive system that people work around. A performance management redesign with no change to incentives produces different metrics but the same behavior.

---

## The Operating Model Diagnostic

Before designing an operating model, diagnose which components are misaligned and how severely. The diagnostic produces a component-by-component heat map that directs design effort toward the highest-leverage interventions.

### The Diagnostic Framework: Five Questions Per Component

For each of the six components, assess:

1. **Is it fit for the strategy?** Does this component enable the organization to execute its strategy, or does it constrain it?
2. **Is it internally consistent?** Does this component work as designed, or does it generate internal friction, workarounds, or failure modes?
3. **Is it aligned with the other five components?** Does this component reinforce or undermine the design of the adjacent components?
4. **What does the data show?** What operational metrics, survey data, or financial indicators are diagnostic of this component's performance?
5. **What do the people say?** When employees and managers describe their experience of operating in this organization, what does the pattern of frustration, confusion, or inefficiency point to?

### Structure Diagnostic

**Indicators of structural misalignment:**
- Decision rights are unclear or contested — the same decision is being made by different people in different parts of the organization
- P&L accountability is not co-located with the authority to manage the cost and revenue drivers
- Coordination costs are high — teams spend disproportionate time in cross-functional meetings to compensate for the structural lack of integration
- Layer count is higher than comparable organizations; span of control is below benchmark

**Diagnostic data sources:** Org chart analysis, decision mapping exercise (see `references/decision-rights-architecture.md`), span-and-layer benchmarking, coordination cost survey (what % of leadership time is spent on internal alignment vs. external value creation).

### Process Diagnostic

**Indicators of process misalignment:**
- Cycle times for core processes are significantly above industry benchmarks
- Rework rates are high — a significant % of work must be redone because it was done incorrectly or without needed input the first time
- Handoffs between functions are the primary source of delay and quality loss
- Process exceptions are the norm rather than the exception — the standard process is not actually how work gets done

**Diagnostic data sources:** Process mapping (current-state SIPOC or swimlane maps), cycle time analysis, defect and rework tracking, exception rate analysis.

### Governance Diagnostic

**Indicators of governance misalignment:**
- Escalation rate is too high — too many decisions that should be made at lower levels are being escalated to senior leadership
- Decision cycle time is long — weeks or months for decisions that should take days
- Accountability for outcomes is unclear — when something goes wrong, it is not immediately clear whose responsibility it was
- Risk appetite is inconsistently applied — similar decisions are made differently in different parts of the organization

**Diagnostic data sources:** Decision inventory and classification (see `references/decision-rights-architecture.md`), escalation rate analysis, governance observation (attending decision meetings and mapping the actual vs. intended governance process).

### People and Culture Diagnostic

**Indicators of people/culture misalignment:**
- Critical roles have persistent performance gaps that are not being addressed
- Leadership behaviors do not model the values the organization espouses
- The culture (how people actually behave) does not support the strategy (e.g., a strategy requiring cross-functional collaboration in a culture that rewards individual performance)
- Attrition is high in high-value roles; talent acquisition for critical capabilities is consistently difficult

**Diagnostic data sources:** Employee engagement survey analysis, 360 feedback patterns, attrition analysis by role and tenure, cultural assessment (observation, focus groups, structured interviews with questions designed to surface actual rather than stated norms).

### Technology and Data Diagnostic

**Indicators of technology/data misalignment:**
- Manual workarounds are pervasive — people are doing in spreadsheets what systems should do
- Data quality is poor — decision-makers report frequently encountering inconsistent, incomplete, or unreliable data
- System fragmentation — the same information exists in multiple systems, and integration between them is manual or absent
- Technology decisions are made at functional level without an architecture view, producing an increasingly complex and brittle system landscape

**Diagnostic data sources:** System landscape map (application portfolio), data quality assessment, workaround audit (document the top 20 manual workarounds and the processes they substitute for), technology cost benchmarking.

### Performance Management Diagnostic

**Indicators of performance management misalignment:**
- Metrics measure activity rather than outcomes — the organization knows how busy it is but not how effective
- Incentives reward behavior that is strategically misaligned (e.g., sales incentives that reward revenue growth in declining margin segments)
- Performance issues are not addressed promptly — known underperformers persist in roles long past the point where the evidence of underperformance is clear
- Leading indicators are absent — the organization only knows how it performed last month, not what is likely to happen next month

**Diagnostic data sources:** KPI review (what is measured and at what frequency), incentive structure analysis, performance management process review (what actually happens when performance is below standard), leading vs. lagging indicator ratio.

---

## The Operating Model Design Sequence

The six components must be designed in a sequence that respects their interdependencies. Designing them simultaneously produces a coherent model; designing them sequentially in the wrong order produces a model where later components are constrained by earlier design choices.

**The correct design sequence:**

**Step 1 — Strategy and capabilities (the anchor).** What must the organization be able to do, at what performance level, to execute the strategy? (See `references/zero-based-org-design.md` Stage 1 for the capability specification format.) Every subsequent design choice must be tested against the capability requirements.

**Step 2 — Structure and P&L design.** Where is accountability for the primary value drivers concentrated? What is the P&L structure? (See `references/zero-based-org-design.md` Stage 3 for the structural design methodology.) Structure is designed before process because the process design will follow the structural logic — processes should flow across the structure, not work against it.

**Step 3 — Governance and decision rights.** What decisions are made where, by whom, with what escalation paths? (See `references/decision-rights-architecture.md` for the full methodology.) Governance is designed after structure because the governance model defines how the structural units interact.

**Step 4 — Process design.** How does work flow through the structure to produce the required outputs? Process design is done after structure and governance because the structure and governance define the handoff points and decision moments around which processes are built.

**Step 5 — Performance management.** What does the organization measure, and how does it motivate the behavior the strategy requires? Performance management is designed after the other components because it must incentivize performance in the structure, processes, and governance model that have been designed — not in the legacy model.

**Step 6 — People, culture, and technology.** What capabilities and behaviors are required? What systems and data enable the model? People and technology design is completed last not because it is least important — it is frequently the hardest to change — but because the requirements for people and technology can only be fully specified once the structure, governance, processes, and performance management design is established.

---

## The Operating Model Translation: Making It Actionable

The most common failure of operating model engagements is the production of a model that is theoretically coherent but practically incomprehensible. The translation challenge — converting an operating model design into something a leadership team can use to make decisions and guide implementation — is as important as the design itself.

### The Operating Model on a Page

Every operating model design should produce a one-page visualization that communicates the design choices for all six components and their relationships. The one-pager serves three purposes: alignment (ensures all leadership team members have a shared understanding of the design), communication (can be shared with the broader organization to explain what is changing and why), and navigation (during implementation, the one-pager is the reference point for checking whether specific decisions are consistent with the design intent).

**One-pager structure:**
- Center: the core value creation logic of the business (1–2 sentences)
- Surrounding: the six components displayed as interlocking elements (not as a list — as a system)
- For each component: 2–3 design principle statements (what is true about this component in the new design)
- Connecting threads: lines showing where specific components must work together to produce a specific outcome

This is a design artifact, not a presentation slide. It should be built collaboratively with the leadership team and iterated until every leader can look at it and recognize the design choices they made.

### The "So What" Test for Each Component

Before finalizing the operating model design, apply the "so what" test to each component: "If we implemented this component exactly as designed, what specifically would be different from today? What would an employee notice on their first day in the new model?"

If the answer to this test is vague ("things would be more efficient," "accountability would be clearer"), the design is not specific enough to be actionable. The test forces specificity that the design process may not have produced.

Examples of passing the "so what" test:
- **Structure:** "The commercial director in Germany will now own the full P&L for the German market — they will have authority to make pricing decisions up to €5M without headquarters approval."
- **Governance:** "The commercial committee will meet weekly rather than monthly, with authority to approve investments up to €10M without board referral."
- **Performance management:** "The quarterly bonus calculation will include a 30% weighting on customer retention, which was not previously measured."

### The Component Interdependency Map

For complex operating model designs, produce a one-page interdependency map showing which design choices in each component depend on design choices in other components. This serves as an implementation sequencing guide — changes that are interdependent must be made simultaneously, not sequentially.

**Example interdependency:** "The new governance model (monthly commercial committee with €10M authority) will not work effectively until the management reporting system provides committee members with the data they need to make those decisions — so the technology component (reporting enhancement) must be implemented before or simultaneously with the governance change, not after."

Interdependency failures are the primary cause of operating model implementation stalling after initial progress — the organization implements two or three components and then discovers that the remaining components cannot work without changes that have not yet been made.

---

## The Operating Model Communication: Three Audiences

The operating model must be communicated differently to three audiences with different needs.

### Audience 1: The Board and Owners

**What they need:** Confidence that the operating model enables the strategy and that the transformation program is addressing the right things. They do not need component-level detail — they need evidence that the design is coherent and that the leadership team has made clear choices.

**Communication format:** The operating model on a page, plus a 2–3 slide summary of the key design choices and their strategic rationale. The strategic rationale should connect each design choice to a specific capability required by the strategy. "We are centralizing procurement governance because our strategy requires €50M in cost reduction over 3 years, and the current fragmented model makes that impossible to achieve."

### Audience 2: The Leadership Team

**What they need:** Enough detail to govern the implementation and to make day-to-day decisions that are consistent with the design intent. They need to understand not just what the design says, but why — so that when specific situations arise that the design document did not anticipate, they can make a design-consistent call.

**Communication format:** The full operating model document (component-by-component design, interdependency map, implementation sequencing), plus a leadership workshop in which the team works through 3–5 scenarios to test their application of the design.

**The scenario test:** Present the leadership team with realistic situations that will arise during implementation and ask them to apply the operating model to decide what to do. "Under our new governance model, this investment proposal would go to the commercial committee rather than the CEO. But the amount is €8M and it's time-sensitive — what do we do?" If the leadership team cannot answer consistently, the design is not yet internalized and the communication is not complete.

### Audience 3: The Broader Organization

**What they need:** Enough to understand what is changing in their specific part of the organization, why it is changing, and what they need to do differently. They do not need the full operating model — they need the implications of the operating model for their day-to-day work.

**Communication format:** A cascade briefing structure — leaders brief their teams on the components of the operating model that affect them, using materials tailored to their level and function. The common mistake is distributing the full operating model document to the organization. The full document is useful for leadership; for the broader organization, it creates confusion without the context to interpret it.

---

## Common Failure Modes

**The org chart deliverable.** The operating model engagement produces a new org chart and a governance model, but leaves process, performance management, people, and technology unchanged. The client declares the operating model work complete. Six months later, performance has not improved because four of the six components are still aligned to the old model.

**The sequential implementation.** The implementation program works through the six components sequentially over 24 months: structure first, then process, then governance, then everything else. By the time the later components are implemented, the earlier components have been operating in an environment for which they were not designed, and the organization has adapted to the gaps in ways that make the later changes harder. Prevention: identify the minimum viable set of simultaneous changes required for the model to function, and implement them together.

**The missing performance management redesign.** The operating model design is comprehensive on structure, process, and governance, but the performance management component is left unchanged because "HR needs to lead that." The result: all other components change, but people continue to be measured and rewarded for the behaviors aligned to the old model. Culture follows incentives; culture does not change because the org chart changed.

**The technology assumption.** The operating model design assumes that specific technology capabilities exist or will be available at the time they are needed. The technology delivery is delayed (as it almost always is). The operating model implementation stalls because the structural and process changes assumed a system that is not yet live. Prevention: make technology dependencies explicit in the interdependency map; design interim-state processes that can operate without the technology while it is being built.

**The missing translation.** The operating model is designed in precise technical language that the design team understands perfectly. The leadership team nods along in the steering committee. Implementation begins. Within 90 days, different leaders are making different design-inconsistent decisions because they never internalized the design principles — they accepted the deliverable without understanding its implications. Prevention: the operating model communication to the leadership team must include scenario testing, not just information transfer.
