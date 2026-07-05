# 05 — Outcomes

**PRISMA-P items:** 5 (Outcomes), 12 (Data items)
**PROSPERO sections:** Main outcomes, Additional outcomes, Measures of effect

---

## PART I: LEARNINGS & BEST PRACTICES

### 5.1 What Makes a Good Outcome Specification

**The examples show a spectrum of specificity:**

| Example | Primary outcome | Secondary outcomes | Specificity grade |
|---------|----------------|-------------------|------------------|
| #1 BTX-A+HA | Clinical efficacy (WSRS/GAIS), Patient satisfaction (PROMs), Safety (AEs) | None listed | Strong — names instruments, timing |
| #2 Collagen | GAIS (physician- or patient-assessed) | Other aesthetic/satisfaction/durability outcomes | Strong — single primary, flexible secondary |
| #3 PN | "Influence of PN on skin layers; skin regeneration; hair restoration" | AEs, QoL | Weak — vague, no named instruments |
| #4 ReCell | Complete epithelialization healing time | 10 secondary outcomes (preparation area, pain, scar score, DLQI, etc.) | Excellent — objective primary, comprehensive secondary |
| #5 Exosomes | GAIS, wrinkle reduction (PRIMOS/VISIA) | 6 domains (pigmentation, elasticity, texture, histology, AEs, satisfaction) | Strong — named devices and scales |
| #6 RFMN | Qualitative (patient/clinician perceptions, satisfaction narrative) | None | Appropriate for qualitative design |

> **⚠️ Observation:** #3 Lampridou (the existing PN SR) has the weakest outcome specification of all 6 examples. "Influence of PN on the anatomy and physiology of different skin layers" is not an outcome — it's a mechanism. This vagueness likely contributed to their inability to perform meta-analysis: you can't pool data if you haven't specified what you're pooling.

**For your protocol: specificity is everything.** As a meta-analysis, you must pre-specify:
- What your primary outcome is (the one that drives sample size / power)
- What instruments/measurement methods you accept for each outcome
- What time points you will analyse
- How you will handle multiple instruments measuring the same construct

### 5.2 Outcome Instruments Used in PN Research

From the user's identified papers and the broader literature, the common instruments include:

| Instrument | What it measures | Type | Used in PN studies |
|------------|-----------------|------|-------------------|
| GAIS (Global Aesthetic Improvement Scale) | Overall aesthetic improvement | 5-point clinician/patient scale | ✓ (Jeong 2020, Lee 2022, Araco 2023) |
| WSRS (Wrinkle Severity Rating Scale) | Wrinkle severity | 5-point scale | ✓ (Jeong 2020) |
| Cutometer | Skin elasticity (R0-R7 parameters) | Suction device | ✓ (Araco 2023) |
| Corneometer | Skin hydration | Capacitance device | ✓ (Araco 2023) |
| VISIA | Wrinkle, texture, pore, pigmentation analysis | Multispectral imaging | ✓ (Choi 2025) |
| PRIMOS | 3D wrinkle depth/area | Optical profilometry | ✓ |
| VAS (Visual Analog Scale) | Patient satisfaction, pain | 0–10 or 0–100 scale | ✓ |
| DLQI (Dermatology Life Quality Index) | QoL impact | 10-item questionnaire | ✓ |
| MELASQoL | Melasma-specific QoL | 10-item questionnaire | ✓ |
| Investigator/Subject Satisfaction | Satisfaction | Various Likert scales | ✓ |

**Critical issue for meta-analysis:** Different instruments measure the same construct (e.g., "wrinkle improvement") in different units and ranges. You need to pre-specify how you will standardise — typically by using **standardised mean difference (SMD)** for continuous outcomes when instruments differ across studies.

### 5.3 Primary vs Secondary — What PROSPERO Expects

PROSPERO's form asks you to distinguish:
- **Main outcomes** — the outcomes that drive your review question
- **Additional outcomes** — everything else you'll collect

**Best practice from the examples:**
- 1 primary outcome (the one most consistently reported across trials)
- 3–6 secondary outcomes covering different domains
- Each outcome should specify: measurement tool, timing, who assesses (clinician vs patient)

### 5.4 Time Point Specification

Aesthetic treatments have multiple follow-up time points (4 weeks, 3 months, 6 months). **You cannot pool 4-week and 6-month data in the same analysis without justification.**

From the examples:
- #1 BTX-A+HA specified: "baseline, 4 weeks, 3 months, 6 months"
- #5 Exosomes: "All time points reported for GAIS will be included" (flexible, but risks heterogeneity)

**Recommended approach:**
- Pre-specify your primary time point (e.g., 3 months post-treatment — most common in PN trials)
- If multiple time points reported, use the primary time point for main analysis
- Analyse other time points as sensitivity analyses (to see if effect is durable)

---

## PART II: YOUR PROTOCOL DRAFT

### Draft Outcomes

> **Primary outcome:**
> **Global Aesthetic Improvement** — measured by the Global Aesthetic Improvement Scale (GAIS) or equivalent clinician- or patient-reported global improvement instrument at 3 months post-treatment (or the nearest available time point). GAIS is the most consistently reported outcome across PN trials and allows standardisation across studies. Where GAIS is reported as a categorical variable (improved vs not improved), risk ratios will be calculated. Where GAIS is reported as a continuous variable (mean score), standardised mean differences will be used.
>
> **Secondary outcomes:**
> 1. **Wrinkle severity** — measured by the Wrinkle Severity Rating Scale (WSRS), or validated wrinkle grading scales, or 3D imaging systems (PRIMOS, VISIA). Primary analysis at 3 months. Reported as SMD.
> 2. **Skin elasticity** — measured by Cutometer (R2 gross elasticity, or other elasticity parameters). Reported as SMD.
> 3. **Skin hydration** — measured by Corneometer capacitance values. Reported as mean difference (MD) if same instrument used across studies, or SMD if different instruments.
> 4. **Patient satisfaction** — measured by patient-reported satisfaction scales or Visual Analog Scale. Reported as SMD.
> 5. **Safety/adverse events** — incidence and type of adverse events (injection site reactions, bruising, swelling, pain, nodule formation, asymmetry). Reported as risk ratios where comparator data available; otherwise as narrative summary.
>
> **Time points:**
> - Primary analysis time point: 3 months (range: 8–16 weeks)
> - Secondary time points for sensitivity analyses: 1 month (≤6 weeks) and 6 months (≥20 weeks)
> - If multiple time points are reported, the time point closest to 3 months will be used for the primary analysis
>
> **Handling multiple instruments:**
> Where different instruments measure the same outcome construct (e.g., Cutometer R2 and R5 for elasticity; VISIA and PRIMOS for wrinkle depth), the standardised mean difference (SMD) with Hedges' g correction will be used to pool across instruments. For each instrument, the direction of effect will be standardised so that higher values represent improvement.

---

*References:*
- PRISMA-P 2015 item 5 (Outcomes) and item 12 (Data items). Shamseer et al. BMJ 2015;349:g7647
- Cochrane Handbook v6.5, Chapter 18: Patient-reported outcomes. Section 18.4: Selecting measures
- Williamson PR, Altman DG, Bagley H, et al. The COMET Handbook: version 1.0. Trials. 2017;18(Suppl 3):280. doi:10.1186/s13063-017-1978-4 (core outcome set methodology)
- For GAIS use in aesthetic trials: Carruthers A, Carruthers J. A validated facial grading scale: the future of facial ageing measurement. Dermatol Surg. 2010;36(Suppl 3):1762-71
- For Cutometer parameters in PN research: Araco A, et al. J Cosmet Dermatol. 2023;22(1):101-110
