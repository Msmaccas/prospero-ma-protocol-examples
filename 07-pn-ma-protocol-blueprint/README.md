# PN Meta-Analysis Protocol Blueprint

> **A structured reference for writing your PROSPERO protocol: "Polynucleotides for Skin Rejuvenation: A Meta-Analysis of Randomized and Split-Face Controlled Trials"**

This folder contains a **section-by-section protocol blueprint** — each file covers one part of a PROSPERO SR/MA protocol. Each section is split into:

1. **Learnings & Best Practices** (~80%) — extracted from the 6 PROSPERO examples in this repo, plus deep research into PRISMA-P 2015 guidelines, Cochrane Handbook methodology, and aesthetic dermatology SR-specific considerations
2. **Your Protocol Draft** (~20%) — a script/style draft for that section of your polynucleotide meta-analysis protocol, written so you can critically evaluate and adapt

---

## Why This Blueprint Exists

You're planning a systematic review and meta-analysis of injectable polynucleotides (PN/PDRN) for skin rejuvenation. Two SRs already exist on this topic:

| Review | Year | Studies | Analysis | Limitation |
|--------|------|---------|----------|------------|
| Lampridou et al. (*J Cosmet Dermatol*) | 2025 | 9 (219 patients) | Narrative only | No meta-analysis; wide inclusion (all PN uses) |
| Kream et al. (*Dermatol Surg*) | 2026 | Broader derm scope | Narrative | Overview across all derm PN/PDRN uses; no pooled analysis |

**Your gap:** Sufficient randomized and split-face controlled trial data has accumulated (2020–2025) to support a **quantitative meta-analysis** of PN efficacy for skin rejuvenation outcomes. Neither existing SR performed one.

This blueprint helps you write a protocol that is:
- **Methodologically sound** — follows PRISMA-P 2015 and Cochrane MECIR standards
- **Specifically tailored** — handles split-face trial designs, multiple PN formulations, and aesthetic outcome measures
- **Realistic** — addresses the known heterogeneity challenges in aesthetic dermatology SRs
- **Publication-ready** — structured for PROSPERO registration and eventual journal submission

---

## Protocol Structure

This blueprint follows the PRISMA-P 2015 17-item checklist and the PROSPERO registration form structure.

| Section File | PRISMA-P Items | PROSPERO Section |
|---|---|---|
| `01-title-and-rationale.md` | 1a, 1b, 2 | Review title, rationale/background |
| `02-objectives-and-pico.md` | 3, 4, 5 | Review question, objectives, PICO |
| `03-eligibility-criteria.md` | 6, 7, 8 | Population, intervention, comparator, study design, context |
| `04-search-strategy.md` | 9, 10, 11 | Databases, search string, screening, date restrictions |
| `05-outcomes.md` | 12 | Primary & secondary outcomes, measurement tools |
| `06-data-extraction.md` | 13a, 13b | Data items, extraction process, handling paired/split-face data |
| `07-risk-of-bias.md` | 14 | Quality assessment, RoB-2, ROBINS-I, split-face considerations |
| `08-data-synthesis.md` | 15a, 15b, 15c, 16 | Meta-analysis models, heterogeneity, subgroups, sensitivity |
| `09-timeline-team-funding.md` | 17, 18, 19, 20 | Timeline, team, funding, COI, dissemination |
| `10-combined-draft.md` | ALL | Complete assembled protocol draft |

---

## How to Use

1. **Read the sections in order** — each builds on the previous
2. **Study the "Learnings" first** — this is where the craft lives
3. **Critically evaluate the "Your Draft"** — it's a starting script, not final text. Mark it up, change it, argue with it
4. **Open the 6 example PROSPERO records** in folders 01–06 when you need to see how other derm SR teams handled similar decisions
5. **Assemble** into `10-combined-draft.md` when ready

---

## Key Methodological References

- **PRISMA-P 2015 Statement:** Shamseer et al. *BMJ* 2015;349:g7647. doi:10.1136/bmj.g7647
- **PRISMA-P 2015 Checklist:** https://www.prisma-statement.org/prisma-p/
- **Cochrane Handbook v6.5 (2024):** https://training.cochrane.org/handbook
- **PROSPERO Registration Guide:** https://www.crd.york.ac.uk/prospero/#guidance
- **RoB 2 Tool:** Sterne et al. *BMJ* 2019;366:l4898. doi:10.1136/bmj.l4898
- **GRADE:** Guyatt et al. *BMJ* 2008;336:924-6. doi:10.1136/bmj.39489.470347.AD

---

*Part of [prospero-ma-protocol-examples](https://github.com/Msmaccas/prospero-ma-protocol-examples) — a living reference collection.*
