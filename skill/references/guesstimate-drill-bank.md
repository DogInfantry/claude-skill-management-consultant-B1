# Guesstimate Drill Bank — Organised by Method, With the Classic Errors Fixed

Thirty-five worked guesstimates, grouped by the **sizing method** each one exercises (Parts A–D) or, for physical and geometric prompts, by the formula that constrains them (Part E), not by topic. Every drill shows the tree, the math, a sanity check against an outside anchor, and, where the "obvious" answer goes wrong, an **Error fixed** callout. Those callouts are the point of this file: most candidates lose guesstimates on a logic slip, not on arithmetic.

Companion to `references/guesstimation.md` (technique catalogue), `references/guesstimates-and-frameworks-quantified.md` (worked math, method decision box) and `references/india-guesstimates-and-cases.md` (India benchmark numbers). All figures are `[ILLUSTRATIVE]` structuring assumptions unless marked otherwise. Anchors marked *verify* are order-of-magnitude reference points to refresh before quoting.

---

## Part 0 — The four methods and when each wins

```
  METHOD                 START FROM                         REACH FOR IT WHEN
  ─────────────────      ────────────────────────────       ─────────────────────────────────────
  Top-down (demand)      Largest universe → filters          Consumer products, users, ownership
  Bottom-up              One replicable unit → scale up      Revenue of a site/store/route; B2B
  Supply / bottleneck    The constrained step in the flow    Queues, venues, runways, lanes, lifts,
                                                             anything with a physical ceiling
  Two-method reconcile   Run two of the above, compare       Always, if time allows — it is the
                                                             single strongest credibility signal
```

**The six-step routine (works for all four):**
1. **Clarify scope.** Clarify who, what unit, what time slice (per day? at 5 PM?), and stock vs. flow. Ask only for data you will use: a candidate who asks for a gender split and never applies it signals a checklist, not a plan.
2. **Say the method out loud** and why it fits.
3. **Draw the tree.** Keep each split MECE (age bands must not overlap; e.g. 0–18 / 19–45 / 46–60 / 60+).
4. **Assign round numbers and justify each one** in a phrase.
5. **Compute** in a tidy table and sanity-check each intermediate number, not just the final one.
6. **Reconcile** against an anchor or a second method, then state the one assumption the answer is most sensitive to.

**Bottleneck logic in one line:** output = min(demand, capacity). A food stall, a runway, a toll lane and a lift bank each have a hard ceiling. Size the ceiling first, then ask whether demand ever reaches it.

**Direction and lens are separate choices.** Top-down vs. bottom-up is the *direction* of the build; demand vs. supply is the *lens*. A bottom-up supply build (one toll lane, then the plaza) and a top-down demand build (population, then filters) are both legitimate. Pick one of each and say both out loud. Physical and geometric prompts (Part E) follow the same routine, with a formula instead of a population as the constraint.

**Capacity build (mini-card).** Use it for any plant, kitchen, clinic, assembly line or service counter.
```
  Production hours / month = working days × shifts × hours per shift
  Output / month           = production hours × parallel lines ÷ cycle time per unit (per line)
  Delivered output         = min(demand, capacity)
  Utilisation              = delivered ÷ capacity   → plan at ~80–85%, never 100%

  Example: 20 days × 2 shifts × 8 h           = 320 h/month
           320 h × 8 lines ÷ 2 h per car      = 1,280 cars/month → 15,360/yr
           Levers when demand > capacity, cheapest first:
           third shift (+50% output) → faster cycle time → new lines
```

**Segmentation menu (ranked by how often it earns its place).** Split only where the rate differs between segments. A split that applies the same rate to every branch adds arithmetic and no information.
1. **Demographic:** age bands, gender, income tier, household size. Data exists, so the rates are defensible.
2. **Usage intensity:** heavy / regular / light / non-user, each with its own rate. Weights must sum to 100%. Non-users belong *either* in an upstream filter *or* in a zero-rate tier, never both (see A10).
3. **Ownership and access:** owns vs. doesn't (replacement vs. first purchase), smartphone or internet access, shared vs. personal equipment (see A6).
4. **Geographic:** urban/rural, city tier, climate zone, dense core vs. the rest of the city (see C9).
5. **Attitudinal (psychographic):** use only when the prompt supplies data; otherwise it is a guess with a label on it.

**One base table per session.** Every India drill below draws from this table. Deriving "smartphone users" a different way in each of three estimates (825M in one, 960M in the next, 1B+ in a third) is an internal-consistency failure an interviewer will catch.
```
  Population          ~1.4B            Households        ~300M (÷ ~4.6); urban cities ÷ ~4
  Urban : rural       ~35 : 65         Income mix        ~10 / 40 / 50 high / middle / low
  Smartphone users    ~720M            Internet users    ~840M (~60%, verify)
  Ages 14–24          ~1.8% of population per year of age → ~20% for the 11-year band
```

---

## Part A — Top-down demand drills

### A1. Stock investors on a discount-broking app (~60M registered users)
```
  Users 60M
   ├─ 18–25 (40%) × 80% trade stocks = 19.2M
   ├─ 25–45 (40%) × 60%              = 14.4M
   └─ 45–60 (20%) × 40%              =  4.8M
                                       ─────
                     Stock investors ≈ 38.4M  (64% of base)
```
- **Sanity check.** 64% of *registered* users trading stocks is high. Registered is not active. Apply an active-user ratio of ~35% `[ILLUSTRATIVE]` and you get ≈ 13M active stock investors, which is the number a business would actually plan on.
- **Error fixed.** The original run collected a gender split (40M/20M) and never used it. Either use it, e.g. if risk appetite differs by gender, or don't ask for it.
- **Trap.** Buckets that skip ages (no <18, no 60+) are not collectively exhaustive. State the exclusions explicitly ("minors can't self-trade; 60+ is negligible on this app").

### A2. Laptops sold per day to consumers in a ~30M metro
**The original answer, ~10,000/day.** 30M × 70% working-age × 70% (excluding the lowest income band) = 14.7M. Of those, 30% don't own a laptop (4.41M) and 80% of them prefer a laptop, giving 3.53M. Divided by 365, that is ≈ 9,700/day.

**Error fixed.** Two logic errors:
1. It assumes **every non-owner buys within one year**.
2. It **ignores replacement demand** from the 70% who already own one, which is the bigger flow in any durable-goods market.

Sanity check: ~3.5M/yr is on the order of a quarter of all PCs sold nationally (~14M/yr, *verify*), in a city holding ~2% of the population. It fails.

```
  Target adults 14.7M
   ├─ Own a laptop 25%  = 3.68M installed ÷ 5-yr life   = 0.74M/yr replacement
   └─ Don't own    75%  = 11.0M × 2%/yr first purchase  = 0.22M/yr new
                                                          ─────────
                                          Annual ≈ 0.96M → ≈ 2,600/day
```
**Pattern:** installed base ÷ life + net adds. It is the same engine used for two-wheelers in `india-guesstimates-and-cases.md`.

### A3. Credit-card holders (and cards) in a ~20M metro
**Error fixed (three slips in the original).**
1. It split an almost fully urban capital **40/60 urban/rural** (real ≈ 97% urban). It then silently used a different base (18M × 60%) without saying why.
2. It reported **6.48M "unique holders"**, but that figure counted *cards*: upper-class members were counted twice for their second card. The same inputs give **≈ 4.9M holders**.
3. Its summary diagram used a third split (30/70). **Keep one set of numbers.**

```
  Pop 20M × 97% urban × 62% aged 18–65          = 12.0M adults
   ├─ Upper  15% = 1.80M × 90% hold = 1.62M holders × 2.5 cards = 4.06M cards
   ├─ Middle 40% = 4.81M × 35% hold = 1.68M holders × 1.3 cards = 2.19M cards
   └─ Lower  45% = 5.41M ×  5% hold = 0.27M holders × 1.0 card  = 0.27M cards
                                       ─────────────               ────────────
                                Holders ≈ 3.6M                Cards ≈ 6.5M
```
- **Anchor.** Roughly 100M+ cards are in force nationally (*verify*). A wealthy metro carrying 5–7% of them gives 5–7M cards ✓.
- **Aha.** "Holders" and "cards" are different questions. Say which one you are answering in the first 20 seconds.

### A4. Ride-hail car rides per weekday in a tier-2 city (~1.5M people)
**The original answer, ~100,000/day.** 1.5M × 70% upper/middle × 80% smartphone × 30% use cab apps × 40% platform share = 100.8k users. It then assumed **each rides once every day**.

**Error fixed.** Tier-2 cab-app users ride a few times a *month*. The original supply cross-check also divided rides by "2 passengers per trip", but rides are trips. That produced a fleet of ~4,600 cars, which should itself have been a red flag.

```
  1.5M × 45% upper+middle (tier-2 mix) × 80% smartphone × 20% cab-app users
       = 108k × 40% platform share = 43.2k users
       × 4 rides/month ÷ 30                              ≈ 5,800 rides/day
  Supply check: 5,800 ÷ ~11 trips per car-day           ≈ 520 active cars ✓ plausible
```
**Most sensitive assumption:** ride frequency. Say so.

### A5. Cricket balls in the air at 5 PM on a Saturday (~20M metro)
**The original answer, ~32,000.** It started from 20M × 30% "urban", then 40% aged 6–25, giving 2.4M. It then took **80% "because most games are in the evening"**, giving 1.92M players, divided by 10 players per team to get 192k balls, and assumed each ball is airborne 1/6 of the time.

**Error fixed (three compounding slips).**
1. The metro is ~97% urban, not 30%.
2. "80% of games happen in the evening" does not mean "80% of young people are playing at 5 PM". You need *participation on that day* first.
3. A game has **two** teams sharing **one** ball, and a ball is airborne for ~2 seconds of a ~40-second delivery cycle, not 10 minutes an hour.

```
  20M × 97% × 35% aged 6–25                  = 6.79M
   × 10% play cricket that Saturday          = 679k
   × 30% of them are mid-game at 5 PM         = 204k players
   ÷ 16 players per informal game             = 12.7k balls in play
   × 5% of the time airborne                  ≈ 640 balls in the air
```
**Aha.** "At an instant" prompts are **time-slice** problems: (units in use) × (fraction of time in the state asked about). The original answer was ~50× too high because each slip multiplied the one before it.

### A6. Cricket bats sold per day in India
```
  1.4B × 50% aged 5–40                               = 700M
   ├─ Male   350M × 60% play at least occasionally   = 210M
   └─ Female 350M × 10%                              =  35M
                                                       ─────
                                           Players ≈ 245M
  Segment       Players  ÷ players per bat  = bats in use  ÷ life  = bats/yr
  Casual  70%   171.5M   ÷ 10 (street game) = 17.2M        ÷ 3 yr  =  5.7M
  Regular 25%    61.3M   ÷ 4  (colony/club) = 15.3M        ÷ 2 yr  =  7.7M
  Serious  5%    12.3M   ÷ 1  (own bat)     = 12.3M        ÷ 1 yr  = 12.3M
                                                                     ─────
                                              ≈ 25.6M/yr → ≈ 70,000 bats/day
```
- **Error fixed.** The tempting build treats every player as owning a bat: ~245M players replacing every one to three years gives ~122.5M bats a year (~3.4 lakh a day). Informal cricket shares one bat across a whole game, so *bats in use*, not players, drive replacement, and the answer falls ~5×. The same build applies one participation rate to both genders; split it, because the rates differ ~6×.
- **Sanity check.** ~26M bats a year is one bat per ~12 households a year. Cheap plastic and tennis-ball bats for children carry most of the volume. A value estimate needs a willow vs. plastic split, because prices differ ~10×.
- **Aha.** Shared equipment: users ÷ sharing ratio = units in use; units in use ÷ life = annual sales. The same step applies to footballs, carrom boards and any household-shared durable.
- **Trap.** Calling this top-down. It starts top-down but the engine is a stock/replacement cycle; say both.

### A7. Petrol consumed per day by private vehicles in a ~15M north-Indian capital
```
  15M ÷ 4 per urban household = 3.75M households
  Tier          Share   Households  2W/HH  Cars/HH   Two-wheelers   Cars
  Upper           5%     0.19M      1.0    1.5       0.19M          0.28M
  Upper-middle   25%     0.94M      1.0    0.6       0.94M          0.56M
  Lower-middle   50%     1.88M      0.8    0.1       1.50M          0.19M
  Lower          20%     0.75M      0.2    0         0.15M          0
                                                     ─────          ─────
                                                     2.78M          1.03M   (2W ≈ 73% of fleet ✓)
  2W:   2.78M × 20 km/day ÷ 50 km/l                         = 1.11M l  (≈ all petrol)
  Cars: 1.03M × 25 km/day ÷ 12.5 km/l = 2.06M l × 65% petrol = 1.34M l  (rest diesel/CNG)
                                                              ────────
                                           Private petrol ≈ 2.45M litres/day
```
- **Error fixed.** The tempting tree gives lower-middle households 0.75 cars each, which yields more cars (2.55M) than two-wheelers (1.73M), then takes a 20% diesel haircut off the whole total, two-wheelers included. Two-wheelers are roughly three-quarters of an Indian city's private fleet and run almost entirely on petrol, so apply the diesel/CNG cut to cars only. Its answer (≈ 4.6M l/day) can still land near a city-sales anchor, because an inverted fleet mix is offset by low car mileage (10 km/l). Also use ~4 people per urban household (Part 0 table), not 5.
- **Sanity check.** 2.45M l ÷ ~400 pumps (C4's scale for a city this size) ≈ 6,100 l per pump per day, a plausible urban forecourt (verify). City-wide sales also include taxis, commercial vehicles and cars from neighbouring towns, so the private figure must sit *below* total city sales.
- **Aha.** Sanity-check the intermediates (here the two-wheeler : car mix), not just the final number. A right total built on a wrong middle does not survive the first follow-up question.

### A8. Air-conditioner working hours in a ~15M north-Indian city
**Clarify the unit first.** "Average AC working hours" asks for hours *per AC* (a year or a day), not the city-wide total. Compute the per-AC figure; the total is a by-product.
```
  Calendar (must sum to 365):
   Peak summer   Apr–Jun   30+31+30      =  91 days × 10 h =   910 h
   Shoulder      Mar, Jul  31+31         =  62 days ×  5 h =   310 h
   Humid/autumn  Aug–Oct   31+30+31      =  92 days ×  3 h =   276 h
   Winter        Nov–Feb   30+31+31+28   = 120 days ×  0 h =     0 h
                                           ────────          ───────
                                           365 days          1,496 h per AC per year
                                                             ≈ 4.1 h/day averaged over the year
  Peak-day profile: afternoon 3 h + evening 2 h + night 5 h = 10 h
  City total (by-product): 3.75M HH × 30% own × 1.5 ACs = 1.69M ACs × 1,496 h ≈ 2.5B AC-hours/yr
```
- **Error fixed (three slips).** 1) Counting Aug–Oct as 91 days (it is 92), so the seasons sum to 364; check that the calendar sums to 365 before multiplying. 2) Reporting a city-wide total (~1.2B hours) when the question asks for an average. 3) One blended "summer" from March to July with more morning than afternoon use. Split peak from shoulder months: the three peak months carry ~60% of the hours.
- **Sanity check.** ~1,500 h × ~1.3 kW `[ILLUSTRATIVE]` ≈ 1,950 kWh a year per AC, consistent with cooling being the dominant summer load of an AC-owning urban home (verify).
- **Trap.** Capping ownership at one AC per household understates upper-income homes. That moves the city total, not the per-AC average; say which answer an assumption affects.

### A9. India SUV tyre market (units and value)
```
  Stock (parc):
   High-income HH  30M × 40% own an SUV × 1.2 per owning HH  = 14.4M
   Middle HH      120M ×  3%            × 1.0                =  3.6M
                                                               ─────
                                                   SUV parc ≈ 18M   (verify: ~15–20M)
  Flow: new SUVs/yr = replacement 18M ÷ 15-yr life (1.2M) + net adds 10% × 18M (1.8M) = 3.0M
  OEM tyres         = 3.0M new SUVs × 5 (four + spare)                        = 15.0M
  Replacement tyres = 18M parc × 4 (spares rarely replaced) ÷ 5-yr tyre life  = 14.4M
                                                                                ─────
                                                         Tyres ≈ 29.4M units/yr
  Value: 15.0M × ₹6,000 (OEM) + 14.4M × ₹8,000 (replacement) ≈ ₹9,000 cr + ₹11,520 cr ≈ ₹20,500 cr/yr
```
- **Error fixed (three slips).** 1) **Stock + flow added:** "parc 42M + 2.8M replacements = 44.8M". Replacement units swap out old SUVs; they do not add to the parc. New-SUV sales = replacement + net adds. 2) The stated assumptions exclude replacement tyres, yet the final step (fleet tyres ÷ tyre life) *is* replacement demand, and OEM fitment is dropped. Multiplying by 5 tyres and dividing by a 5-year life cancel, so the "tyre market" silently equals the SUV count. 3) A parc built as 10% of all households owning ~1.4 SUVs each (42M) is 2–3× the real fleet; household car ownership nationally is below 10%. On that inflated base the correct flow math gives ~69M tyres (35M OEM + 33.6M replacement), so the method and the base both have to be fixed.
- **Sanity check.** 3.0M new SUVs a year sits in the range of national SUV sales (verify). "Size of the industry" wants a rupee figure as well as units; give both.
- **Aha.** Any consumable market = OEM fitment on the new-unit **flow** + replacement on the installed **stock** ÷ consumable life. Two engines, and neither is added to the stock.

### A10. Ketchup and tomato-sauce retail revenue in Europe
**Clarify.** Narrow "sauce" to ketchup/tomato sauce by asking, not assuming. Retail value at consumer prices; ~750M people.
```
  750M ÷ 2.3 per household                          = 326M households
  Tier (share of ALL households)    500 g bottles/month
   Heavy     20%                    1.5              = 0.30
   Moderate  40%                    0.75             = 0.30
   Light     20%                    0.25             = 0.05
   Non-user  20%                    0                = 0
                                                       ────
                              Average per household  = 0.65 bottles/month
  Volume = 326M × 0.65 × 12 × 0.5 kg                 ≈ 1.27M tonnes/yr (≈ 1.7 kg per person)
  Price  = 60% branded × €5/kg + 40% private label × €2/kg = €3.8/kg
  Retail value ≈ 1,272M kg × €3.8                    ≈ €4.8B/yr
```
- **Error fixed.** The tempting build filters twice: "80% of households buy sauce", then multiplies those buyers by a tier average that already contains a 20% zero-rate non-user tier (and rounds it up). Each exclusion must live in exactly one place: all 326M households × 0.65, *or* the 261M buyers × 0.8125 (0.65 ÷ 0.8). Both give ~212M bottles a month; the double filter gives ~170M, 20% short. A household size of 3 instead of ~2.3 cuts the household count by another ~23%.
- **Sanity check.** ~1.7 kg per person a year is plausible for a continent where ketchup is a staple condiment in the north and west and a minor one in the south (verify per-capita data before quoting).
- **Aha.** Usage-intensity tiers and an upstream buyer filter are two ways of making the same exclusion. Pick one.

### A11. T-shirts sold per day by a leading online marketplace (India)
```
  Internet users 840M × 50% shop online × 30% buy fashion online = 126M shoppers
  T-shirts per shopper per year, all channels:
   frequent 20% × 8 + occasional 80% × 3                          = 4.0
  × 50% of those bought online (the rest in stores and markets)   = 2.0 online
  126M × 2.0                                                      = 252M online T-shirts/yr
  × 25% share for the leading marketplace                         = 63M/yr ≈ 173,000/day
```
- **Error fixed.** The tempting tree assumes every T-shirt an online fashion shopper buys is bought online. These shoppers still buy most basics offline; without a channel split the answer doubles. It also gives women more T-shirts than men with no stated reason. Split by gender only when the rates actually differ.
- **Sanity check.** At ~2 T-shirts per person a year nationally (~2.8B), 252M online units is ~9%, in line with online's share of apparel (verify). The marketplace share is the swing assumption: fashion-specialist platforms lead this category, so a generalist's share may be lower.

### A12. India sports-shoe market (pairs and rupees)
**Clarify the unit.** "How many sports shoes are sold" wants pairs a year. Compute pairs first, then value.
```
  Filters (weighted averages, multiplied as if independent; say so):
   Location: rural 65% × 70% availability + urban 35% × 100%       = 80.5%
   Gender:   male 50% × 80% + female 50% × 30%                     = 55.0%
   Age:      <15 25%×40% + 15–30 25%×80% + 30–45 20%×60%
             + 45–60 20%×40% + 60+ 10%×2%
             = 10% + 20% + 12% + 8% + 0.2%                         = 50.2%
  Wearers = 1.4B × 0.805 × 0.55 × 0.502                            ≈ 311M
  × 0.8 pairs per wearer per year (a pair lasts ~15 months)        ≈ 249M pairs/yr
  Value: 60% × ₹500 + 30% × ₹1,200 + 10% × ₹3,000 = ₹960 a pair   → ≈ ₹23,900 cr/yr
```
- **Error fixed.** The age filter's weighted average is 50.2%, not the "≈ 60%" an eyeball gives; sum the products, never guess the blend. At 60% the wearer base is ~20% too high. Two further slips: answering in rupees when the question asks for pairs, and assuming every wearer buys exactly one pair a year (a stock treated as a flow).
- **Sanity check.** National footwear consumption is ~2.5–3B pairs a year (verify); ~250M sports pairs is ~9% of it, a plausible share.

### A13. AI-assistant prompts per day at a ~1,400-student business school
**Clarify.** A typical teaching day, not placement or exam week. All AI tools, or one assistant?
```
  1,400 students × 90% daily active              = 1,260
   ├─ Power   20% = 252 × 25 prompts             =  6,300
   ├─ Regular 50% = 630 × 10                     =  6,300
   └─ Casual  30% = 378 ×  5                     =  1,890
                                                   ──────
                          All AI tools           ≈ 14,490 prompts/day
  × 60% share for the leading assistant           ≈  8,700 prompts/day
```
- **Error fixed.** Applying a 60% share is valid only if the per-student rates count prompts to *all* AI tools. If the tiers were built as "prompts to the leading assistant", taking 60% again double-applies the share and understates by 40%. Label every rate with its unit.
- **Sanity check.** 14,490 ÷ 1,260 ≈ 11.5 prompts per active student a day, two or three short working sessions. Plausible.
- **Aha.** In a usage-intensity split the heavy tier carries the volume: 20% of users generate ~43% of prompts. The power-user rate is the swing assumption.

### A14. Short videos created per day on a dominant short-video app (India)
```
  Smartphone users 720M (Part 0 table) × 60% on the app  = 432M
  × 70% daily active                                      = 302M DAU
  × 5% creators (post at least weekly)                    = 15.1M
  × 0.5 videos per creator per day (~3.5 a week)          ≈ 7.6M videos/day
```
- **Error fixed (two slips).** 1) Defining a creator as someone who posts "at least one video a day" and then assigning 0.5 videos a day is self-contradictory. Define creators as weekly posters (as here), or use a rate of at least 1. 2) Rebuilding the smartphone base inside the drill (1.5B × 55% ≈ 825M, then rounded to 800M) when another estimate in the same session used 960M. Take the base from the Part 0 table.
- **Sanity check.** 7.6M ÷ 302M ≈ 2.5% of daily users post on a given day, consistent with the rule of thumb that a low single-digit share of users create and the rest watch.
- **Trap.** Calling this "supply side". Counting creators is still a top-down user build; a supply build would start from upload or moderation capacity.

### A15. Messages sent per day on the dominant messaging app (India)
```
  Smartphone users 720M × 75% active on the app            = 540M users (15+)
  Messages sent per user per day (high / medium / low intensity):
   15–40 (70%): 60 / 30 / 20 msgs at 60 / 25 / 15% of users  = 46.5
   40–60 (20%): 30 / 20 / 10      at 30 / 40 / 30%           = 20.0
   60+   (10%): 25 / 15 /  5      at 10 / 30 / 60%           = 10.0
  Weighted: 0.7 × 46.5 + 0.2 × 20 + 0.1 × 10                 = 37.55
  540M × 37.55                                               ≈ 20B messages sent/day
```
- **Error fixed (two slips).** 1) **Base:** building users from households (a middle-class household of five owning four smartphones) gives 960M, then assumes all of them use the app and are 15+, about 90% of the 15+ population. Use the Part 0 table and an app-penetration filter. 2) **Arithmetic:** 960M × 37.55 = 36,048M, not 36,481M (a transposition). Say each product out loud.
- **Sanity check.** ~20B a day from ~540M users is plausible against global volumes on the order of 100B messages a day (verify), for the app's largest national user base.
- **Aha.** Name the unit: a group message counts once when *sent* and many times when *received*. The two answers differ by the average group size.

### A16. Study hours lost per day to a social-media app among Indian students
```
  Ages 14–24: 1.4B × 20% (Part 0 table)                            = 280M
   ├─ 14–18 (5 of 11 cohorts, ~45%) = 126M × 70% in school          = 88.2M
   │    × 60% smartphone access × 50% on the app = 26.5M × 0.5 h     = 13.2M h
   └─ 19–24 (6 of 11, ~55%) = 154M × 28% enrolled (GER, verify)     = 43.1M
        × 90% smartphone × 85% on the app = 33.0M × 0.8 h            = 26.4M h
                                                                       ──────
                                        Student time on the app ≈ 39.6M h/day
  × 50% of app time that actually displaces study                  ≈ 20M study hours lost/day
```
- **Error fixed (three slips).** 1) A 60/40 school/college split of the 14–24 band; count single-year cohorts instead: 14–18 is 5 of 11 (~45%), 19–24 is 6 of 11. 2) A 50% higher-education enrolment rate against a national gross enrolment ratio of ~28%, which overstates college students ~1.8×. 3) Treating every app minute as a study minute lost, when much of it displaces other leisure.
- **Sensitivity.** Displacement is the swing assumption: one-third to two-thirds gives ≈ 13–26M hours a day.
- **Aha.** The question asks for hours *lost*, not hours *spent*. The last filter (displacement) is the one the prompt is actually about.

---

## Part B — Ratio / benchmark drills

### B1. Daily revenue of a budget-hotel aggregator in a ~20M metro
```
  Rooms   = 20M ÷ 400 people per room          = 50,000
  × aggregator share 30%                        = 15,000 rooms
  × occupancy 60%                               =  9,000 room-nights/day
  × ₹1,500 average tariff                       = ₹1.35 cr GMV/day
  × 20% take rate                               = ₹27 lakh/day  (≈ ₹99 cr/yr)
```
- **Why it works.** "People per hotel room" is a benchmark ratio that replaces a whole demand tree. State where the ratio comes from: a capital city with heavy transit and business travel has more rooms per head.
- **Upgrade.** Cross-check from demand: (visitors/day × nights) ÷ occupancy should land near 50k rooms.
- **Trap.** Quoting GMV as revenue. The aggregator earns the take, not the tariff.

### B2. Charter-plane takeoffs per day from a major western-Indian metro airport
**The tempting route, ~27/day.** 150 airports × 1.2 runways × 100 flights per runway per day = 18,000 flights nationally; × 2% charter × 15% city share × 50% takeoffs ≈ 27.

**Error fixed.** 100 movements per runway per day is busy-hub *capacity* applied to every airport; national traffic is closer to ~8,000 movements a day (verify). It is C3's slip, capacity used as demand, and the answer looks plausible only because the unverifiable 2% and 15% happen to offset it. Define the unit too: a movement is a takeoff *or* a landing, so takeoffs = movements ÷ 2.

```
  Ratio route:  this airport's movements ~950/day (verify)
                × 4% non-scheduled (charter + business aviation)  = 38 movements
                ÷ 2 (takeoffs only)                               ≈ 19 takeoffs/day
  Fleet check:  ~100 non-scheduled aircraft based in the region
                × ~70 departures from base per aircraft per year ÷ 365 ≈ 19/day ✓
```
- **Answer.** ≈ 14–24 takeoffs a day across a 3–5% non-scheduled share `[ILLUSTRATIVE]`. Visiting aircraft flying out push toward the top of the range.
- **Aha.** A ratio off the one number you can anchor (this airport's daily movements) beats a national tree built from infrastructure. Use the narrowest reliable anchor.

---

## Part C — Supply / bottleneck drills

### C1. How many lifts for a 20-storey residential tower?
Setup: 8 flats per floor × 4 people = 640 residents. Floors 1–2 take the stairs, leaving 576 lift users. 40% of them travel in the rush (school + office), which is ≈ 230 people.

**Error fixed.** The original divided 230 by a 15-person car, got "16 lifts in a single trip", then cut to 6. But by its own math, 6 lifts × 15 × 30 trips/hr = 2,700 people/hr, against 230 people. **One lift** (450/hr) would already clear the hour. The recommendation contradicted the calculation. The real design constraint is the **busiest 5 minutes** and **waiting time**, not the hour.

```
  Rush-hour users 230, bunched: busiest 5 min ≈ 25%       ≈ 58 people
  Round trip with ~6 stops over 18 floors ≈ 3 min → 1.67 trips per 5 min
  Load 80% of 15 = 12 per trip → 20 people per car per 5 min
  Cars needed = 58 ÷ 20 ≈ 2.9 → 3 passenger lifts
  + 1 service/stretcher lift for redundancy & maintenance → 4 lifts
```
**Aha.** Capacity questions are sized on the **peak within the peak** plus a service-level target (e.g. wait < 60 s), with N+1 redundancy. Average hourly throughput always makes the system look oversized.

### C2. Daily car revenue at a single toll lane
```
  Peak    8 h × 60 min × 3 cars/min   × ₹120 = ₹1,72,800
  Normal 10 h × 60 min × 1 car/min    × ₹120 = ₹  72,000
  Night   6 h × 60 min × 0.3 car/min  × ₹120 = ₹  12,960
                                               ──────────
                                  Per lane/day ≈ ₹2.6 lakh
```
- **Error fixed.** The original treated all 16 off-peak hours at the daytime rate (₹2.88 lakh). Night traffic is a fraction of that. Split the day into at least three bands.
- **Bottleneck check.** An electronic-toll lane clears roughly 5–6 cars/min at best `[ILLUSTRATIVE]`. At 3/min the lane is ~50–60% utilised, so revenue is **demand-bound**, not capacity-bound. That changes the advice: adding lanes won't raise revenue.
- **Scale-up.** For a real plaza, multiply by the lanes carrying cars, then net out monthly passes and exempt vehicles.

### C3. Passengers leaving the country by air on a given day
**The original answer, 672,000/day.** 30 international airports × 80 international departures each × 280 passengers.

**Error fixed.** "One departure every 15 minutes for 20 hours" describes **runway capacity**, not **international demand**. Only the two mega-hubs run anywhere near that. Against the anchor, the answer is ~7× too high.

```
  2 mega-hubs     × 80 intl departures/day = 160
  5 large metros  × 25                     = 125
  ~20 others      ×  4                     =  80
                                           ─────
  365 departures × 220 avg seats × 85% load  ≈ 68,000 passengers/day
  Anchor: ~35M outbound international passengers/yr (verify) ≈ 96,000/day
  → same order of magnitude; the gap says hub frequency is understated. Refine upward.
```
**Aha.** Never size demand from infrastructure capacity. Capacity is the *ceiling* in a min(demand, capacity) check, not the answer.

### C4. Petrol pumps in a ~20M metro (city limits)
```
  5M households: high 10% × 2 veh = 1.0M · middle 60% × 1 = 3.0M · low 30% × 0.2 = 0.3M
  Vehicles 4.3M × 70% petrol = 3.0M → weekly fill → 430,000 fills/day
  Pump throughput: 8 nozzles × 10 fills/hr × 18 hr = 1,440/day at 100%
  Pumps = 430k ÷ 1,440 ≈ 300 (full)   |   ÷ (1,440 × 60%) ≈ 500 (realistic)
```
- **Error fixed.** The original quoted "10 stations × 10 nozzles × 15 vehicles/hr × 10 hr", which is 15,000/day, then used 1,500. Write the throughput product out loud; that one habit catches slips like this.
- **Answer.** A range of 300–500, with utilisation as the swing assumption. Two-wheelers fill more often but in smaller amounts, which roughly offsets.

### C5. Tourist boats at a busy riverfront landing in a tier-2 pilgrimage city
```
  City 1.5M × 10% visit the riverfront each evening × 1.3 tourist uplift ≈ 200k visitors
  ~100 landings: 10 high-activity take 33% → ≈ 6,600 visitors per busy landing
  × 30% take a boat ride = ~2,000 riders
  Boat turnover = 5 seats × 6 trips per evening = 30 riders/boat
  Boats ≈ 2,000 ÷ 30 ≈ 66
```
- **Method.** Peak-demand sizing with demand = supply at peak. Boats = peak riders ÷ (capacity × turns).
- **Sensitivity.** A 10% nightly visitation rate is aggressive; at 3% the answer drops to ~20 boats. Larger motorboats (10–20 seats) cut the count further. Give a range, not a point.

### C6. Cars per day on an 8-lane tolled sea bridge
**Clarify.** Vehicle crossings or unique cars? Are two-wheelers allowed (often not on sea bridges)? Cash or electronic tolling?
```
  Ceiling: 8 toll lanes × 5 cars/min × 60            = 2,400 cars/hour
  Load bands as UTILISATION of that ceiling (never above 100%):
   Peak    6 h × 2,400 × 100%                         = 14,400
   Day    12 h × 2,400 ×  60%                         = 17,280
   Night   6 h × 2,400 ×  20%                         =  2,880
                                                        ──────
                                   Crossings/day     ≈ 34,600
  Unique cars: 70% of crossings are return commuters (2 crossings each)
   = 0.7 × 34,560 ÷ 2 + 0.3 × 34,560                  ≈ 22,500 cars
```
- **Error fixed.** The tempting build names the toll plaza as the bottleneck, then sets peak load at "2× capacity" (28,800 in 6 hours). A bottleneck cannot pass more than its ceiling, so peak is at most 14,400. The tell: its total (64,800 = 0.5×, 1× and 2× bands) exceeds the 24-hour ceiling of 2,400 × 24 = 57,600. Express every band as a utilisation of capacity.
- **Re-run the bottleneck if tolling is electronic.** A tag lane clears roughly twice as many cars, so recompute the ceiling and check whether the carriageway (~1,800 cars per lane-hour) or peak demand now binds.
- **Aha.** "Multiplier" and "utilisation" are different words for a reason. Once you have named a ceiling, every band is a fraction of it.

### C7. A capital city's metro: daily ridership (snapshot vs. daily flow)
Setup, busiest line: 90-minute end-to-end run; 8 coaches × 150 per coach; 20 operating hours; 8 rush hours at a 2-minute headway, 12 other hours at 5 minutes.
```
  Runs per direction = 8 h × 30/h + 12 h × 12/h           = 384 → 768 runs/day both ways
  Effective headway  = 1,200 min ÷ 384                     = 3.125 min
  Trains on track    = 90 ÷ 3.125 × 2 directions           ≈ 58
  Riders aboard      = 58 × 8 × 150 × 60% all-day load     ≈ 41,500   ← a SNAPSHOT
  Daily flow = riders aboard × (operating minutes ÷ average ride time)
             = 41,472 × (1,200 ÷ 36 min)                   ≈ 1.4M journeys/day on this line
  Check by runs: 768 runs × 720 aboard × 2.5 turnovers per run (90 ÷ 36) = 1.38M ✓
  Network: 10 lines, average line ≈ 40% of the busiest → 10 × 0.4 × 1.38M ≈ 5.5M/day
```
- **Error fixed (two slips).** 1) The tempting build multiplies trains on the track by riders per train (≈ 45,000) and calls it daily ridership. That is how many people are aboard *at one instant*. It lists 20 operating hours and 40 stations and never uses either, the tell of a missing time dimension. 2) It averages headways ((8 × 2 + 12 × 5) ÷ 20 = 3.8 min) instead of frequencies (3.125 min), which undercounts trains by ~18%. Its network answer, ~4.5 lakh a day, is ~12× low.
- **Sanity check.** Large capital-city metro networks carry on the order of 5–7M journeys a day (verify) ✓. Line boardings exceed journeys because an interchange counts on two lines; say which you are counting.
- **Aha.** Snapshot → flow is Little's law: throughput = number in the system ÷ time each unit spends in it. It is A5 run in reverse: A5 turns a daily flow into "balls in the air"; this turns "riders aboard" into riders per day.

### C8. Ride-hail trips after a sold-out stadium concert
Setup: ~60,000 attendees (a 50,000-seat stadium plus ~10,000 standing on the field), a ~90-minute egress window, late at night.
```
  Demand
   60,000 × 45% want a cab (public transport thins late; inbound cab share was ~35%)
        = 27,000 people ÷ 2.5 per car                 = 10,800 car trips
        × 50% platform share                          =  5,400 trips requested
  Supply (the binding side)
   Cars within reach at the end + cars pulled in by surge ≈ 2,500 + 1,500 = 4,000
  Trips in the window = min(5,400, 4,000)             ≈ 4,000
  Kerb check: 4,000 ÷ 90 min ≈ 44 pickups/min → ~22 bays each loading a car every 30 s
```
- **Error fixed.** The tempting build takes inbound cab rides, adds 20%, applies platform share and then an "80% of bookings succeed" haircut (≈ 3,360), with no supply check. Failed bookings retry, so a flat success rate is not the limit; the cars that can reach the venue are. The late-night shift should also move *people* from public transport to cabs, not inflate rides by a flat 20%.
- **So what.** The ~1,400 unmet trips spill into the next hour or to other modes. That is the case for a designated pickup zone and pre-positioned supply.
- **Aha.** Event egress = attendance × mode split ÷ occupancy × platform share, capped by min(demand, reachable supply) and by the kerb's loading rate.

### C9. Micro-warehouses for 15-minute delivery in a ~30M capital region
Setup: 15 minutes = 3 pick + 2 rider assignment + 10 transit. At 15 km/h a rider covers 2.5 km in a straight line (≈ 20 km²), but roads wind (circuity ~1.3), so the effective radius is ≈ 1.9 km and each store covers π × 1.92² ≈ 11.6 km².
```
  One boundary for population AND area: ~30M over a ~2,500 km² served urban footprint
  Orders: 7.5M households × 5% order on a given day = 375k orders/day
  Zone         Area       Orders       Coverage need      Capacity need (÷ 2,500/store)  Stores = max
  Dense core     500 km²  60% = 225k     500 ÷ 11.6 ≈ 43  225k ÷ 2,500 = 90              90 (capacity binds)
  Rest         2,000 km²  40% = 150k   2,000 ÷ 11.6 ≈ 172 150k ÷ 2,500 = 60             172 (coverage binds)
  + 20% peak buffer on the capacity-bound core (+18)                         Total ≈ 280 stores
```
- **Error fixed.** The tempting build computes the delivery radius and never uses it: it sizes on orders alone (2.1M ÷ 10,000 per store = 210, + 20% ≈ 250). Stores = max(coverage need, capacity need), zone by zone. Its inputs also need fixing: population from the ~30M region paired with the smaller capital territory's ~1,500 km²; 2.1M orders a day for one platform, roughly an order of magnitude above category volumes (verify); and 10,000 orders per store a day, 3–5× typical dark-store throughput of ~2–3k (verify). It also rounded 60% and 40% of 2.1M to 1.2M and 0.9M (they are 1.26M and 0.84M); the store count survived only because the two rounding errors cancel.
- **So what.** In the outer zone coverage binds, so each store serves only ~870 orders a day (150k ÷ 172), ~35% of its capacity. That is the business answer: promise 15 minutes in the core and denser pockets, and 30 minutes elsewhere.
- **Aha.** Network sizing = max(coverage, capacity) per zone. Capacity binds where demand is dense; coverage binds where it is sparse.

---

## Part D — Two-method reconciliation drills

### D1. Daily revenue of an amusement park — supply method
Rides and seats: 5 small (10 seats), 10 medium (20) and 5 large (30), for **400 seats**. Over 8 operating hours, 4 run at 80% occupancy and 4 at 50%.

**Error fixed.** The original computed seats × occupancy × hours = 2,080 and called it *visitors*. That assumes one ride cycle per hour, and it equates seat-rides with people. Two corrections:
1. **Cycles.** A ~10-minute cycle means 6 per hour, so 2,080 × 6 = **12,480 seat-rides**.
2. **People.** At ~4 rides per visitor, that is **≈ 3,120 visitors**.

```
  Entry  3,120 × ₹500                                     = ₹15.6 lakh
  Parking 3,120 × 50% by car ÷ 3 per car × ₹100           = ₹0.52 lakh   (not 1 car per visitor)
  F&B    3,120 × 70% × ₹200                               = ₹4.37 lakh
  Ads/sponsorship (flat)                                  = ₹0.50 lakh
                                                            ───────────
                                                 Total    ≈ ₹21 lakh/day  (≈ ₹673 per visitor)
```

### D2. The same park — demand method, then reconcile
Demand: 7,000 visitors; 80% ride (5,600); 4 rides each = 22,400 ride-trips, split 1 premium ride (₹300) to 3 regular rides (₹150).

**Error fixed.** The original applied ride "occupancy" (a supply concept) to *riders* (a demand count). Its table also used 1 premium and 2 regular rides after stating 4 rides per visitor.

```
  Premium  5,600 × ₹300 = ₹16.8 lakh
  Regular 16,800 × ₹150 = ₹25.2 lakh
  F&B      7,000 × 70% × ₹250 = ₹12.25 lakh
                              ───────────
  Demand-side total ≈ ₹54 lakh/day (≈ ₹775 per visitor)
```

**Reconcile.**
- **Spend per visitor agrees.** ₹673 vs ₹775, within ~15%, so the pricing logic is consistent.
- **Attendance does not.** Serving 22,400 trips over 8 hours needs 2,800 seat-rides/hr. With 5 premium rides of ~24 seats and 10 regular rides of ~35 seats (~470 seats), 6 cycles give 2,820/hr, which is **99% utilisation all day**. That is impossible without hour-long queues.
- **Fix.** At a realistic 65% utilisation the park clears ~14,700 trips, which supports ≈ 4,600 visitors, and revenue ≈ ₹35 lakh/day.

**Aha.** Demand estimates must be capped by capacity. A reconciliation that fails is useful: it tells you which assumption to cut.

### D3. Flight bookings per day on an online travel agency, busiest domestic trunk route (one direction)
**The original answer, ~613 bookings.** 12 flights/day (one every 2 hours) × 250 seats × 70–90% load gave 2,450 passengers; × 25% "margin" gave 613.

**Error fixed (four slips).**
1. Busy trunk routes run ~50+ departures a day, not 12.
2. Domestic narrowbodies seat ~180, not 250.
3. A **booking** often carries ~1.5 passengers.
4. The 25% was labelled *margin* but used as *share*. Keep the two words separate.

```
  55 departures × 180 seats × 85% load        = 8,400 passengers/day
  ÷ 1.5 passengers per booking                 = 5,600 bookings
  × 30% OTA share of bookings                  ≈ 1,700 bookings/day
  Cross-check: national domestic ~5 lakh pax/day (verify) × ~1.7% route share ≈ 8,500 ✓
```
**Steady-state note.** Today's bookings are for future dates. In steady state, bookings per day ≈ passengers flown per day ÷ passengers per booking.

### D4. EV launch in a ~50M-population country: demand vs. production capacity
**The tempting build.** Demand: 50M × 2% EV penetration = 1M × 10% first-year share = 100k, + 5% growth = 105k. Capacity: the Part 0 mini-card, 15,360 cars a year. The two numbers sit side by side and are never compared.

**Error fixed (three slips).**
1. **Unreconciled.** Output = min(demand, capacity), so the tempting answer is ~15k, not 105k. Serving 105k would need ~55 lines (105,000 ÷ 1,920 cars per line-year).
2. **Stock read as flow.** "2% penetration" describes EVs on the road. Read as one year's sales, 1M EVs is roughly the entire new-car market of a 50M-person country.
3. **Periods and labels mixed.** Adding growth inside year 1 mixes time periods, and "market × our share" is capturable demand, not the addressable market.

```
  Demand (flow): new-car sales 50M × 20 per 1,000 people        = 1.0M/yr
                 × 10% EV share of new sales                     = 100k EVs/yr
                 × 20% our share of EV sales                     = 20,000 cars/yr
  Capacity:      20 days × 2 shifts × 8 h × 8 lines ÷ 2 h × 12   = 15,360/yr
  Output = min(20,000, 15,360) = 15,360 → demand exceeds capacity by ~30%
  Cheapest lever: third shift → 20 × 3 × 8 × 8 ÷ 2 × 12          = 23,040/yr
                  utilisation = 20,000 ÷ 23,040                  ≈ 87% (top of the planning band)
```
- **Aha.** When capacity is below demand, capacity sets the answer and the case becomes a capacity-expansion question. Size the gap before prescribing: a 30% gap calls for a third shift, not ~50 new lines.
- **Trap.** A 2-hour per-car cycle is illustrative. Real assembly lines run takt times of a minute or two, so real output per line is far higher. Keep the structure and swap in the real cycle time.

### D5. Ad revenue per match of a women's franchise T20 league
**Method 1: inventory × rate × sell-through.**
```
  Breaks: 38 between overs + ~12 wickets + 4 timeouts + innings break (~6 breaks' worth) ≈ 60
  60 × 30 s = 1,800 s ÷ 10-s slot                           = 180 slots
  × ₹3.5 lakh per 10 s × 70% sell-through                   = ₹4.41 cr TV
  + digital at 35% of TV                                    = ₹1.54 cr
                                                              ────────
                                     Ad revenue/match      ≈ ₹6 cr
```
**Method 2: what the broadcaster paid.** Rights of ~₹190 cr a season `[ILLUSTRATIVE]` over ~22 matches ≈ ₹8.6 cr per match. A competitive rights auction leaves the winner a thin margin, so ad revenue per match should land within roughly 0.7–1.5× the rights cost per match. For a young league the low end is normal, with subscriptions and sponsorship packages covering the rest.

**Reconcile.** ₹6 cr ÷ ₹8.6 cr ≈ 0.7× ✓, at the low end, as expected for a new property.

- **Error fixed.** The tempting build uses ~90 breaks, a ₹7 lakh slot rate and 100% sell-through: 270 slots × ₹7 lakh = ₹18.9 cr TV, ₹25.5 cr with digital. Over 22 matches that is ~₹560 cr a season, ~3× the rights fee. A broadcaster earning 3× its cost would have been outbid, so the check says cut the rate and the sell-through. The rights fee was known and never used. Forty overs also yield ~55–65 breaks, not 90.
- **Aha.** Ad revenue = inventory seconds ÷ slot length × rate × sell-through, then sanity-checked against the rights fee. The two methods bracket each other.

---

## Part E — Physical & geometric estimates

No population and no filters: the constraint is a formula. Clarify the object (interior or exterior? standard size? smallest unit that counts?), pick the formula, then apply the real-world haircut (packing, obstructions, road circuity).
```
  Box volume            = L × W × H          → use INTERIOR dimensions, then deduct obstructions
  Sphere volume         = 4/3 π r³ = π d³ ÷ 6 ≈ 0.52 d³
  Packing fraction      ≈ 0.52 simple cubic stack · ≈ 0.64 random pour · ≈ 0.74 ideal (hexagonal)
  Count in a container  = usable volume × packing fraction ÷ unit volume
  Sphere surface        = 4 π r²             → Earth, r ≈ 6,371 km: ≈ 510M km²
  Length from area      = area ÷ average width
  Count from area       = area ÷ average unit size (a MEAN, set by the smallest unit you count)
```

### E1. Tennis balls in a school bus
**Clarify.** Full-size school bus, seats left in, standard ball (6.7 cm), windows shut.
```
  Interior 11 m × 2.3 m × 1.9 m                        ≈ 48 m³
  − 15% for seats, wheel arches and the driver area    ≈ 40.9 m³
  Ball volume 0.52 × 0.067³                            ≈ 0.000157 m³
  Count = 40.9 × 0.64 (random pour) ÷ 0.000157         ≈ 166,000
  Range: 0.52 stacked ≈ 135k · 0.74 ideal ≈ 192k        → answer ≈ 150–200k
```
- **Error fixed.** The tempting build uses a 10 × 5 × 7 m "bus" (350 m³, ~7× the real interior), a 10-cm ball (~1.5× the real diameter, so ~3.3× the volume), no packing factor and no deduction for seats, for ~700,000. It even rounds its own ball volume down (0.0005 vs. 0.000524 m³). The volume and packing slips outweigh the oversized ball, so the answer is ~4× too high.
- **Aha.** Interior volume and packing fraction move the answer more than the division does. State both before dividing.

### E2. Lakes in the world
**Clarify.** Fix the smallest lake you count first. The mean lake size, and so the answer, depends on it.
```
  Earth's surface 4π × 6,371²                         ≈ 510M km²
  × 29% land                                          ≈ 148M km²
  × 2% inland water                                   ≈ 2.96M km²
   ├─ Lakes              80%  ≈ 2.37M km²
   ├─ Ponds/reservoirs   15%
   └─ Rivers & wetlands   5%   (label it: the split must sum to 100%)
  Mean lake size 150 m × 150 m = 0.0225 km²
  Lakes ≈ 2.37M ÷ 0.0225                              ≈ 105M → ~100M lakes
```
- **Error fixed.** An inland-water split of lakes 80% + ponds 15% sums to 95%; label the missing 5% or the tree is not collectively exhaustive. And 0.0225 km² is a *mean* over a size distribution dominated by tiny lakes. Picture a familiar ~1 km² lake instead and the count collapses ~45×, to ~2.4M.
- **Sanity check.** Satellite inventories count on the order of 100M lakes above a small minimum size (verify) ✓. Using 6,400 km for the radius gives 515M km², an immaterial difference.
- **Aha.** With no population to anchor on, size by area ÷ average unit size, and set the minimum size in the clarifying step.

### E3. Road length in a capital city
**Clarify.** Centreline length of all public roads within a ~1,500 km² city boundary.
```
  Land use: residential 30 + commercial 25 + forest/agriculture 10 + roads 20 + other 15 = 100%
  Road area = 1,500 km² × 20%                         = 300 km²
  Class (by width/function)       Share   Area      Width   Length = area ÷ width
  Local lanes                      35%    105 km²    5 m    21,000 km
  Connector roads                  25%     75 km²   10 m     7,500 km
  Arterial main roads              15%     45 km²   15 m     3,000 km
  State highways                   10%     30 km²   20 m     1,500 km
  National highways/expressways    15%     45 km²   25 m     1,800 km
                                                            ─────────
                                                    Total ≈ 34,800 km
```
- **Error fixed.** A top-level tree of municipal 35% + state 50% + central 15% + "others" 15% sums to 115%, and highways sit under both the state and the central bucket. Classify by width and function, not by owner, so the buckets cannot overlap, and make every level sum to 100% (the land-use line needs its 15% "other").
- **Sensitivity.** Width is the swing assumption, and the narrowest class dominates: local lanes are 35% of road area but 60% of length. At 4 m instead of 5 m they add 5,250 km (≈ 40,000 km in total, +15%).
- **Sanity check.** Large Indian capitals report road networks of roughly 30,000–35,000 km (verify) ✓.
- **Aha.** Length = area ÷ width, class by class.

---

## Error checklist (run before you say your number)

| Slip | Seen in | Guard |
|---|---|---|
| Stock mistaken for flow ("all non-owners buy this year") | A2 | Installed base ÷ life + net adds |
| Capacity used as demand | C3 | Size demand, then check it against the ceiling |
| Averages hide the peak | C1 | Size on the busiest 5 minutes + service level |
| Cards ≠ holders; share ≠ margin; GMV ≠ revenue | A3, D3, B1 | Name the unit in the first sentence |
| Inconsistent base numbers across steps | A3, C4 | Write each product out; reuse one table |
| Probabilities chained without a participation step | A5 | Add "who is doing it on that day/at that time" |
| Demand not capped by capacity | D2 | output = min(demand, capacity) |
| Unused clarifying data | A1 | Only ask for what the tree consumes |
| Snapshot counted as daily flow | C7, A5 | Flow = number in the system ÷ time each unit spends in it (Little's law) |
| Multiplier above capacity ("2× capacity at peak") | C6 | Load bands are utilisation, ≤ 100% of the named ceiling |
| Filter applied twice (upstream cut + zero-rate tier) | A10 | Each exclusion lives in exactly one place |
| Answer in the wrong unit (₹ when asked for pairs; a total when asked for an average) | A12, A8 | Restate the question's unit before the first multiplication |
| Stock and flow added together | A9 | Stock ÷ life = replacement flow; new sales = replacement + net adds |
| A different base number in each estimate of one session | A14, A15 | Draw every shared figure from the Part 0 base table |

**Closing move.** End every guesstimate by naming the one assumption that swings the answer most, and giving the range it implies. See `references/case-cracking-drills.md` for fast case-math drills.
