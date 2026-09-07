# 4.0 Design Log

Decisions locked, work outstanding, questions open. Companion to [`BRIEF.md`](BRIEF.md).

---

## Decided

| Decision | Value | Date |
|---|---|---|
| Repo name | `hybrid-gorilla-v4` | 2026-09-07 |
| Storage key | `hybrid-gorilla-v4` — 3.0 data untouched, not migrated | from brief |
| Running anchor | **Continues from Mon Aug 17 2026.** No reset — 4.0 picks up mid-block | 2026-09-07 |
| Scope | Lifting only. Running out of scope and carried over verbatim | from brief |
| Effort scale | v5 vocabulary. No 1RM % anchors. `Challenge` retired in favor of `As Heavy as Possible to Complete` | from brief |
| Source material | Method only. No verbatim workouts, tables, or sequences. PDFs stay outside the repo | from brief |

### Equipment

Steve has the full recommended equipment list **except balls of any kind** — no slam balls, no medicine balls.

| Available | Not available |
|---|---|
| Barbells · Dumbbells · Kettlebells · Adjustable bench · Cable station · Resistance bands · Pull-up station/bars · Lebert Equalizers · Parallettes · Battle rope · Suspension trainer | **Slam balls · Medicine balls** |

This matters more than it looks. Slam-ball work carries the explosive/metabolic conditioning slot throughout the source material — squat slams, squat-to-ascending-overhead-press ladders, descending-press complexes. That whole family needs substitution, and the substitutes must respect the standing preference for **free weights and cables only**, with landmine as an alternate rather than a prescription.

**Substitution map for the ball-driven patterns:**

| Pattern being replaced | Substitute | Why |
|---|---|---|
| Squat slam (explosive triple extension → ground) | **Kettlebell swing** | Closest available explosive hip hinge; already free-weight |
| Squat to ascending overhead press ladder | **KB or DB clean to ascending overhead press** | Preserves the ladder exactly; clean-to-press already native to the method |
| Squat-slam metabolic finisher | **Battle rope** (jump slams, anacondas, jumping jacks) | Already used as the source's own listed alternate; he has the rope |
| Squat side-lunge slam complex | **Goblet squat → lateral lunge complex** | Same movement chain, KB loaded |
| Descending-press slam complex | **DB thruster, descending reps** | Squat-to-press in one movement, reps ladder down |

No slot is lost — the rope covers metabolic, the kettlebell covers explosive. Worth noting the battle rope becomes load-bearing in 4.0 in a way it wasn't in 3.0, so Travel Best / Travel Worst modes need their own alternates for every rope prescription.

### Effort ladder

Ascending:

```
Warmup
Light / Medium
Medium to Moderate
Medium Plus
Heavy                            ~2 reps left
As Heavy as Possible to Complete prescribed reps and no more
To Failure
```

**RIR 3 is deleted outright.** Isolation work goes to RIR 0–1 / As Heavy as Possible — it's systemically cheap and won't affect the next day's run. Compound-to-failure is expensive and stays rare. 3.0 paid the recovery tax on both and collected on neither.

### Block types

Lettered A → B → C → D, completed in order, one fully finished before the next. Header declares type and rest interval.

- **Specific Warmup Sets** — its own lettered block, not an afterthought
- **Superset** — two movements back to back, no rest
- **Giant Set** — three or more back to back, no rest
- **Sequence** — a fixed pattern repeated for rounds
- **Finisher** — terminal, reinforces contraction and exhausts what was trained

Rest: 1–3 min between rounds, 2–3 min between blocks.

### Wave loading — the headline structure

Same movement, ascending intensity across rounds, descending reps.

| Rounds | Reps | Effort |
|---|---|---|
| 1–2 | high | Medium |
| 3–4 | mid | Medium Plus |
| 5–8 | low | Heavy → As Heavy as Possible |

Applies to Monday heavy upper and Wednesday heavy lower, replacing flat `3 × 6–10`. Gives a built-in ramp to a genuine top set — fixes the pump problem and the strength problem in one shape.

### Structures to adopt

1. **Ladders** — e.g. clean then 1 press, clean then 2, up to 10. Large stimulus per unit time; mentally the opposite of a flat set.
2. **Built-in drop-set series** — a lateral raise set defined as 10 reps, drop, 10 more, drop, 10 more = *one set*. Exactly what the delt work needs. Costs ~3 minutes.
3. **Terminal metabolic finishers** — where the pump days should end.

---

## Change list

1. Delete RIR 3. Pump days become As-Heavy-as-Possible on isolation; same exercises, same time, last set to failure.
2. Wave loading on Monday heavy upper and Wednesday heavy lower.
3. Metabolite/finisher block on Tue and Thu — one long high-rep sequence, minimal rest.
4. Rebuild Saturday upper as a real chest/arm session. Fix chest frequency (currently ~5 hard sets/wk, all Monday).
5. Exercise rotation across the block — 4 variants per slot.
6. Intensifiers weeks 3–7: drop sets and rest-pause, **isolation only**. (Carried from the J3U approach in 2.0.)
7. Specific warmup as its own lettered block.
8. Convert the data model from RIR to effort labels, and from flat `sets × reps` to per-round prescriptions.

---

## ~~Blocked~~ — cleared 2026-09-07

### Rotation table — **unblocked**

Five volumes read (May 2020, June 2020, Volume 01, v5, v6). The rotation logic is no longer a guess:

> One slot, one `TARGET:` muscle group, one movement pattern, four implement/angle variants, a rotating wave shape on the primary, and a deliberately boring supporting cast.

Full analysis in [`METHOD.md`](METHOD.md). Three findings that changed the plan:

1. **The brief's premise about 1RM anchors was slightly off.** Volume 01 had already dropped the percentages — it wasn't a v5 change. The whole late era abandons percentage-based prescription in favor of effort-as-condition. Strengthens the case for adopting the vocabulary wholesale.
2. **Round counts fell over time** (Volume 01: 6–8 · v6: 2–4) while structural complexity rose. Take the v6 direction — round count is exactly where the running tax gets paid.
3. **There are five wave shapes, not one** — Ramp, Classic, Pyramid, Double Wave, Autoregulated Ascent. And waves get applied to *isolation*, not just compounds. A waved lateral raise is the direct answer to the pump problem and costs the same time as three flat sets.

### Data model — sharpened

The round is the atomic unit. Each round independently carries **movement** (it can change mid-block), reps, effort label, an optional effort *condition* ("failure at or before 20 reps"), and an optional load back-reference ("same weight as round 3"). Change-list item #8 is confirmed and larger than first scoped. Alternates ("X or Y") are a schema field, not a footnote — they map straight onto the gym modes.

---

## Open questions

1. ~~Repo name~~ — **resolved**: `hybrid-gorilla-v4`
2. ~~Running block anchor~~ — **resolved**: continues from Aug 17 2026
3. **Nutrition phase.** **Surplus ruled out** by decision (2026-09-07). Deficit vs. maintenance modeled on real inputs in [`NUTRITION.md`](NUTRITION.md) — recommendation is maintenance, but weakly. **Still to decide**, and it gates session design: round counts, finisher volume, and intensifier schedule differ between the two.

   Real inputs: **210 lb · 12–18% BF · 3,300 kcal/day · 20–25 mi/wk.** Energy availability computes to **~32 kcal/kg FFM** — *above* the low-availability threshold, contrary to the first pass on illustrative numbers. The deficit is a modest brake, not the cause of the stall. Revised attribution: (1) 3.0's lift stimulus was genuinely insufficient, (2) concurrent-training interference from 7-day running, (3) advanced training status at 43. **The lift rebuild is the bigger lever; nutrition is the smaller one.**

   Open sub-item: the −400 figure implies maintenance ≈ 3,700 but the model says ≈ 3,480. A 2–3 week intake audit at 3,300 with daily weigh-ins resolves whether the real deficit is −400 or −180.

---

## Build order

1. ~~Repo scaffold~~ ✅
2. ~~Collect source volumes → extract the method → rotation logic~~ ✅ — see [`METHOD.md`](METHOD.md)
3. ~~**Rotation table** — 4 variants per slot, mapped to equipment and gym modes~~ ✅ — see [`ROTATION.md`](ROTATION.md)
4. Session design — write the seven daily templates out as concrete lettered blocks with per-round prescriptions ← *next*
5. Data model — round as atomic unit, block types, individually checkable rounds
6. App build — carry 3.0 architecture forward into a new single-file `index.html`
7. Deploy to GitHub Pages
