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

## Blocked

### Rotation table — needs more source volumes

Sklar never repeats a workout inside a 28-day cycle. 4.0 should rotate exercise selection across the 8-week block: same movement pattern per slot, rotating implement and angle across ~4 variants.

**Two volumes (July 2020 and v5) is not enough of a sample to infer the rotation logic.** Before the rotation table can be finalized, pull the **leg slot, shoulder slot, and chest slot** across three or four volumes.

→ Drop additional volumes in `~/hybrid-gorilla-reference/sklar-volumes/`. That folder's README lists exactly what gets extracted.

---

## Open questions

1. ~~Repo name~~ — **resolved**: `hybrid-gorilla-v4`
2. ~~Running block anchor~~ — **resolved**: continues from Aug 17 2026
3. **Nutrition phase.** Whether to run a maintenance or slight-surplus block. This is a separate decision from programming, but it determines whether the hypertrophy work can actually pay off. Seven days running + seven days lifting at a ~400 cal deficit at 43 is why composition stalled; the lift rebuild fixes the *pump*, not the *size*. Unresolved.

---

## Build order

1. ~~Repo scaffold~~ ✅
2. Collect additional source volumes → extract leg/shoulder/chest slots → **rotation table**
3. Session design — the seven daily templates, per day, with real time budgets
4. Data model — per-round prescription array, block types, individually checkable rounds
5. App build — carry 3.0 architecture forward into a new single-file `index.html`
6. Deploy to GitHub Pages
