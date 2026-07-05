# 04 — Search Strategy

**PRISMA-P items:** 9 (Search strategy), 10 (Study records — data management), 11 (Study records — selection process)
**PROSPERO sections:** Searches, Study design, Selection process

---

## PART I: LEARNINGS & BEST PRACTICES

### 4.1 Database Selection — What the Examples Use

| Example | Databases | Adequacy |
|---------|-----------|----------|
| #1 BTX-A+HA | PubMed, Embase, Web of Science, Cochrane | Solid 4-database core |
| #2 Collagen | Cochrane Library, Embase, PubMed, Scopus, Google Scholar | Strong — adds Scopus and Google Scholar |
| #3 PN (Lampridou) | Embase, MEDLINE, Cochrane Library, ClinicalTrials.gov | Missing Web of Science |
| #4 ReCell | PubMed, Embase, Cochrane, Web of Science | Solid 4-database core |
| #5 Exosomes | MEDLINE (Ovid), Embase, Web of Science, Cochrane CENTRAL, ClinicalTrials.gov, DLINE, Trip | Most comprehensive — 7 sources |
| #6 RFMN | CENTRAL, LILACS, PubMed | **Weak** — only 3 databases, no Embase |

**For your PN review**, the minimum acceptable database set is:
1. **PubMed/MEDLINE** — biomedical core
2. **Embase** — broader pharma/aesthetic coverage than PubMed, many PN studies indexed here
3. **Web of Science / Scopus** (at least one) — catches interdisciplinary and cosmetic science journals
4. **Cochrane CENTRAL** — trial registry
5. **ClinicalTrials.gov** — unpublished/ongoing trials
6. **Google Scholar** (as supplement) — catches grey literature and non-indexed journals

### 4.2 Search String Construction

**What the examples do well:**
- #5 Exosomes provides the most complete approach: named specific databases with vendor details ("MEDLINE (Ovid, Ovid Therapeutics...), Embase (Elsevier...)")
- #2 Collagen uploaded a full search strategy PDF to PROSPERO — this is best practice
- #3 PN (Lampridou) kept it minimal: "Search terms include: 'polynucleotide', 'polydeoxyribonucleotide', 'aesthetic medicine' and 'facial aesthetic'" — too brief for reproducibility

**What the examples do poorly:**
- Most don't show their Boolean operators or MeSH term mappings
- Most don't describe how they adapted searches across databases (different syntax for PubMed vs Embase)
- None explicitly mention search filters (RCT filter, human filter)

**For your PN search string, considerations:**

Your user already has a draft Boolean search:
> (polynucleotide OR "PN" OR "polydeoxyribonucleotide" OR PDRN) AND (rejuvenation OR "skin" OR "anti-aging" OR "anti-wrinkle" OR "facial" OR "biostimulat*")

Issues to address:
- "PN" as a search term will generate massive noise (PN = parenteral nutrition, practice nurse, etc.) — consider removing or using in title-only
- Add formulation-specific terms: "PN-HPT", "highly purified polynucleotide"
- Add outcome-specific terms for sensitivity: "GAIS", "Cutometer", "VISIA", "elasticity", "hydration"
- Add study design terms for specificity: "split-face", "split-face", "randomized"

### 4.3 The Screening Process — What's Realistic

**Dual independent screening is the gold standard.** Here's how the examples handle it:

| Example | Screening model | Notes |
|---------|----------------|-------|
| #1 Yassa | 2 independent reviewers | Gold standard |
| #3 Lampridou | 2 independent reviewers + 3rd for arbitration | Gold standard + arbitration |
| #2 Tiewrungruangsuk | 1 reviewer, 2 rounds (separate Covidence accounts) | Creative but pragmatic — explicitly acknowledged resource limitation |
| #4 Lou | Not specified | Weakness |
| #6 Kumar | "At least 2 people (or person/machine combination)" | Pragmatic — acknowledges AI-assisted screening |

**For you:** Realistically, as a single junior researcher (MBChB student), you may not have 2 reviewers. The #2 model (single reviewer, two independent rounds via separate accounts) is a defensible approach that explicitly addresses resource limitations. If you have a collaborator (supervisor, fellow student), dual screening is always better.

### 4.4 Other Search Methods

**The examples identify three supplementary approaches:**
1. **Snowballing/reference checking** (#1, #2, #5) — looking through reference lists of included studies and existing reviews
2. **Citation tracking** (#2) — looking through articles that cite included studies
3. **Trial registry searching** (#6) — ClinicalTrials.gov, WHO ICTRP

**For your review:** All three are relevant. The existing Lampridou and Kream reviews have extensive reference lists that will likely identify studies your database search misses.

### 4.5 PRISMA-P Requirements

PRISMA-P item 9 specifies:
> "Present the planned search strategy in sufficient detail to be reproducible, including the planned search terms, databases, and any limits or filters."

The E&E paper emphasises that **the search strategy should be pilot-tested** and that presenting the strategy for at least one major database (typically PubMed/MEDLINE) is expected for reproducibility.

---

## PART II: YOUR PROTOCOL DRAFT

### Draft Database List

> **Electronic databases:**
> 1. PubMed/MEDLINE (via National Library of Medicine)
> 2. Embase (via Elsevier)
> 3. Web of Science Core Collection (via Clarivate)
> 4. Cochrane Central Register of Controlled Trials (CENTRAL)
> 5. Scopus (via Elsevier)
>
> **Trial registries:**
> 6. ClinicalTrials.gov (via US National Library of Medicine)
> 7. WHO International Clinical Trials Registry Platform (ICTRP)
>
> **Supplementary sources:**
> 8. Google Scholar (first 200 results sorted by relevance)
> 9. Reference lists of included studies and existing systematic reviews (Lampridou 2025, Kream 2026)

### Draft PubMed Search String

> **PubMed (MeSH + free text):**
> ```
> #1 "polynucleotides"[MeSH Terms]
> #2 "polydeoxyribonucleotide"[Title/Abstract]
> #3 "polynucleotide"[Title/Abstract]
> #4 "PN-HPT"[Title/Abstract]
> #5 "highly purified polynucleotide"[Title/Abstract]
> #6 "PDRN"[Title/Abstract]
> #7 #1 OR #2 OR #3 OR #4 OR #5 OR #6
> #8 "skin aging"[MeSH Terms]
> #9 "rejuvenation"[MeSH Terms]
> #10 "rejuvenation"[Title/Abstract]
> #11 "anti-aging"[Title/Abstract]
> #12 "anti-wrinkle"[Title/Abstract]
> #13 "facial"[Title/Abstract]
> #14 "skin"[Title/Abstract] AND ("elasticity"[Title/Abstract] OR "hydration"[Title/Abstract] OR "texture"[Title/Abstract])
> #15 #8 OR #9 OR #10 OR #11 OR #12 OR #13 OR #14
> #16 #7 AND #15
> #17 "randomized controlled trial"[Publication Type] OR "controlled clinical trial"[Publication Type]
> #18 "split-face"[Title/Abstract] OR "split face"[Title/Abstract] OR "within-patient"[Title/Abstract]
> #19 #17 OR #18
> #20 #16 AND #19
> #21 Limit #20 to: English language, Humans, Publication date 2015–2026
> ```

> This search will be adapted for each database's syntax and controlled vocabulary. The complete search strategies for all databases will be uploaded as a supplementary file to PROSPERO.

### Draft Screening Process

> **Title and abstract screening:** Titles and abstracts of all retrieved records will be independently screened by two reviewers against the predetermined eligibility criteria. If dual independent screening is not feasible due to limited personnel, a single reviewer will conduct two independent screening rounds using separate user accounts in the review management platform (Covidence), separated by a minimum of 7 days, to simulate independent verification.
>
> **Full-text screening:** Full texts of potentially eligible studies will be retrieved and independently assessed by the same two reviewers. Reasons for exclusion at the full-text stage will be documented and reported in the PRISMA flow diagram.
>
> **Disagreement resolution:** Discrepancies at any stage will be resolved through discussion. If consensus cannot be reached, a third reviewer (supervisor) will make the final decision.
>
> **Screening platform:** Covidence or Rayyan will be used for screening management. Duplicates will be identified and removed at the import stage.

---

*References:*
- PRISMA-P 2015 items 9–11. Shamseer et al. BMJ 2015;349:g7647
- Cochrane Handbook v6.5, Chapter 4: Searching for and selecting studies. Section 4.4: Designing search strategies
- Lefebvre C, Glanville J, Briscoe S, et al. Technical Supplement to Chapter 4: Searching for and selecting studies. Cochrane Handbook. 2022 (https://training.cochrane.org/handbook)
- Bramer WM, Rethlefsen ML, Kleijnen J, Franco OH. Optimal database combinations for literature searches in systematic reviews: a prospective exploratory study. Syst Rev. 2017;6(1):245. doi:10.1186/s13643-017-0644-y
