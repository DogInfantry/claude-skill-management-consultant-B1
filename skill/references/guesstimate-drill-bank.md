# Guesstimate Drill Bank — Organised by Method, With the Classic Errors Fixed

Fourteen worked guesstimates, grouped by the **sizing method** each one exercises, not by topic. Every drill shows the tree, the math, a sanity check against an outside anchor, and, where the "obvious" answer goes wrong, an **Error fixed** callout. Those callouts are the point of this file: most candidates lose guesstimates on a logic slip, not on arithmetic.

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

**Closing move.** End every guesstimate by naming the one assumption that swings the answer most, and giving the range it implies. See `references/case-cracking-drills.md` for fast case-math drills.
