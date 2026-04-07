# MBB Management Consultant AI Skill for Claude

> A free, open-source consulting knowledge base for Claude, built to help students, MBA candidates, and early-career professionals think more clearly, prep for case interviews, and apply consulting frameworks practically.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Compatible](https://img.shields.io/badge/Claude-Compatible-blueviolet)](https://claude.ai)
[![Skill Type](https://img.shields.io/badge/Type-Management%20Consulting-blue)]()
[![Audience](https://img.shields.io/badge/Audience-MBA%20%7C%20Consultants%20%7C%20Business%20Professionals%20%7C%20Students-green)]()

---

**TL;DR:** Install this skill to give Claude a structured consulting workflow, useful for case prep, framework practice, or thinking through real business problems. Free, open-source, contributions welcome.

---

## What This Is

This repository contains a consulting knowledge base for [Claude](https://claude.ai), Anthropic's AI assistant. When installed, it gives Claude a structured senior-consultant workflow, built around MBB-style problem-solving and communication patterns built by distilling publicly available MBB frameworks, case prep resources, and consulting methodology into a single knowledge base.

This is not a simple prompt. It is a structured knowledge system with 80+ reference files covering every dimension of consulting work, from MECE issue trees and Pyramid Principle communication to due diligence, post-merger integration, GenAI enterprise strategy, and case interview coaching.

**It is completely free.**

---

## Who This Is For

| Audience | How You Benefit |
|----------|----------------|
| **MBA students and candidates** | Practice case interviews, learn consulting frameworks, build structured thinking from scratch |
| **MBB / Big 4 consultants** | Faster decks, sharper issue trees, better synthesis |
| **Business professionals** | Apply consulting-grade thinking to real problems without hiring a firm |
| **Founders and operators** | Structure strategy, diagnose profitability issues, build board-ready narratives |
| **AI / Claude enthusiasts** | Fork, extend, and build your own specialist skills on top of this architecture |
| **Students and academics** | Learn how high-performance problem-solvers actually think |

---

## What's Inside

```
management-consultant-claude-skill/
├── README.md                    <- You are here
├── INSTALL.md                   <- Step-by-step setup guide
├── FRAMEWORKS.md                <- Complete consulting frameworks reference
├── CASE-STUDIES.md              <- 3 worked case examples with full solutions
│
└── skill/
    ├── SKILL.md                 <- The main skill definition (install this)
    └── references/              <- 80+ deep-knowledge reference files
        ├── frameworks.md
        ├── case-interview.md
        ├── guesstimation.md
        ├── issue-hypothesis-trees.md
        ├── storylining.md
        ├── pyramid-to-diamond.md
        ├── healthcare-life-sciences.md
        ├── financial-services.md
        ├── genai-enterprise-strategy.md
        ├── post-merger-integration.md
        ├── corporate-restructuring-financial-distress.md
        └── ... 70+ more
```

---

## Capabilities

Once installed, Claude can assist you with:

### Strategic Problem-Solving
- **MECE issue trees**: decompose any problem into mutually exclusive, collectively exhaustive branches
- **Hypothesis-driven analysis**: start with a point of view, test it with evidence
- **80/20 prioritization**: focus on the 20% of drivers that create 80% of impact
- **First-principles thinking**: break assumptions, reason from fundamentals

### Consulting Frameworks (Full Toolkit)
- Porter's Five Forces, 3C's, McKinsey 7-S, Ansoff Matrix, BCG Growth-Share
- Value Chain Analysis, Blue Ocean Strategy, GE-McKinsey 9-Box
- PESTEL, TAM/SAM/SOM, STP, Jobs-to-Be-Done
- DuPont Analysis, Unit Economics (CAC/LTV), DCF basics
- Profitability frameworks, Kotter's 8 Steps, RACI, Three Horizons

### Case Interview Coaching
- Full McKinsey / Bain / BCG case formats
- Practice cases across all case types (profitability, market entry, M&A, pricing, growth)
- Scoring rubrics and structured feedback
- PEI (Personal Experience Interview) preparation with STAR coaching
- Math and estimation drills

### Communication and Deliverables
- **Pyramid Principle**: lead with the answer, support with evidence
- **SCR structure**: Situation, Complication, Resolution
- Executive-grade slide action titles, memos, one-pagers
- Storylining: from 200 facts to 5 messages with a red thread
- Communication under pressure, hostile Q&A, executive presence

### Industry Reference Files
- Healthcare and Life Sciences (hospital P&L, pharma pipeline, FDA, CMS)
- Financial Services (NIM, ROE, Basel IV, insurance, fintech)
- Energy and Utilities (LCOE, IRA, energy transition, FERC)
- Technology, Media and Telecom (SaaS unit economics, platform dynamics, 5G)
- Consumer, Retail and CPG (GMROI, trade spend, DTC disruption)
- Industrial and Manufacturing (OEE, Lean/TPS, S&OP, Industry 4.0)
- Public Sector and Defense (FAR/DFARS, GovCon, IDIQ)
- Real Estate and Infrastructure (cap rates, NOI, REPE, REIT)
- Hospitality and Travel (RevPAR, ADR, airline CASK)

### Specialist Methods
- Due diligence (commercial, operational, financial, ESG)
- Post-merger integration (IMO, synergy framework, Day 1 readiness)
- Corporate restructuring and financial distress (Chapter 11, DIP, 13-week cash flow)
- GenAI enterprise strategy (pilot purgatory, RAG, LLMOps, EU AI Act)
- Pricing and revenue management (conjoint, Van Westendorp, price waterfall)
- Org design and workforce planning (Galbraith Star, spans and layers, SBO)
- Change management (ADKAR, Kotter, resistance management)
- Climate strategy and net-zero (SBTi, MAC curves, CSRD, CBAM)
- Process mining (Celonis, Signavio, conformance checking)
- Sales force effectiveness (quota setting, coverage models, CRM analytics)

---

## Quick Start

### 1. Get Claude
You need access to [Claude](https://claude.ai). Free tier works; Pro is recommended for heavy use.

### 2. Install the Skill
See **[INSTALL.md](./INSTALL.md)** for the full setup guide. The short version:

1. Download `skill/SKILL.md` and the entire `skill/references/` folder
2. Follow the Cowork/Claude Code installation steps in `INSTALL.md`
3. Start a new conversation and type: *"Act as my management consultant"*

### 3. Try These Prompts
```
"Help me structure a profitability analysis for a $500M retail chain whose margins have been declining."

"I have a case interview at McKinsey next week. Run me through a market entry case."

"Size the US electric vehicle charging market from first principles."

"My company is considering acquiring a SaaS competitor. Build me an M&A issue tree."

"Write me an executive summary for a cost reduction initiative in the logistics function."

"I need to present a go-to-market strategy to the board. Help me structure the narrative."
```

---

## For Case Interview and Competition Prep

This skill is built for active practice, not just passive reading.

**For case interview prep:**
- Ask Claude to run you through a case as an interviewer (McKinsey-led, BCG candidate-led, Bain collaborative)
- Get scored on structure, hypothesis, quant, synthesis, and recommendation
- Practice market sizing, profitability, market entry, M&A, pricing across all formats
- Drill behavioral / PEI stories with real-time STAR coaching

**For case competitions:**
- Use Claude to stress-test your team's issue tree before the presentation
- Get a second opinion on your recommendation and the risks you may have missed
- Sanity-check your market sizing assumptions and financial math
- Sharpen your slide action titles and executive narrative

**For self-study and groundwork:**
- Work through the 3 case studies in [CASE-STUDIES.md](./CASE-STUDIES.md) before attempting live cases
- Use [FRAMEWORKS.md](./FRAMEWORKS.md) as your active reference, not just a read-once guide
- Build the habit of structuring every problem MECE before answering

```
"Run me through a McKinsey-style profitability case. Play the interviewer."

"Score my structure on this market entry case on a 1-4 scale across all dimensions."

"My case comp team has 48 hours. Help us stress-test our recommendation."

"Give me 10 market sizing questions and coach me through each one."
```

---

## The Consulting Mindset

Top consultants operate with a specific cognitive architecture that most people are never explicitly taught:

- They lead with the answer, not the analysis
- They think in structures, not lists
- They form hypotheses before gathering data, not after
- They apply 80/20 thinking ruthlessly
- They communicate in pyramids: governing thought, then evidence

This skill is a scaffold for building those habits. It is not a replacement for judgment, but a way to practice the patterns consistently.

---

## Frameworks Quick Reference

See **[FRAMEWORKS.md](./FRAMEWORKS.md)** for the complete reference. Highlights:

| Problem | Framework |
|---------|-----------|
| Why is profit declining? | Profitability tree, DuPont, Value chain |
| Should we enter market X? | 3C's + Market sizing, Porter's Five Forces |
| How to grow revenue 20%? | Ansoff Matrix + Solution issue tree |
| Should we acquire Company Y? | 3C's + Synergy analysis + DCF |
| How to optimize operations? | Lean / Value stream, DMAIC |
| How to build a strategy? | Porter's Five Forces + 3C's + Blue Ocean |
| How to restructure the org? | 7S + Kotter + RACI + Talent 9-Box |
| How to price a new product? | Value-based pricing + Competitive positioning |

---

## Case Studies

See **[CASE-STUDIES.md](./CASE-STUDIES.md)** for 3 fully worked cases with prompts, structures, analysis, and recommendations:

1. **The Falling Star**: Profitability decline at a $800M specialty beverage company
2. **New Frontier**: Market entry strategy for a European athletic apparel brand entering the US
3. **The Big Question**: Market sizing for the US pet insurance market (PE due diligence)

Each case shows how a senior consultant would structure it, analyze it, and recommend.

---

## Contributing

This is a living knowledge base — the more industries, benchmarks, and cases it covers, the more useful it becomes for everyone.

**See [CONTRIBUTING.md](./CONTRIBUTING.md)** for the full guide: file structure, quality bar, and how to submit a PR.

**Open issues (good places to start):**
- [Add reference file: Cybersecurity Consulting](https://github.com/DogInfantry/claude-skill-management-consultant-B1/issues/3)
- [Add reference file: Education & EdTech](https://github.com/DogInfantry/claude-skill-management-consultant-B1/issues/4)
- [Update benchmarks: genai-enterprise-strategy.md](https://github.com/DogInfantry/claude-skill-management-consultant-B1/issues/5)
- [Add case study: PE / LBO case](https://github.com/DogInfantry/claude-skill-management-consultant-B1/issues/6)
- [Add reference file: Semiconductor & Hardware](https://github.com/DogInfantry/claude-skill-management-consultant-B1/issues/7)

You don't need to be ex-MBB to contribute. If you've worked in any industry, finance role, or ops team, you have something concrete to add.

---

## If This Helped You

If this skill helped you prep for an interview, win a case comp, solve a real business problem, or just think more clearly, consider:

- ⭐ **Starring the repo** so others can find it
- 🔁 **Sharing it** with someone preparing for consulting interviews or working through a hard problem
- 🛠️ **Contributing** a case study, framework, or industry reference

Built for free, meant to stay free.

---

## License

MIT License. Free to use, fork, adapt, and distribute. See `LICENSE` for details.

---

*Pass it on.*
