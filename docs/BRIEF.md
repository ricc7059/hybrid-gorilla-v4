# Hybrid Gorilla 4.0 — Build Brief

Handoff from a chat session. Purpose: rebuild the **lifting** side of Hybrid Gorilla 3.0 around Sklar-style block programming, in a new repo, without touching the running side.

---

## 1. Where things stand

**Existing repos**

- `ricc7059/hybrid-gorilla` — v2.0. 36-week race program, body-part split, ended Dec 31 2026. Archived reference.
- `ricc7059/hybrid-gorilla-fullbody` — v3.0. Current live program. Full-body lift + run every day, rolling 8-week blocks, no end date. Anchor date Mon Aug 17 2026. Storage key `hybrid-gorilla-v3`.

**4.0 goes in a new repo.** Name TBD. v3.0 stays untouched — its localStorage data should not be migrated or clobbered. Use a new storage key (`hybrid-gorilla-v4`).

**What is NOT changing.** The running program is working and is out of scope:

- 7 days/wk running, easy Mon/Wed/Fri/Sun, quality Tue/Thu, long run Sat
- Rotating 8-week blocks: A Threshold → B VO2max → C Economy
- VDOT zones in Peloton mph (E 7.7–8.4 / T 9.0–9.5 / I 9.5–10.5 / R 10.5–11.5)
- 3-mile TT on the Saturday of every deload week; recalibrate zones after each
- Deload = week 8 of every block, mandatory

Also carrying over unchanged: Home / Travel Best / Travel Worst gym modes with independent weight logs, the action-registry onclick pattern, per-exercise weight + done logging, session notes, fasted 4:30am training, and the nutrition/supplement protocol.

---

## 2. The problem being solved

Reported: *"the lifting feels like I'm not getting enough stimulus."* On follow-up, two specifics — **no pump or fatigue during the session**, and **size/composition has stalled**.

These have different causes.

### 2a. The pump problem is programming

v3.0 was built to protect the running and overcorrected. Four of seven lift sessions (Tue, Thu, Sat pump days) are RIR 3 and capped at ~25 minutes. Only Monday and Wednesday are genuinely hard. Three sets shy of failure on a lateral raise produces neither stimulus nor sensation.

Second cause: **the v3.0 lift template is byte-identical in every block, forever.** Only the RIR wave and the running menu change. There is no exercise rotation and no structural novelty across an entire 8-week cycle, let alone across cycles.

Third: chest gets roughly 5 hard sets a week, all on Monday. Saturday's "optional upper pump" sits after the long run with zero leg work — that slot is being wasted.

### 2b. The size problem is mostly not programming

7 days/wk running + 7 days/wk lifting at a ~400 cal deficit, age 43. Stalled composition is the expected outcome. **No restructuring of the lift program fixes this.** Flag it, don't silently try to program around it. Worth a separate decision about whether to run a maintenance or slight-surplus phase.

---

## 3. Sklar method — what to import

Source: Paul Sklar Fit 365 monthly volumes (July 2020 and v5 reviewed). **These are paid, explicitly non-redistributable documents. Do not copy his workouts, tables, or exercise sequences into the repo.** Import the *method* and write original sessions. The PDFs are on Steve's machine if you need to reference them directly.

### 3a. Wave loading inside a giant set — the headline change

Same movement, ascending intensity across rounds, descending reps. Roughly:

| Rounds | Reps | Effort |
|---|---|---|
| 1–2 | high | Medium |
| 3–4 | mid | Medium Plus |
| 5–8 | low | Heavy → As Heavy as Possible |

This is the single most important structure to adopt. It gives a built-in ramp to a genuine top set, fixes the pump problem and the strength problem in one shape, and replaces the flat `3 × 6–10` on Monday and Wednesday.

Note: the v5 glossary **dropped the 1RM percentage anchors** the 2020 volume used (Medium 60%, Medium Plus 70%, Heavy 80%, ~90%). v5 defines effort by contraction quality and by whether reps beyond the prescription are achievable. Use v5 vocabulary. `Challenge` is gone; `As Heavy as Possible to Complete` replaces it.

### 3b. Effort labels replace RIR

Ladder, roughly ascending: Warmup → Light/Medium → Medium to Moderate → Medium Plus → Heavy (about two reps left) → As Heavy as Possible to Complete (prescribed reps and no more) → To Failure.

**Delete RIR 3 entirely.** Isolation work goes to RIR 0–1 / As Heavy as Possible. Isolation-to-failure is systemically cheap and won't affect the next day's run; compound-to-failure is expensive. v3.0 pays the recovery tax on both and collects on neither.

### 3c. Block types

Lettered blocks A → B → C → D, completed in order, one fully finished before the next. Header declares the type and rest interval.

- **Superset** — two movements back to back, no rest
- **Giant Set** — three or more back to back, no rest
- **Sequence** — a fixed pattern repeated for rounds
- **Finisher** — terminal block, reinforces contraction and exhausts what was trained
- **Specific Warmup Sets** — its own lettered block, not an afterthought. Fits the 4:30am fasted cold start better than v3.0's current opening.

Rest: 1–3 min between rounds, 2–3 min between blocks.

### 3d. Three structures to steal outright

1. **Ladders** — clean then 1 press, clean then 2, up to 10. Or deadlift-to-ascending-shrug. Large stimulus per unit time, and mentally the opposite of a flat set.
2. **Built-in drop-set series** — a lateral raise set defined as 10 reps, drop, 10 more, drop, 10 more = one set. Exactly what the delt work needs; costs about three minutes.
3. **Terminal metabolic finishers** — where the pump days should end.

### 3e. Rotation

Sklar never repeats a workout inside a 28-day cycle. 4.0 should rotate exercise selection across the 8-week block — same movement pattern per slot, rotating implement and angle across ~4 variants.

**Still needed:** how a given slot varies across volumes. Two volumes isn't enough of a sample to infer the rotation logic. Steve has more Sklar volumes; pull the leg slot, shoulder slot, and chest slot across three or four of them before finalizing the rotation table.

---

## 4. Design constraints

The hard one: **Sklar assumes 2 full rest days and no running.** Steve runs 7 days a week. His round counts (5–10 per block, 60 min sessions) cannot be bolted onto a 7-day running week without buying the volume somewhere.

- Hard leg work only ever lands before easy runs. Heavy lower stays Wednesday.
- Saturday gets zero leg work — the long run is the leg work. But the upper slot there should become a real session, not optional filler.
- Sunday and Saturday are the slack days and should absorb most of the added volume. Mon/Wed/Fri stay roughly where they are on time.
- Time budget varies by day — no uniform session length. Don't assume a flat 40 min.
- Recovery is still the limiting variable. Total weekly hard sets should go up, but redistributed and structured, not simply added.

---

## 5. Change list

1. Delete RIR 3. Pump days become As-Heavy-as-Possible on isolation; same exercises, same time, last set to failure.
2. Wave loading on Monday heavy upper and Wednesday heavy lower.
3. Add a metabolite/finisher block to Tue and Thu — one long high-rep sequence, minimal rest.
4. Rebuild Saturday upper as a real chest/arm session. Fix chest frequency, currently ~5 hard sets/wk all on one day.
5. Exercise rotation across the block — 4 variants per slot.
6. Intensifiers weeks 3–7: drop sets and rest-pause, isolation only. (Carried from the J3U approach in 2.0.)
7. Specific warmup as its own lettered block.
8. Convert the app's data model from RIR to effort labels, and from flat `sets × reps` to per-round prescriptions (wave loading means round 1 and round 5 differ in both reps and effort — the current schema can't express this).

---

## 6. App notes

Single-file `index.html`, mobile-first, 393px target, no dependencies. Carry the v3.0 architecture forward.

Schema change worth planning before writing UI: exercises need to carry an optional per-round prescription array rather than a single reps/effort pair. Block types (Superset / Giant Set / Sequence / Finisher) need to render distinctly in session modals, and rounds need to be individually checkable so a wave can be tracked mid-session.

Keep the existing localStorage key patterns but under `hybrid-gorilla-v4`.

---

## 7. Open questions

- Repo name.
- Whether the running block anchor date resets or 4.0 picks up mid-block from v3.0's Aug 17 2026 anchor.
- Whether to run a maintenance/surplus nutrition phase (see 2b) — separate decision, but it determines whether the hypertrophy work can actually pay off.
