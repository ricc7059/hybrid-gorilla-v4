# 🦍 HYBRID GORILLA 4.0 — Block Programming

**Same running. Rebuilt lifting.**

Built for: Steve Ricci · Age 43 · Runner who lifts
Running anchor: **Monday, August 17, 2026** — carried forward unchanged from 3.0
Storage key: `hybrid-gorilla-v4`

Successor to [Hybrid Gorilla 3.0](https://github.com/ricc7059/hybrid-gorilla-fullbody), which stays live and untouched. 4.0 rebuilds the **lifting** side around block programming — lettered blocks, wave loading, effort labels, and exercise rotation. The running program is out of scope and carries over verbatim.

> **Status: scaffolding.** The program is designed but not yet written. See
> [`docs/DESIGN.md`](docs/DESIGN.md) for decisions locked and questions open, and
> [`docs/BRIEF.md`](docs/BRIEF.md) for the originating build brief.

---

## Why 4.0 exists

Two complaints, two different causes.

**"No pump or fatigue during the session."** This one is programming, and it's fixable. 3.0 was built to protect the running and overcorrected — four of seven lift sessions sit at RIR 3 and cap at ~25 minutes. Only Monday and Wednesday are genuinely hard. Three sets shy of failure on a lateral raise produces neither stimulus nor sensation. Worse, the 3.0 lift template is byte-identical in every block, forever: no exercise rotation, no structural novelty across an entire 8-week cycle.

**"Size and composition have stalled."** This one is **not** programming. Seven days a week of running plus seven days a week of lifting at a ~400 calorie deficit, at 43, produces exactly this outcome. No restructuring of the lift program fixes it. Modeled properly in [`NUTRITION.md`](docs/NUTRITION.md): the useful lens is *energy availability*, not calorie balance, and at this training volume the current deficit likely sits below the threshold where the body starts suppressing the anabolic signaling hypertrophy depends on. That makes the environment hostile to building rather than merely neutral — and it gates how aggressively 4.0 gets built.

---

## What changes from 3.0

| | 3.0 | 4.0 |
|--|-----|-----|
| Effort scale | RIR (0–3) | **Effort labels** — Warmup → Medium Plus → Heavy → As Heavy as Possible → To Failure |
| Pump days | RIR 3, ~25 min | **Isolation to failure.** Same exercises, same time, real stimulus |
| Heavy days | Flat `3 × 6–10` | **Wave loading** — ascending intensity, descending reps across rounds |
| Session structure | Exercise list | **Lettered blocks** A → B → C → D, each declaring type and rest interval |
| Block types | — | **Superset · Giant Set · Sequence · Finisher · Specific Warmup Sets** |
| Warmup | Afterthought at the top | **Its own lettered block** — fits a 4:30am fasted cold start |
| Exercise selection | Identical every block, forever | **Rotates across the 8-week block** — 4 variants per slot |
| Tue / Thu | Ends when the list ends | **Terminal metabolic finisher** |
| Saturday upper | Optional filler after the long run | **A real chest/arm session** |
| Chest frequency | ~5 hard sets/wk, all Monday | **Redistributed across the week** |
| Intensifiers | — | **Drop sets and rest-pause, weeks 3–7, isolation only** |
| Data model | Flat `sets × reps` + single RIR | **Per-round prescription array** — round 1 and round 5 differ in both reps and effort |

**Carried over unchanged:** the entire running program, Home / Travel Best / Travel Worst gym modes with independent weight logs, the action-registry onclick pattern, per-exercise weight + done logging, session notes, fasted 4:30am training, and the nutrition/supplement protocol.

---

## Running — unchanged, out of scope

Working, and not being touched:

- 7 days/wk. Easy Mon/Wed/Fri/Sun · quality Tue/Thu · long run Sat
- Rotating 8-week blocks: **A Threshold → B VO2max → C Economy**
- VDOT zones in Peloton mph — E 7.7–8.4 · T 9.0–9.5 · I 9.5–10.5 · R 10.5–11.5
- 3-mile time trial on the Saturday of every deload week; recalibrate zones after each
- Deload = week 8 of every block, mandatory

The anchor stays **Monday, August 17, 2026**. 4.0 picks up mid-block rather than restarting the running cycle.

---

## The hard constraint

Sklar-style block programming assumes **two full rest days and no running.** Steve runs seven days a week. Round counts of 5–10 per block across 60-minute sessions cannot simply be bolted onto a 7-day running week — the volume has to be bought somewhere.

- Hard leg work only ever lands **before easy runs**. Heavy lower stays Wednesday.
- Saturday gets **zero** leg work — the long run is the leg work.
- **Saturday and Sunday are the slack days** and absorb most of the added volume.
- Mon/Wed/Fri stay roughly where they are on time.
- Time budget varies by day. There is no flat session length.
- Recovery is still the limiting variable. Weekly hard sets go **up**, but redistributed and restructured — not simply added.

---

## Source material policy

The method behind 4.0's block structure comes from Paul Sklar's Fit 365 monthly volumes. **These are paid, explicitly non-redistributable documents.**

Nothing from them is reproduced in this repo — not workouts, not tables, not exercise sequences. We import the *method* and write original sessions. The PDFs live outside this repo entirely, in `~/hybrid-gorilla-reference/`, which is not a git repository and never will be. `.gitignore` here blocks them as a second line of defense.

---

## Technical

Single-file `index.html`. Mobile-first, 393px target. No dependencies, no backend, no framework. All state in localStorage under `hybrid-gorilla-v4` — 3.0's data is neither migrated nor clobbered.

---

## Lineage

- [`ricc7059/hybrid-gorilla`](https://github.com/ricc7059/hybrid-gorilla) — 2.0. 36-week race program, body-part split, ended Dec 31 2026. Archived reference.
- [`ricc7059/hybrid-gorilla-fullbody`](https://github.com/ricc7059/hybrid-gorilla-fullbody) — 3.0. Full-body lift + run daily, rolling 8-week blocks. **Still live.**
- **4.0** — this repo. Lifting rebuilt on block programming.
