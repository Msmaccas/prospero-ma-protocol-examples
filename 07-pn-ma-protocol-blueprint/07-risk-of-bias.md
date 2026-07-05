# 07 — Risk of Bias Assessment

**PRISMA-P items:** 14 (Risk of bias in individual studies)
**PROSPERO sections:** Risk of bias (quality) assessment

---

## PART I: LEARNINGS & BEST PRACTICES

### 7.1 Which Tool to Use — And Why It Matters

**The 6 examples use 4 different tools:**

| Tool | Used by | Best for |
|------|---------|----------|
| **Cochrane RoB 2** | #5 Exosomes (#1, #4 also mention it) | Parallel-group RCTs — gold standard |
| **ROBINS-I** | #5 Exosomes (#2 also mentions) | Non-randomised controlled studies |
| **CASP checklists** | #3 PN (Lampridou) | Mixed study designs — quick, study-design-specific |
| **JBI checklists** | #6 RFMN (Kumar) | Qualitative studies and non-RCTs |

**Which tool is right for YOUR review?**

Your studies are primarily:
1. **Parallel-group RCTs** → **Cochrane RoB 2** (Sterne et al., BMJ 2019)
2. **Split-face RCTs** → **Cochrane RoB 2** (modified for within-patient design — see below)
3. **Non-randomised controlled trials** → **ROBINS-I** (Sterne et al., BMJ 2016)

**Why NOT CASP or JBI:** While CASP is simpler and faster, it generates domain-level assessments without an overall risk-of-bias judgment. RoB 2 gives you "low risk / some concerns / high risk" which is what GRADE and meta-analyses expect.

### 7.2 The RoB 2 Domains and Your Studies

RoB 2 has 5 domains:
1. **Randomisation process** — Was the allocation sequence random? Was it concealed?
2. **Deviations from intended interventions** — Were participants and personnel blinded?
3. **Missing outcome data** — Was loss to follow-up low and balanced?
4. **Measurement of the outcome** — Was the outcome assessor blinded?
5. **Selection of the reported result** — Is there evidence of selective reporting?

**For split-face designs specifically:**

Domain 1 (Randomisation) is different in split-face trials — the unit is the hemiface, not the patient. The key question is: which side gets which treatment? Was this randomly allocated? Was the allocation concealed from the injector?

Domain 4 (Outcome measurement) is critical — split-face studies typically blind the outcome assessor (patient and/or independent rater) to which side received which treatment. If blinding is successful, this is a strength. If the patient knows which side is which, this is a major source of bias.

**Lampridou (#3)** used CASP — the simpler approach. But for a meta-analysis, **you need RoB 2**. This is another way your protocol differentiates from the existing PN SR.

### 7.3 Reporting Bias (Publication Bias)

**What the examples do:**
- #2 Collagen: "visual inspection of funnel plots and Egger's test for small-study effects" — standard
- #4 ReCell: Egger's regression test + "trim and fill" method + fail-safe N — comprehensive
- #5 Exosomes: funnel plots + Egger's test (if >10 studies) — standard
- Others: not specified

**For your review:** Publication bias is a real concern in aesthetic dermatology because:
- Small studies with positive results are more likely to be published
- Industry-sponsored studies may not publish negative results
- Split-face studies with small sample sizes (n=10–30) are common

The fail-safe N approach (#4) adds an extra layer that demonstrates robustness.

### 7.4 Certainty of Evidence (GRADE)

**What the examples do:**
- #2 Collagen: explicit GRADE plan (high/moderate/low/very low) — best practice
- #5 Exosomes: mentions GRADE in context
- #6 RFMN: "Certainty of findings will not be assessed" — acceptable for qualitative reviews
- #1, #3, #4: not mentioned

**For your meta-analysis, you should plan to use GRADE.** This is expected by most journals (especially *J Cosmet Dermatol* and *Dermatol Surg*) for meta-analyses.

---

## PART II: YOUR PROTOCOL DRAFT

### Draft Risk of Bias Assessment Plan

> **Primary tool:** The revised Cochrane Risk of Bias tool for randomized trials (RoB 2) will be used to assess all included randomized controlled trials, including split-face/split-body designs.
>
> **Split-face adaptations:** For split-face trials, the RoB 2 tool will be applied with the following domain-specific considerations:
> - Domain 1 (Randomisation): Assessment will focus on the method of allocating which hemiface receives the intervention vs. control (e.g., computer-generated random sequence, coin toss, minimisation). Allocation concealment at the hemiface level will be assessed.
> - Domain 2 (Deviations from intended interventions): Assessor blinding will be evaluated — specifically, whether the treating clinician was blinded to the side allocation at the time of injection.
> - Domain 4 (Measurement of outcome): The blinding of the outcome assessor (whether clinician, independent rater, or patient/device) is of particular importance in split-face designs.
>
> **Non-randomised studies:** For non-randomised controlled trials, the ROBINS-I tool (Risk of Bias in Non-randomised Studies of Interventions) will be used.
>
> **Assessment process:** Two reviewers will independently assess risk of bias. Disagreements will be resolved through discussion; a third reviewer (supervisor) will be consulted if necessary. Results will be presented as domain-level judgments (low risk / some concerns / high risk) and as an overall per-study judgment, following Cochrane guidance.
>
> **Reporting bias:** Publication bias will be assessed through visual inspection of funnel plot asymmetry for meta-analyses including ≥10 studies. Egger's regression test will be used as a statistical test for funnel plot asymmetry. If evidence of publication bias is detected, the Duval and Tweedie "trim and fill" method will be used to estimate an adjusted effect size accounting for potentially missing studies. The fail-safe N will be reported to indicate the number of null studies needed to推翻 the observed effect.
>
> **Certainty of evidence (GRADE):** The Grading of Recommendations, Assessment, Development and Evaluations (GRADE) approach will be used to assess the certainty of evidence for each outcome. Evidence will be rated as high, moderate, low, or very low based on: risk of bias, inconsistency (heterogeneity), indirectness, imprecision, and publication bias. A GRADE summary of findings table will be prepared for the primary outcome and key secondary outcomes.

---

*References:*
- Sterne JAC, Savović J, Page MJ, et al. RoB 2: a revised tool for assessing risk of bias in randomised trials. BMJ. 2019;366:l4898. doi:10.1136/bmj.l4898
- Sterne JA, Hernán MA, Reeves BC, et al. ROBINS-I: a tool for assessing risk of bias in non-randomised studies of interventions. BMJ. 2016;355:i4919. doi:10.1136/bmj.i4919
- Page MJ, McKenzie JE, Bossuyt PM, et al. The PRISMA 2020 statement: an updated guideline for reporting systematic reviews. BMJ. 2021;372:n71. doi:10.1136/bmj.n71
- GRADE Working Group. Grading quality of evidence and strength of recommendations. BMJ. 2008;336(7654):924-6. doi:10.1136/bmj.39489.470347.AD
- For split-face RoB considerations: Leshem OA, et al. Methodological considerations for split-face trials. J Am Acad Dermatol. 2024
