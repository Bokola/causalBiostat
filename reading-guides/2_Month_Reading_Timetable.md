# 2-Month Reading Timetable
### Causal ML for HTE — Full Paper List (Main Bibliography + TMLE/N-of-1 Supplement)
*8 weeks, ~5 reading days/week, ~1 hour/day minimum (dense papers get 2–3 sessions)*

**Total corpus: ~50 papers** across three bibliographies:
- Main bibliography (tutorials, methods, applied, Ghent/KU Leuven) — 25 papers
- TMLE for HTE — 10 papers
- N-of-1 trials — 8 papers
- DHIS2/malaria applied papers (thesis-specific grounding) — 7 papers

**Sequencing logic:** foundational methods first (so later papers make sense), then applied/case-study papers, then the two supplementary tracks (TMLE, then N-of-1), ending with a synthesis week.

---

## Week 1 — Core Foundations (Tier 1)
*Goal: understand causal forests and meta-learners well enough to explain them from memory.*

| Day | Paper | Notes |
|---|---|---|
| Mon–Tue | Sverdrup, Petukhova & Wager (2025) — causal forest tutorial | Most accessible; read fully, run the `grf` code examples if possible |
| Wed | Künzel et al. (2019) — meta-learners, *PNAS* | Defines S-/T-/X-learner — know these cold |
| Thu–Fri | Wager & Athey (2018) — causal forests, *JASA* | Denser/more technical; the theory behind `grf` |

**End of week:** write a 1-page personal summary of causal forests vs. meta-learners.

---

## Week 2 — Orthogonal Learners (Tier 1, continued)
*Goal: master the orthogonal-learner framework that underpins your proposal's core method.*

| Day | Paper | Notes |
|---|---|---|
| Mon–Wed | Morzywołek, Decruyenaere & Vansteelandt (2023/2024) — orthogonal learners, arXiv:2303.12687 | Your primary methodological reference — budget 3 days, it's theory-heavy |
| Thu | Nie & Wager (2021) — quasi-oracle/R-learner, *Biometrika* | Read alongside the orthogonal-learner paper; it's the R-learner they generalize |
| Fri | Buffer + synthesis | Consolidate notes on Weeks 1–2; draft how these three estimator families relate |

---

## Week 3 — Case-Study Grounding (Tier 2)
*Goal: understand the real-world papers your case studies (Kenya/Uganda malaria) will extend.*

| Day | Paper | Notes |
|---|---|---|
| Mon | Verstraete et al. (2023) — COPD causal forest, *Thorax* | Structural template for writing up applied results |
| Tue | RTS,S Malaria Vaccine Implementation Programme impact evaluation (Kenya, PMC13501692) | Directly relevant to Case Study A |
| Wed | Orech et al. (2026) — IRS in Amolatar, Uganda | Directly relevant to Case Study B; note its stated limitations |
| Thu | Malaria Journal (2025) — DHIS2/source-document concordance study | Essential for your data-quality section — extract the actual numbers |
| Fri | Vansteelandt & Morzywołek (2025) — orthogonal prediction of counterfactual outcomes | Extension of Week 2's core paper |

---

## Week 4 — Background & Remaining Methods Papers
*Goal: fill in secondary methodology and epidemiology framing.*

| Day | Paper | Notes |
|---|---|---|
| Mon | Komura et al. (2026) — practical guide, *IJE* | Good second explanation of meta-learners vs. forests |
| Tue | Huts et al. (2026) — KU Leuven COPD/ICS paper | Second applied KU Leuven example |
| Wed | Pryce et al. (2025, missing data) + Pryce et al. (2026, survival curves) | Batch read — both extend the Ghent orthogonal-learner line |
| Thu | Kim (2026, Kernel Ridge CATE) + Swaroop et al. (2026, representation learning) | Lighter/skim — theory-forward, note key ideas only |
| Fri | BART for RDD (2503.00326) + Multi-CATE (2405.18206) | Note their simulation-design approaches — useful models for your own simulation study |

---

## Week 5 — Remaining Main Bibliography (Applied + Belgium)
*Goal: finish the main bibliography.*

| Day | Paper | Notes |
|---|---|---|
| Mon | Ensemble methods (2407.03690) + Deep learning comparison (2405.03130) + Relative error framework (2510.16419) + Monte Carlo evidence (1810.13237) | Batch/skim — comparative and evaluation-focused, lower depth needed |
| Tue | Morocco cash transfer (2401.07075) + distributed confidential data (2402.02672) + survival subgroup discovery (Lifetime Data Anal.) + manifold causal networks (Mathematics 2026) | Batch — applied papers, skim for method + result, don't over-invest |
| Wed | Rank-Learner (Ghent, 2602.03517) + Olaya/Coussement/Verbeke uplift survey (KU Leuven) | Completes the Belgium section |
| Thu | Remaining DHIS2 papers: ETL/ramptools pipeline, Uganda space-time malaria model, Mwebesa anaemia paper | Practical/data-pipeline focus — read for method, not theory |
| Fri | "From Prediction to Prescription" review (2025) + full synthesis of main bibliography | Write a 1-page map: estimator family → paper → relevance to your thesis |

---

## Week 6 — TMLE Deep Dive (Part 1)
*Goal: understand TMLE fundamentals before tackling HTE-specific TMLE extensions.*

| Day | Paper | Notes |
|---|---|---|
| Mon | Luque-Fernandez et al. (2018) — TMLE tutorial, *Stat in Medicine* | Read this **first** in the TMLE track — foundational |
| Tue | Van der Laan & Rose (2011) — *Targeted Learning* textbook | Selected chapters only (intro + CATE-relevant chapter); not cover-to-cover |
| Wed | VIM-TMLE for HTE (2309.13324) | Direct HTE application of TMLE |
| Thu | A-TMLE (2605.01671) | Adaptive/data-driven CATE working model |
| Fri | Positivity truncation in TMLE (2604.20059) + One-step WATE TMLE (2604.00198) | Batch — both address practical estimation issues you'll likely hit with DHIS2 |

---

## Week 7 — TMLE Deep Dive (Part 2) + N-of-1 Start
*Goal: finish TMLE track; begin N-of-1 (separate, lower-priority track).*

| Day | Paper | Notes |
|---|---|---|
| Mon | Competing-risks subgroup TMLE (2407.18389) | Only deep-read if you anticipate survival/competing-risks outcomes |
| Tue | Survival HTE via TMLE (*J. Biomedical Informatics*, 2020) + Bayesian TMLE for UQ (2507.15909) | Batch/skim |
| Wed | Adaptive-TMLE for RCT + real-world data (2405.07186) | Relevant if combining a pilot/stepped rollout with routine DHIS2 data |
| Thu | Piccininni et al. (2025) — causal inference for N-of-1 trials | Foundational N-of-1 paper — read fully even though track is lower priority |
| Fri | IV approach to N-of-1 (ISTOP study, 2306.14019) | |

---

## Week 8 — N-of-1 Finish + Full Synthesis
*Goal: close out N-of-1 track; consolidate everything into thesis-ready notes.*

| Day | Paper | Notes |
|---|---|---|
| Mon | Anytime-valid inference in N-of-1 trials (Malenica et al.) | Van der Laan-lineage — bridges back to TMLE track |
| Tue | Bayesian adaptive N-of-1 trials (1911.00878) | |
| Wed | Multimodal N-of-1 (2309.06455) + methodological review of N-of-1 trials (*Trials*, 2024) | Batch/skim |
| Thu | RWE from N-of-1 (PMC10565195) + Nikles & Mitchell textbook (skim only) | Closes N-of-1 track |
| Fri | **Full synthesis day** | Consolidate all notes into one annotated master document; revisit your thesis proposal's Section 5 (Methodology) and confirm/revise your estimator choice in light of everything read |

---

## Practical Tips

- **Reading depth varies by paper.** "Deep read" (2–3 hrs, notes on assumptions/proofs) applies to ~12 papers (Tier 1 core + orthogonal learner + TMLE tutorial + N-of-1 foundational). Everything else can be a **focused read** (30–60 min: abstract, method summary, results, one key figure) or a **skim** (15 min: abstract + conclusion + note relevance).
- **Keep a running one-line entry per paper** (method used, key result, relevance to your thesis 1–5) — this becomes your annotated bibliography for the thesis literature review chapter.
- **Weekends are buffer**, not scheduled reading — use them only if a week runs over, or to re-read something from Week 1–2 that clicks better after Week 6 (TMLE)'s technical grounding.
- If time is tight, the **minimum viable path** is Weeks 1–5 (main bibliography, 25 papers) — the TMLE/N-of-1 weeks (6–8) are supplementary and can be compressed or deferred if your supervisor confirms orthogonal learners/causal forests as your final estimator choice.
