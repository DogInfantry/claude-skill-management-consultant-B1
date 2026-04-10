# Technology Vendor Selection

This file covers the consulting methodology for enterprise technology vendor selection — how to structure a rigorous selection process, design evaluation criteria that are genuinely discriminating, run a request for proposal (RFP) process that produces actionable results, score vendor responses rigorously, conduct reference checks and demos that go beyond the vendor's prepared show, and manage the commercial negotiation. It is distinct from `references/due-diligence-deep-dive.md` (which covers technology risk as one component of M&A due diligence) and `references/operating-model-translation.md` (which covers technology as one component of an operating model design). This file covers technology vendor selection as a standalone consulting engagement type.

The operating reality: enterprise technology vendor selection is one of the most consequential decisions a large organization makes — a major ERP, CRM, or platform selection will shape operations for 7–15 years and costs of major enterprise implementations routinely run to 8–9 figures. Despite this, the selection process is frequently structured around what the vendors offer rather than what the organization needs, RFP criteria are not weighted by strategic importance, demo scripts are provided by the vendors rather than designed by the client, and reference checks are conducted with references the vendor has hand-selected. The result: selections that are technically defensible but often strategically wrong.

---

## The Selection Process Architecture

A well-structured vendor selection process has five phases. Each phase has a defined objective, deliverable, and decision gate.

### Phase 1: Requirements Definition (3–6 weeks)

**Objective:** Define what the organization needs, before engaging any vendor.

The most common vendor selection failure begins here: requirements are defined reactively (by reviewing vendor capabilities) rather than proactively (by working forward from business requirements). Requirements defined reactively are shaped by what vendors offer; requirements defined proactively are shaped by what the organization actually needs.

**Requirements definition methodology:**

**1. Business capability requirements:** What business capabilities must the technology enable? (Not features — capabilities.) Derived from the operating model design and the strategic priorities. "Enable real-time inventory visibility across all distribution centers" is a business capability requirement. "Track inventory in real time" is a feature. The business capability framing forces precision about what the organization needs the technology to do, not what the technology can do.

**2. Functional requirements:** The specific functions the technology must perform. Organized by priority: must-have (deal-breakers if absent), should-have (significant value, but workarounds exist), nice-to-have (marginal value). The must-have / should-have / nice-to-have distinction is critical — RFP processes that treat all requirements equally produce evaluations where vendors that score 75% on must-haves receive the same total score as vendors that score 100% on must-haves.

**3. Non-functional requirements:** Performance, security, scalability, availability, integration, and compliance requirements. These are frequently underspecified in the requirements definition and then surface as problems during or after implementation.

**4. Integration requirements:** The specific systems the new technology must integrate with, and the integration architecture required. Integration is the most frequently underestimated technical complexity in enterprise technology selection.

**5. Implementation and change management requirements:** Timeline, internal implementation capacity, change management complexity, and phasing constraints that will affect vendor selection.

**Deliverable:** A requirements document that is used to structure the RFP, design the demo script, and score vendor responses. Requirements that are not in the requirements document should not be scored in the evaluation.

**Decision gate:** Leadership team approval of requirements before any vendor engagement begins.

### Phase 2: Market Scan and Long-list (2–3 weeks)

**Objective:** Identify all credible vendors and create a long-list of 6–10.

**Long-list development sources:**
- Analyst firm assessments (Gartner Magic Quadrant, Forrester Wave) for broad category coverage. Caveat: analyst assessments reflect the analysts' view of the general market, not the specific client's requirements.
- Peer company reference: which vendors have comparable organizations selected, and what has their experience been?
- Expert network interviews: practitioners who have implemented these systems and can provide unfiltered views of vendor performance
- Consultant knowledge base: the firm's proprietary experience with vendor performance across multiple client implementations

**Long-list screening criteria:** Apply a brief screen to remove vendors that cannot plausibly meet the must-have requirements before investing in a detailed RFP process. A vendor that clearly cannot meet a must-have requirement wastes both parties' time in a full RFP.

**Deliverable:** Long-list of 6–10 vendors with brief rationale for inclusion.

### Phase 3: RFP Process (4–8 weeks)

**Objective:** Gather structured, comparable responses from all long-listed vendors.

**RFP design principles:**

**Be specific in the questions.** Generic RFP questions ("please describe your approach to customer service") produce generic answers that are not evaluable. Specific questions ("what is your average response time for P1 incidents, measured against SLA, for clients of comparable size in our sector — please provide the data from the last 12 months") produce specific, evaluable answers.

**Design scenarios, not just feature checklists.** Require vendors to describe how they would handle specific use cases that reflect the client's actual operating environment. Scenarios produce more useful information than feature checklists because they force vendors to describe actual system behavior rather than claim feature presence.

**Require evidence, not assertions.** For every claim that can be evidenced, require evidence. "Please describe your security architecture" is not evaluable; "please provide your most recent penetration test summary and your SOC 2 Type II report" is.

**Size the response appropriately.** RFPs that allow unlimited response length produce documents of 300+ pages that are impossible to evaluate consistently. Set page limits for each section; weight the sections by importance.

**Pricing structure:** Require vendors to provide pricing in a standard format that enables comparison. Vendor pricing structures are designed to be incomparable — each vendor bundles and unbundles differently, uses different metrics, and layers different components. Design a standardized pricing template that requires all vendors to price the same defined scope.

**Deliverable:** Comparable vendor responses to the structured RFP.

### Phase 4: Evaluation and Due Diligence (4–6 weeks)

**Objective:** Score vendors rigorously, conduct demos, and perform reference checks.

**The scoring methodology:**

Weight criteria by strategic importance before seeing vendor responses. Weighting criteria after reviewing responses introduces bias — the natural tendency is to weight heavily the criteria where a preferred vendor excels. The weighting should reflect the requirements document; must-have requirements should carry the majority of the functional score.

**Demo design:**

The most important rule in demo design: write your own script, not the vendor's. Vendors who are given a demo script will prepare an optimized presentation for exactly that script. A demo of a script the vendor prepared tells you the vendor can perform optimized demos; it does not tell you what the system actually does.

**The client-designed demo script:**
1. Select 4–6 scenarios from the client's actual operating context that represent the most important use cases
2. Require each vendor to demo the scenarios using their standard system (not a specially configured demo environment)
3. Include at least one scenario that represents a use case the system is likely to struggle with — the stress scenario. A vendor who smoothly handles the stress scenario has a system that can genuinely handle it. A vendor who says "we'd handle that differently in practice" has revealed a limitation.
4. Reserve 30–45 minutes for the client team to drive the system themselves — not a vendor-facilitated show, but unguided exploration

**Reference check design:**

The critical rule: do not accept only vendor-provided references. Vendor references are invariably satisfied customers who have agreed to be advocates. The information value of vendor references is therefore low for selection purposes but high for specific technical and implementation questions.

**Reference sourcing strategy:**
- Ask the vendor for references; use them for specific technical and implementation questions where objective validation is needed
- Independently source references: peer network (colleagues at comparable organizations who have implemented the system), analyst community (Gartner research can provide reference names), LinkedIn (identify implementation project leads at vendor clients and reach out directly)
- The independent references provide the unfiltered view; the vendor references provide the detailed technical validation

**Reference conversation design:**
- Open: "What was the original business case for the implementation, and to what degree was it achieved?"
- Technical: "What were the most significant integration challenges, and how were they resolved?"
- Implementation: "What would you do differently if you were doing the implementation again?"
- Vendor: "How did the vendor perform against their implementation commitments — timeline, scope, quality? Were there moments where you felt the vendor overpromised?"
- Final: "If you were selecting today, knowing what you know now, would you select this vendor again? Is there another vendor you would consider?"

**Deliverable:** Scored evaluation matrix with rationale; reference check summary; recommendation with clear decision logic.

### Phase 5: Commercial Negotiation (4–8 weeks)

**Objective:** Secure the best available commercial terms from the preferred vendor.

**Negotiation principles:**

**Maintain optionality through at least the start of negotiation.** Tell the preferred vendor you are in the final stage but have not yet made a selection decision. A vendor who believes they have the deal has no incentive to provide their best commercial terms. The moment you tell a vendor they have been selected, your negotiating leverage disappears.

**Negotiate all dimensions simultaneously, not sequentially.** License fee, implementation fee, support terms, SLA commitments, termination rights, data portability, price escalation caps — all should be on the table simultaneously. Vendors are sophisticated negotiators who prefer to negotiate sequentially (close on one dimension before opening the next); sequential negotiation removes the ability to trade across dimensions.

**The price components that most clients underweight:**
- Annual price escalation caps (enterprise software contracts with CPI-plus escalation can compound significantly over a 10-year contract period)
- Termination for convenience rights (the right to exit the contract without cause, and the cost of doing so — often a more significant economic exposure than the annual license fee)
- Data portability rights (what does the vendor do with the client's data if the relationship ends? In what format, at what cost, on what timeline?)
- Service credit mechanisms for SLA breaches (how much of the annual fee is genuinely at risk if the vendor fails to meet SLAs?)

**The best-and-final-offer move:** After initial negotiation rounds, request a best-and-final-offer from the finalists. This reveals where the vendor's true limits are without requiring the client to drive the negotiation themselves through multiple rounds.

---

## The Build vs. Buy Decision

Before committing to any vendor selection process, test whether the technology should be built internally rather than purchased from a vendor. The build vs. buy decision is not always obvious, and the bias in most organizations is toward buy (because building is organizationally visible and politically risky) when build may be the superior strategic choice.

**Build may be preferable when:**
- The capability enabled by the technology is a core differentiator and is not well-served by any existing vendor solution
- The organization has genuine software engineering capability that can build and maintain the solution
- The total cost of ownership of building is materially lower than buying (common when vendor pricing is high and the scope is narrow)
- The vendor market is immature and available solutions require so much customization that the vendor solution provides limited value over a clean build

**Buy is almost always preferable when:**
- The capability is a commodity (financial reporting, HR administration, standard CRM) where vendor solutions are mature and well-established
- The organization lacks software engineering capability
- The functionality required is a standard implementation of a well-understood process
- The time to implement is constrained — build timelines are nearly always longer than buy timelines

**The common build underestimation:** The cost of building software is routinely underestimated; the cost of maintaining it (which continues indefinitely) is almost always dramatically underestimated. A build option that looks cost-competitive in Year 1 often looks inferior in Year 5 when the total cost of ownership — including maintenance, security patching, and feature development — is accumulated.

---

## Common Failure Modes

**The requirements written for a specific vendor.** The requirements are so aligned with a specific vendor's product that the selection process is pre-determined. This typically results from the client having an existing relationship with a vendor and structuring the requirements to justify the relationship. The outcome is a selection process that looks rigorous but is actually political. Prevention: requirements must be reviewed by an independent party before the RFP is issued.

**The feature checklist selection.** The evaluation scores vendors on the number of features they claim to have, rather than on their ability to perform the business capabilities the client actually needs. A vendor that claims 180 of 200 features may perform poorly on the 10 features that are strategically critical. Prevention: design the evaluation around scenario-based demonstration of critical capabilities, not feature checklists.

**The integration underestimation.** The vendor selection process evaluates the core system thoroughly but does not evaluate integration capability with the client's existing system landscape. Integration is consistently the most difficult and most expensive part of enterprise technology implementation. A system that performs beautifully in isolation may perform poorly in the client's actual environment. Prevention: make integration scenarios a mandatory part of the demo; require vendors to describe the integration architecture for the client's specific system landscape.

**The reference shortcut.** The reference check is conducted exclusively with vendor-provided references in a 30-minute courtesy call. The reference provides uniformly positive feedback. The client concludes that references are positive and moves forward. The independently sourced references that would have revealed material implementation challenges are never obtained. Prevention: require independent reference checks for any vendor under serious consideration.

**The legal review deferral.** The vendor is selected, a Letter of Intent is signed, and legal review of the contract begins only after the commercial negotiation is effectively complete. The legal review then reveals contractual terms (data portability, termination rights, liability caps) that are commercially significant — but the client has insufficient leverage to renegotiate because the selection is already made. Prevention: legal review must occur in parallel with commercial negotiation, not after it.
