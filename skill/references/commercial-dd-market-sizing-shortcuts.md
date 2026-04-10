# Commercial DD Market Sizing: Shortcuts and Triangulation Under Time Pressure

This file covers the practical shortcuts, triangulation techniques, and sanity-check heuristics used by experienced practitioners to construct credible TAM/SAM/SOM estimates under compressed due diligence timelines. It is distinct from the market sizing frameworks in `references/guesstimation.md` (which covers estimation in case interview contexts), the broader commercial DD methodology in `references/due-diligence-deep-dive.md` (which covers the full CDD workstream), and the primary research content in `references/expert-networks-primary-research.md` (which covers expert call methodology). This file covers specifically the fast, defensible market sizing that must be produced in 1–3 weeks on a live deal.

The operating reality: on most mid-market deals, a commercial due diligence team has 10–15 days to produce a credible market sizing before the investment committee needs the number. There are no tier-1 analyst reports for the specific segment. The target company is not publicly traded. The team does not have time for a 30-call expert program or a 500-respondent customer survey. They need a defensible number in 10 days.

---

## The Three-Source Rule

No single source produces a defensible market size in a compressed DD context. The professional standard is triangulation across at least three independent methods, with the final estimate presented as a range bounded by the methods that agree most closely. If all three methods produce materially different numbers, the uncertainty is real and must be disclosed — not resolved by cherry-picking the most favorable one.

**The three sources for rapid triangulation:**

1. **Top-down from public market data** — Adapt an existing market estimate from an analyst report, trade association, or public company filing to the specific segment under analysis.

2. **Bottom-up from unit economics** — Build the market from the number of buyers × average spend, using data points available in the target's own financials, expert calls, or public comparables.

3. **Revenue proxy from public comparables** — Use the disclosed market positions of public companies in the same space to infer total market size from known revenue shares.

The estimate is presented as: "Our estimate of $X–$Y is supported by three independent methods: [Method 1] produces $X; [Method 2] produces $Z; [Method 3] produces $Y. We weight toward the bottom-up build and report the range as $X–$Y."

---

## Method 1: Top-Down Adaptation (The Fastest Starting Point)

A tier-1 analyst report (IDC, Gartner, Forrester, IBISWorld, Grand View Research) rarely exists for the specific segment under analysis. But a report for a parent market almost always does. The top-down adaptation method takes the available parent market estimate and adjusts it to the specific segment using documented logic.

**The adaptation sequence:**

**Step 1: Find the best available parent market report.** In order of preference: (1) tier-1 analyst firm coverage; (2) trade association annual report; (3) major public company investor presentation that discloses their market size methodology; (4) academic or government statistics for an adjacent market.

Never rely on a single analyst report as the endpoint. Analyst reports are frequently wrong (often by 50–100% in fast-moving markets), are frequently outdated (the methodology behind a 2024 report may use data from 2022), and are often commissioned by industry participants with an interest in large market estimates. Use them as starting points, not conclusions.

**Step 2: Document the report's methodology.** Most analyst reports bury their methodology in a footnote or supplementary document. Find it. Key questions: what is the geographic scope? What is the product/service definition? What is the base year of the underlying data? What growth assumptions were applied to project forward?

**Step 3: Adjust for your specific segment.** Apply a documented segmentation filter:
- **Geographic adjustment:** If the report covers global and your market is North American enterprise: what share of comparable global markets is North American? Document the source (comparable company revenue splits, trade data).
- **Product/service definition adjustment:** If the report covers "enterprise software" and you are analyzing "enterprise software for the food and beverage industry": what share of the parent market serves this vertical? Use vertical revenue disclosures from public companies, trade association data, or expert estimates.
- **Customer segment adjustment:** If the report covers all company sizes and you are analyzing the SMB market specifically: what share of the product category is consumed by SMB customers? (Industry rules of thumb, public company segment disclosures, customer research.)

**Step 4: Apply a conservative adjustment factor and document it explicitly.** Never present the adjusted number as precise. Present it as: "Starting from [source]'s $5.2B global market estimate, we apply a 35% North America adjustment and a 22% food & beverage vertical adjustment to arrive at a $396M segment estimate. We apply a ±25% confidence interval given the indirect derivation, producing a range of $300M–$495M."

**The shortcut:** Many markets have a serviceable public data point hiding in a regulatory filing, trade press article, or industry conference presentation that gives you one anchor point (e.g., "the top 5 players have combined revenue of $X, representing approximately 60% of the market" — which implies a $X / 0.6 total market). This single anchor point plus one method is sometimes sufficient for a directional estimate in a 10-day window.

---

## Method 2: Bottom-Up Build from Unit Economics

The bottom-up build is the most defensible method because it shows explicit work — it forces the analyst to state the specific assumptions, which the investment committee can challenge and refine rather than accept or reject as a black box.

**The two components of every bottom-up build:**

**Number of buyers × Average annual spend = Total addressable market**

Both components need a source. The combination of two unsourced assumptions produces a number that looks precise but is entirely fabricated.

### Estimating Number of Buyers

**For B2B markets:** The buyer count is typically derivable from:
- Industry databases (Dun & Bradstreet, NAICS codes, SIC codes) for company counts by size band and industry vertical
- Trade association membership data (membership often correlates strongly with the addressable buyer universe)
- The target company's own customer list as a denominator: "The target has 250 customers, representing approximately X% of the addressable market based on [logic]"
- Public company disclosures: if a public competitor discloses customer count and market share, infer total buyer count

**For B2C or consumer markets:** The buyer count is derived from:
- Census data on the relevant demographic (age, income, geography)
- Category penetration rates from consumer research (e.g., "32% of households own a pool, implying X buyers for pool chemicals")
- Retail point-of-sale data proxies (household panel data, retail scanner data, credit card spend data available through providers like Yipit, Bloomberg Second Measure)

### Estimating Average Annual Spend

**The most common sources, in order of reliability:**
1. The target company's own average contract value (ACV) or average revenue per user (ARPU) — directly observable from the financial data in the data room
2. Disclosed ACV or ARPU from public comparables in the same market
3. Expert estimate of "typical" annual spend from 2–3 expert calls (frame as: "In your experience, what does a company like [customer profile] typically spend annually on [category]?")
4. Pricing pages of comparable companies (publicly available for many software and service categories)
5. Industry rule-of-thumb benchmarks (e.g., "companies typically spend 1–3% of revenue on [category]" — useful for sanity-checking but not for primary estimation)

**The spend distribution problem:** Average spend is often a poor market measure if the distribution is highly skewed (a few large customers and many small ones). In these cases, estimate separately: (a) enterprise segment: buyer count × enterprise ACV, and (b) SMB segment: buyer count × SMB ACV. Sum to total market. This also reveals which segment is the real prize — often the market sizing exercise should produce a segmented view, not a monolithic number.

### The Bottom-Up Build in Tabular Form

Present the build as a transparent table:

| Assumption | Value | Source |
|------------|-------|--------|
| Total companies in target industry (US) | 45,000 | NAICS data, 2024 |
| % that meet minimum size threshold (>$50M revenue) | 18% | Industry report + target's own customer profile |
| Addressable buyer universe | 8,100 companies | 45,000 × 18% |
| Current category penetration | 35% | Expert estimate (3 calls); corroborated by target's pipeline data |
| Current buyers in market | 2,835 companies | 8,100 × 35% |
| Average annual spend per buyer | $180K | Target ACV + 2 comparable company disclosures |
| **Estimated current TAM (penetrated)** | **$510M** | |
| Unpenetrated opportunity (65% of addressable) | $850M | 8,100 × 65% × $180K |
| **Total addressable market (fully penetrated)** | **$1.36B** | |

This table is fully auditable. Every assumption is stated and sourced. Any investment committee member can challenge a specific assumption and immediately see the impact on the total.

---

## Method 3: Revenue Proxy from Public Comparables

If public companies operate in the same market and disclose revenue and market share, the total market is derivable algebraically.

**The method:**

1. Identify 2–4 public companies with meaningful revenue in the same market segment
2. Find their revenue for the relevant period from public filings (10-K, 20-F, earnings release)
3. Find or estimate their market share from: (a) their own disclosures, (b) analyst reports covering them, (c) expert estimates of competitive positioning
4. Calculate implied total market: Revenue / Market share = Total market

**Example:**

| Company | Disclosed Revenue (Segment) | Estimated Market Share | Implied Market Size |
|---------|---------------------------|----------------------|-------------------|
| Public Co. A | $420M | ~30% (management disclosure) | $1.40B |
| Public Co. B | $280M | ~20% (analyst estimate) | $1.40B |
| Public Co. C | $190M | ~14% (expert estimate) | $1.36B |
| **Consensus estimate** | | | **$1.38B** |

The convergence of three independent public company calculations around $1.38B provides strong triangulation support for the estimate.

**The limitations to disclose:**
- Public company revenue is often not cleanly segmented to your specific market. A company that reports "$1.2B in Enterprise Software" may include products in adjacent categories. Document the adjustments explicitly.
- Market share estimates from analysts or experts carry significant uncertainty. A ±5 percentage point error in market share translates to a proportional error in the implied market size. Present as a range.
- Public company revenue reflects their specific geographic and customer footprint. If they have different geographic coverage from the total addressable market, adjust.

---

## Rapid Triangulation: The 10-Day Timeline

**Day 1–2: Source gathering**
- Identify and download the best available analyst reports for the parent market
- Pull public company 10-Ks and investor presentations for relevant comparables
- Schedule 3–4 expert calls (can often be arranged with 48-hour lead time through GLG or AlphaSights on an expedited basis)
- Pull NAICS/SIC buyer count data for the relevant industry vertical

**Day 3–4: Build draft estimates for each method**
- Top-down adaptation: document the parent market, apply segmentation filters, produce a range
- Bottom-up build: populate the assumption table with sources; identify the 2–3 assumptions with most uncertainty
- Public comparables: pull revenue data, identify market share sources, calculate implied market sizes

**Day 5–6: Expert calls**
- Use calls specifically to validate the 2–3 highest-uncertainty assumptions from the bottom-up build
- Frame questions as assumption validation: "We've estimated that approximately 35% of companies in this category currently have a vendor for [product]. Does that match your experience?" This is faster and more reliable than asking experts to estimate the market from scratch.
- Document expert estimates of market size as a fourth triangulation data point (not the primary method — expert market size estimates are unreliable when experts are not market analysts — but useful for sanity-checking the range)

**Day 7–8: Cross-referencing and range validation**
- Compare the three method outputs. If they agree within ±30%, the range is credible.
- If they diverge significantly, identify the assumption that drives the divergence and investigate it specifically
- Produce the final estimate as a range with the three methods displayed

**Day 9–10: Presentation and sensitivity analysis**
- Build the market sizing exhibit for the client deliverable (see below)
- Run a 1-variable sensitivity: "If the penetration rate is 25% rather than 35%, the market is $Y rather than $X" — this frames the uncertainty constructively for the investment committee

---

## The Market Sizing Exhibit

The standard commercial DD market sizing exhibit presents three things on one slide:

1. **The headline range** with the point estimate clearly identified: "We estimate the total addressable market at $1.1B–$1.5B, with a central estimate of $1.3B"

2. **The three-method triangulation** showing that the estimate is convergent across methods (not dependent on a single source)

3. **The key assumptions and their sources**, with a sensitivity showing the impact of the most uncertain assumption

**The intellectual honesty standard:** The market sizing exhibit must disclose the uncertainty, not hide it. An investment committee that receives a market sizing without a stated range or confidence interval will form their own estimate of the uncertainty — and they will assume it is higher than it is. Explicitly disclosing the range and the assumptions that drive it builds more credibility than presenting a false point estimate.

---

## Sanity Checks: The 5-Minute Tests

Before presenting any market size estimate, apply these sanity checks:

**The revenue share sanity check.** The target company's revenue divided by the estimated market size should produce a market share that is plausible given the competitive context. If the target has $50M revenue and the estimated market is $100M, the target has 50% market share — which would be remarkable and would need to be explicitly noted. If the estimated market is $50B, the target has 0.1% market share — which implies enormous whitespace or a market that is so broad as to be meaningless for investment purposes.

**The growth rate consistency check.** The market's implied CAGR over the stated period should be consistent with: (a) the target company's own revenue growth rate (a company growing at 30% should be in a market growing faster than 5%), and (b) the growth rates disclosed by public comparables.

**The revenue-per-buyer reasonableness check.** The average annual spend per buyer in the bottom-up build should be consistent with: (a) the target's own ACV; (b) publicly disclosed pricing for comparable products; (c) the expert's intuition about what a typical customer spends. If the implied spend per buyer is 5× the target's own ACV, the build contains an error.

**The "does anyone care?" check.** If the estimated TAM is below $500M for a deal being priced at $100M+, the market sizing is telling you something important about the growth ceiling. If the estimated TAM is $50B for a $50M ARR company with 3% market share, the market definition is probably too broad to be useful. Resize to the specific segment that the target actually competes in.

---

## Disclosing Uncertainty Professionally

The standard of commercial DD market sizing is not precision — it is defensibility. A range of $900M–$1.4B, derived from three converging methods and disclosed with explicit assumptions, is more credible than a point estimate of $1.1B derived from a single analyst report. Present uncertainty explicitly. The investment committee will respect the intellectual honesty, and it protects you from being held accountable for a false precision you never intended.

The language: "Our central estimate of $X is supported by three independent methods. The primary uncertainty is [specific assumption]. If [assumption] is at the low end of the range, the market is $Y; at the high end, $Z. We have used the central assumption of [value] based on [source]. This is a 90-day estimate — we recommend refreshing the market sizing with primary research if the deal advances to exclusivity."
