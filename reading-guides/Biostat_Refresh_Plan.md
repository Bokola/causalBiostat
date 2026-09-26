# MS Biostatistics: Quick Refresh Plan

One refresher reading and one R package per topic, at about an hour a session. Skip any topic you already know well.

Before citing any reference, verify its details via its DOI or journal page.

## Topics at a glance

| # | Topic | Refresher reading | Code |
|---|---|---|---|
| 1 | GLMs and mixed models | Bolker et al. (2009) | `lme4`, `glmmTMB` |
| 2 | Overdispersed repeated measures | Molenberghs et al. (2010) | `lme4` |
| 3 | Bayesian workflow | Gelman et al. (2020) | `brms`, `loo` |
| 4 | Longitudinal and GEE | Verbeke et al. (2014) | `geepack`, `nlme` |
| 5 | Missing data | Sterne et al. (2009) | `mice` |
| 6 | Survival and competing risks | Putter et al. (2007) | `survival`, `mstate` |
| 7 | Bootstrap and simulation | Morris et al. (2019) | `boot`, `rsimsum` |
| 8 | Penalized models and GAMs | Pedersen et al. (2019) | `glmnet`, `mgcv` |
| 9 | Clinical trials | Pallmann et al. (2018) | `rpact` |
| 10 | Surrogate endpoints | Buyse et al. (2000) | `Surrogate` |

## One-month timetable (5 sessions a week, about 1 hour each)

**How to read the reference codes:** `R#` is a paper in this file's bibliography below. `B#` is a paper in *Bayesian_JAGS_NIMBLE_Stan_Bibliography.md*, where `B0` is that file's section 0 (the engine papers).

| Week | Session 1 | Session 2 | Session 3 | Session 4 | Session 5 |
|---|---|---|---|---|---|
| 1 | GLMs and mixed models [R1] | Overdispersed repeated measures [R2] | Bayesian engines: fit one model in JAGS, NIMBLE, and Stan [B0] | Bayesian workflow [R3] | Longitudinal and GEE [R4] |
| 2 | Missing data [R5] | Bayesian mixed model in raw Stan [B10, B13] | `brms` and joint models (`JMbayes`) [B11, B12] | Survival and competing risks [R6] | Survival exercise on `survival::pbc` |
| 3 | Expert elicitation with `SHELF`, passing the prior to Stan [B14, B15] | Elicitation for trial design [B18, B17] | Bayesian trial reanalysis with sceptical and enthusiastic priors [B1, B7] | Historical borrowing with MAP priors in `RBesT` [B4, B5] | Adaptive designs, frequentist vs Bayesian [R9, B6] |
| 4 | Bootstrap and simulation [R7] | Penalized models and GAMs [R8] | Surrogate endpoints [R10] | N-of-1 I: hierarchical model in JAGS or Stan [B20, B22] | N-of-1 II: HIAlab repo and sample size [B24, B26] |

**Each session:** about 20 minutes skimming the paper's key sections, then about 40 minutes rerunning the package vignette or your old course code.
**Optional background, whenever it's useful:** B2, B3, B8, B9, B16, B19, B21, B23, B25.

## Bibliography with code references

1. Bolker, B. M., Brooks, M. E., Clark, C. J., et al. (2009). Generalized linear mixed models: a practical guide for ecology and evolution. *Trends in Ecology & Evolution*, 24(3), 127–135.
   **Code:** `lme4` (Bates et al., 2015, *JSS* 67(1)); `glmmTMB`

2. Molenberghs, G., Verbeke, G., Demétrio, C. G. B., & Vieira, A. (2010). A family of generalized linear models for repeated measures with normal and conjugate random effects. *Statistical Science*, 25(3), 325–347. (Hasselt / KU Leuven)
   **Code:** `lme4`

3. Gelman, A., Vehtari, A., Simpson, D., et al. (2020). Bayesian workflow. arXiv:2011.01808.
   **Code:** `brms` (Bürkner, 2017, *JSS* 80(1)); `loo` (Vehtari et al., 2017, *Statistics and Computing* 27, 1413–1432)

4. Verbeke, G., Fieuws, S., Molenberghs, G., & Davidian, M. (2014). The analysis of multivariate longitudinal data: a review. *Statistical Methods in Medical Research*, 23(1), 42–59. (KU Leuven / Hasselt)
   **Code:** `geepack` (Halekoh et al., 2006, *JSS* 15(2)); `nlme`

5. Sterne, J. A. C., White, I. R., Carlin, J. B., et al. (2009). Multiple imputation for missing data in epidemiological and clinical research: potential and pitfalls. *BMJ*, 338, b2393.
   **Code:** `mice` (van Buuren & Groothuis-Oudshoorn, 2011, *JSS* 45(3))

6. Putter, H., Fiocco, M., & Geskus, R. B. (2007). Tutorial in biostatistics: competing risks and multi-state models. *Statistics in Medicine*, 26(11), 2389–2430.
   **Code:** `survival`; `mstate` (de Wreede et al., 2011, *JSS* 38(7))

7. Morris, T. P., White, I. R., & Crowther, M. J. (2019). Using simulation studies to evaluate statistical methods. *Statistics in Medicine*, 38(11), 2074–2102.
   **Code:** `boot`; `rsimsum`

8. Pedersen, E. J., Miller, D. L., Simpson, G. L., & Ross, N. (2019). Hierarchical generalized additive models in ecology: an introduction with mgcv. *PeerJ*, 7, e6876.
   **Code:** `mgcv` (full code in the paper's supplement); `glmnet` (Friedman et al., 2010, *JSS* 33(1))

9. Pallmann, P., Bedding, A. W., Choodari-Oskooei, B., et al. (2018). Adaptive designs in clinical trials: why use them, and how to run and report them. *BMC Medicine*, 16, 29.
   **Code:** `rpact`; `gsDesign`

10. Buyse, M., Molenberghs, G., Burzykowski, T., Renard, D., & Geys, H. (2000). The validation of surrogate endpoints in meta-analyses of randomized experiments. *Biostatistics*, 1(1), 49–67. (Hasselt)
    **Code:** `Surrogate` (CRAN)

## Backbone textbooks (for looking things up)

- Verbeke, G., & Molenberghs, G. (2000). *Linear Mixed Models for Longitudinal Data*. Springer.
- Molenberghs, G., & Verbeke, G. (2005). *Models for Discrete Longitudinal Data*. Springer.
- Molenberghs, G., & Kenward, M. G. (2007). *Missing Data in Clinical Studies*. Wiley.
- Lesaffre, E., & Lawson, A. B. (2012). *Bayesian Biostatistics*. Wiley.
- Harrell, F. E. (2015). *Regression Modeling Strategies* (2nd ed.). Springer. Code: `rms`.

## Setup

```r
install.packages(c("lme4", "glmmTMB", "brms", "loo", "geepack", "nlme",
                   "mice", "survival", "mstate", "boot", "rsimsum",
                   "glmnet", "mgcv", "rpact", "Surrogate",
                   # Bayesian additions
                   "rjags", "R2jags", "runjags", "nimble", "RBesT",
                   "OncoBayes2", "SHELF", "JMbayes", "bayesplot"))
# cmdstanr: install.packages("cmdstanr", repos = c("https://stan-dev.r-universe.dev", getOption("repos")))
# then run cmdstanr::install_cmdstan()
# JAGS itself must be installed separately: mcmc-jags.sourceforge.io
```
