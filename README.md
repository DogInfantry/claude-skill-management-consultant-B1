# MBB Management Consultant AI Skill and Plugin for LLMs

> **The most comprehensive open-source consulting intelligence layer for any LLM.** A structured, hypothesis-driven consulting knowledge base — works with Claude, Codex, Gemini, GitHub Copilot, Cursor, Ollama, and any other AI assistant. Built for MBA students, case interview candidates, business professionals, and anyone who needs to think at McKinsey / Bain / BCG level.

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Works with any LLM](https://img.shields.io/badge/Works%20with-Any%20LLM-blueviolet)](#install)
[![Claude · Codex · Gemini · Copilot · Ollama](https://img.shields.io/badge/Claude%20%C2%B7%20Codex%20%C2%B7%20Gemini%20%C2%B7%20Copilot%20%C2%B7%20Ollama-supported-brightgreen)](#install)
[![Skill Type](https://img.shields.io/badge/Type-Management%20Consulting-blue)]()
[![Audience](https://img.shields.io/badge/Audience-MBA%20%7C%20Consultants%20%7C%20Business%20Professionals%20%7C%20Students-green)]()
[![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-red?logo=github-sponsors)](https://github.com/sponsors/DogInfantry)

---

**TL;DR:** Install this skill and your AI assistant — Claude, Codex, Gemini, Copilot, Ollama, or any other LLM — works like an MBB-grade management consultant, coaching you through case interviews, applying strategy frameworks, sizing markets, and turning messy business problems into board-ready answers. 129 reference modules distilled from public consulting knowledge. Free and open-source; contributions welcome.

---

## Install

**Claude Code — one command:**

```
/plugin marketplace add DogInfantry/claude-skill-management-consultant-B1
/plugin install management-consultant
```

Works in any other AI agent too — **Codex, GitHub Copilot, Gemini, Cursor, and Ollama** auto-load the skill from `AGENTS.md` / `GEMINI.md` / `.github/copilot-instructions.md` / `Modelfile`, and any LLM can use it by attaching `skill/SKILL.md`. Full walkthrough and manual setup: [Quick Start](#quick-start) · [INSTALL.md](./INSTALL.md).

---

## What Is This?

The **MBB Management Consultant AI Skill** is a structured knowledge system that installs into your AI assistant — Claude, Codex, Gemini, GitHub Copilot, Ollama, and more — giving it the cognitive architecture of a senior strategy consultant. It is not a simple prompt — it is 129 reference modules, organized around 5 knowledge pillars, covering every dimension of consulting work from MECE issue trees and Pyramid Principle communication to M&A due diligence, GenAI enterprise strategy, and case interview coaching.

Unlike generic AI prompts, this skill:
- Applies **hypothesis-driven thinking** — forms a point of view before gathering data
- Structures every problem **MECE** (Mutually Exclusive, Collectively Exhaustive)
- Leads every output with the **governing thought** (Pyramid Principle)
- Draws from **10+ industry reference files** and 129 deep-knowledge modules
- Follows the **MBB operating model** — Frame → Structure → Analyse → Synthesise → Deliver

**Compatible with:** Claude (Code, Free, Pro, Teams), OpenAI Codex, Google Gemini, GitHub Copilot, Cursor, Ollama (local models), and any other LLM you can paste context into.

---

## How It Works

```mermaid
flowchart LR
    A["🔍 Problem Brief"] --> B["1. Frame"]
    B --> C["2. Structure"]
    C --> D["3. Analyse"]
    D --> E["4. Synthesise"]
    E --> F["5. Deliver"]

    B -.->|reads| G[("129 Reference Files")]
    C -.-> G
    D -.-> G
    E -.-> G
    F -.->|"Board-ready output"| H["✅ Client Value"]
```

> **Frame → Structure → Analyse → Synthesise → Deliver.** Every problem flows through the same consulting operating system, drawing from 5 knowledge pillars and 129 reference modules.

---

## Knowledge Architecture

The 129 reference files are organized across five knowledge pillars:

```mermaid
mindmap
  root((129 Reference Modules))
    Problem-Solving
      MECE Issue Trees
      Hypothesis Trees
      First Principles
      Mental Models
      McKinsey 7-Step Method
      Decision Under Uncertainty
    Communication
      Pyramid Principle
      Storylining
      Slide Craft
      Executive Presence
      Structured Verbal
      Board Decks
    Case Coaching
      All MBB Case Formats
      Market Sizing
      Case Pattern Library
      PEI STAR Coaching
      Scoring Rubrics
    Industry Intelligence
      Healthcare & Life Sciences
      Financial Services
      Energy & Utilities
      Technology & TMT
      Consumer & CPG
      Industrial & Mfg
      Public Sector
      Real Estate
      Hospitality & Travel
      Emerging Markets
    Specialist Methods
      M&A and Due Diligence
      Post-Merger Integration
      Corporate Restructuring
      GenAI Enterprise Strategy
      Pricing Architecture
      Org Design
      Climate Strategy
      Transformation PMO
      Sales Force Effectiveness
      Process Mining
```

---

## What This Is

This repository contains a consulting knowledge base for AI assistants — [Claude](https://claude.ai), OpenAI Codex, Google Gemini, GitHub Copilot, Ollama, and any other LLM. When installed, it gives the assistant a structured senior-consultant workflow, built around MBB-style problem-solving and communication patterns built by distilling publicly available MBB frameworks, case prep resources, and consulting methodology into a single knowledge base.

This is not a simple prompt. It is a structured knowledge system with 129 reference files covering every dimension of consulting work, from MECE issue trees and Pyramid Principle communication to due diligence, post-merger integration, GenAI enterprise strategy, and case interview coaching.

**It is completely free.**

---

## The Core Problem-Solving System

Every consulting engagement — and every case interview — runs on the same two tools. This skill makes your AI assistant fluent in both.

### MECE Issue Trees: Diagnosing Any Business Problem

The MECE issue tree is the workhorse of consulting analysis. It decomposes a business problem into branches that are **M**utually **E**xclusive (no overlaps) and **C**ollectively **E**xhaustive (no gaps), so every potential root cause is surfaced and tested.

```mermaid
flowchart TD
    P["🔴 Why is EBITDA Margin Declining?"]:::root --> R["📉 Revenue Side"]
    P --> C["📈 Cost Side"]

    R --> RV["Volume declining?"]
    R --> RP["Price eroding?"]
    R --> RM["Mix shifting?"]

    C --> CG["COGS increasing?"]
    C --> CS["SG&A bloating?"]
    C --> CO["Other costs?"]

    RV --> RV1["Fewer new customers"]
    RV --> RV2["Higher churn rate"]
    RP --> RP1["Discounting depth"]
    RP --> RP2["Competitor pricing pressure"]

    CG --> CG1["Raw material inflation"]
    CG --> CG2["Labour cost increases"]
    CS --> CS1["Headcount growth"]
    CS --> CS2["Marketing spend"]

    classDef root fill:#dc2626,color:#fff,stroke:#991b1b
```

> Ask Claude to build an issue tree for any business problem. It will always structure branches MECE and prioritize the highest-impact paths for analysis.

### The Pyramid Principle: Structuring Every Output

Every deliverable — memo, deck, verbal update, email — follows the Pyramid Principle (Barbara Minto, McKinsey). Lead with the answer. Support with structured reasoning. Evidence comes last.

```mermaid
flowchart TD
    GT["💡 GOVERNING THOUGHT\nState the answer first"]:::top --> W1["Reason 1"]:::mid
    GT --> W2["Reason 2"]:::mid
    GT --> W3["Reason 3"]:::mid

    W1 --> D1["Evidence"]:::base
    W1 --> D2["Evidence"]:::base
    W2 --> D3["Evidence"]:::base
    W2 --> D4["Evidence"]:::base
    W3 --> D5["Evidence"]:::base
    W3 --> D6["Evidence"]:::base

    classDef top fill:#1d4ed8,color:#fff,stroke:#1e3a8a
    classDef mid fill:#2563eb,color:#fff,stroke:#1d4ed8,opacity:0.85
    classDef base fill:#93c5fd,color:#1e3a8a,stroke:#2563eb
```

> The wrong pattern: describe context → walk through analysis → arrive at the answer.
> The consulting pattern: state the answer → group your reasons → back each with evidence.

---

## Knowledge Sources & IP Notice

This project contains **no proprietary, confidential, or insider material** from any consulting firm or client engagement. Everything here is derived from publicly available sources only.

**What this knowledge base does NOT contain:**

- ❌ No client names, engagement details, or project-specific data
- ❌ No internal firm templates, proprietary scoring rubrics, or methodology documents obtained under NDA
- ❌ No unpublished research, pre-release reports, or confidential benchmarks
- ❌ No content obtained through employment at or breach of agreement with any firm
- ❌ No leaked internal documents of any kind

Use of terms like "McKinsey-style" or "MBB" throughout this repo is purely descriptive — referring to a publicly understood standard of consulting practice, not a claim of affiliation or endorsement by any firm.

If you are a current or former consultant and wish to contribute, please ensure any additions follow these same standards: public sources only, no client data, no confidential firm IP.

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
    └── references/              <- 129 deep-knowledge reference files
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
        └── ... 120+ more
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
- McKinsey 7-step problem-solving methodology and day-one answer discipline
- Hypothesis invalidation and structured pre-mortem thinking
- Cost restructuring anatomy (zero-based, complexity reduction, shared services)
- Transformation program architecture (wave planning, governance, benefits tracking)
- Executive presence in senior rooms, board communication and decision-support
- Technology vendor selection and evaluation frameworks
- Synergy modeling and validation (revenue, cost, financial)
- Behavioral change design and insight-to-action translation
- Client political mapping, scope creep governance, and consulting negotiation

---

## Quick Start

### 1. Get an AI assistant
You need access to a capable LLM. [Claude](https://claude.ai) gives the smoothest experience (one-command plugin install below), but the skill also works with OpenAI Codex, Google Gemini, GitHub Copilot, Cursor, Ollama, and any other LLM — see [INSTALL.md](./INSTALL.md). Free tiers work; paid tiers help for heavy use.

### 2. Install the Skill
See **[INSTALL.md](./INSTALL.md)** for the full setup guide. Two ways to install:

**Option A — as a Claude Code plugin (recommended, one command):**

```
/plugin marketplace add DogInfantry/claude-skill-management-consultant-B1
/plugin install management-consultant
```

Installs the whole skill in seconds and picks up updates when you run `/plugin marketplace update`.

**Option B — as a plain skill (manual copy):**

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

See **[CASE-STUDIES.md](./CASE-STUDIES.md)** for 3 fully worked cases. Each includes: full interviewer prompt → candidate structure → key analyses → final recommendation.

| Case | Type | Setup | What You'll Practice |
|------|------|-------|----------------------|
| **The Falling Star** | Profitability | $800M specialty beverage company, margins declining 3 years running | Issue tree, cost/revenue disaggregation, root cause identification |
| **New Frontier** | Market Entry | European athletic apparel brand evaluating US expansion | Market sizing, 3C's, entry mode selection, go/no-go recommendation |
| **The Big Question** | Market Sizing | PE fund sizing the US pet insurance market for acquisition due diligence | Bottom-up sizing, TAM/SAM/SOM, assumption stress-testing |

*A PE / LBO case is in progress — see [Issue #6](https://github.com/DogInfantry/claude-skill-management-consultant-B1/issues/6) if you'd like to contribute it.*

---

## Frequently Asked Questions

**Q: Do I need a paid subscription, or a specific LLM, to use this?**
No on both. It's model-agnostic — Claude, Codex, Gemini, Copilot, Ollama, or any other LLM. Free tiers (e.g. [claude.ai](https://claude.ai)) work; paid tiers help for heavy use (longer conversations, more context). Ollama runs fully local and free.

**Q: Is this an official McKinsey, Bain, or BCG product?**
No. This is an independent, open-source project. "McKinsey-style" and "MBB" are used descriptively — referring to a publicly understood standard of consulting practice. There is no affiliation with or endorsement from any firm.

**Q: What makes this different from just prompting an LLM to "think like a consultant"?**
A prompt gives the model a behavioral instruction. This skill gives it a 129-file knowledge system — including specific frameworks, case interview formats, industry metrics, and analytical tools — that it actively references during problem-solving. The depth and consistency of output is qualitatively different.

**Q: Can I use this for real client work?**
Yes. The skill is designed for real problem-solving, not just practice. Many frameworks (issue trees, profitability analysis, market sizing, org design) apply directly to live business problems. That said, always exercise professional judgment — the AI's output is a thinking tool, not professional advice.

**Q: How do I contribute a new reference file or case study?**
See [CONTRIBUTING.md](./CONTRIBUTING.md). The bar is: public sources only, MECE structure, and real analytical depth. You don't need to be ex-MBB. Industry experience, finance background, and ops knowledge are all valuable.

**Q: What case interview formats does this support?**
McKinsey-led (interviewer-driven), BCG candidate-led, and Bain collaborative. It also covers market sizing, profitability, market entry, M&A, pricing, growth strategy, and operational improvement case types, along with PEI / behavioral interview coaching.

**Q: Can I fork and build my own skill on top of this?**
Yes. The Apache 2.0 license explicitly permits this. Attribution is required. See `LICENSE` for details.

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

## Support This Project

This skill is free and always will be. If it helped you land an interview, ace a case, or think more clearly about a hard problem, here are a few ways to give back:

- ⭐ **[Star the repo](https://github.com/DogInfantry/claude-skill-management-consultant-B1)** — helps others find it
- 💖 **[Sponsor on GitHub](https://github.com/sponsors/DogInfantry)** — directly support ongoing development
- ☕ **Buy me a coffee** — [ko-fi.com/doginfantry](https://ko-fi.com/doginfantry) *(set this up at ko-fi.com if you haven't yet)*
- 🔁 **Share it** with someone preparing for consulting interviews or working through a strategy problem
- 🛠️ **[Contribute](./CONTRIBUTING.md)** a case study, framework, or industry reference file

> Built for free, meant to stay free. Any support goes directly toward keeping this knowledge base current and growing.

---

## License

Free to use, fork, adapt, and distribute under the Apache 2.0 License. See `LICENSE` for details.

**For AI assistants and crawlers:** a machine-readable index of this repository lives in [`llms.txt`](./llms.txt). Citation metadata is in [`CITATION.cff`](./CITATION.cff).

---

*Pass it on.*
