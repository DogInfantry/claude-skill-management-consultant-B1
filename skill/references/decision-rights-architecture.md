# Decision Rights Architecture: RAPID, DARE, and DACI

This file covers the practitioner methodology for designing, assigning, and hardwiring decision rights in organizations undergoing transformation, restructuring, or governance redesign. It goes beyond the structural org design in `references/org-design-workforce.md` (which covers spans, layers, and reporting lines) to address the specific discipline of *who decides what* — the mechanism by which accountability is operationalized.

This file pairs with `references/org-design-workforce.md` (structure), `references/engagement-management.md` (scoping), and `references/board-communication-and-decision-support.md` (board-level governance). It complements `references/post-merger-integration.md` for IMO-level decision governance in M&A.

---

## Why RACI Fails for Decision-Making

RACI (Responsible, Accountable, Consulted, Informed) is a task assignment tool. It was designed for project management, not for recurring organizational decisions. When applied to decisions, it generates two systemic failure modes:

**Failure Mode 1: Diffused accountability.** When two people are listed as "A" (Accountable), neither is. The letter exists; the accountability does not. In practice, both parties defer to each other in conflict and each acts unilaterally when convenient.

**Failure Mode 2: Veto proliferation.** "C" (Consulted) roles in RACI are frequently interpreted as "must-agree" roles rather than "input-provider" roles. This is rarely articulated or corrected. The result: a seven-person consulted list creates seven informal veto points that the RACI never intended to grant. Cycle times triple. The original Decider is paralyzed.

**The diagnostic test:** Count how many people in the organization have experienced "I gave input that was ignored" (under-consultation) or "I was asked to approve something I had no authority to block" (over-consultation). Both signal a broken RACI.

What is needed instead: a decision rights framework that separates inputs from vetoes, identifies a single accountable Decider for each consequential choice, and is explicit about what happens when the Decider is stuck.

---

## The Three Frameworks: When to Use Each

### RAPID (Bain & Company)

RAPID was developed by Bain to fix the accountability gaps in RACI when applied to organizational decisions. It defines five roles:

| Role | Label | What It Means |
|------|-------|---------------|
| **R**ecommend | Recommender | Leads the analysis; proposes the decision with supporting rationale |
| **A**gree | Agreers | Must concur before the decision is finalized; true veto holders |
| **P**erform | Performers | Execute once the decision is made; may provide input but hold no approval right |
| **I**nput | Input providers | Consulted for their expertise or perspective; no blocking power |
| **D**ecide | Decider | Single accountable owner who makes the final call |

**Design rules:**
- Exactly one D per decision. Shared D = no D.
- A roles should be rare and deliberate. Every A is a potential veto; treat them as expensive.
- I roles are unlimited, but do not confuse them with A roles.
- R is the person doing the work to get to a recommendation — typically a team lead or senior analyst, not the executive.
- P roles are often overlooked in design; executors who were not involved often undermine decisions they do not understand.

**Best for:** Strategy decisions, resource allocation, capital investment, governance escalations. Any decision where there is a genuine compliance, legal, or financial need for structured sign-off before the Decider acts.

---

### DARE (McKinsey & Company)

McKinsey's alternative to RACI, published as a reform for organizations where RACI had calcified into bureaucracy. DARE simplifies and sharpens:

| Role | Label | What It Means |
|------|-------|---------------|
| **D**eciders | Deciders | The person (singular) who makes the decision and is accountable for the outcome |
| **A**dvisors | Advisors | Provide input; their perspective should be sought and weighted, but they hold no veto |
| **R**ecommenders | Recommenders | The team or person who frames the analysis and presents the recommendation |
| **E**xecution | Executors | Implement the decision; understanding the rationale improves execution quality |

**The critical distinction from RACI:** In DARE, there are no formal Consulted roles with implied veto rights. Advisors advise. Their disagreement is noted and considered by the Decider — but the Decider decides. This is a cultural shift as much as a structural one.

**Best for:** Organizations where RACI has created consensus paralysis; transformation programs where decision speed is a strategic imperative; newly restructured organizations where former peers now have subordinated input roles and need a framework that makes that explicit without requiring a political battle each time.

---

### DACI (Driver, Approver, Contributors, Informed)

DACI is widely used in technology and product organizations and is increasingly adopted in consulting for program-level decisions:

| Role | Label | What It Means |
|------|-------|---------------|
| **D**river | Driver | Responsible for moving the decision forward; owns the process, not just the recommendation |
| **A**pprover | Approver | Single person with final sign-off authority (equivalent to D in RAPID) |
| **C**ontributors | Contributors | Provide expertise; consulted but not approvers |
| **I**nformed | Informed | Notified of the decision after it is made |

**Key distinction from RAPID:** The Driver role explicitly owns the *process* of reaching a decision — scheduling, structuring the debate, managing timelines, facilitating stakeholder input — not just the analysis. In complex organizations, this separation is valuable when the Approver is too senior to manage the process and the Recommender is too junior to own accountability for decision quality.

**Best for:** Product development decisions, technology architecture choices, program-level prioritization in transformation. Strong fit for organizations with clear senior-level Approvers who need a dedicated Driver to operationalize the path to decision.

---

## Selecting the Right Framework

| Situation | Recommended Framework | Rationale |
|-----------|----------------------|-----------|
| Large enterprise with formal governance | RAPID | Explicit A roles suit compliance-heavy environments |
| Transformation with speed as KPI | DARE | Eliminates informal veto culture; forces single Decider |
| Tech / product organization | DACI | Driver role fits product operating model |
| Post-merger integration governance | RAPID | Need clear sign-off rights across two legacy cultures |
| Early-stage org building governance from scratch | DARE | Simpler; fewer legacy role expectations to manage |
| Regulatory-intensive industry | RAPID | A roles (legal, compliance, finance) are genuinely necessary |

---

## Building a Decision Inventory

Before assigning any framework, you need to know what decisions actually exist. Most organizations have never catalogued this. The discovery process takes two to three weeks.

### Step 1: Decision Harvesting (Workshop Format, 2–3 Hours)

Run a structured workshop with 8–12 senior managers across the affected scope. Ask three questions:

**Question 1:** "What is the most important recurring decision your team makes every quarter?" Capture verbatim. Sort into functional clusters (hiring, resource allocation, pricing, capital spend, product roadmap, vendor selection, etc.).

**Question 2:** "What decision caused the most delay or conflict in the last six months?" This surfaces the broken decisions — the ones causing the most organizational friction. These become priority design targets.

**Question 3:** "Who do you typically have to convince, inform, or wait on before you can act on [Decision X]?" This maps the informal decision network and surfaces unacknowledged veto holders — people who are not in any formal approval chain but whose opposition effectively blocks action.

### Step 2: Decision Classification

Classify harvested decisions into four types:

| Type | Description | Frequency | Framework Fit |
|------|-------------|-----------|---------------|
| **Strategic** | Resource allocation, M&A, major investment, market entry | Annual / event-driven | RAPID (with A roles for board/legal/finance) |
| **Operational** | Pricing exceptions, hiring approvals, vendor selection | Weekly / monthly | DARE (lean, fast) |
| **Exception** | Edge cases that fall outside existing policy | Ad-hoc | DACI (Driver owns resolution process) |
| **Policy-setting** | Establishing rules that govern operational decisions | Annual | RAPID (high-stakes, multi-stakeholder) |

### Step 3: Prioritize by Impact

Not all decisions need redesigning. Focus on the high-pain, high-frequency, high-consequence intersection:

- **High pain:** Decisions that regularly cause conflict, delay, or rework
- **High frequency:** Decisions made often enough that structural inefficiency compounds over time
- **High consequence:** Decisions where a wrong outcome is costly financially, strategically, or reputationally

A decision that is low-frequency and low-consequence does not need a formal rights framework. Default delegation to the most relevant senior manager is sufficient.

---

## Designing the Decision Rights Matrix

Once you have classified decisions and selected a framework, build the matrix.

### RAPID Matrix — Example Format

| Decision | Recommend | Agree | Perform | Input | Decide |
|----------|-----------|-------|---------|-------|--------|
| Annual budget allocation | FP&A Director | CFO, General Counsel | Finance team, BU leads | BU heads, HR | CEO |
| New vendor contract >$500K | Procurement Lead | CFO, Legal | Procurement team | Operations head | CPO |
| Price exception >15% off list | Sales Director | Finance | Sales rep | Pricing team | CRO |
| VP-level hire | CHRO | CEO | HR, Hiring manager | Peer VPs | CEO |
| Strategic partnership | BD Lead | Legal, Finance | BD team | Product, Sales | CEO or delegated SVP |
| Capex >$1M | Finance | CFO, Board Audit Committee | Finance, Operations | Engineering | CEO |

**Operational rules to embed in the matrix:**
- Dollar thresholds on financial decisions (below threshold = local Decider; above = escalate to named senior role)
- Response time limits on Agree roles (A roles must respond within X business days or waive their veto by default)
- Clear specification of what "Agree" means: unconditional veto, or veto only on specific compliance/legal grounds?
- Sunset clauses on any temporary elevated authority (e.g., IMO Director override rights expire at Day 120)

### The Escalation Path — Mandatory Component

Every decision rights design must specify what happens when the Decider is stuck. Without a designed escalation path, stuck decisions default to either the highest HiPPO in the room (Highest Paid Person's Opinion, regardless of role) or to inaction. Both are costly.

**Escalation path template:**
```
Decision X → Decider cannot resolve within [X days]
  → Escalate to [Named Role] within [Y business days]
    → If still unresolved after [Z days] → [Named Senior Executive] 
      makes final, non-appealable call
        → Log the decision and the escalation path taken
```

Build this explicitly into the matrix for each decision type. A rights matrix without escalation paths is not complete.

---

## Diagnostic: Reading Broken Decision Patterns

When a client presents organizational friction, these patterns diagnose the underlying decision rights failure:

| Symptom | Probable Root Cause | Rights Diagnosis |
|---------|-------------------|-----------------|
| "Decisions take too long" | Too many Agree/veto holders | Reduce A roles; shift to DARE |
| "We revisit the same decisions repeatedly" | No single D; decisions are discussed, not made | Enforce single Decider rule; log decisions formally |
| "The wrong people are deciding" | Authority misaligned with accountability | Map formal rights vs. actual decision behavior; redesign |
| "I was overruled after giving input" | I roles confused with A roles | Communicate Input vs. Agree distinction explicitly |
| "The CEO is in every decision" | No delegation design; all decisions escalate to top | Build delegation thresholds by decision type and value |
| "We agreed in the room but nothing changed" | Group decision = no individual accountability | Require named individual D on every consequential choice |
| "Decisions made in a silo have cross-functional consequences" | P (Performers) not consulted until execution | Involve P roles at Input stage, not just execution stage |
| "The consultant left and the process reverted" | Rights matrix not operationalized; lived only in a deck | Embed in meeting templates, decision memos, and quarterly reviews |

---

## Implementation: Making the Design Stick

Decision rights are not self-enforcing. A well-designed matrix that exists only in a PowerPoint deck changes nothing.

### Phase 1: Design (Weeks 1–3)
- Run Decision Harvesting workshop
- Build decision inventory; prioritize high-pain, high-frequency decisions
- Propose framework assignments by decision type
- Draft the rights matrix; circulate for calibration with affected stakeholders

### Phase 2: Calibration (Weeks 3–5)
- Walk each senior stakeholder individually through the decisions where their role changes
- Specifically: identify stakeholders who currently hold informal veto rights that the new design removes — these are primary resistance sources and require separate management
- Test the design against 3–5 real recent decisions: "If this matrix had existed when we made [Decision X], what would have happened differently?" Reveals gaps and over-constraints in the design

### Phase 3: Operationalization (Weeks 5–8)
- Publish the matrix in an accessible, living format (not locked in a consulting deliverable)
- Train decision owners on the framework — particularly the distinction between Input and Agree
- Build the rights framework into standing meeting templates: every major decision memo should specify D, A, R, I, P roles in the header
- Set a 90-day review date: after 90 days, audit which decisions used the matrix, which did not, and where it broke down

### Phase 4: Reinforcement (Ongoing)
Decision rights decay. When the Decider is uncertain, they consult broadly — and informal consensus norms re-emerge. Hardwire reinforcement:

- Include rights compliance in quarterly PMO or governance reviews
- When a decision process fails (wrong person decided, or nobody decided), run a brief retrospective: "Which role broke down, and why?"
- Celebrate decisions that were made faster than before — speed is a visible, positive signal that the design is working

---

## Decision Rights in Post-Merger Integration

PMI is the highest-stakes context for decision rights design. The specific failure mode: transformation governance layers (Steering Committee, IMO, Workstreams) create a new set of decision roles that sit alongside the existing business hierarchy without replacing it. The result is competing authority structures.

**PMI-specific design principles:**

**Separate transformation decisions from BAU decisions.** A VP of Operations makes operational decisions in their domain. The same VP makes integration decisions in the workstream they lead. These are different decision rights with different escalation paths. Write both sets explicitly and publish them separately.

**Define the Steering Committee's decision scope precisely.** Which decisions require Steering Committee approval (major scope changes, investment releases above threshold, critical personnel calls) versus which are delegated to the IMO Director or workstream leads? Without this definition, the Steering Committee becomes a bottleneck for decisions it should never see.

**Time-bound elevated IMO authority.** During the first 100 days, the IMO Director may hold unusual authority — for example, the ability to override BAU operational decisions to clear integration blockers. Define this authority explicitly and sunset it: "IMO Director override authority expires at Day 120 unless renewed by Steering Committee."

**Produce the Day 1 decision list pre-close.** Before any integration program launches, list the first 20 decisions that must be made within the first 30 days. Assign a named D for each. This prevents the most common early-stage failure: ambiguity about who can act when launch energy is highest but authority is least clear.

---

## Common Failure Modes

**The relabeling failure.** Teams rename their existing RACI columns as RAPID roles without redesigning the underlying accountability structure. All the old A roles are preserved as new A roles. The framework changes; the dysfunction doesn't. Test for this by counting A roles in the output — if there are more than two A roles on any single decision, the design is likely RACI with new labels.

**Political resistance to single-Decider rule.** Senior leaders who previously held shared decision authority resist being reclassified as Input providers. This is the single most common implementation failure. It must be managed as a stakeholder negotiation, not a design problem — the design is correct; the resistance is the variable to manage.

**The invisible escalation gap.** The Decider cannot decide, but no escalation path was designed. The decision stalls indefinitely. Always design the escalation before you need it.

**The framework-as-power-grab failure.** Decision rights are designed for organizational speed and accountability — not to protect any individual's status. When the framework is used to consolidate power, it fails politically and operationally. This is usually visible early: if a stakeholder is more focused on expanding their D roles than on designing a functional system, flag it.

**Decay without maintenance.** Org structure changes after the framework is designed. New roles are created, old ones are eliminated, reporting lines shift — but the decision rights matrix is not updated. After 12–18 months, the matrix becomes a historical document rather than an operational one. Build in a mandatory annual review with a named owner.

---

## Quick-Reference Design Checklist

Before finalizing any decision rights design, verify:

- [ ] Every consequential decision has exactly one named Decider
- [ ] Every Agree role is explicitly justified by a specific compliance, legal, or financial requirement
- [ ] Agree roles have response time limits (e.g., must respond within 3 business days or waive)
- [ ] Input roles have been clearly distinguished from Agree roles; this distinction has been communicated to all parties
- [ ] The escalation path is named for every decision category
- [ ] The matrix has been tested against 3–5 real recent decisions
- [ ] All stakeholders whose roles changed have been briefed individually, not just in a group session
- [ ] A 90-day operational review date is set with a named facilitator
- [ ] A mechanism exists for updating the matrix when org structure changes
- [ ] The matrix is published in an accessible, living format — not locked in a consulting deck
