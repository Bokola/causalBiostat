# Causal Machine Learning for Heterogeneous Treatment Effects (HTE) Estimation
### Annotated Bibliography — Tutorials, Methodological Papers, and Applied Studies
*Compiled September 2026*

---

## 1. Tutorials & Practical Guides

**1.1 Sverdrup, E., Petukhova, M., & Wager, S. (2025).**
"Estimating Treatment Effect Heterogeneity in Psychiatry: A Review and Tutorial With Causal Forests."
*International Journal of Methods in Psychiatric Research*, 34(2), e70015.
- Journal (publisher): https://onlinelibrary.wiley.com/doi/full/10.1002/mpr.70015
- Free full text (PMC): https://pmc.ncbi.nlm.nih.gov/articles/PMC11966565/
- Preprint PDF (arXiv:2409.01578): https://arxiv.org/pdf/2409.01578
- **Code:** R package `grf` (used throughout tutorial): https://github.com/grf-labs/grf
- Real-data application: US Army soldiers' resilience to combat stress (secondary analysis)

**1.2 Komura, T., Bargagli-Stoffi, F. J., Arah, O. A., & Inoue, K. (2026).**
"Estimating and Discovering Heterogeneous Treatment Effects Using Machine Learning in Epidemiological Studies: A Practical Guide."
*International Journal of Epidemiology*, 55(3), dyag092.
- Journal (publisher): https://academic.oup.com/ije/article/55/3/dyag092/8707559
- Free full text (PMC): https://pmc.ncbi.nlm.nih.gov/articles/PMC13264450/
- PubMed record: https://pubmed.ncbi.nlm.nih.gov/42287695/
- Note: includes statistical code for meta-learners and causal forests in the supplement

**1.3 Jacob, D. (2021, updated).**
"CATE Meets ML — The Conditional Average Treatment Effect and Machine Learning." (Tutorial)
- arXiv abstract/PDF: https://arxiv.org/abs/2104.09935
- **Code:** Quantlets (companion repository referenced in paper — search "CATEmeetsML" on QuantLet.com)
- Real-data applications: microcredit availability & borrowing; 401(k) eligibility & net financial assets

**1.4 From Prediction to Prescription: Machine Learning and Causal Inference for the Heterogeneous Treatment Effect**
Abécassis, J., Dumas, É., Alberge, J., & Varoquaux, G. (2025).
*Annual Review of Biomedical Data Science*, 8, 381–404.
- Journal: https://doi.org/10.1146/annurev-biodatasci-103123-095750

---

## 2. Recent Methodological Papers (Theory / Simulation / Code)

**2.1 Kim, S.-J. (2026).**
"Optimal and Structure-Adaptive CATE Estimation with Kernel Ridge Regression."
*arXiv:2602.18958* [stat.ME]
- Abstract: https://arxiv.org/abs/2602.18958
- PDF: https://arxiv.org/pdf/2602.18958

**2.2 Swaroop, M., et al. (2026).**
"Representation Learning for Sample-Efficient CATE Estimation by Leveraging Multiple Outcomes."
*arXiv:2609.06294*
- Abstract: https://arxiv.org/abs/2609.06294

**2.3 (2025).**
"A Bayesian Additive Regression Tree Model for Learning Conditional Average Treatment Effects in Regression Discontinuity Designs."
*arXiv:2503.00326*
- PDF: https://arxiv.org/pdf/2503.00326
- **Code:** GitHub repository with modifiable simulation protocol (linked in paper's footnote 3 — see PDF for repo URL, not indexed independently)

**2.4 Multi-CATE: Multi-Accurate Conditional Average Treatment Effect Estimation Robust to Unknown Covariate Shifts**
*arXiv:2405.18206*
- Abstract/HTML: https://arxiv.org/html/2405.18206v1
- PDF: https://arxiv.org/pdf/2405.18206
- **Code + data (OSF repository):** https://osf.io/zxjvw/?view_only=a622c123414e4be6a218f121ded191d3
- Real-data application: Women's Health Initiative (observational + RCT fusion)
- R packages used: `ranger`, `grf`, `rlearner`, `causalToolbox`, `mcboost`

**2.5 "Robust CATE Estimation Using Novel Ensemble Methods."**
*arXiv:2407.03690*
- PDF: https://arxiv.org/pdf/2407.03690
- Simulation-based comparison of X-RF, X-BART, X-AGLM, T-Linear, DR-RF, and stacking ensembles (CBA, R-Stacking, T-Stacking, Causal-Stacking)

**2.6 "Deep Learning for Causal Inference: A Comparison of Architectures for Heterogeneous Treatment Effect Estimation."**
*arXiv:2405.03130*
- HTML: https://arxiv.org/html/2405.03130v1
- PDF: https://arxiv.org/pdf/2405.03130

**2.7 "A Relative Error-Based Evaluation Framework of Heterogeneous Treatment Effect Estimators."**
*arXiv:2510.16419*
- PDF: https://arxiv.org/pdf/2510.16419

**2.8 "Machine Learning Estimation of Heterogeneous Causal Effects: Empirical Monte Carlo Evidence."**
*arXiv:1810.13237*
- PDF: https://arxiv.org/pdf/1810.13237

---

## 3. Applied / Real-World Data Analyses

**3.1 Rehill, P., & Biddle, N. (2024).**
"Heterogeneous Treatment Effect Estimation with High-Dimensional Data in Public Policy Evaluation — An Application to the Conditioning of Cash Transfers in Morocco Using Causal Machine Learning."
Centre for Social Research and Methods, Australian National University.
- PDF: https://arxiv.org/pdf/2401.07075
- Real data: Moroccan conditional cash transfer RCT (1,936 pre-treatment variables)
- Proposes a novel interpretable causal tree method

**3.2 "Estimation of Conditional Average Treatment Effects on Distributed Confidential Data."**
*arXiv:2402.02672* (v5, 2025)
- HTML: https://arxiv.org/html/2402.02672v5
- Method: "data collaboration double machine learning"; simulation + distributed real-data setting

**3.3 "Estimation of the Interpretable Heterogeneous Treatment Effect with Causal Subgroup Discovery in Survival Outcomes."**
*Lifetime Data Analysis*, 32(1), 11 (2026).
- Free full text (PMC): https://pmc.ncbi.nlm.nih.gov/articles/PMC13218393/
- Combines meta-learners + tree-based subgroup discovery for censored survival CATE; introduces "DEA-learner"

**3.4 "Manifold Causal Conditional Deep Networks for Heterogeneous Treatment Effect Estimation and Policy Evaluation."**
*Mathematics* (MDPI), 14(4), 738 (2026).
- Journal: https://doi.org/10.3390/math14040738
- High-dimensional HTE + policy evaluation framework; compares exploitative vs. exploratory action-selection policies on CATE RMSE

---

## 4. Belgium — Ghent University (Stijn Vansteelandt's Group)

**4.1 Morzywołek, P., Decruyenaere, J., & Vansteelandt, S. (2023).**
"On a General Class of Orthogonal Learners for the Estimation of Heterogeneous Treatment Effects."
*arXiv:2303.12687*
- Abstract: https://arxiv.org/abs/2303.12687
- PDF: https://arxiv.org/pdf/2303.12687
- Foundational paper unifying T-, DR-, and R-Learner as a general weighted Neyman-orthogonal learner class, with oracle bounds

**4.2 Morzywołek, P., Decruyenaere, J., & Vansteelandt, S. (2024).**
"On Weighted Orthogonal Learners for Heterogeneous Treatment Effects." (extended/revised version)
*arXiv:2303.12687*
- PDF: https://arxiv.org/pdf/2303.12687

**4.3 Vansteelandt, S., & Morzywołek, P. (2025).**
"Orthogonal Prediction of Counterfactual Outcomes."
*Journal of Causal Inference*, 13(1), 20240051.
- DOI: https://doi.org/10.1515/jci-2024-0051
- Free full text (PMC): https://pmc.ncbi.nlm.nih.gov/articles/PMC12658738/
- PubMed record: https://pubmed.ncbi.nlm.nih.gov/41323102/

**4.4 Pryce, M., Diaz-Ordaz, K., Keogh, R. H., & Vansteelandt, S. (2025).**
"Causal Machine Learning for Heterogeneous Treatment Effects in the Presence of Missing Outcome Data."
*Biometrics*, 81(3), ujaf098.
- Journal (publisher): https://academic.oup.com/biometrics/article/81/3/ujaf098/8220015
- Preprint (arXiv:2412.19711): https://arxiv.org/abs/2412.19711
- Preprint PDF: https://arxiv.org/pdf/2412.19711
- Real data: GBSG2 breast cancer trial (hormonal vs. non-hormonal therapy)
- Proposes mDR-learner and mEP-learner

**4.5 Pryce, M., Diaz-Ordaz, K., Keogh, R. H., & Vansteelandt, S. (2026).**
"Targeted Learning of Heterogeneous Treatment Effect Curves for Right Censored or Left Truncated Time-to-Event Data."
*arXiv:2603.26502*
- Abstract: https://arxiv.org/abs/2603.26502
- PDF: https://arxiv.org/pdf/2603.26502
- Introduces **surv-iTMLE**; extensive simulations + real trial data (via Roche collaboration)

**4.6 Arno, H., Demeester, T. (Ghent), Frauen, D., Javurek, E., & Feuerriegel, S. (LMU Munich) (2026).**
"Rank-Learner: Orthogonal Ranking of Treatment Effects."
*arXiv:2602.03517*
- PDF: https://arxiv.org/pdf/2602.03517

---

## 5. Belgium — KU Leuven

**5.1 Huts, H., Verstraete, K., Staes, M., Beersaerts, A., De Vos, M., & Janssens, W. (2026).**
"Uncovering the Heterogeneous Effect of Inhaled Corticosteroids on COPD Exacerbations with Causal Machine Learning."
*Respiratory Research*, published online 2026.
- Journal (open access): https://link.springer.com/article/10.1186/s12931-026-03799-9
- Real data: KU Leuven / University Hospitals Leuven COPD cohort

**5.2 Verstraete, K., Gyselinck, I., Huts, H., Das, N., Topalovic, M., De Vos, M., & Janssens, W. (2023).**
"Estimating Individual Treatment Effects on COPD Exacerbations by Causal Machine Learning on Randomised Controlled Trials."
*Thorax*, 78(10), 983–989.
- DOI: https://doi.org/10.1136/thorax-2022-219382
- PubMed record: https://pubmed.ncbi.nlm.nih.gov/37012070/
- Free full text (PMC, PMCID PMC10511983): https://pmc.ncbi.nlm.nih.gov/articles/PMC10511983/
- Open-access repository copy (KU Leuven LIRIAS): https://lirias.kuleuven.be/server/api/core/bitstreams/609d466c-cdc3-4582-b32f-737852aefaea/content
- Real data: SUMMIT trial (n=8,151, fluticasone furoate/vilanterol) + IMPACT trial validation

**5.3 Olaya, D., Coussement, K., & Verbeke, W. (KU Leuven).**
"A Survey and Benchmarking Study of Multitreatment Uplift Modeling."
*Data Mining and Knowledge Discovery*, 34(2), 273–308.
- *Note: direct open-access link not confirmed in search results — recommend retrieving via KU Leuven Lirias repository or publisher (Springer) using the DOI from the journal's table of contents.*

---

## Summary Table — Code & Data Availability

| Paper | Code Available | Real-World Data |
|---|---|---|
| Sverdrup et al. (Psychiatry tutorial) | ✅ R package `grf` | ✅ US Army soldiers |
| Multi-CATE (arXiv:2405.18206) | ✅ OSF repo | ✅ Women's Health Initiative |
| BART for RDD (arXiv:2503.00326) | ✅ GitHub (see PDF) | Simulation only |
| Rehill & Biddle (Morocco) | Not confirmed | ✅ Morocco cash transfer RCT |
| Ghent — Pryce et al. (Biometrics) | Not confirmed | ✅ GBSG2 breast cancer trial |
| Ghent — Pryce et al. (surv-iTMLE) | Not confirmed | ✅ Roche trial data |
| KU Leuven — Verstraete et al. (Thorax) | Not confirmed | ✅ SUMMIT + IMPACT COPD trials |
| KU Leuven — Huts et al. (Resp. Research) | Not confirmed | ✅ COPD cohort |
| CATE meets ML tutorial | ✅ Quantlets | ✅ Microcredit, 401(k) data |

---

*Note: "Not confirmed" means no public code repository was found during search — the paper may still include code in supplementary materials not indexed separately, or code may be available on request from the authors.*
