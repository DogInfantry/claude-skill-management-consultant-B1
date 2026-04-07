# Contributing to claude-skill-management-consultant-B1

Thanks for wanting to contribute. This is a living knowledge base — the more industries, case types, and methods it covers, the more useful it becomes for everyone.

---

## What You Can Contribute

- **New industry reference files** — any industry not yet covered (see gaps below)
- **New case studies** — worked examples across different case types
- **Framework updates** — corrections, newer benchmarks, emerging methods
- **Benchmark refreshes** — update existing files with 2025–26 data
- **Bug fixes** — factual errors in any existing file

---

## Confirmed Gaps (Start Here)

These are missing and high priority. Pick one and open a PR:

| Area | File to create | Notes |
|------|---------------|-------|
| Education & EdTech | `skill/references/education-edtech.md` | K-12, higher ed, LMS platforms, ed-tech unit economics, government funding models |
| Agriculture & Food Systems | `skill/references/agriculture-food.md` | Agri input markets, food processing, cold chain, commodity dynamics, ESG in food |
| Aerospace & Defense | `skill/references/aerospace-defense.md` | MRO, OEM, government contracting, ITAR, defense budgeting cycles |
| Cybersecurity | `skill/references/cybersecurity.md` | Zero trust, SOC operations, incident response consulting, MSSP economics |
| Semiconductor & Hardware | `skill/references/semiconductor-hardware.md` | CHIPS Act, fab economics, fabless vs IDM, geopolitical supply chain |
| Wealth Management | `skill/references/wealth-management.md` | Family office, RIA economics, fee compression, alternatives allocation |
| Consulting Tools (2026) | `skill/references/consulting-tools-2026.md` | AlphaSense, Tegus, McKinsey Lilli, BCG Gamma, AI in the engagement stack |
| PE/LBO Case Study | `CASE-STUDIES.md` addition | Full LBO case with value creation levers, entry/exit multiples, recommendation |
| Startup / Venture Case Study | `CASE-STUDIES.md` addition | Series B growth strategy or burn rate / runway case |

---

## Benchmark Updates Needed in Existing Files

If you have domain expertise, these files need 2025–26 data refreshes:

| File | What needs updating |
|------|-------------------|
| `skill/references/financial-services.md` | NIM ranges, ROE benchmarks, Basel IV implementation, fintech multiples |
| `skill/references/genai-enterprise-strategy.md` | ROI benchmarks (MGI 2025 data), EU AI Act compliance, agentic AI patterns |
| `skill/references/esg-sustainability.md` | EU CSRD (live 2024), SEC climate disclosure rules, CBAM 2026 |
| `skill/references/pe-context.md` | Entry multiples reset (8–10x vs 2021's 12–14x), current deal structures |
| `skill/references/corporate-restructuring-financial-distress.md` | Post-rate-cycle distress patterns, 2024–25 restructuring wave data |

---

## Reference File Structure

All `skill/references/` files follow this structure. **Match it exactly** so Claude can use the files consistently.

Use [`skill/references/healthcare-life-sciences.md`](skill/references/healthcare-life-sciences.md) as the quality benchmark — that's the standard to aim for.

```markdown
# [Industry/Topic Name]: MBB Consulting Reference

> One-line description of what this file covers and who it's for.

---

## Executive Overview
[3–5 sentences: what this domain is, its scale, why it matters in consulting,
which firms have dedicated practices here]

---

## Industry Economics and Margin Structure
[Revenue models, gross/operating margins by segment, cost structure breakdown,
benchmark ranges with sources or basis]

---

## Key Metrics and KPIs
[The 10–15 metrics a consultant must know cold in this industry.
Each metric: definition + typical benchmark range + what drives variance]

---

## Regulatory and Compliance Framework
[Key regulations, enforcement bodies, compliance obligations that affect
strategy and operations. Not legal advice — consulting-relevant framing only]

---

## Structural Industry Dynamics
[Consolidation trends, competitive structure, disruption forces,
M&A activity, PE/investor interest]

---

## Common Consulting Engagement Types
[3–5 engagement archetypes: what the client problem is, how a consultant
structures it, what the typical recommendation looks like]

---

## Case Interview Angles
[How this industry shows up in case interviews. Specific case types,
common hypotheses, traps to avoid]

---

## Benchmarking Standards
[Summary benchmark table: key metrics with low/median/high ranges]

---

## Consulting Watchouts
[What junior consultants get wrong. Industry-specific traps,
data interpretation errors, client communication landmines]
```

**Length target:** 8,000–20,000 words. Depth over breadth — one well-sourced metric beats five vague ones.

---

## How to Submit

1. **Fork** the repo
2. **Create your file** following the structure above
3. **Submit a Pull Request** with title format: `Add: [industry/topic name] reference file`
4. **In the PR description**, include:
   - What you added or changed
   - Your background in this area (optional but helps with review)
   - Any sources or basis for benchmarks used
   - If updating an existing file, what specifically changed and why

---

## Quality Bar

Before submitting, check your file against these:

- **Factual accuracy** — benchmarks must reflect real consulting practice, not textbook theory
- **No invented data** — if you're unsure of a benchmark, write "varies by segment" or give a range rather than a false specific
- **Consulting framing** — write for someone doing client work, not academic study. Every section should answer: "what does a consultant actually do with this?"
- **MECE structure** — sections should not overlap; each should add distinct value
- **Current** — benchmarks should reflect 2024–26 conditions where possible; flag anything older

---

## What We Won't Accept

- Files that are just framework lists without benchmarks or engagement context
- Copied or paraphrased content from published firm materials (legal risk)
- Files under 3,000 words (too shallow to be useful)
- Content that duplicates an existing reference file without clear differentiation

---

## Questions?

Open an issue and tag it `question`. We'll respond within a few days.

---

*Built for free. Meant to stay free.*
