# Nutrition — Deficit vs. Maintenance

Two scenarios modeled side by side. **Surplus is off the table** by decision, so it isn't
modeled here.

This decision gates session design, so it comes first. The round counts, finisher volume, and
intensifier schedule in 4.0 should differ between these two scenarios — it is not "build the
program, then decide what to eat."

---

## 1. Why the stall isn't really about calories

The useful lens for a hybrid athlete is **energy availability (EA)**, not calorie balance:

```
EA = (intake − exercise energy expenditure) ÷ kg fat-free mass
```

It measures what's left to run the body *after* training takes its cut. The thresholds are
well established in the sports-science literature:

| EA (kcal/kg FFM/day) | State |
|---|---|
| **< 30** | Low energy availability. Testosterone, T3, and IGF-1 fall. Muscle protein synthesis is suppressed. Bone turnover and immune function degrade. |
| **30–45** | Adequate. Maintenance is possible; adaptation is muted. |
| **~45** | Optimal for adaptation and tissue accrual. |

This matters because calorie balance and energy availability come apart badly at high training
volumes. A modest-sounding deficit stacked on top of seven days of running and seven days of
lifting can push EA under 30 — at which point **the body actively downregulates the anabolic
signaling that hypertrophy depends on.** That's a different problem from "not enough surplus to
build." It means the environment is hostile to building rather than merely neutral.

That, rather than the lift programming, is the most likely explanation for stalled composition.

---

## 2. The model

Inputs marked ⬜ are estimates — **replace them with your real numbers** and the rest recomputes.

| Input | Example value | Notes |
|---|---|---|
| ⬜ Bodyweight | 175 lb / 79.4 kg | |
| ⬜ Body fat | ~15% | → FFM ≈ 149 lb / 67.5 kg |
| ⬜ Running volume | 35 mi/wk | 7 days; easy ×4, quality ×2, long ×1 |
| Lifting | 7 sessions/wk | ~35 min at giant-set density |

**Resting metabolic rate** (Katch-McArdle, FFM-based — the right formula for a lean trained
person):
`370 + (21.6 × 67.5 kg) = 1,828 kcal`

**Non-exercise activity + TEF** at ~1.3× (desk work): `1,828 × 1.3 ≈ 2,376 kcal`

**Exercise energy expenditure:**
- Running: `35 mi × 0.72 kcal/lb/mi × 175 lb ≈ 4,410/wk ≈ 630/day`
- Lifting: `7 × ~300 ≈ 2,100/wk ≈ 300/day`
- **Total ≈ 930 kcal/day**

**TDEE ≈ 2,376 + 930 ≈ 3,300 kcal/day**

### The result

| | Intake | EA calculation | **EA** | Verdict |
|---|---|---|---|---|
| **Deficit (−400)** | 2,900 | (2,900 − 930) ÷ 67.5 | **29.2** | 🔴 Below the LEA threshold |
| **Maintenance** | 3,300 | (3,300 − 930) ÷ 67.5 | **35.1** | 🟡 Adequate, not optimal |

**This is the finding.** At the current deficit you are plausibly sitting just *under* the low-
energy-availability line — not dramatically, but under it. That is a mechanistic explanation for
the stall, and it predicts that no amount of lift restructuring fixes composition while it holds.

Maintenance clears the threshold with room to spare but lands well short of the ~45 that's
optimal for tissue accrual. So maintenance makes the hypertrophy work *possible*; it does not
make it fast.

### Sensitivity

The conclusion is not fragile, but it moves with running volume:

| Running volume | Deficit EA | Maintenance EA |
|---|---|---|
| 25 mi/wk | 31.8 | 37.7 |
| **35 mi/wk** | **29.2** | **35.1** |
| 45 mi/wk | 26.6 | 32.5 |

More running pushes both scenarios down. Above ~40 mi/wk the deficit is unambiguously in LEA
territory, and even maintenance starts to look thin.

---

## 3. Scenario A — hold the deficit

**What it buys:** continued fat loss, roughly 0.4 lb/week at −400.

**What it costs:** hypertrophy, essentially entirely. Expect a brief apparent response in the
first 3–4 weeks purely because 4.0's stimulus is genuinely novel after 3.0's unchanging template
— then a return to stall. Run quality degrades slowly as carbohydrate availability tightens.
Recovery debt accumulates against a 7-day running week.

**How 4.0 should be built under this scenario** — throttled deliberately:

| Element | Deficit setting |
|---|---|
| Round counts | Low end: **3–5** |
| Wave loading | **Keep — it's ideal here.** Delivers a genuine heavy top set at minimal total volume, which is exactly what preserves muscle in a deficit |
| Finishers (Tue/Thu) | Keep but short — **2 rounds**. Cheap, and they deliver the sensation the pump problem is about |
| Intensifiers | **Weeks 5–7 only**, not 3–7. Drop sets in a deficit buy fatigue more than growth |
| Saturday rebuild | Moderate version |
| Honest goal | Preserve muscle · fix the pump · add strength on wave top sets. **Not grow.** |

**Macros at 2,900 kcal:**

| | Target | g/kg |
|---|---|---|
| Protein | **190 g** | 2.4 — deliberately high; protein needs *rise* in a deficit to protect lean mass |
| Fat | **70 g** | 0.9 — do not go below 0.8 g/kg; hormonal function is already under pressure |
| Carbohydrate | **378 g** | 4.8 — thin for this running load. Front-load onto quality Tue/Thu and long-run Saturday |

---

## 4. Scenario B — maintenance

**What it buys:** an anabolic-permissive environment. Slow recomposition becomes possible —
realistically **0.5–1.5 lb of lean mass per few months**, not per month, at 43, trained, running
seven days a week. Modest but real, and it compounds. Secondary gains show up faster than the
muscle does: better run quality at the same heart rate, better sleep, better recovery between
quality sessions, restored drive.

**What it costs:** the scale stops moving. If you're currently losing, maintenance will *feel*
like stopping — which is why the success metrics have to change (see §6).

**How 4.0 should be built under this scenario** — as designed:

| Element | Maintenance setting |
|---|---|
| Round counts | **4–6**, up to **8** on the slack days (Sat/Sun) |
| Wave loading | Full — Ramp, Classic, Pyramid, Double Wave across slots |
| Finishers (Tue/Thu) | **3–4 rounds** |
| Intensifiers | **Weeks 3–7** as originally scoped |
| Saturday rebuild | Full chest/arm session |
| Honest goal | Slow recomp with a real hypertrophic signal |

**Macros at 3,300 kcal:**

| | Target | g/kg |
|---|---|---|
| Protein | **165 g** | 2.1 |
| Fat | **75 g** | 0.95 |
| Carbohydrate | **491 g** | 6.2 — comfortable for 7-day running with two quality days and a long run |

---

## 5. Two things that apply either way

**Protein distribution matters more at 43 than it did at 33.** Anabolic resistance means older
muscle needs a larger per-meal dose to trigger protein synthesis — roughly **0.4–0.55 g/kg per
sitting**, so **32–44 g per meal across 4–5 feedings**, not 190 g arriving mostly at dinner.
A ~40 g pre-sleep casein dose is well supported for overnight synthesis in this age group.

**Fasted 4:30am training is a real handicap — for the lifting specifically.** For running it's
fine and arguably useful. For hypertrophy it means training in a catabolic state at the daily
cortisol peak with no circulating amino acids, and that compounds with a deficit.

The brief carries fasted training over unchanged, so this is flagged as a **lever, not a
prescription**: 20–25 g of whey or EAAs on waking would meaningfully change the lifting response
while leaving essentially all of the fasted-run adaptations intact. It's the single
highest-leverage change available that doesn't touch total calories. Worth considering
independently of the deficit/maintenance decision.

**Deload weeks (week 8) should not drop calories.** That's when the recovery you've been
deferring actually gets taken.

---

## 6. Success metrics — they differ

Scale weight is the wrong instrument for the maintenance scenario, and using it will make a
working program look like a failing one.

| | Deficit | Maintenance |
|---|---|---|
| Bodyweight | Down ~0.4 lb/wk | **Flat — this is success, not stagnation** |
| Waist circumference | Down | Flat or slowly down |
| Wave top-set loads | Hold | **Up** |
| Run pace at fixed HR | Flat or slowly worse | **Improves** |
| Progress photos | Every 4 weeks | Every 4 weeks — the primary instrument here |
| Deload-week 3-mile TT | Flat | Flat or improving |

---

## 7. Recommendation

**Run maintenance**, and build 4.0 at the full settings in §4.

The reasoning is narrow and doesn't depend on the exact numbers: at your training volume the
deficit is close enough to the LEA threshold that it plausibly explains the stall on its own, and
every hour spent restructuring the lifting is wasted while that holds. You can return to a
deficit later from a better hormonal baseline and hold more muscle through it than you would now.

If you'd rather keep losing fat first, that's entirely legitimate — but then build the **deficit
column** of the program and set expectations accordingly. The failure mode to avoid is building
the maintenance program and eating the deficit, which is roughly what 3.0 became.

---

## 8. To pin these numbers down

The model above uses estimates. Three real numbers would replace them:

1. **Current bodyweight** (and body fat, if you have a recent estimate)
2. **Current daily intake** — what the −400 deficit is actually 400 below
3. **Weekly running mileage** — or average session duration, which I can convert

With those, the EA figures become yours rather than illustrative, and I can say whether the
deficit is a near-miss or well under the line.
