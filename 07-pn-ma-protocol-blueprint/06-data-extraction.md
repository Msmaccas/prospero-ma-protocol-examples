# 06 — Data Extraction

**PRISMA-P items:** 13a (Data management), 13b (Data items)
**PROSPERO sections:** Data extraction (selection and coding), Data extraction from published articles and reports

---

## PART I: LEARNINGS & BEST PRACTICES

### 6.1 What Data to Extract

The examples show a standard set of extraction fields plus some domain-specific ones:

**Common fields across all examples:**
- Author(s), year, country, study design
- Sample size
- Participant demographics (age, gender, baseline condition)
- Intervention details (type, dose, frequency, duration)
- Outcomes (measurement tools, time points, results)

**Domain-specific additions:**

| Example | Additional fields unique to their topic |
|---------|----------------------------------------|
| #3 PN (Lampridou) | PN dose, PN administration mode, treatment area, cosmetic indication, follow-up duration |
| #4 ReCell | Skin cell suspension type, dosage, duration of intervention, preparation required area, available area for repair |
| #5 Exosomes | Exosome source (adipose, platelet, bovine milk), delivery method (topical, MN-assisted, laser-assisted) |

**For your PN review, you'll need:**
- PN formulation (PN vs PDRN vs PN-HPT) and manufacturer
- PN concentration and volume per session
- Number of treatment sessions and intervals between sessions
- Treatment area (periorbital, full face, perioral, neck)
- Delivery method (direct injection, microneedling-assisted, laser-assisted)
- Follow-up duration
- Outcome data at each time point (mean, SD, n per group for continuous; event counts for categorical)
- For split-face studies: within-patient correlation coefficient (if reported) or raw paired data

### 6.2 Extraction Process — What's Realistic for a Solo Reviewer

**Gold standard:** Dual independent extraction by two reviewers (#1, #3, #5)
**Pragmatic standard:** One person extracts, second person checks (#2, #6)
**Weak:** Not specified (#4)

**For you:** "Data will be extracted by one reviewer (TH) and verified by [supervisor] for a random sample of included studies" is realistic and transparent.

### 6.3 Handling Split-Face Data — The Key Technical Challenge

**This is perhaps the single most important methodological decision in your review.**

Split-face studies produce **paired data** — each patient contributes two observations (treated side and control side). The observations are correlated within each patient. Standard meta-analysis formulas that assume independence between groups (e.g., two-sample t-test formulas for SMD) will give incorrect variance estimates if applied to split-face data as if they were from separate groups.

**Options for handling paired data in meta-analysis:**

1. **Use paired analysis** (best, but requires within-patient correlation or raw difference scores)
   - Calculate the mean difference (MD) and SD of the difference within patients
   - If the SD of the difference is not reported, impute a correlation coefficient (typically 0.5 for skin halves in facial aesthetics)
   - Formula: SD_diff = sqrt(SD_pre² + SD_post² - 2 × r × SD_pre × SD_post)

2. **Treat as independent groups** (simpler, but conservative — yields wider CIs)
   - Treat each hemiface as an independent observation
   - This ignores within-patient correlation → potentially overestimates variance → wider confidence intervals → fewer significant findings

3. **Use one side only** (wasteful, discards data)
   - Take only the treated side data and compare to baseline (loses the controlled comparison)

**What the examples do:**
- None of the 6 examples explicitly address how they handle paired data from split-face studies. This is a notable gap in all of them (many include split-face designs but don't mention the paired-data issue).

**You should explicitly address this in your protocol.** This shows methodological sophistication and pre-specification.

---

## PART II: YOUR PROTOCOL DRAFT

### Draft Extraction Fields

> **General study information:**
> - Author(s), publication year, journal, country
> - Study design (parallel-group RCT, split-face RCT, controlled clinical trial)
> - Sample size (total participants; for split-face: number of hemifaces)
> - Funding source and conflict of interest declarations
>
> **Participant characteristics:**
> - Age (mean ± SD), sex distribution
> - Fitzpatrick skin type distribution (if reported)
> - Baseline skin condition/wrinkle severity
> - Prior aesthetic treatment washout period
>
> **Intervention details:**
> - PN formulation (PN, PN-HPT, PDRN) and manufacturer
> - PN concentration (mg/mL), volume per session (mL), and total dose
> - Number of treatment sessions, intervals between sessions
> - Injection technique (intradermal, subcutaneous, microinjection)
> - Delivery method (direct injection only vs. assisted by microneedling, laser, or topical)
> - Treatment area(s) (periorbital, full face, perioral, neck, combined)
>
> **Comparator details:**
> - Type of comparator (placebo, no treatment, HA, other active)
> - For split-face: which side received which treatment
>
> **Outcome data:**
> - For each outcome at each prespecified time point:
>   - Continuous: mean, SD, and n per group (parallel) or mean difference, SD of difference (paired/split-face)
>   - Categorical: event counts and total n per group
>   - For split-face studies: within-patient correlation coefficient for continuous outcomes if reported
> - Time points reported (baseline, post-treatment visits)
> - Instruments used (GAIS, WSRS, Cutometer, Corneometer, VISIA, etc.)
> - Assessor type (clinician, patient, independent rater, device)
>
> **Adverse events:**
> - Number and type of AEs per group
> - Severity grading (mild, moderate, severe) and duration
> - Proportion of patients experiencing ≥1 AE

### Draft Extraction Process

> Data will be extracted independently by two reviewers using a pre-piloted data extraction form in Covidence/Microsoft Excel. For split-face studies, paired data (mean difference and SD of the difference) will be extracted where reported. Where only pre- and post-treatment means and SDs per hemiface are reported, the SD of the within-patient difference will be imputed using a correlation coefficient of r = 0.5, consistent with published guidance for within-patient aesthetic trials. Sensitivity analyses will use correlation coefficients of r = 0.25 and r = 0.75 to assess the impact of this assumption.
>
> If required outcome data are not reported, study authors will be contacted by email (maximum 2 attempts, 2 weeks apart). If data remain unavailable, the study will be included in narrative synthesis but excluded from the relevant meta-analysis.

---

*References:*
- PRISMA-P 2015 items 13a–13b. Shamseer et al. BMJ 2015;349:g7647
- Cochrane Handbook v6.5, Chapter 5: Collecting data
- For paired data from split-face designs: Higgins JPT, White IR, Anzures-Cabrera J. Meta-analysis of skewed data: combining results reported on log-transformed or raw scales. Stat Med. 2008;27(29):6072-92
- For correlation coefficient assumptions in within-patient studies: Abrams KR, Gillies CL, Lambert PC. Meta-analysis of heterogeneously reported trials assessing change from baseline. Stat Med. 2005;24(24):3823-44
