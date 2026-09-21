# Pricing Strategy: The Full Toolkit

Pricing is the highest-leverage lever in any P&L. A 1% improvement in price typically generates 3-5x more EBITDA impact than a 1% improvement in volume or a 1% reduction in variable costs. Yet it's systematically underinvested in most companies.

---

## The Three Pricing Approaches (and Their Limits)

**Cost-plus pricing:** Price = Cost × (1 + target margin). Simple, predictable, defensible internally. The problem: it's entirely inward-looking. It ignores what customers are willing to pay and what competitors charge. In competitive markets, cost-plus either over-prices (losing volume) or under-prices (leaving money on the table).

**Competitor-based pricing:** Price to win relative to alternatives. Useful when you're entering a market or when there's a clear reference price. The problem: it anchors you to competitors' pricing mistakes. If the market is collectively under-pricing, you under-price with it.

**Value-based pricing:** Price = share of the economic value you create for the customer. The theoretically correct approach. The problem: it requires you to understand customer value creation deeply, which most companies don't. When done well, it's the highest-margin pricing approach.

In practice, sophisticated pricing uses all three as inputs — value-based sets the ceiling, competitor-based establishes the reference range, cost-plus establishes the floor.

---

## Understanding Willingness to Pay

Willingness to pay (WTP) is the maximum price a customer will pay before choosing the next-best alternative. WTP varies by:
- Customer segment (enterprise vs. SMB vs. consumer)
- Use case (the value created in one application vs. another)
- Context (urgency, switching costs, alternatives)
- Relationship maturity

**How to measure WTP:**

*Van Westendorp Price Sensitivity Meter (best for new products/services):*
Survey customers with four questions:
1. At what price would this product feel too cheap (raising quality concerns)?
2. At what price would this product feel like a bargain?
3. At what price would this product feel expensive but still worth it?
4. At what price would this product feel too expensive to consider?

Plot the cumulative % curves for each response. Four intersections emerge:
- **Point of Marginal Cheapness (PMC):** Too cheap × Expensive curves intersect — lower bound of acceptable pricing
- **Point of Marginal Expensiveness (PME):** Too expensive × Cheap curves intersect — upper bound
- **Indifference Price Point (IPP):** Where Cheap × Expensive curves intersect — neutral point
- **Optimal Price Point (OPP):** Where Too Cheap × Too Expensive intersect — highest acceptance

The PMC-to-PME range is your acceptable price range. OPP is your anchor for initial pricing decisions.

*Conjoint analysis (best for established products with multiple attributes):*
Present customers with sets of product configurations (varying price, features, terms) and ask them to choose. Statistical analysis reveals the implicit weight customers place on each attribute including price. More sophisticated than Van Westendorp but requires larger sample and more setup.

*Direct competitive benchmarking:*
Map your price vs. competitor prices vs. the value differential. If you deliver 20% more value than Competitor A but price 5% below them, you're leaving significant money on the table.

---

## Economic Value to the Customer (EVC): A Worked Calculation

Stated willingness to pay tells you what customers *say*. EVC tells you what the product is *worth* to them: the price at which a rational customer is indifferent between your product and the next-best alternative, once every cost difference over an equal horizon is counted.

**EVC = reference price (next-best alternative, adjusted to equal life/output) + positive differentiation value (costs avoided, revenue gained) − negative differentiation value (switching cost, perceived risk)**

**Worked example [ILLUSTRATIVE]: a longer-life industrial conveyor belt.** The incumbent belt costs $10,000 and lasts 12 months. The new belt lasts 18 months and runs with lower friction. Each changeover costs the customer $8,000 ($6,000 of lost production during downtime plus $2,000 of labour). The lower friction saves $1,500 of energy a year. Switching means a one-off $3,000 trial and requalification. Compare over 36 months, the first horizon on which both belts complete whole lives:

```
Incumbent: 3 belts × ($10,000 + $8,000 changeover)            = $54,000
New:       2 belts × P + 2 × $8,000 − $4,500 energy + $3,000 switching
Indifference: 2P + $14,500 = $54,000                    →  P = $19,750 (EVC)

Per new belt:
  Life-adjusted reference: 1.5 × $10,000                        $15,000
  + Changeover avoided: $8,000 ÷ 2                             + $4,000
  + Energy saved: $4,500 ÷ 2                                   + $2,250
  − Switching cost: $3,000 ÷ 2                                 − $1,500
  EVC                                                           $19,750
  Differentiation value vs the $10,000 reference                 $9,750
```

**Setting the price inside the range.** Cost floor (unit cost $7,000) < reference ($10,000) < price < EVC ($19,750). Pricing *at* EVC leaves the customer no reason to switch. A new entrant typically captures 30–60% of the differentiation value. At **$15,000**, the supplier takes ~51% ($5,000 of the $9,750) and the customer saves $4,750 a belt, which is $9,500 (≈18%) off the 36-month total cost of $54,000. That saving is the sales story.

**Error fixed:** "The belt lasts 50% longer, so it is worth 50% more: $15,000" -> that is only the life-adjusted reference. Adding avoided changeovers, energy and switching cost gives an EVC of **$19,750**. (Candidates compare purchase prices instead of total cost over an equal horizon. The largest value is often avoided downtime, not the product.)

**Aha.** EVC differs by segment because the differentiation drivers do. A site that runs 24/7 loses far more per changeover than a single-shift site, so one list price either under-prices the first or prices the second out. Use the EVC drivers to set segment prices or value-based tiers.

**Trap.** Building EVC from the supplier's view of product benefits instead of the customer's P&L, and forgetting negative differentiation (switching cost, new-supplier risk). Also check that the claimed benefit exists in use. A "longer life" is worth nothing if the customer replaces the product on a fixed schedule anyway.

For a full B2B case with the three-lens triangulation, landed cost and channel margin, see Case 15 in `references/practice-cases-quantified.md`. For drill-length pricing cases, see Part C of `references/case-bank-worked.md`.

---

## The Price Waterfall

Most B2B companies don't know their real selling price. List price and pocket price are often 25-40% apart.

**Mapping the waterfall:**
Start with list price and identify every discount layer:
1. Contractual discounts (negotiated annually, by segment or account size)
2. Volume rebates (paid at end of period based on purchase volume)
3. Promotional discounts (time-limited promotions)
4. Payment term discounts (early payment incentives — 2/10 net 30 means 36% annualized)
5. Off-invoice allowances (marketing development funds, co-op advertising, training support)
6. Distributor/channel margins (if applicable)
7. Returns and credits

*Example for a B2B software company:*
- List price: $100k
- Contractual discount (-20%): -$20k
- Volume rebate (-5%): -$5k
- Early payment discount (-2%): -$1.6k
- Implementation absorbed (-8%): -$8k
- **Pocket price: $65.4k** (35% below list)

The analysis question: where is value leaking that could be recovered? Typical opportunities:
- **Discount rationalization:** Are discounts correlated with deal size, strategic value, or risk — or are they just salespeople negotiating? If there's no pattern, you're giving away margin arbitrarily.
- **Off-invoice allowances:** Often untracked and unrecovered. Map them and tie them to specific outcomes (co-op allowances paid against measurable marketing activity).
- **Payment term arbitrage:** 2% for early payment sounds small but at scale it adds up. Model the cost and see if it's worth paying.

---

## Price Architecture

Price architecture is the structure of your pricing — tiers, bundles, usage bases — distinct from price levels.

**Good/Better/Best (versioning):**
Three tiers (basic, standard, premium) anchored by the premium tier. Anchoring effect: most customers choose the middle tier, but the premium tier's existence makes the middle tier feel reasonable. The premium tier also captures high-willingness-to-pay customers who would have paid more for the standard.

Designing tiers: the Good tier should feel complete but limited. The Better tier should feel like the obvious default. The Best tier should feel aspirational but justified.

**Usage-based pricing:**
Price per transaction, per unit consumed, per API call, per active user. Aligns your revenue with the value customers receive — which means customers pay more when they get more value. Reduces adoption barrier (low commitment to start) but creates revenue variability.

Best fit: when customer value scales clearly with usage, and when there's a simple, auditable usage metric. SaaS companies increasingly move here from seat-based pricing.

**Outcome-based pricing:**
You charge based on results delivered, not inputs consumed. The highest form of value-based pricing. Also the hardest to implement — requires clear outcome measurement, attribution agreement, and risk tolerance on both sides.

Best fit: when outcomes are clearly measurable, attributable to your product/service, and significant enough to share economically.

**Bundle vs. unbundle:**
Bundling combines multiple offerings at a discount to list — increases perceived value, reduces price sensitivity, raises switching costs (they're using multiple products). Unbundling separates offerings so customers only buy what they need — lowers adoption barrier, can reveal willingness to pay by component, often used to match a lower-cost competitor.

---

## Scarcity and Auction Pricing

When supply is fixed and tiny and buyers' willingness to pay is wide and hard to observe, a posted price is a guess that is either too low (the seller forgoes surplus, and a resale market captures it) or too high (the product goes unsold). Auctions let buyers reveal what the product is worth. Typical cases are inaugural or limited-edition goods, landing slots, spectrum, prime real estate and one-off luxury experiences.

**Run the capacity and demand checks before choosing a mechanism.** Worked example [ILLUSTRATIVE]: a private operator flies a 10-seat luxury space round trip (3 premium, 7 standard seats). A flight takes 24 hours, followed by 48 hours of turnaround maintenance.

```
Capacity:  8,760 h ÷ (24 + 48) h           ≈ 121 flights/yr at most
Plan:      12 flights/yr                     → one flight per ~730 h (≈30 days);
           the binding constraint (launch windows, crew, licensing) must be stated
Posted-price anchor: 3 × $20M + 7 × $2M      = $74M per flight
           × 12 flights                      = $888M/yr; 36 premium + 84 standard seats
Cost floor: ($10M vehicle amortisation + $15M operating) ÷ 10 seats = $2.5M/seat average

Demand pool (premium): a $20M seat at ≤5% of net worth → ≥ $400M net worth
           ~6,000 such individuals × 3% interested and medically eligible ≈ 180 buyers
           at 36 seats/yr → ~5 years of demand; at 121 flights (363 seats/yr) → ~6 months
Demand pool (standard): $2M at ≤5% → ≥ $40M net worth; ~150,000 × 1% ≈ 1,500 buyers
           at 84 seats/yr → ~18 years
```

Demand, not turnaround, is the binding constraint for the premium class. Ration flights to protect scarcity. Note also the class economics: three premium seats at a $15M floor raise $45M, which is 1.8× the full flight cost. Standard seats then earn pure contribution, so their price should follow willingness to pay, not allocated cost.

**Mechanism design:**
- **Class-based tiers.** Auction only the class with few units and the widest spread in willingness to pay (premium seats, the inaugural flight, seat number one). Sell the deeper class at a posted price with deposits and a waitlist.
- **Ascending (open) auction.** Use it when bidders' values are interdependent, as with status goods, where each bidder's value rises with others' visible interest. Public bidding lifts the price and creates a published anchor for later posted prices. The winner pays roughly the second-highest valuation.
- **Sealed-bid (first-price) auction.** Use it when bidders want discretion, when a dominant bidder would deter others from entering an open auction, or when collusion is a risk. Risk-averse bidders bid closer to their true value in a first-price sealed auction.
- **The theory baseline.** With independent private values and risk-neutral bidders, formats yield the same expected revenue (revenue equivalence). Choose the format by which of those assumptions fails.
- **Reserve price.** Set it at the higher of the cost floor and the posted price you could otherwise get, never at cost alone. It matters most when bidders are few. With two serious bidders valuing a seat at $30M and $16M, an ascending auction clears at ~$16M. A $22M reserve lifts that to $22M (+$6M), at the risk of no sale if the top value falls below the reserve.
- **Several identical units.** A uniform price (all winners pay the highest losing bid) encourages truthful bidding. Pay-as-bid extracts more when bidders shade little but invites shading.

**Error fixed:** "At $10,000 an hour, saving two weeks of travel justifies a $15–25M seat" -> 2 weeks × 24 h × $10,000 = **$3.36M**, far below the price. (For a once-in-a-lifetime experience, time saved is the wrong value driver. Status, experience and scarcity drive willingness to pay, and the benchmarks, a ~$0.45M suborbital hop and a $50M+ multi-day orbital mission [ILLUSTRATIVE], frame it.)

**Error fixed:** "A $20M premium seat is half the $50M orbital benchmark" -> half is $25M; $20M is **40%**. And "24-hour flights with 48-hour turnaround allow about 12 flights a year" -> the turnaround allows ~**121**; 12 needs a stated constraint.

**Aha.** Scarcity pricing is a demand-pool problem, not a cost problem. Count the buyers who can afford the seat, divide by the seats sold a year, and ration supply so the queue lasts. Then let an auction find the top of the distribution.

**Trap.** Offering early-bird discounts on a product whose demand exceeds supply. That just transfers surplus to the first buyers. Use non-refundable deposits and prices that rise as seats fill.

---

## Access and Tiered Pricing in Emerging Markets

When the objective is broad access, typically for patented medicines, vaccines, seeds or essential technology in low- and middle-income markets, price is set by tier and channel, not by one global value calculation. The economics follow Ramsey logic: recover common costs such as R&D from the markets least sensitive to price (high-income), and price the most price-sensitive tiers towards marginal cost plus a contribution.

**Design the tiers:**
- **Segment by ability to pay** (income group, or GNI per capita bands), not by geography alone. Set the reference for each tier from what the payer buys today (e.g., the annual cost of the incumbent regimen).
- **Tier floor = marginal cost** (COGS + distribution). Anything above it contributes to R&D recovery, which is judged across all tiers over the remaining exclusivity window.
- **Channels.** Serve upper-middle-income markets through private branded sales. Serve lower-middle-income markets through government tenders, and low-income markets through donor-funded pooled procurement, often with multi-year volume commitments that de-risk uptake.
- **Voluntary licensing.** License generic makers to supply the lowest tier for a royalty. The originator gives up margin it would barely earn there, gains speed and volume, and removes the case for a compulsory licence.
- **Compulsory-licensing risk.** A government can authorise generic production without the patent holder's consent on public-health grounds. The incentive grows with the gap between the tender price and the generic cost. A licence in one market also sets a precedent and invites reference pricing in higher tiers.
- **Leakage controls.** Use differentiated packs, controlled distribution and confidential net prices, so low-tier product does not flow back into high-price markets and high-income payers do not reference low-tier prices.
- **Protection is territorial.** Exclusivity comes from patents and regulatory data protection filed in each market. The patent term runs from filing, not grant, so check the remaining years before fixing the recovery window.

**Worked tier check [ILLUSTRATIVE]: once-yearly patented therapy, marginal cost $4 per dose.**

```
Tier / channel                           Patients   Price    Contribution/yr
Upper-middle income, private branded       0.5M     $400     0.5M × $396 = $198M
Lower-middle income, government tender     3.0M     $40      3.0M × $36  = $108M
                                           (or)     $15      3.0M × $11  =  $33M
Low income, voluntary licence to generics 10.0M     $8 generic × 5% royalty = $4M

Compulsory-licence (CL) incentive in the tender tier (local generic supply at $6/dose):
  at $40: budget $120M vs $18M → government saves $102M/yr → P(CL) ≈ 60%
  at $15: budget  $45M vs $18M → saves $27M/yr            → P(CL) ≈ 10%
  If CL happens: tender contribution → 0, and precedent halves the private tier (−$99M)

Expected contribution/yr
  at $40: $198M − 60% × $99M + 40% × $108M + $4M = $185.8M
  at $15: $198M − 10% × $99M + 90% × $33M  + $4M = $221.8M   → $15 wins by $36M/yr
```

**Error fixed:** "Price the tender tier at $40 because it earns $108M against $33M at $15" -> **$15** maximises expected contribution across tiers ($221.8M vs $185.8M) once the compulsory-licence probability and its spillover to the private tier are priced in. (Candidates optimise each tier in isolation. The tiers are linked through licensing precedent and reference pricing.)

**Aha.** In access pricing the constraint is not willingness to pay but **policy tolerance**. The sustainable price in each tier is the highest one that does not trigger a compulsory licence, diversion or reference-pricing contagion. R&D is recovered from the portfolio of tiers, above all the high-income markets, not from each tier's own price.

**Trap.** Building one "emerging-market price" from R&D ÷ doses. That ignores marginal cost, the time value of money, the remaining patent life, uptake ramps, and the fact that tenders and donors, not patients, are the payers. For the full recovery-floor arithmetic (epidemiological funnel, discounted doses, tier cross-subsidy), see Case 14 in `references/practice-cases-quantified.md`.

---

## Pricing Execution: Where Margin Leaks in Sales

The best pricing strategy fails if sales doesn't execute it. The most common execution failures:

**Undisciplined discounting.** Sales reps offer discounts reactively (when the customer asks) rather than strategically (when it's necessary to close a deal that wouldn't otherwise close). Fix: implement a discount approval matrix — small discounts pre-approved, larger discounts require management sign-off. Track discount rate by rep and make it visible.

**No price discipline on renewals.** Acquiring new customers at better pricing than renewing existing ones. Fix: price increases on renewals should be planned and systematic — not a surprise to the customer, not an afterthought to the sales team.

**No value anchoring before price.** Salespeople discussing price before establishing value context. Fix: train sales to quantify economic value created before introducing price. "You'll save X hours per week across your 50 analysts at $Y per hour loaded cost — that's $Z per year. Our pricing is..." frames the conversation very differently.

**Ignoring competitive price response.** When a competitor drops price, the reflexive response is to match. Often this is wrong — price wars destroy value for everyone. Before matching, ask: Is this competitor move rational? Can they sustain it? What's our value differential that justifies our premium?

---

## Pricing Diagnostics: Where to Start

When diagnosing a pricing problem, run these analyses in sequence:

1. **Build the price waterfall** — understand realized vs. list price by segment and channel
2. **Analyze discount patterns** — correlation of discount depth with deal size, rep, segment, sales cycle length
3. **Compare realized price vs. value delivered** — are you capturing an appropriate share of value?
4. **Benchmark vs. competitors** — are you priced appropriately for your value positioning?
5. **Analyze price elasticity** — what happened to volume when you raised/lowered prices historically?
6. **Assess architecture fit** — is your pricing structure aligned with how customers derive value?

Most companies find their biggest opportunity in steps 2 and 3: margin leaking through undisciplined discounting, and systematic under-pricing relative to value delivered.
