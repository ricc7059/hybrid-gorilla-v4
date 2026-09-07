# Nutrition — Deficit vs. Maintenance

Two scenarios modeled side by side on **real inputs** (2026-09-07). Surplus is off the table by
decision and isn't modeled.

This decision gates session design — round counts, finisher volume, and the intensifier schedule
differ between the two scenarios.

---

## 1. The lens: energy availability

For a hybrid athlete, calorie balance is the wrong instrument. The right one is
**energy availability (EA)** — what's left to run the body *after* training takes its cut:

```
EA = (intake − exercise energy expenditure) ÷ kg fat-free mass
```

| EA (kcal/kg FFM/day) | State |
|---|---|
| **< 30** | Low energy availability. Testosterone, T3, IGF-1 fall. Muscle protein synthesis suppressed. |
| **30–45** | Adequate. Maintenance possible; adaptation muted toward the bottom of the band. |
| **~45** | Optimal for adaptation and tissue accrual. |

---

## 2. The model — your numbers

| Input | Value |
|---|---|
| Bodyweight | **210 lb / 95.25 kg** |
| Body fat | **12–18%** → FFM 78.1–83.8 kg (midpoint 81.0 kg) |
| Current intake | **3,300 kcal/day** |
| Running | **20–25 mi/wk** across 7 days |
| Lifting | 7 sessions/wk, ~35 min at giant-set density |

**RMR** (Katch-McArdle, FFM-based): `370 + (21.6 × 81.0) ≈ 2,120 kcal`
**+ non-exercise activity and TEF** at ~1.3×: `≈ 2,756 kcal`

**Exercise energy expenditure (net, above rest):**
- Running: `22.5 mi × 0.63 kcal/lb/mi × 210 lb ≈ 2,977/wk ≈ 425/day`
- Lifting: `7 × ~300 ≈ 2,100/wk ≈ 300/day`
- **Total ≈ 725 kcal/day**

**Modeled TDEE ≈ 2,756 + 725 ≈ 3,480 kcal/day**

### Result

| | Intake | EA | Verdict |
|---|---|---|---|
| **Current (3,300)** | 3,300 | **31.8** | 🟡 Above the LEA line, low in the adequate band |
| **Maintenance (~3,500)** | 3,500 | **34.3** | 🟡 Adequate |
| **Maintenance (3,700 if your −400 is right)** | 3,700 | **36.7** | 🟢 Comfortably adequate |

Across the whole 12–18% body-fat range the current figure only moves from **31.0 to 33.3** — so
the conclusion doesn't depend on pinning your body composition down.

---

## 3. Correction: you are not in low energy availability

My earlier illustrative model used 175 lb and 35 mi/wk and landed at EA 29.2 — under the
threshold. **Your actual numbers don't reproduce that.** At 210 lb with 20–25 mi/wk you're at
roughly **32**, which is above the line.

The difference is mostly running volume: at your mileage, running costs about 425 kcal/day, not
the ~630 I'd assumed. You carry more lean mass, which raises the denominator, but you also spend
much less on aerobic work, which raises the numerator more.

**So the brief's framing — "no restructuring of the lift program fixes this" — is too strong.**
Your deficit is suppressing adaptation modestly, not shutting it down. It is not the smoking gun.

### Then what did cause the stall?

Three things, in what I'd now judge as descending order of importance:

1. **The lift stimulus in 3.0 was genuinely insufficient.** Four of seven sessions at RIR 3,
   capped at ~25 minutes, with a byte-identical template for an entire 8-week block. That is a
   real and sufficient explanation on its own, and it's the one thing 4.0 directly fixes.
2. **Concurrent-training interference.** Seven days a week of running keeps AMPK signaling
   elevated against the mTOR signaling hypertrophy requires. Nutrition doesn't overcome this;
   only redistributing the running would, and running is out of scope.
3. **Training status and age.** 210 lb at 12–18% is already a well-developed physique. At 43,
   trained, with that much existing lean mass, further hypertrophy runs at maybe 1–2 lb of lean
   mass per *year* under good conditions. Some of the "stall" may be a calibration problem rather
   than a physiology problem.

**Net effect on the plan: the lift rebuild is now the bigger lever, and nutrition is the smaller
one.** That inverts the brief's priority — good news, since the lift rebuild is the part we
control.

### One loose thread worth pulling

You describe a −400 deficit at 3,300 intake, which implies maintenance ≈ 3,700. The model says
≈ 3,480. If the model is closer, **your actual deficit is nearer −180 than −400** — which would
independently explain slow fat loss.

Before committing either way, worth a **2–3 week audit**: hold intake at 3,300, weigh daily,
take the weekly average. Flat average means 3,300 *is* maintenance. That single measurement
resolves the discrepancy and costs nothing.

---

## 4. Scenario A — hold the deficit

**Buys:** continued fat loss. At a true −400, ~0.4 lb/wk; at a true −180, ~0.2 lb/wk.

**Costs:** hypertrophy runs muted rather than absent. EA ~32 supports maintenance of lean mass
and strength gains, but tissue accrual will be very slow. At your running volume, carbohydrate
isn't a limiting factor — run quality should hold.

**4.0 built under this scenario:**

| Element | Deficit setting |
|---|---|
| Round counts | **3–5** |
| Wave loading | **Keep — ideal here.** A genuine heavy top set at minimal total volume is exactly what preserves lean mass in a deficit |
| Finishers (Tue/Thu) | **2 rounds** |
| Intensifiers | **Weeks 5–7 only** |
| Saturday rebuild | Moderate |
| Honest goal | Preserve mass · fix the pump · add strength on wave top sets |

**Macros at 3,300:**

| | Target | g/kg |
|---|---|---|
| Protein | **220 g** | 2.3 — raised deliberately; protein needs climb in a deficit |
| Fat | **80 g** | 0.84 — floor is 0.8 g/kg for hormonal function |
| Carbohydrate | **425 g** | 4.5 — comfortable at 20–25 mi/wk |

---

## 5. Scenario B — maintenance

**Buys:** EA rises to ~34–37, moving adaptation from muted to reasonable. Realistic accrual is
still slow — call it **1–3 lb of lean mass over a full 8-week block**, and that's an optimistic
read given training age. Secondary effects arrive faster and more reliably: better recovery
between quality runs, better sleep, better session quality on the heavy days.

**Costs:** the scale stops moving. Fat loss pauses.

**The change is small.** You're 180–400 kcal from maintenance depending on whose number is right.
That's one meal component, not a diet overhaul — which makes this a cheap experiment with a
short path back.

**4.0 built under this scenario:**

| Element | Maintenance setting |
|---|---|
| Round counts | **4–6**, up to **8** on the slack days (Sat/Sun) |
| Wave loading | Full — Ramp, Classic, Pyramid, Double Wave across slots |
| Finishers (Tue/Thu) | **3–4 rounds** |
| Intensifiers | **Weeks 3–7** as scoped |
| Saturday rebuild | Full chest/arm session |
| Honest goal | Slow recomp with a real hypertrophic signal |

**Macros at ~3,600:**

| | Target | g/kg |
|---|---|---|
| Protein | **190 g** | 2.0 |
| Fat | **85 g** | 0.9 |
| Carbohydrate | **519 g** | 5.4 |

---

## 6. Applies either way

**Protein distribution matters more at 43 than the total does.** Anabolic resistance means the
per-meal dose has to clear a higher threshold: **0.4–0.55 g/kg per sitting = 40–52 g per meal**
at your bodyweight, across 4–5 feedings. 190 g arriving mostly at dinner does noticeably less
than 190 g spread properly. A ~40 g pre-sleep casein dose is well supported for overnight
synthesis in this age group.

**Fasted 4:30am training is a real handicap — for the lifting specifically.** Fine, arguably
useful, for the running. For hypertrophy it means training at the daily cortisol peak with no
circulating amino acids. The brief carries fasted training over unchanged, so this is a **lever,
not a prescription**: 20–25 g of whey or EAAs on waking would meaningfully improve the lifting
response while leaving the fasted-run adaptations essentially intact.

Given that nutrition turns out to be the *smaller* lever here, this one is arguably the highest-
value nutritional change available to you — it targets the lifting directly, costs almost no
calories, and doesn't require choosing between deficit and maintenance at all.

**Deload weeks (week 8) shouldn't drop calories.** That's when deferred recovery gets taken.

---

## 7. Success metrics

| | Deficit | Maintenance |
|---|---|---|
| Bodyweight | Down 0.2–0.4 lb/wk | **Flat — that's success, not stagnation** |
| Waist circumference | Down | Flat or slowly down |
| Wave top-set loads | Hold or slowly up | **Up** |
| Run pace at fixed HR | Flat | Flat or improving |
| Progress photos | Every 4 weeks | Every 4 weeks — the primary instrument |
| Deload-week 3-mile TT | Flat | Flat or improving |

---

## 8. Recommendation

**Run maintenance — but the case is weaker than I first stated, and the reason has changed.**

It's no longer "you're suppressing your endocrine system." It's simply that you're 180–400
calories from a better adaptive environment, the change is trivially small, and there's no
competing goal — you've already decided fat loss isn't the priority for this phase.

Two caveats worth holding onto:

- **Don't expect the nutrition change to be what fixes this.** On your numbers, the insufficient
  lift stimulus in 3.0 is the better explanation for the stall. 4.0's programming is the main
  intervention; maintenance just removes a modest brake.
- **Audit true maintenance first** (§3). Three weeks of daily weights at 3,300 tells you whether
  you're at −400 or −180, and that determines how much you're actually adding.

If you'd rather keep the deficit, that's a perfectly reasonable call at EA 32 — build the
**deficit column** and expect strength and pump, not size. The failure mode to avoid is building
the maintenance program and eating the deficit, which is roughly what 3.0 became.
