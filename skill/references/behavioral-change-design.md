# Behavioral Change Design: COM-B, EAST, and Nudge Architecture

This file covers the behavioral science layer of transformation and change management. It is distinct from the ADKAR and Kotter content in `references/change-management.md` (which covers the organizational sequence and individual readiness model) and the resistance mapping aspects of `references/stakeholder-mapping.md`. Where ADKAR tells you what stage a person is stuck at, behavioral science tells you *why* they remain stuck there and *what specific intervention design* will move them.

Behavioral change design is increasingly used by BCG's Center for Behavioral Science, McKinsey's Organizational Change practice, and EY's People Advisory Services as a complement to — and in some cases a replacement for — conventional change management playbooks.

---

## Why Conventional Change Management Falls Short

The dominant change management frameworks (ADKAR, Kotter, Lewin) were designed to manage planned, top-down organizational transitions. They assume that if people understand the change (Awareness), want the change (Desire), know how to change (Knowledge), can change (Ability), and are reinforced (Reinforcement), the change will stick.

The assumption that is consistently wrong: that understanding and desire are sufficient to produce behavior change. Decades of behavioral economics research — beginning with Kahneman and Tversky's work on cognitive bias and extending through Thaler and Sunstein's nudge theory — demonstrate that people reliably fail to behave in accordance with their stated intentions. This is not irrationality in the pejorative sense; it is a predictable feature of how human decision-making actually works.

**The intention-behavior gap in organizational settings:**

- Employees who genuinely endorse the change in survey responses and still revert to old processes when under pressure
- Managers who intellectually agree with new performance management expectations and still conduct reviews the same way they always have
- Leaders who publicly champion a digital transformation and privately route decisions through the channels that existed before the transformation
- Teams that complete training on new systems and then call the helpdesk to have someone complete the task for them in the old system

The behavioral science toolkit addresses these gaps with intervention designs that work with — rather than against — how people actually decide and act.

---

## The COM-B Model: Diagnosing Why Behavior Isn't Happening

COM-B (Capability, Opportunity, Motivation — Behaviour) is a behavioral diagnostic framework developed by Susan Michie and colleagues at University College London. It is used by the UK's Behavioural Insights Team, WHO behavior change programs, and increasingly by management consulting practices designing transformation interventions.

The model holds that any behavior occurs when three conditions are sufficiently present:

### Capability

The individual's psychological and physical capacity to perform the behavior.

**Psychological capability:** Knowledge, cognitive skills, self-regulation ability.
- Does the person know what the new behavior looks like in practice?
- Can they perform it under typical working conditions (stress, time pressure, ambiguity)?
- Do they have the cognitive habit (automaticity) of the old behavior working against them?

**Physical capability:** The physical or motor skills required.
- In operational or manufacturing contexts, does the new behavior require physical actions the person has not yet practiced?
- Are there ergonomic or environmental barriers (e.g., new equipment layout that makes the old habit physically easier)?

**Common consulting application:** Most training programs address psychological capability — they build knowledge of the new behavior. They systematically under-address the automaticity problem: years of cognitive habit make the old behavior effortless and the new behavior effortful. Effective interventions must reduce the cognitive cost of the new behavior, not just increase the person's knowledge of it.

### Opportunity

The external conditions that permit or prompt the behavior.

**Physical opportunity:** The environment makes the behavior possible.
- Are the tools, systems, and processes configured to support the new behavior?
- Does the physical or digital environment make the old behavior easier than the new one?

**Social opportunity:** Norms, cues, and social context that prompt or enable the behavior.
- What do the informal leaders in this person's team or peer group actually do? (If informal leaders are not modeling the new behavior, social opportunity for behavior change is low regardless of formal messaging.)
- What does the organizational culture reward and punish at the informal level?

**Common consulting application:** Opportunity failures are the most structurally solvable category but the most frequently overlooked. If a new procurement process requires three additional approval steps in a system that is slower and less intuitive than email — which was the old process — the physical opportunity to adopt the new behavior is deliberately worse than the old one. No amount of communication or training will fix an opportunity barrier; only environmental redesign will.

### Motivation

The brain processes that energize and direct behavior.

**Reflective motivation:** Explicit beliefs, goals, and intentions. This is the level conventional change management primarily addresses — building the rationale for change, the vision, the case for why the new behavior is better.

**Automatic motivation:** Habits, emotions, and implicit associations. This is the level that actually drives most behavior in the context of established routines and under conditions of stress or cognitive load.

**Common consulting application:** Transformation programs almost exclusively target reflective motivation (building understanding and intent) while ignoring automatic motivation (the habits, emotional associations, and reflexive responses that govern behavior when people are not actively deliberating). Effective behavioral change design operates at both levels.

### The COM-B Diagnostic Process

Before designing any behavior change intervention, apply the diagnostic:

**Step 1:** Define the specific target behavior with precision. Not "adopt the new culture" or "use the new system." Specific: "Complete the weekly progress report in the new project management platform rather than emailing a summary to the manager."

**Step 2:** For that specific behavior, assess each COM-B component:
- Is capability present? (Does the person know how? Can they do it under normal working conditions?)
- Is opportunity present? (Does the environment permit it? Does the social context cue it?)
- Is motivation present? (Do they intend to? Does it feel natural or does it require deliberate override of an established habit?)

**Step 3:** Identify the binding constraint. What is the single most limiting factor? Design your intervention to address that factor first. Addressing motivation when the binding constraint is opportunity is waste.

**Intervention-to-component mapping:**

| COM-B Component | Intervention Type | Examples |
|----------------|------------------|----------|
| Psychological capability | Education, training, job aids, cognitive tools | Micro-learning, checklists, decision support tools |
| Physical capability | Practice, simulation, graduated exposure | Supervised practice sessions, role-play exercises |
| Physical opportunity | Environmental redesign | Default settings, system simplification, layout changes |
| Social opportunity | Norm change, peer influence, modeling | Peer champions, visible senior leader behavior, social proof |
| Reflective motivation | Persuasion, goal-setting, incentives | Communication, OKRs, performance management |
| Automatic motivation | Habit disruption, implementation intentions | Cue-routine-reward redesign, "if-then" planning |

---

## The EAST Framework: Intervention Design Principles

EAST (Easy, Attractive, Social, Timely) is the applied behavioral design framework developed by the UK Behavioural Insights Team (BIT, or "the Nudge Unit"). It translates behavioral science into actionable design principles for intervention creation. Where COM-B is a diagnostic tool, EAST is a design tool.

### Make It Easy

The most powerful behavioral intervention is reducing friction. Every additional step, cognitive load, or decision point between intention and behavior reduces execution probability.

**Default design:** Set the desired behavior as the default. People overwhelmingly accept defaults even when they are aware they can change them. In organizational settings: default the new system rather than requiring opt-in; default meeting templates in the new format; auto-populate required fields that people regularly skip.

**Reduce steps:** Count the number of actions required to perform the new behavior. For every action that is not strictly necessary, eliminate it. If the old process required two steps and the new process requires five, adoption will lag regardless of the quality of communication.

**Simplify language:** Instructions, policies, and guidelines that are jargon-heavy or require cross-referencing other documents increase cognitive load and reduce compliance. Rewrite to the minimum necessary complexity.

**Harness pre-commitment:** If you can get people to commit to the new behavior in advance — in writing, in a specific context, in front of colleagues — follow-through rates increase significantly. Implementation intention contracts ("I will do X at time Y in situation Z") are particularly effective.

### Make It Attractive

Behavior is more likely when it is associated with positive feelings, salient rewards, or engaging presentation.

**Salience:** Make the new behavior and its benefits visible. When people are not actively thinking about a behavior, they default to habit. Making the right behavior visually prominent in the environment (signage, screen prompts, physical cues) increases salience and changes behavior without requiring conscious deliberation.

**Personalization:** People respond more to messages and incentives that feel relevant to their specific situation. A blanket communication about the importance of data security is less effective than a message tailored to a specific team's actual data handling context.

**Incentive design:** When incentives are used, design them behaviorally:
- Immediate rewards outperform delayed rewards at the same expected value (temporal discounting)
- Loss-framed incentives ("you will lose this benefit if you do not complete by X") outperform gain-framed incentives of equivalent size for many behavior categories
- Non-financial recognition (public acknowledgment, peer recognition) drives behavior in ways that financial incentives do not — particularly for professionals whose identity is connected to expertise and competence

### Make It Social

Humans are profoundly social animals. Behavior is strongly shaped by what we believe others in our reference group are doing and what they approve of.

**Social norms:** People overestimate the prevalence of non-compliant behavior and underestimate the prevalence of compliant behavior. Correcting this perception — "85% of your colleagues in this region have already completed the updated compliance training" — drives behavior without requiring any structural change.

**Peer influence:** Identify the informal opinion leaders in each affected team or unit. These are not necessarily the most senior people; they are the people whose judgment colleagues trust most. Convert these informal leaders first. Their behavior signals to others what the new norm actually is.

**Commitment in social contexts:** Public commitments are more binding than private ones. If you can get individuals to state their intention to adopt a behavior in front of colleagues — in a team meeting, in a shared tracker — follow-through rates increase.

**Social proof:** Visible evidence that others are doing the new thing. Leaderboards, progress counters, peer stories. These work particularly well in the early adoption phase, before the new behavior has become the established norm.

### Make It Timely

The impact of a behavioral intervention is highly sensitive to when it is delivered relative to the moment of decision.

**Point-of-decision prompts:** The most effective time to influence behavior is at the moment the relevant decision is being made, not weeks before. Sending a training on the new expense reporting process in January has much less impact than presenting a brief reminder when the employee opens the expense tool in March.

**Critical moments:** Identify the specific moments in the workflow where the old behavior is triggered and the new behavior should replace it. Design interventions to activate at those moments. For example: if the old behavior is triggered when an employee receives a request by email, a point-of-decision prompt in email (not a training in a classroom) is the highest-impact intervention.

**Fresh starts:** Behavior change is easier at natural transition points — the beginning of a new role, a new quarter, a new project, return from leave. The "fresh start effect" means people are more open to establishing new habits at these junctures. Design the rollout of new behaviors to coincide with organizational transition points whenever possible.

**Temporal scarcity:** Time-limited windows ("complete this by Friday to be included in the first cohort") increase action rates by making the cost of inaction salient and immediate.

---

## Habit Architecture: Designing for Automaticity

The ADKAR Reinforcement stage addresses the need to sustain new behaviors over time but does not specify *how* reinforcement works mechanically. Behavioral science provides the mechanism: habit formation.

### The Habit Loop (Cue → Routine → Reward)

All habits, including organizational behaviors, operate on a three-part loop:

**Cue:** A trigger that initiates the behavior — a time of day, a location, a preceding action, an emotional state, or a social context.

**Routine:** The behavior itself — the action that follows the cue.

**Reward:** The positive signal that reinforces the loop — a feeling of completion, a social acknowledgment, a tangible outcome, reduced cognitive load.

Old behaviors have established loops with strong cues, well-practiced routines, and familiar rewards. New behaviors start with weak cues, effortful routines, and unfamiliar or delayed rewards. This is why new behaviors require deliberate effort for weeks or months before they begin to feel automatic.

### Designing New Habit Loops

**Identify the existing cue.** What currently triggers the old behavior? (Example: "When I receive a contract approval request, I forward it to my manager by email.") The cue — receiving a contract request — is not going away. The question is whether the routine following that cue can be changed to the new behavior.

**Attach the new routine to the existing cue.** Design the transition so that the same cue triggers the new routine. In the example: configure the contract management system to automatically generate a task when a contract request is received, replacing the email trigger.

**Deliver an immediate reward for the new routine.** The reward does not need to be large; it needs to be immediate and consistent. Progress bars, completion notifications, manager acknowledgment within 24 hours, or simply a reduced number of steps in the workflow (the new routine is easier than the old one) all serve as rewards.

**Plan for cue disruption.** During the transition period, old cues will still prompt old routines — particularly under stress or cognitive load. This is not resistance; it is the normal operation of habit. Design cue disruption: physical or digital changes to the environment that interrupt the old cue-routine connection and redirect to the new one.

### Implementation Intentions

An implementation intention is a specific plan of the form "When [situation X] occurs, I will do [behavior Y] in [place Z]."

Research by Peter Gollwitzer and colleagues across dozens of studies consistently finds that forming implementation intentions increases follow-through on intentions by 20–50% compared to goal-setting alone. The mechanism: the if-then structure creates a mental link between the situational cue and the behavior, automating the response without requiring deliberation.

In consulting implementation, build implementation intention design into training and onboarding:

- At the end of any training session, ask participants to complete: "The next time [specific trigger] occurs, I will [specific new behavior]."
- Have them write this down and share it with a colleague.
- Build a follow-up prompt for 7 days later: "Last week you committed to [behavior] — here's how to check in on your progress."

---

## Measuring Behavioral Change: Beyond Survey Scores

The standard measure of change adoption is the survey ("On a scale of 1–5, how confident are you in using the new system?"). Survey scores are a leading indicator at best; they measure stated intention, not behavior. The intention-behavior gap means that high survey scores are compatible with low actual adoption.

**Behavioral metrics to design into every change program:**

| Behavior Category | Measurable Behavioral Indicator |
|------------------|--------------------------------|
| System adoption | Login frequency, feature usage rates, transaction volume in new vs. old system |
| Process compliance | Completion rates for required steps; error rates; exception volumes |
| Capability development | Task completion without helpdesk escalation; quality of outputs in new format |
| Cultural behaviors | Frequency of target behaviors in observed settings (e.g., meeting recordings, manager observations) |
| Social norm shift | Peer reporting of observed behaviors; informal leader modeling rates |

**The baseline-and-track discipline:** Before rollout, establish behavioral baselines for each metric. Measure weekly for the first 90 days. Behavioral change does not happen linearly — it often shows early gains as novelty motivates action, a dip at 30–60 days as novelty fades and habit has not yet formed, and a recovery as the new behavior becomes easier. Design interventions for the dip period specifically.

---

## Integration with ADKAR: Using Both Frameworks Together

ADKAR diagnoses the stage of individual change. COM-B explains the mechanism of why someone is stuck at that stage. EAST provides the design toolkit for the intervention.

| ADKAR Stage | COM-B Lens | EAST Intervention |
|-------------|-----------|------------------|
| **A**wareness gap | Reflective motivation absent | Make it Attractive (salient, personalized messaging) and Timely (point of decision) |
| **D**esire gap | Reflective or automatic motivation absent | Make it Social (peer norms, public commitment) and Attractive (align with identity and values) |
| **K**nowledge gap | Psychological capability absent | Make it Easy (simplified job aids, decision support) and Timely (point-of-need, not classroom) |
| **A**bility gap | Physical capability or physical opportunity absent | Make it Easy (environmental design, reduce steps) and social (supervised practice with peers) |
| **R**einforcement gap | Automatic motivation absent; habit not formed | Habit loop redesign (cue-routine-reward); implementation intentions; behavioral tracking |

When ADKAR says a person is stuck at "Desire," COM-B tells you whether the desire gap is motivational (they don't want to) or opportunistic (they want to but social norms around them make it too costly). EAST then tells you whether to design a social proof intervention, a peer norm communication, or a commitment device.

---

## Common Failure Modes in Behavioral Change Design

**The information fallacy.** Assuming that giving people information about why the change matters will change behavior. Information changes beliefs; it rarely changes behavior directly. The intention-behavior gap is well-documented. Design for behavior, not just for understanding.

**The training substitution.** Running a training program as the primary behavior change intervention. Training changes knowledge; it does not change habit or opportunity structure. Training is effective only when capability (knowledge) is the binding constraint. Audit your COM-B diagnosis before defaulting to training.

**Addressing motivation when opportunity is the constraint.** The most common mismatch: spending budget on communication campaigns when the actual barrier is that the new system is harder to use than the old one. Fix the system before running the campaign.

**Designing for the average user.** Different people are stuck at different COM-B components. A one-size-fits-all intervention is inefficient and often counterproductive. Segment your population by COM-B profile and design differentiated interventions.

**Measuring adoption too early.** Behavioral change takes 30–90 days to manifest in measurable habit formation. Measuring adoption at week two and declaring failure or success is premature. Design a 90-day measurement window as standard.

**Ignoring informal norms.** Formal communications say the new behavior is expected. Informal norms among peers signal that the old behavior is still acceptable, or even preferable. Formal interventions that do not address informal norms will produce visible compliance and invisible non-compliance. Measure actual behavior, not stated intention.
