# Prioritized Reading List
### Causal ML for HTE — DHIS2 Kenya/Uganda Thesis Proposal
*Compiled September 2026*

Papers are grouped by priority tier, in the suggested reading order below. Suggested order: **Tier 1: #2 → #4 → #1 → #3, then Tier 2 (#5–#8) once you've picked your case study, then Tier 3 as needed.**

---

## Tier 1 — Read First (Core Methodology)

**1. Morzywołek, P., Decruyenaere, J., & Vansteelandt, S. (2023/2024).**
"On a General Class of Orthogonal Learners for the Estimation of Heterogeneous Treatment Effects."
*arXiv:2303.12687*
- Abstract: https://arxiv.org/abs/2303.12687
- PDF: https://arxiv.org/pdf/2303.12687
- **Why:** Primary methodological foundation — the orthogonal-learner estimator in your proposal is built on this paper.

**2. Sverdrup, E., Petukhova, M., & Wager, S. (2025).**
"Estimating Treatment Effect Heterogeneity in Psychiatry: A Review and Tutorial With Causal Forests."
*International Journal of Methods in Psychiatric Research*, 34(2), e70015.
- Journal: https://onlinelibrary.wiley.com/doi/full/10.1002/mpr.70015
- Free full text (PMC): https://pmc.ncbi.nlm.nih.gov/articles/PMC11966565/
- Preprint PDF: https://arxiv.org/pdf/2409.01578
- Code (R package `grf`): https://github.com/grf-labs/grf
- **Why:** Your applied workflow template (BLP tests, Qini/TOC curves). Best starting point — most accessible.

**3. Wager, S., & Athey, S. (2018).**
"Estimation and Inference of Heterogeneous Treatment Effects Using Random Forests."
*Journal of the American Statistical Association*, 113(523), 1228–1242.
- DOI: https://doi.org/10.1080/01621459.2017.1319839
- **Why:** Foundational causal forest paper — you'll cite this constantly.

**4. Künzel, S. R., Sekhon, J. S., Bickel, P. J., & Yu, B. (2019).**
"Metalearners for Estimating Heterogeneous Treatment Effects Using Machine Learning."
*Proceedings of the National Academy of Sciences*, 116(10), 4156–4165.
- DOI: https://doi.org/10.1073/pnas.1804597116
- Free full text (PMC): https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6410855/
- **Why:** Defines S-/T-/X-learner, your benchmark estimators.

---

## Tier 2 — Read Before Finalizing Case Study

**5. Verstraete, K., Gyselinck, I., Huts, H., Das, N., Topalovic, M., De Vos, M., & Janssens, W. (2023).**
"Estimating Individual Treatment Effects on COPD Exacerbations by Causal Machine Learning on Randomised Controlled Trials."
*Thorax*, 78(10), 983–989.
- DOI: https://doi.org/10.1136/thorax-2022-219382
- Free full text (PMC): https://pmc.ncbi.nlm.nih.gov/articles/PMC10511983/
- **Why:** Best structural template for writing up an applied causal-forest paper in a clinical/programmatic journal.

**6. "The Malaria Vaccine Implementation Programme Reduced Clinical Malaria in Kenya, 2020 to 2022: Impact Evaluation with Predictive Time-Series Models of Routine Surveillance Data."**
- Free full text (PMC): https://pmc.ncbi.nlm.nih.gov/articles/PMC13501692/
- **Why:** Case Study A directly extends this paper. Read closely to understand what's already been done (facility-level time series, average effects) so you can clearly frame the CATE contribution.

**7. Orech et al. (2026).**
"Malaria Morbidity and Its Association with Indoor Residual Spraying in Amolatar District, Uganda: A Retrospective Ecological Study Using Routine DHIS2 Data."
*Health Science Reports*.
- Journal: https://onlinelibrary.wiley.com/doi/10.1002/hsr2.73092
- **Why:** Case Study B. Short paper — read for the explicit "no comparison district" limitation that your CATE framework is designed to fix.

**8. Malaria Journal (2025).**
"Concordance of Data on Key Malaria Indicators Between DHIS2 and Source Documents, and Influencing Factors at Public Primary Health Facilities in Eastern Uganda: A Mixed Methods Study."
- Journal: https://malariajournal.biomedcentral.com/articles/10.1186/s12936-025-05519-y
- Free full text (PMC): https://pmc.ncbi.nlm.nih.gov/articles/PMC12369219/
- **Why:** Critical for your data-quality section — get the actual concordance numbers to write a credible Section 4.4.

---

## Tier 3 — Background / Context (skim, cite, lower priority)

**9. Nie, X., & Wager, S. (2021).**
"Quasi-Oracle Estimation of Heterogeneous Treatment Effects."
*Biometrika*, 108(2), 299–319.
- DOI: https://doi.org/10.1093/biomet/asaa076

**10. Pryce, M., Diaz-Ordaz, K., Keogh, R. H., & Vansteelandt, S. (2025).**
"Causal Machine Learning for Heterogeneous Treatment Effects in the Presence of Missing Outcome Data."
*Biometrics*, 81(3), ujaf098.
- Journal: https://academic.oup.com/biometrics/article/81/3/ujaf098/8220015
- Preprint: https://arxiv.org/abs/2412.19711
- **Relevance:** Model for writing a methods-extension paper; content-relevant only if you hit missing-outcome problems.

**11. Pryce, M., Diaz-Ordaz, K., Keogh, R. H., & Vansteelandt, S. (2026).**
"Targeted Learning of Heterogeneous Treatment Effect Curves for Right Censored or Left Truncated Time-to-Event Data."
*arXiv:2603.26502*
- Abstract: https://arxiv.org/abs/2603.26502
- **Relevance:** Only relevant if you pivot to time-to-event outcomes.

**12. Huts, H., Verstraete, K., Staes, M., Beersaerts, A., De Vos, M., & Janssens, W. (2026).**
"Uncovering the Heterogeneous Effect of Inhaled Corticosteroids on COPD Exacerbations with Causal Machine Learning."
*Respiratory Research*.
- Journal: https://link.springer.com/article/10.1186/s12931-026-03799-9
- **Relevance:** Second KU Leuven example, lower priority than #5.

**13. Komura, T., Bargagli-Stoffi, F. J., Arah, O. A., & Inoue, K. (2026).**
"Estimating and Discovering Heterogeneous Treatment Effects Using Machine Learning in Epidemiological Studies: A Practical Guide."
*International Journal of Epidemiology*, 55(3), dyag092.
- Journal: https://academic.oup.com/ije/article/55/3/dyag092/8707559
- Free full text (PMC): https://pmc.ncbi.nlm.nih.gov/articles/PMC13264450/
- **Relevance:** A second, more epidemiology-flavored explanation of meta-learners vs. causal forests.

**14. "Data Processing Pipelines and Tools for Routine Health Facility Malaria Surveillance in Uganda"** (ETL / ramptools).
- PDF: https://www.medrxiv.org/content/10.64898/2026.07.22.26357569.full.pdf
- **Relevance:** Read when you actually start building your DHIS2 extraction pipeline, not now.

**15. "The Effect of Case Management and Vector-Control Interventions on Space–Time Patterns of Malaria Incidence in Uganda"** (2013–2016 DHIS2 data).
- Free full text (PMC): https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5898071/
- **Relevance:** Background for Case Study C.

**16. Mwebesa et al. (2026).**
"Estimating Causal Effects of Malaria Infection on Anaemia Among Children Under Five Years in Uganda: Evidence from a Cross-Sectional Malaria Indicator Survey."
*Health Science Reports*.
- Journal: https://onlinelibrary.wiley.com/doi/10.1002/hsr2.73001
- **Relevance:** Background only, lower direct relevance to the CATE approach.

---

*All links verified as of September 2026. Where a free-access copy (PMC, arXiv) exists alongside a paywalled journal version, both are listed.*
