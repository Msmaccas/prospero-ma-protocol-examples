# 08 — Data Synthesis (Meta-Analysis Plan)

**PRISMA-P items:** 15a (Data synthesis — narrative), 15b (Data synthesis — quantitative), 15c (Data synthesis — heterogeneity), 16 (Meta-bias)
**PROSPERO sections:** Strategy for data synthesis, Analysis of subgroups or subsets

---

## PART I: LEARNINGS & BEST PRACTICES

### 8.1 What a Good Synthesis Plan Looks Like

The 6 examples reveal a **clear hierarchy of synthesis ambition:**

| Example | Approach | Model | Heterogeneity plan | Software |
|---------|----------|-------|-------------------|----------|
| #1 BTX-A+HA | MA planned (contingent on homogeneity) | Fixed or random (depending on I²) | I² 25/50/75 thresholds, subgroup analysis, sensitivity, meta-regression | Not specified |
| #2 Collagen | MA planned (random-effects) | Random-effects (assumed heterogeneous) | I², subgroup by study design and agent type | Not specified |
| #3 PN (Lampridou) | Narrative (MA if ≥3 studies on same outcome) | N/A (contingent) | I² briefly mentioned | Not specified |
| #4 ReCell | MA planned | Fixed (I²<50%) or random (I²>50%) | I², subgroup, leave-one-out sensitivity, Egger's test, trim-and-fill, fail-safe N | StataSE 15.1 ✓ |
| #5 Exosomes | MA planned | Fixed (homogeneous) or random (heterogeneous) | I²>50%, χ² test p<0.10, subgroup, meta-regression | Not specified |
| #6 RFMN | Narrative/thematic only | N/A (qualitative) | N/A | Excel |

**#4 (Lou) has the most detailed synthesis plan** — and it's the right model for you. They pre-specify:
- When to use fixed vs random effects (by I² threshold)
- Multiple heterogeneity exploration methods (subgroup, sensitivity)
- Multiple publication bias methods (Egger's, funnel, trim-and-fill, fail-safe N)
- **Named software (StataSE 15.1)** — this matters for credibility
- Explicit significance thresholds

### 8.2 The Random-Effects Decision

**For your PN review, a random-effects model is almost certainly appropriate.** Here's why:

1. **Clinical heterogeneity is expected** — different PN formulations (PN vs PDRN vs PN-HPT), different treatment areas, different outcome instruments
2. **Statistical heterogeneity is likely** — you're pooling across small studies with variable effect sizes
3. **Generalisation is the goal** — you want to estimate the average treatment effect across a range of clinical scenarios

The examples show that random-effects is the default for most aesthetic derm MAs (#2, #5). Fixed-effects is only appropriate when you believe there is ONE true effect and all studies estimate the same thing — unlikely in PN research.

**You should still describe the conditions under which you'd use each model.**

### 8.3 Heterogeneity Exploration

**Minimum plan:**
- I² statistic (25%/50%/75% thresholds)
- Chi-squared test (p<0.10 threshold, as per Cochrane)

**If heterogeneity is moderate-high (I² > 50%):**
- Pre-specified subgroup analyses (see 8.4)
- Leave-one-out sensitivity analysis
- Meta-regression if ≥10 studies

### 8.4 Subgroup Analyses — Planned in Advance

From the examples:

| Example | Subgroup variables | Strength |
|---------|-------------------|----------|
| #1 | Treatment type (simultaneous vs sequential), baseline skin condition | Well-motivated |
| #2 | Type of biostimulator, study design (RCT vs non-RCT) | Clear, testable |
| #5 | Mode of application (topical/MN/laser), exosome source | Well-motivated |
| #3 | None planned | Weakness |
| #6 | RF modality (exploratory) | Appropriate for qualitative |

**For your PN review, pre-specify:**

1. **PN formulation type** (standard PN vs PN-HPT vs PDRN) — different formulations may have different potency
2. **Treatment area** (periorbital only vs. full face vs. neck) — periorbital skin may respond differently
3. **Comparator type** (placebo/saline vs. HA filler vs. no treatment vs. baseline)
4. **Study design** (parallel-group RCT vs. split-face RCT vs. non-randomised) — study design is a known source of bias

### 8.5 Sensitivity Analyses

**Essential sensitivity analyses from the examples:**
- **Leave-one-out analysis** (#4) — removing one study at a time to check if any single study drives the result
- **Risk of bias** (#5, #2) — excluding high-risk studies to see if the result changes
- **Fixed vs random effects** — reporting both and noting discrepancies
- **Correlation assumption** (for split-face data) — testing r=0.25, r=0.5, r=0.75

### 8.6 Software

**From the examples:** Only #4 (Lou) specifies software — StataSE 15.1. This is a strength, not a minor detail.

**Options for you:**
- **R** (meta or metafor packages) — free, powerful, reproducible
- **RevMan** — Cochrane's free software, easier but less flexible
- **Stata** — institutional license may be available
- **Jamovi/JASP** — free, GUI-based

Name the software and packages you'll use. This shows you've thought about implementation.

---

## PART II: YOUR PROTOCOL DRAFT

### Draft Data Synthesis Plan

> **Narrative synthesis:** A narrative synthesis of all included studies will be conducted regardless of meta-analysis feasibility. Studies will be tabulated by design (parallel-group RCT vs. split-face RCT vs. non-randomised controlled trial) and summarised in terms of participant characteristics, PN formulation, treatment protocol, outcome measures, and key findings.
>
> **Quantitative synthesis (meta-analysis):**
>
> A meta-analysis will be performed when ≥2 studies report the same outcome construct (e.g., GAIS, wrinkle severity, skin elasticity) at comparable time points using combinable data.
>
> **Effect measures:**
> - Continuous outcomes (GAIS scores, Cutometer parameters, Corneometer values, wrinkle grading scales): standardised mean difference (SMD) with Hedges' g correction will be used when different instruments measure the same construct. Mean difference (MD) will be used when the same instrument or measurement unit is used across studies.
> - Dichotomous outcomes (proportion of patients reporting improvement, incidence of adverse events): risk ratio (RR) with 95% confidence intervals.
> - For split-face studies, the SMD or MD will be calculated using the within-patient mean difference and its standard deviation. If individual patient data are available, paired analyses will be conducted directly.
>
> **Meta-analysis model:** A random-effects meta-analysis will be used as the primary approach for all analyses, given the anticipated clinical and methodological heterogeneity across studies (different PN formulations, treatment areas, outcome instruments, and study designs). A fixed-effects model will be reported as a sensitivity analysis for comparison.
>
> **Heterogeneity assessment:**
> - Statistical heterogeneity will be quantified using the I² statistic, with thresholds of 25% (low), 50% (moderate), and 75% (high).
> - The chi-squared test for heterogeneity will be considered significant at p<0.10.
> - If moderate-to-high heterogeneity is detected (I² > 50%), sources will be explored through pre-specified subgroup analyses and, if ≥10 studies are available, random-effects meta-regression.
>
> **Subgroup analyses (pre-specified):**
> 1. PN formulation: PN-HPT vs. standard PN vs. PDRN
> 2. Treatment area: periorbital only vs. pan-facial vs. neck
> 3. Comparator type: placebo/saline vs. active comparator (HA, other biostimulators) vs. baseline
> 4. Study design: parallel-group RCT vs. split-face RCT vs. non-randomised study
>
> **Sensitivity analyses:**
> 1. Leave-one-out analysis (removing each study sequentially to assess its influence)
> 2. Restricting to studies at low risk of bias (RoB 2 overall judgment)
> 3. Fixed-effects model (vs. primary random-effects model)
> 4. For split-face studies: varying the assumed within-patient correlation (r = 0.25, 0.5, 0.75) for outcome SD imputation
> 5. Publication bias-adjusted estimates using trim-and-fill (if ≥10 studies)
>
> **Publication bias:** Funnel plots will be visually inspected for asymmetry. Egger's regression test will be used for statistical assessment (if ≥10 studies). The Duval and Tweedie trim-and-fill method will estimate an adjusted effect size. Fail-safe N will be calculated.
>
> **Software:** All analyses will be conducted in R (version 4.x) using the `meta` (Schwarzer, 2024) and `metafor` (Viechtbauer, 2010) packages. RevMan 5.4 (Cochrane) will be used for forest plot generation if needed. The metafor package will be used for meta-regression. All code will be made available as supplementary material.

### 8.7 The SWiM Framework for Narrative Synthesis

The SWiM (Synthesis Without Meta-analysis) guidelines (Campbell et al., BMJ 2020, doi:10.1136/bmj.l6890) should be referenced if narrative synthesis is needed. Pre-specify:

> **SWiM Item 1 — Grouping:** Studies grouped by (a) PN formulation (PN-HPT vs standard PN vs PDRN), (b) treatment area (periorbital, full-face, neck), (c) comparator type (placebo, HA, other).
>
> **SWiM Item 2 — Standardised metric:** Proportion of patients achieving ≥1-point GAIS improvement. If ≥3 studies report this, it's the primary narrative focus.
>
> **SWiM Item 3 — Synthesis method:** No vote-counting for N<15/arm. Structured narrative comparing effect sizes, CIs, and study characteristics.
>
> **SWiM Item 4 — Data presentation:** Structured tables per outcome group with study characteristics, effect estimate (95% CI), RoB, direction of effect.

### 8.8 Meta-Analysis Decision Tree

> **Meta-analysis performed if:** ≥2 studies report the same outcome at a comparable time point, sufficient clinical homogeneity, and data obtainable.
>
> **Narrative synthesis (SWiM) if:** insufficient studies, excessive heterogeneity (I² > 75% post-subgrouping), or incompatible outcome measures.
>
> **Decision rule:** If I² > 75% after subgroup analysis and sensitivity exploration, and direction of effect is inconsistent across subgroups, pooling is abandoned for narrative synthesis.

---

*References:*
- PRISMA-P 2015 items 15a–15c, 16. Shamseer et al. BMJ 2015;349:g7647
- Cochrane Handbook v6.5, Chapter 10: Analysing data and undertaking meta-analyses. Section 10.10: Heterogeneity
- Chapter 11: Network meta-analyses. Section 11.2: Data synthesis
- Decks JJ, Higgins JPT, Altman DG (eds). Chapter 10: Analysing data and undertaking meta-analyses. In: Cochrane Handbook. 2024
- Viechtbauer W. Conducting meta-analyses in R with the metafor package. J Stat Softw. 2010;36(3):1-48. doi:10.18637/jss.v036.i03
- Balduzzi S, Rücker G, Schwarzer G. How to perform a meta-analysis with R: a practical tutorial. Evid Based Ment Health. 2019;22(4):153-160. doi:10.1136/ebmental-2019-300117
