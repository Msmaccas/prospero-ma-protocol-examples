# 02 — Review Objectives & PICO Framework

**PRISMA-P items:** 3 (Objectives), 4 (Eligibility criteria — PICO), 5 (Outcomes)
**PROSPERO sections:** Review question, Objectives, PICO breakdown

---

## PART I: LEARNINGS & BEST PRACTICES

### 2.1 What Objectives Look Like in Practice

The 6 examples show two distinct approaches:

**Approach A — Question format (PICO as a question):**
> "What are the comparative clinical efficacy, patient satisfaction, and safety outcomes for patients undergoing botulinum toxin type A and hyaluronic acid combination therapy against those undergoing botulinum monotherapy?" *(CRD42024559256 — Yassa & Attar)*

This works well for a single, focused comparative question. It forces you to state the comparator explicitly.

**Approach B — Declarative statement (objectives as action items):**
> "To systematically evaluate and compare the aesthetic outcomes of collagen biostimulator injections for facial rejuvenation using the Global Aesthetic Improvement Score (GAIS) as the primary outcome measure." *(CRD420251020585 — Tiewrungruangsuk & Kaewkes)*

> "To evaluate the effectiveness of exosome-based therapies in facial rejuvenation compared to standard or placebo treatments in human clinical studies." *(CRD420250655353 — Stack et al.)*

Approach B is more common in PROSPERO records and maps better to the PROSPERO form, which asks for "Review question(s)/Objectives" as a structured field.

**Approach C — Multiple objectives (primary + secondary):**
The Exosomes record (#5) is the gold standard here:
- Primary: "To evaluate the effectiveness..."
- Secondary: 5 bullet points covering specific outcomes, delivery methods, sources, adverse effects, and quality assessment

**What works best:**
- A single primary objective (the main meta-analysis question)
- 2–4 secondary objectives (subgroup analyses, safety, quality assessment)
- Each secondary objective should map to a planned analysis (not just wishful thinking)

### 2.2 The PICO Framework — Getting It Right

**PROSPERO specifically asks you to break down:**
- Population (P)
- Intervention (I)
- Comparator (C)
- Outcomes (O)
- Study design (S) — sometimes added as PICOS

**From the examples, here's what a good PICO looks like:**

**Population — be specific but not overly restrictive:**

| Example | Population phrasing | What makes it good |
|---------|-------------------|-------------------|
| #1 BTX-A+HA | "Adults (likely middle-aged to older adults) seeking treatment for facial wrinkles, volume loss, and other signs of aging" | Broad enough to capture the clinical reality, specific enough to exclude irrelevant populations |
| #2 Collagen | "Healthy adults (≥18 years) receiving collagen biostimulator injections for facial aesthetics" | Age cut-off, health status specified |
| #4 ReCell | "Patients of all ages with skin lesion caused by different reasons and complete the trial in hospital" | Too broad — no age floor, no specific condition |

**For your PN protocol:** Population is relatively straightforward — adults receiving PN for facial rejuvenation. But you need to decide: do you include studies that combine PN with other treatments (microneedling, laser)? The example protocols show that combination treatments are usually included if the primary intervention data can be isolated.

**Intervention — list formulations explicitly:**

The collagen biostimulators protocol (#2) does this well:
> "Including but not limited to poly-L-lactic acid (PLLA), calcium hydroxylapatite (CaHA), polydioxanone (PDO), poly-D,L-lactic acid (PDLLA), and polycaprolactone (PCL)."

For your PN protocol: list PN, PDRN, PN-HPT, specify formulations, concentrations, and delivery methods.

**Comparator — a critical decision for your review:**

The examples show three patterns:
- **Active comparator:** BTX-A+HA vs BTX-A alone (#1)
- **Placebo/sham:** Saline or sham intervention (#5 Exosomes)
- **Baseline/within-patient:** Pre- vs post-treatment in split-face designs (#3 Polynucleotides, #6 RFMN)
- **No comparator:** Studies without comparators included for narrative data (#6 RFMN)

**For YOU:** Your review's comparator decisions are nuanced because you have split-face studies (one side PN, other side control/HA/no treatment) AND parallel-group RCTs. Your PICO must acknowledge both designs.

### 2.3 The Split-Face Design Challenge

Split-face (within-patient) trials are common in aesthetic dermatology but methodologically distinct from parallel-group RCTs. **PROSPERO does not have a dedicated field for split-face designs**, so you need to handle this in your description.

**What the existing PN PROSPERO (#3 Lampridou) did:**
> "All study types with a pre-intervention/post-intervention and/or a control group (standard of care or group with no intervention) and/or alternative method of skin rejuvenation."

This is vague — it includes split-face by implication but doesn't address the paired-data implications.

**What you should do instead:**
- Explicitly name split-face/split-body RCTs as eligible designs
- Note that paired data from split-face studies will be handled using paired analysis methods (accounting for within-patient correlation)
- State whether you will treat split-face data as paired or (if raw paired data unavailable) use a conservative approximation

### 2.4 PRISMA-P Requirements

PRISMA-P item 3 specifies:
> "State the research question, including the participants, interventions, comparators, and outcomes (PICO)."

The E&E paper emphasises that the objective should be **"specific, clear, and unambiguous"** — vague objectives lead to vague reviews.

---

## PART II: YOUR PROTOCOL DRAFT

### Draft Objectives

> **Primary objective:**
> To evaluate the efficacy of injectable polynucleotide (PN) and polydeoxyribonucleotide (PDRN) therapies for facial skin rejuvenation in adults, compared to placebo, no treatment, hyaluronic acid fillers, or other active comparators, as measured by validated clinician- and patient-reported outcome instruments.
>
> **Secondary objectives:**
> 1. To assess the impact of PN therapy on individual skin aging domains: wrinkle reduction (depth, area, severity), skin elasticity, hydration, texture, and pigmentation
> 2. To compare efficacy across PN formulations (PN-HPT, standard PN, PDRN) and delivery methods (injection alone vs. injection with microneedling or laser assistance)
> 3. To evaluate the safety profile of PN therapy by synthesising adverse event data (injection site reactions, bruising, swelling, nodule formation)
> 4. To assess the methodological quality of included studies and consistency of outcome measurement across trials

### Draft PICO Framework

> **Population (P):** Adults (≥18 years) of any sex, ethnicity, or Fitzpatrick skin type receiving injectable polynucleotide therapy for facial skin rejuvenation. Studies limited to periorbital rejuvenation, full-face treatment, or neck rejuvenation will be included. Studies of PN for non-rejuvenation indications (acne scars, wound healing, alopecia) will be excluded unless rejuvenation outcomes are separately reported.
>
> **Intervention (I):** Injectable polynucleotide (PN), highly purified polynucleotide (PN-HPT), or polydeoxyribonucleotide (PDRN) preparations administered via intradermal or subcutaneous injection for facial aesthetic purposes. All formulations, doses, treatment intervals, and injection techniques are eligible. Studies combining PN with concurrent procedures (microneedling, laser, topical delivery) will be included if the PN component can be isolated.
>
> **Comparator (C):** Placebo (saline or vehicle injection), no treatment (untreated control side in split-face designs), hyaluronic acid filler injections, other biostimulatory agents (CaHA, PLLA), or baseline within-patient comparison. Studies without a comparator arm will be included only for safety outcomes and descriptive synthesis.
>
> **Outcomes (O):** See section 05 for full outcome specification.
>
> **Study design (S):** Randomized controlled trials (parallel-group or split-face/split-body), prospective controlled clinical trials, and within-patient controlled trials. Case series, case reports, narrative reviews, and animal/in vitro studies will be excluded.

---

*References:*
- PRISMA-P 2015 checklist items 3–5. Shamseer et al. BMJ 2015;349:g7647
- Higgins JPT, Thomas J, Chandler J, et al. Cochrane Handbook for Systematic Reviews of Interventions version 6.5 (2024). Chapter 2: Determining the scope and questions
- For split-face design considerations: Leshem OA, et al. How to conduct and report a split-face study. J Am Acad Dermatol. 2024 (general guidance on within-patient trials in dermatology)
