# Installation Guide — MBB Management Consultant Skill for Claude

This guide walks you through installing the management consultant skill on Claude. Three methods depending on which Claude product you're using.

---

## Method 0: Claude Code Plugin — Fastest (One Command)

If you use [Claude Code](https://claude.ai/code), install the whole skill as a plugin — no downloads, no file copying:

```
/plugin marketplace add DogInfantry/claude-skill-management-consultant-B1
/plugin install management-consultant-B1
```

That's it. To pick up future updates, run `/plugin marketplace update`.

---

## Method 1: Claude Cowork (Desktop App) — Recommended

[Claude Cowork](https://claude.ai) is Anthropic's desktop tool for file and task management. It supports skills natively.

### Step 1: Download the Skill Files

Download this entire repository as a ZIP file:
- Click the green **Code** button at the top of this GitHub page
- Select **Download ZIP**
- Unzip it to a folder on your computer (e.g., `~/claude-skills/management-consultant/`)

### Step 2: Locate Your Claude Skills Folder

In Cowork, skills live in a `.claude/skills/` folder inside your workspace. To find or create it:

1. Open Claude Cowork on your desktop
2. Click **Settings → Workspace**
3. Note your workspace folder path (e.g., `~/Documents/Claude Workspace`)
4. In Finder/Explorer, navigate to that folder
5. Create a folder path: `.claude/skills/management-consultant/`

> **Note**: The `.claude` folder is hidden by default on Mac. Press `Cmd + Shift + .` in Finder to show hidden files.

### Step 3: Copy the Skill Files

Copy the contents of the downloaded `skill/` folder into your `.claude/skills/management-consultant/` folder:

```
Your Workspace/
└── .claude/
    └── skills/
        └── management-consultant/
            ├── SKILL.md          ← The main skill file
            └── references/       ← All 80+ reference files
                ├── frameworks.md
                ├── case-interview.md
                └── ...
```

### Step 4: Restart Claude Cowork

Close and reopen Claude Cowork. The skill will be automatically detected.

### Step 5: Test It

Start a new conversation and type:
```
Help me structure a profitability analysis using consulting frameworks.
```

Claude should respond as a senior MBB consultant.

---

## Method 2: Claude Code (CLI) — For Developers

[Claude Code](https://claude.ai/code) is Anthropic's command-line tool for agentic coding tasks.

### Step 1: Download the Skill

```bash
git clone https://github.com/DogInfantry/claude-skill-management-consultant-B1.git
```

### Step 2: Move to Your Claude Skills Directory

```bash
mkdir -p ~/.claude/skills/
cp -r claude-skill-management-consultant-B1/skill/ ~/.claude/skills/management-consultant/
```

### Step 3: Verify the Installation

```bash
ls ~/.claude/skills/management-consultant/
# Should show: SKILL.md  references/
```

### Step 4: Use It

In any Claude Code session:
```bash
claude "Help me build an issue tree for a market entry decision"
```

The skill will be loaded automatically.

---

## Method 3: Manual Prompting (No Installation Required)

If you just want to try this without installing anything, you can paste the contents of `skill/SKILL.md` directly into a Claude conversation as your opening message.

1. Open `skill/SKILL.md` from this repository
2. Copy the entire contents
3. Paste it as your first message in a Claude conversation at [claude.ai](https://claude.ai)
4. Follow with your consulting question

> **Limitation**: This method doesn't automatically load the reference files. For the full experience (especially for specialist topics like due diligence, post-merger integration, or industry verticals), use Method 1 or 2.

---

## Verifying It's Working

The skill is working correctly when Claude:

✅ **Leads with the answer** — not a preamble, not "great question!"
✅ **Structures problems MECE** — mutually exclusive, collectively exhaustive branches
✅ **Uses hypothesis-driven language** — "My initial hypothesis is X because..."
✅ **Quantifies claims** — numbers, ranges, benchmarks, not vague assertions
✅ **Applies the Pyramid Principle** — governing thought → supporting arguments → evidence
✅ **Asks good clarifying questions** — context, complication, constraints

If Claude still sounds generic or hedge-everything, try restarting the conversation and explicitly invoking the skill:
```
You are my MBB management consultant. Help me with the following...
```

---

## Troubleshooting

**Q: The skill doesn't seem to be loading.**
A: Make sure the folder is named exactly `management-consultant` and is inside `.claude/skills/`. Restart Claude Cowork after copying files.

**Q: Claude is giving generic consulting advice, not specialist depth.**
A: For specialist topics (e.g., post-merger integration, corporate restructuring, GenAI strategy), explicitly ask Claude to reference the relevant deep-dive. Example: *"Using your due diligence reference, walk me through a commercial DD framework."*

**Q: Can I use this with Claude API?**
A: Yes. Include the contents of `SKILL.md` in your system prompt. For reference file content, you'll need to include the relevant reference files in your context as needed.

**Q: Is this compatible with Claude Sonnet, Opus, and Haiku?**
A: Yes, all Claude models. Claude Sonnet 4.5+ and Opus 4 give the richest consulting responses due to their reasoning depth. Haiku works well for quick framework lookups and case math practice.

---

## File Structure Reference

```
skill/
├── SKILL.md                              # Main skill definition — install this
└── references/
    ├── frameworks.md                     # Complete consulting frameworks toolkit
    ├── case-interview.md                 # McKinsey/Bain/BCG case prep
    ├── guesstimation.md                  # Market sizing & Fermi estimation
    ├── case-types.md                     # Profitability, M&A, market entry, etc.
    ├── issue-hypothesis-trees.md         # MECE decomposition methods
    ├── logic-and-synthesis.md            # Deductive vs. inductive, synthesis
    ├── first-principles-thinking.md      # Challenging assumptions
    ├── mental-models.md                  # Cognitive tools & traps
    ├── structured-case-approach.md       # 5-move structure in 2 minutes
    ├── cross-industry-pattern-recognition.md
    ├── quantitative-toolkit.md           # Back-of-envelope, unit economics
    ├── quantitative-analysis.md          # Financial diagnostics, Excel tools
    ├── qualitative-analysis.md           # Interview coding, affinity mapping
    ├── data-visualization.md             # Chart selection, McKinsey standards
    ├── tools-and-analysis.md             # Operational diagnostics
    ├── industry-heuristics.md            # Sector benchmarks
    ├── industry-intelligence.md          # Rapid orientation for 8 sectors
    ├── universal-business-analysis.md    # 5 decoding questions, 48-hr method
    ├── corporate-strategy.md             # TSR, parenting advantage, portfolio
    ├── pricing-strategy.md               # WTP, conjoint, price architecture
    ├── competitive-intelligence.md       # Win/loss, positioning maps
    ├── scenario-planning.md              # War-gaming, Red/Blue teams
    ├── esg-sustainability.md             # GRI/SASB/TCFD, scope 1/2/3
    ├── ceo-board-agenda.md               # Capital allocation, board governance
    ├── board-governance-future.md        # Skills matrix, governance evolution
    ├── problem-playbooks.md              # Cost transformation, turnaround, etc.
    ├── pe-context.md                     # CDD, investment thesis, 100-day plan
    ├── emerging-markets.md               # Global strategy, cross-border entry
    ├── functional-deep-dives.md          # Supply chain, IT, HR transformation
    ├── deliverables.md                   # Deck, memo, toolkit architecture
    ├── output-craft.md                   # Communication deliverable standards
    ├── storylining.md                    # SCR, ghost deck, narrative arc
    ├── structured-verbal-communication.md
    ├── communication-under-pressure.md   # Hostile Q&A, executive composure
    ├── email-written-communication.md
    ├── executive-presence.md             # Gravitas, credibility, room-reading
    ├── micro-skills-executive-presence.md
    ├── negotiations.md                   # BATNA, M&A deal terms
    ├── negotiation-practitioner.md       # Anchoring, tradeoffs, walk-away
    ├── commercial-contracting.md         # SOW, pricing models, scope creep
    ├── business-development.md           # Proposals, BD, pricing engagements
    ├── proposal-writing.md               # Scoping, fee structures
    ├── value-creation-measurement.md     # Definite vs. derived value, ROI
    ├── ecosystem-alliance-strategy.md    # Multi-partner deals, alliances
    ├── stakeholder-interviewing.md       # Expert networks, VoC, synthesis
    ├── research-and-interviewing.md      # Survey design, triangulation
    ├── stakeholder-mapping.md            # Power/interest, coalition building
    ├── client-management.md              # Pre-wiring, hard messages
    ├── tactical-empathy-trust.md         # Trust-building, political navigation
    ├── managing-analysts.md              # Briefing, reviewing, feedback
    ├── workshop-facilitation.md          # Design, group dynamics
    ├── change-management.md              # ADKAR, Kotter, resistance
    ├── engagement-management.md          # Scoping, workplan, scope creep
    ├── implementation-practitioner.md    # 100-day plan, governance
    ├── implementation-pmo.md             # PMO, agile delivery
    ├── decision-making-under-uncertainty.md
    ├── ai-ml-analytics.md                # AI/ML strategy, GenAI, ML ROI
    ├── ai-orchestration.md               # Three-Layer AI, human-AI pods
    ├── product-thinking-digital.md       # MVP, agile, digital transformation
    ├── pyramid-to-diamond.md             # Future of consulting structure
    ├── knowledge-management-pkm.md       # PARA, Zettelkasten
    ├── context-adaptation.md             # PE, corporate, startup, government
    ├── consulting-career.md              # Promotion, reputation, alumni exits
    ├── healthcare-life-sciences.md       # Hospital P&L, pharma, FDA, CMS
    ├── financial-services.md             # Banking, insurance, fintech
    ├── energy-resources-utilities.md     # LCOE, IRA, energy transition
    ├── technology-media-telecommunications.md
    ├── public-sector-government-defense.md
    ├── consumer-retail-cpg.md
    ├── industrial-manufacturing.md
    ├── real-estate-infrastructure.md
    ├── hospitality-travel-leisure.md
    ├── pricing-revenue-management.md     # Pocket price waterfall, conjoint
    ├── erm-quantitative-risk.md          # Monte Carlo, VaR, CCAR
    ├── due-diligence-deep-dive.md        # Commercial/Operational/Financial DD
    ├── org-design-workforce.md           # Galbraith Star, spans & layers
    ├── process-mining-operational-intelligence.md
    ├── expert-networks-primary-research.md
    ├── post-merger-integration.md        # IMO, synergies, Day 1 readiness
    ├── genai-enterprise-strategy.md      # Pilot purgatory, RAG, LLMOps
    ├── corporate-restructuring-financial-distress.md
    ├── sales-force-effectiveness.md      # Coverage, quota, compensation
    └── climate-netzero-implementation.md # SBTi, MAC curves, CSRD
```
