# McKinsey-Style Problem Solving — Operational Methodology

This file provides the operational mechanics of structured problem solving as practiced at top-tier consulting firms — not the concept, but the *how*. Use it to run a real engagement, coach a team, or practice the discipline on a live problem.

This file works in close partnership with `references/frameworks.md` (which frameworks to use) and `references/issue-hypothesis-trees.md` (how to decompose a problem). This file covers the *process* that connects those tools into a coherent engagement sequence.

---

## The Core Operating Principle: Hypothesis-First, Not Boil-the-Ocean

The difference between a structured problem solver and a good analyst is one word: hypothesis.

An analyst asks: "What does the data show?"
A structured problem solver asks: "What do I think is true, and what would prove or disprove it?"

This shifts the entire work sequence:
- Hypothesis-first → build the minimum analysis that tests the hypothesis → update or confirm → recommend
- Data-first → analyze everything → try to synthesize → struggle to conclude

The hypothesis is not a guess you're attached to. It is a working bet that focuses your effort. You hold it loosely, update it with evidence, and replace it if the data contradicts it. What you never do is start without one.

---

## The Seven Steps — With Checklists and Artifacts

### Step 0: Read the Brief and Pattern-Match (15 minutes)

Before anything else — read the problem statement and ask: *have I seen this before?*

**Checklist:**
- [ ] What type of problem is this? (Profitability, growth, entry, M&A, operations, pricing, org)
- [ ] What industry? What are the known economics and benchmarks of this sector?
- [ ] Who is the client? (CEO, CFO, board, PE sponsor) — this changes what "a good answer" looks like
- [ ] What is the burning platform? Why is this urgent now?
- [ ] What is the likely shape of the answer? (Fix a cost problem / enter a market / decide on a deal / redesign a process)

**Artifact:** A 3-sentence archetype statement. Example: *"This is a profitability decline case in a B2B SaaS company. The burning platform is investor pressure on margins after a growth round. The answer will likely be in either cost structure or pricing — I'll start with pricing because SaaS businesses typically under-price."*

**Common trap:** Skipping this step and treating every problem as a blank slate. Pattern recognition is the fastest path to a useful Day 1 hypothesis.

---

### Step 1: Define the Problem Statement

A bad problem statement is the most expensive mistake in consulting. Solving the wrong problem perfectly is worse than solving the right problem imperfectly.

**Checklist:**
- [ ] Is the problem framed as a question, not a symptom? ("Why did margins fall?" not "Margins fell.")
- [ ] What is the decision the client actually needs to make? (Every good problem statement ends in a decision.)
- [ ] What are the constraints? (Timeline, budget, political dynamics, regulatory environment)
- [ ] What does success look like? (What metric, by when, at what confidence level?)
- [ ] Is there a hidden problem behind the stated problem? (Management often presents symptoms, not root causes.)

**The SCQA test:** Can you express the problem as Situation / Complication / Question? If the Question is vague, your problem statement isn't finished. See `references/pyramid-principle-and-scqa.md`.

**Artifact:** A written problem statement, one paragraph. Share it with the client sponsor and get explicit agreement before proceeding. Disagreement at this stage is far cheaper than at the end.

**Common traps:**
- Accepting the client's initial framing without pressure-testing it
- Problem statement that describes a symptom, not a decision
- Missing the political problem behind the analytical one (who actually owns the decision?)

---

### Step 2: Build the Issue Tree

An issue tree is a MECE decomposition of the problem into the sub-questions that, if answered, would answer the main question.

**Checklist:**
- [ ] Is the tree MECE? (Mutually exclusive: no overlap. Collectively exhaustive: no gaps.)
- [ ] Does each branch end in a testable question?
- [ ] Is the tree structured logically — either deductively (if all branches are true, the governing thought is true) or inductively (each branch is a component of the answer)?
- [ ] Have you formed an initial hypothesis for each branch? (Not just questions — bets.)

**The 80/20 test on the tree:** Underline the 1–2 branches that, if fully answered, would likely resolve 80% of the client's question. These are the priority workstreams. Everything else is context or backstop.

**Artifact:** Issue tree diagram (or outline). On a real engagement, this lives in the team room — physically visible. Review and update it every few days as you learn more.

**The emerging storyline rule:** Next to your issue tree, maintain a one-page "emerging storyline" that captures your current best answer to each branch and how those answers combine into a governing recommendation. This is the team's north star. It changes as you learn. It never goes away. *This discipline — keeping the emerging storyline visible — is what separates teams that synthesize well from teams that drown in data.*

**Common traps:**
- Building a framework-shaped tree instead of a problem-shaped tree (applying a template rather than reasoning from the problem)
- Too many branches (trying to cover everything instead of the critical path)
- Building the tree without forming hypotheses for each branch

---

### Step 3: Prioritize and Plan

You cannot do everything. The work plan is a prioritization decision, not a task list.

**Checklist:**
- [ ] Which analyses test the hypotheses on the critical branches?
- [ ] What is the minimum viable test for each hypothesis? (Don't design a 3-week analysis when a 3-day proxy will do.)
- [ ] What data do you need, and can you get it? (Never design analyses around data you might not be able to access.)
- [ ] Who owns what? (Each task has a name and a deadline — not "the team.")
- [ ] What are the checkpoints? (When will you see intermediate outputs and course-correct?)

**Artifact:** A one-page work plan. Rows are workstreams. Columns are weeks. Each cell shows the deliverable and owner. The workplan is reviewed at the start of every weekly team meeting and updated.

**Time-boxing principle:** Set the end date first, then work backwards to determine what can actually be done. Never let the analytical wish list drive the timeline. Prioritize analyses that can change the recommendation.

**Common traps:**
- Building a comprehensive plan rather than a prioritized one
- Assigning tasks to "the team" instead of a specific person
- Not building in midpoint synthesis — teams that don't synthesize until the end run out of time to course-correct

---

### Step 4: Analyze

This is where the work gets done. But analysis without discipline creates noise, not insight.

**Checklist (for each analysis):**
- [ ] What hypothesis does this analysis test? If you can't state the hypothesis, don't run the analysis.
- [ ] What would confirm the hypothesis? What would refute it?
- [ ] What is the "so what" if the analysis confirms? If it refutes? (Pre-think the implications before running the numbers.)
- [ ] Have you applied the triangulation principle? (At least two independent sources confirm a key finding before you rely on it.)
- [ ] Sanity check: does the output pass the smell test? If a number looks surprising, rework it before presenting.

**Analytical tools by hypothesis type:**
| Hypothesis Type | Go-To Analysis |
|---|---|
| "The problem is in costs" | Cost decomposition, benchmarking, should-cost model |
| "The problem is in pricing" | Price waterfall, competitive index, WTP research |
| "We're losing share" | Market share trend, win/loss analysis, customer cohort churn |
| "The fix is operational" | Process map, OEE/efficiency benchmarks, capacity analysis |
| "The market is attractive" | TAM/SAM, growth rate, profitability of incumbents, competitive dynamics |
| "This acquisition creates value" | Synergy model, premium vs. NPV of synergies, integration risk |

**Common traps:**
- Running analyses that don't test a hypothesis (fishing for insight instead of testing bets)
- Accepting the first data source (triangulation is not optional on critical findings)
- Presenting analysis without a "so what" (data without implication is not consulting work)

---

### Step 5: Synthesize

This is where most teams fail. They produce excellent analyses and terrible recommendations because they don't make the synthesis leap.

**The synthesis leap:** You've run 10 analyses. What do they collectively say? What is the one thing that is now true that was not obvious at the start? What should the client do?

**Checklist:**
- [ ] Have you identified the governing thought? (One sentence that captures the main recommendation)
- [ ] Do your 3–5 supporting reasons logically support that governing thought?
- [ ] Have you been ruthless about what *not* to include? (Interesting findings that don't change the recommendation belong in the appendix.)
- [ ] Does the recommendation pass the "would I stake my reputation on this?" test?
- [ ] Have you stress-tested the governing thought? (What assumption would break it? Is that assumption reasonable?)

**The emerging storyline review:** Compare today's emerging storyline to where you started. Has it changed? If it hasn't changed at all, you may not have learned anything — or you may have done only analyses that confirmed what you already believed. If it changed dramatically, understand why and make sure the new position is well-grounded.

**Synthesis technique — the 5-message drill:**
1. Write down every finding on a sticky note (or a list).
2. Group them by theme — what naturally clusters together?
3. For each cluster, ask: "What does this *mean* for the recommendation?"
4. Find the 3–5 clusters that matter most.
5. Write one message (a complete, assertive sentence) per cluster. Those are your key messages.

**Common traps:**
- Presenting findings rather than conclusions ("We found that revenue declined by 12%")
- Hedging the recommendation ("There are several options, each with merits...")
- Not passing the "so what" test on every message

---

### Step 6: Build the Storyline and Communicate

Recommendations without communication are academic exercises. The most brilliant analysis loses if it is not communicated compellingly.

**Checklist:**
- [ ] Does the communication open with SCQA? (See `references/pyramid-principle-and-scqa.md`)
- [ ] Is the governing thought in the first 30 seconds or the first slide?
- [ ] Does every slide title state the insight as a complete sentence?
- [ ] Are the supporting reasons MECE and sequenced logically?
- [ ] Is there a clear, specific ask? (What decision does the client need to make, and by when?)

**Pre-wiring the recommendation:** In consulting, you never want your recommendation to be a surprise at the final presentation. Pre-wire with key stakeholders beforehand. Walk the sponsor through your thinking before the full client presentation. Adjust based on their reactions — not to capitulate, but to sharpen the logic and address objections before they surface in the room.

**Artifact:** Ghost deck — an outline of the final document showing each slide title (as action titles) and the exhibit that will support it. Review the ghost deck with the team and sponsor before building the full deck. This is the most underused tool in consulting.

**Common traps:**
- Saving the recommendation for the last slide (see `references/pyramid-principle-and-scqa.md`)
- Topic slide titles instead of action titles
- No explicit decision request

---

### Step 7: Implement and Track

Recommendations without implementation plans are not complete work.

**Checklist:**
- [ ] What specifically needs to happen? (Actions, not aspirations)
- [ ] Who owns each action? (Named, not "the team")
- [ ] What are the milestones and timeline?
- [ ] What are the quick wins (first 30 days) vs. structural changes?
- [ ] How will you measure whether it's working? (KPIs and governance cadence)
- [ ] What are the top 3 risks and their mitigations?

**The 100-day plan:** For transformations and significant changes, build a 100-day plan that distinguishes: stabilize (days 1–30), build momentum (days 31–60), accelerate (days 61–100). See `references/implementation-practitioner.md` for the full playbook.

---

## The Team Room and Emerging Storyline Discipline

The "team room" practice — physically posting the issue tree and emerging storyline where the whole team can see and update them — is a discipline, not a ritual.

**Why it matters:**
- It forces everyone on the team to know where the project is, not just their workstream
- It creates a shared test: "Does my analysis move the storyline?" If not, why am I doing it?
- It enables rapid synthesis because the answer is always partly visible

**What to post:**
1. The problem statement (updated if the problem evolves)
2. The issue tree (updated as branches are resolved or new ones emerge)
3. The emerging storyline — your current best answer, in full sentences
4. The key open questions — what you don't yet know that would change the answer

**Cadence:** Formal team review of the storyline at least weekly. Informal updates daily as major analyses come in.

**For solo work or AI-assisted work:** Maintain a running document with the same four elements. Refer to it before every new analysis. Update it when you learn something that changes the answer.

---

## The McKinsey Problem-Solving Mindset — Key Principles

These are the operating principles that separate structured problem solving from smart analysis:

**1. The Day 1 Answer**
Before running any analysis, ask: *if you had to recommend something right now, what would it be?* This is your Day 1 Answer. It is probably wrong, but it focuses the work. Every analysis either confirms or updates the Day 1 Answer. If an analysis doesn't do either, it is probably not the right analysis.

**2. 70% Conviction Rule**
When you have 70% of the information and conviction, decide. Waiting for 100% means you are always too late. This applies to forming hypotheses, making workplan decisions, and making recommendations. Build in checkpoints to update rather than deferring the decision.

**3. The Single Best Question**
If you could ask one question that would most change your recommendation, what would it be? This is the priority analysis. Do it first.

**4. Disaggregation Before Action**
Never recommend action on an aggregate number. Revenue is down — which segment? Costs are up — which cost type? Margins are low — at which level of the P&L? Always go one level deeper before committing to a diagnosis.

**5. The Pre-Mortem**
Before finalizing any recommendation, run a pre-mortem: *Assume this recommendation is implemented and fails 18 months from now. Why did it fail?* This surfaces the most likely failure modes and often reveals the critical assumption that needs testing before the recommendation is locked.

**6. Intellectual Honesty About Uncertainty**
Separate what you know (high confidence, corroborated), what you believe (working hypothesis, less corroborated), and what you don't know (genuinely uncertain). Never present uncertain assumptions as facts. State your confidence level explicitly. Senior stakeholders respect honesty about uncertainty far more than false precision.
