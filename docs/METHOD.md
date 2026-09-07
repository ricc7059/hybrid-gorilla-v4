# Block Programming — Method Notes

Original analysis written for the 4.0 build. Derived from reading five Fit 365 volumes, but
**contains no reproduced workouts, tables, or exercise sequences** — only the abstracted
method and our own conclusions about what to adopt. Source PDFs live outside this repo.
See [`BRIEF.md`](BRIEF.md) §3 for the policy.

Every worked example below uses **our own** lifts, written to illustrate a shape.

---

## 1. The corpus and its trajectory

Five volumes, read in full or in substantial part, spanning two distinct eras:

| Era | Volumes | Organizing unit | Effort vocabulary | Layout |
|---|---|---|---|---|
| **Early** | May 2020, June 2020 | Week 1–4 | `Challenge` present; explicit 1RM anchors (Medium ≈60%, Medium Plus ≈70%, Heavy ≈80%, AHAP ≈90%) | Prose |
| **Late** | Volume 01 | 20 jump-in-anywhere workouts | `Challenge` retired; **all percentages dropped**; `Light/Medium` and `Medium to Moderate` added; Superset / Giant Set / Finisher formally defined | Prose |
| **Late** | v5, v6 | 20 jump-in-anywhere workouts | Same as Volume 01, plus effort defined by *contraction quality* and *rep-failure point* | **Three-column table** (Exercise · Reps · Weight) with a `TARGET:` muscle header per block |

**Correction to the brief's premise.** The brief treated the loss of 1RM anchors as a v5 change.
It isn't — Volume 01 had already dropped them. The whole late era abandoned percentage-based
prescription in favor of effort defined by what you can and can't complete. That makes the shift
a deliberate methodological stance rather than a formatting quirk, which strengthens the case
for adopting it wholesale in 4.0.

**The trend that matters most for us:** across the late era, round counts came *down* while
structural complexity went *up*. Volume 01 routinely prescribes 6–8 round giant sets; v6 is full
of 2–4 round blocks carrying far more internal structure. That direction of travel is a gift —
v6-era shapes fit a seven-day running week considerably better than Volume 01-era shapes do.

---

## 2. Session grammar

A session is an ordered list of lettered blocks, A → B → C → D, each fully completed before the
next begins. A block declares four things in its header:

```
[LETTER]  TYPE: N ROUNDS
          Rest X Between Rounds
          TARGET: <muscle groups>
```

**Block types.** Superset (two movements, no rest) · Giant Set (three or more, no rest) ·
Sequence / Set (a fixed pattern repeated for rounds) · Finisher (terminal; reinforces contraction
and exhausts what was trained).

**The `TARGET:` header is the single most portable idea in the late format.** It states a block's
purpose independently of its exercises, which is exactly the seam our rotation table needs — the
target stays fixed while the movements underneath it rotate.

**Rest is declared, not implied.** Typically 1–3 min between rounds, 2–3 min between blocks, but
short dense blocks (bands, isolation) drop to 30–60 s and say so.

**Warmup is structural, not a preamble.** General cardio 5–10 min, then the first 1–2 rounds of
the working block are performed at warmup weight for high reps. This is the detail that makes
wave loading and specific warmup *the same mechanism* — which resolves change-list items #2 and
#7 together rather than separately, and suits a 4:30am fasted cold start well.

---

## 3. The effort ladder

Ascending. This replaces RIR outright in 4.0.

| Label | Definition |
|---|---|
| Warmup | Very light. Raise heart rate and blood flow, prepare the joints. |
| Light / Medium | Easy to control through a full range; allows a very strong contraction. |
| Medium to Moderate | Challenging but not overbearing; full range still available. |
| Medium Plus | Heavy enough to take you out of a medium comfort zone. |
| Heavy | Should be able to complete roughly **2 more reps** than prescribed. |
| As Heavy as Possible to Complete | Should **not** be able to complete even one rep beyond the prescription. |
| To Failure | The point at which a rep can no longer be completed with good form. |

The late volumes increasingly express effort as a *condition* rather than a label — "use a weight
such that you reach failure at or before 20 reps," "heavy enough to barely complete the set with
maximum contraction." Worth carrying into 4.0 as an optional free-text qualifier alongside the
label, because it prescribes an outcome instead of a number and self-corrects across gym modes
where the available weights differ.

---

## 4. Wave loading — five distinct shapes

The brief described one wave. There are at least five in the corpus, and they do different jobs.
Named here by us for the app's schema.

**1. Ramp** — reps fixed, effort ascends by round bracket.
> *e.g.* Weighted pull-up, 5 rounds × 6 reps · rounds 1–2 Medium Plus · rounds 3–5 Heavy

**2. Classic wave** — reps descend as effort ascends. The brief's shape.
> *e.g.* Bench press, 4 rounds · R1 10 Medium Plus · R2 10 Medium Plus · R3 8 Heavy · R4 6 AHAP

**3. Pyramid** — ascends to a peak, then backs off to a named earlier round's load.
> *e.g.* Safety bar squat, 8 rounds · R1 15 Light · R2 12 Medium · R3 10 Medium Plus ·
> R4–5 5 Heavy · R6–7 8 Heavy · R8 10 at R3's weight

**4. Double wave** — two peaks in one block, with a deload between.
> *e.g.* Overhead press, 8 rounds · R1–2 15 Medium · R3–4 10 Medium Plus · R5 8 Heavy ·
> R6–7 10 Medium Plus · R8 6 Heavy

**5. Autoregulated ascent** — no prescribed loads; add weight each round until a rep target
collapses. Requires no planning and self-calibrates across gym modes.
> *e.g.* Goblet squat, 15 reps — add weight each round until 15 is no longer reachable

Two further observations:

- **Waves are applied to isolation, not just compounds.** A lateral raise waved
  25 → 20 → 15 → 10 across four rounds, effort climbing Medium → AHAP, is a completely
  different stimulus from three flat sets — and it costs the same time. This is the direct
  answer to the pump problem, and it's cheaper systemically than waving a compound.
- **The exercise itself can change mid-block by round.** Rounds 1–3 run one movement,
  rounds 4–6 another, inside a single lettered block. Our schema has to allow the
  movement to be a per-round field, not just reps and effort.

**Schema consequence.** A round is the atomic unit, and it independently carries: movement,
reps, effort label, optional effort condition, and an optional back-reference to another round's
load ("same weight as round 3"). Change-list item #8 is confirmed and is bigger than it looked.

---

## 5. Rotation logic — the blocked question, now answered

This was the item the brief couldn't resolve on two volumes. Five is enough.

**The cycle.** 20 workouts per 30 days on a ~5-day rotating split, jump in at any number.
No workout repeats inside a cycle. A given muscle slot therefore recurs **about four times per
volume** — which is precisely the "4 variants per slot" the brief guessed at, now evidenced
rather than assumed.

**What holds constant across a slot's four appearances:**
- The `TARGET:` muscle group
- The movement *pattern* (squat stays a squat; horizontal press stays a horizontal press)
- The supporting cast — calf, core, and mobility fillers barely change

**What rotates:**
- **Implement** — barbell → dumbbell → kettlebell → cable → bodyweight → band
- **Angle** — incline → flat → decline/dip → standing
- **Unilateral vs. bilateral**, and alternating vs. simultaneous
- **Press character** — strict → alternating → explosive/clean-to-press → partial-range
- **Which wave shape** the primary carries

**The rule, stated plainly:** *novelty is concentrated in the primary movement; the accessories
are deliberately boring.* One slot, one target, one pattern, four implement/angle variants, and
a rotating wave shape on top. That is the whole rotation table, and it is directly portable.

**For 4.0's 8-week block:** a slot that appears weekly gets 8 exposures. Four variants at two
exposures each (weeks N and N+4) gives novelty *and* a second look at every variant for load
progression — better than eight one-shot variants, which would leave nothing to progress against.

---

## 6. Structural devices worth stealing

**Ladders.** Ascending: one rep of B after each rep of A, climbing to a target. Descending: the
same run backwards. Some volumes program the ascent and the descent as two separate lettered
blocks in one session. Large stimulus per unit time, and mentally the opposite of a flat set.

**Built-in drop-set series.** One "set" is defined as a chain: heavy for a low rep target, drop a
fixed increment, repeat, continuing to a floor weight. The entire chain counts as a single set.
Costs about three minutes. This is what the delt work needs.

**Rep-total blocks.** A block prescribes a *total* — 50 pull-ups, say — as many per round as
possible, superset with something else, continuing until the total is met. Self-scaling to the
day's readiness, which suits a 7-day-running week well.

**Terminal metabolic finishers.** A short timed flow alternating a contraction-focused movement
with a conditioning burst, 2–4 rounds. Where the pump days should end.

**Weight chaining.** Within a giant set, an exercise can inherit the previous one's load, with an
explicit warning to choose a weight that serves both. Forces honest selection and prevents the
giant set from silently becoming two unrelated exercises.

**First-class alternates.** Late volumes write "X *or* Y" directly into the prescription for
equipment substitution. This maps exactly onto Home / Travel Best / Travel Worst gym modes —
we should treat the alternate as a schema field, not a footnote.

---

## 7. What 4.0 takes, adapts, and leaves

| | Decision |
|---|---|
| **Take unchanged** | Effort ladder and vocabulary · lettered blocks with declared type and rest · `TARGET:` headers · warmup-as-first-rounds · the five wave shapes · rotation logic · ladders, drop-set series, rep-totals, finishers · first-class alternates |
| **Adapt** | Round counts — take the v6 direction (2–6) rather than Volume 01's 6–8, since round count is where the running tax gets paid. Slot frequency — Sklar's slot recurs every 5th session across a 30-day cycle; ours recurs weekly across an 8-week block. |
| **Leave** | The 5-day split itself and the 2 rest days it assumes. The 60-minute uniform session. Any assumption that lower-body work can land anywhere in the week. |

**The unresolved tension, stated honestly.** Sklar's method assumes two full rest days and no
running. Steve runs seven days a week. Every structure above is portable; the *volume* is not.
The 4.0 sessions have to buy their rounds somewhere, and per the brief that purchase happens on
Saturday and Sunday, never in front of a quality run or the long run. Recovery remains the
limiting variable — total weekly hard sets go up, but by redistribution and better structure,
not by addition.

---

## 8. What this unblocks

- Rotation table — **unblocked.** Logic in §5 is sufficient to build it.
- Data model — **sharpened.** §4 makes the round the atomic unit and adds movement, effort
  condition, and load back-reference to the fields a round must carry.
- Session design — ready to start, and now the real work.
