# MS Biostatistics: Quick Refresh Kit

A one-month refresh of the core Biostatistics track: GLMs, mixed models, longitudinal and survival analysis, simulation, and clinical trials. It adds a Bayesian strand run in JAGS, NIMBLE, and Stan that covers clinical trials, longitudinal analysis, expert elicitation, and N-of-1 trials.

It's built for review of material you've already taken, not first-time learning. Each topic gets one refresher reading and one R package, at about an hour a session.

## Files

| File | What it contains |
|---|---|
| `README.md` | This overview |
| `Biostat_Refresh_Plan.md` | 10 core topics and papers (`R1`–`R10`), the combined one-month timetable, backbone textbooks, and the full install script |
| `Bayesian_JAGS_NIMBLE_Stan_Bibliography.md` | 26 Bayesian papers (`B1`–`B26`) plus the engine papers (`B0`), each tagged with its engine, with tutorials starred (★) |

## How to use it

1. Run the setup block at the end of `Biostat_Refresh_Plan.md`. JAGS and CmdStan are installed separately from the R packages.
2. Follow the timetable: 4 weeks × 5 sessions.
   - About 20 minutes per session: skim the paper's key sections. Aim for the core idea, the model, and the main pitfalls.
   - About 40 minutes per session: rerun the package vignette, the paper's code, or your old course code.
3. Look up each timetable code in the matching bibliography: `R#` is in `Biostat_Refresh_Plan.md` and `B#` is in the Bayesian bibliography.
4. Skip any topic you're already confident in. The optional `B#` papers are background only.

## Timetable at a glance

| Week | Focus |
|---|---|
| 1 | GLMs and mixed models · overdispersion · Bayesian engines (JAGS, NIMBLE, and Stan compared) · Bayesian workflow · GEE |
| 2 | Missing data · Bayesian mixed models in raw Stan · `brms` and joint models · survival and competing risks |
| 3 | Expert elicitation (`SHELF` → Stan) · Bayesian trial analysis · MAP priors (`RBesT`) · adaptive designs |
| 4 | Bootstrap and simulation (ADEMP) · penalized models and GAMs · surrogate endpoints · N-of-1 trials (two sessions) |

## Software

- **Frequentist core:** `lme4`, `glmmTMB`, `geepack`, `nlme`, `mice`, `survival`, `mstate`, `boot`, `rsimsum`, `glmnet`, `mgcv`, `rpact`, `Surrogate`
- **Bayesian engines:** JAGS (`rjags`, `R2jags`, `runjags`), NIMBLE (`nimble`), Stan (`cmdstanr`, `rstan`, `brms`)
- **Bayesian tools:** `RBesT`, `OncoBayes2`, `SHELF`, `JMbayes`, `bayesplot`, `loo`

## Leuven and Hasselt anchors

Works from KU Leuven and Hasselt (I-BioStat) authors are marked in the files, including Molenberghs et al. (2010), Verbeke et al. (2014), Buyse et al. (2000), and Lesaffre & Lawson (2012). The backbone textbooks by Verbeke & Molenberghs are also listed.

## Tips

- Keep one Quarto notebook per week, with the paper summary at the top and working code below it.
- Save the model code for the Bayesian sessions: JAGS model files, NIMBLE code, and `.stan` files. Most JAGS code ports to NIMBLE with minimal changes.
- The citations were compiled from memory, so check every DOI or journal page before citing.
