# Bayesian Biostatistics with JAGS / NIMBLE / Stan: Refresh Bibliography

**Key:** ★ = tutorial or worked-example paper. The engine column says which software runs the paper's code (JAGS, NIMBLE, Stan, or BUGS/JAGS for code written in BUGS syntax that also runs in JAGS). "Theory" means the paper has no code and gives background only.

Before citing any reference, verify its details via its DOI or journal page.

---

## 0. The engines themselves (pick one to work in)

| Ref | Engine | R interface |
|---|---|---|
| Plummer, M. (2003). JAGS: a program for analysis of Bayesian graphical models using Gibbs sampling. *Proc. DSC 2003*, Vienna. | JAGS | `rjags`, `R2jags`, `runjags` |
| Denwood, M. J. (2016). runjags: an R package providing interface utilities, model templates, parallel computing methods and additional distributions for MCMC models in JAGS. *JSS*, 71(9). ★ | JAGS | `runjags` |
| de Valpine, P., Turek, D., Paciorek, C. J., et al. (2017). Programming with models: writing statistical algorithms for general model structures with NIMBLE. *J. Comput. Graph. Stat.*, 26(2), 403–413. | NIMBLE | `nimble` (user manual at r-nimble.org) |
| Carpenter, B., Gelman, A., Hoffman, M. D., et al. (2017). Stan: a probabilistic programming language. *JSS*, 76(1). | Stan | `cmdstanr`, `rstan`, `brms` |

---

## 1. Clinical trial design and analysis

1. ★ Spiegelhalter, D. J., Freedman, L. S., & Parmar, M. K. B. (1994). Bayesian approaches to randomized trials. *JRSS A*, 157(3), 357–416. *(Theory: sceptical and enthusiastic priors, interim monitoring)*
2. Berry, D. A. (2006). Bayesian clinical trials. *Nature Reviews Drug Discovery*, 5(1), 27–36. *(Theory: short overview)*
3. Neuenschwander, B., Branson, M., & Gsponer, T. (2008). Critical aspects of the Bayesian approach to phase I cancer trials. *Statistics in Medicine*, 27(13), 2420–2439. **Engine:** BUGS/JAGS → Stan via `OncoBayes2`
4. Schmidli, H., Gsteiger, S., Roychoudhury, S., O'Hagan, A., Spiegelhalter, D., & Neuenschwander, B. (2014). Robust meta-analytic-predictive priors in clinical trials with historical control information. *Biometrics*, 70(4), 1023–1032. *(Borrowing from historical controls)*
5. ★ Weber, S., Li, Y., Seaman, J. W., Kakizume, T., & Schmidli, H. (2021). Applying meta-analytic-predictive priors with the R Bayesian evidence synthesis tools. *JSS*, 100(19). **Engine:** Stan via `RBesT`
6. Wason, J. M. S., & Trippa, L. (2014). A comparison of Bayesian adaptive randomization and multi-stage designs for multi-arm clinical trials. *Statistics in Medicine*, 33(13), 2206–2221. *(Design by simulation)*
7. ★ Zampieri, F. G., Casey, J. D., Shankar-Hari, M., Harrell, F. E., & Harhay, M. O. (2021). Using Bayesian methods to augment the interpretation of critical care trials. *Am. J. Respir. Crit. Care Med.*, 203(5), 543–552. **Engine:** Stan via `brms` (code in the supplement)
8. Goligher, E. C., Tomlinson, G., Hajage, D., et al. (2018). ECMO for severe ARDS and posterior probability of mortality benefit in a post hoc Bayesian analysis of a randomized clinical trial. *JAMA*, 320(21), 2251–2259. *(Model reanalysis of a real trial)*
9. Ibrahim, J. G., & Chen, M.-H. (2000). Power prior distributions for regression models. *Statistical Science*, 15(1), 46–60. *(Theory: power priors)*

**Book:** Berry, S. M., Carlin, B. P., Lee, J. J., & Müller, P. (2010). *Bayesian Adaptive Methods for Clinical Trials*. CRC Press.

---

## 2. Longitudinal analysis

10. ★ Sorensen, T., Hohenstein, S., & Vasishth, S. (2016). Bayesian linear mixed models using Stan: a tutorial for psychologists, linguists, and cognitive scientists. *The Quantitative Methods for Psychology*, 12(3), 175–200. **Engine:** Stan (raw Stan code, step by step)
11. ★ Bürkner, P.-C. (2017). brms: an R package for Bayesian multilevel models using Stan. *JSS*, 80(1). **Engine:** Stan
12. ★ Rizopoulos, D. (2016). The R package JMbayes for fitting joint models for longitudinal and time-to-event data using MCMC. *JSS*, 72(7). **Engine:** JAGS (the newer `JMbayes2` uses its own C++ sampler). Rizopoulos did his PhD at KU Leuven.
13. Lambert, P. C., Sutton, A. J., Burton, P. R., Abrams, K. R., & Jones, D. R. (2005). How vague is vague? A simulation study of the impact of the use of vague prior distributions in MCMC using WinBUGS. *Statistics in Medicine*, 24(15), 2401–2428. *(Prior sensitivity for variance components; BUGS/JAGS)*

**Books:**
- Lesaffre, E., & Lawson, A. B. (2012). *Bayesian Biostatistics*. Wiley. KU Leuven; BUGS/JAGS code throughout, including longitudinal chapters.
- Nicenboim, B., Schad, D., & Vasishth, S. *An Introduction to Bayesian Data Analysis for Cognitive Science*. CRC. Free online; uses Stan and `brms` for hierarchical and repeated-measures models.
- Kruschke, J. K. (2015). *Doing Bayesian Data Analysis* (2nd ed.). Academic Press. JAGS and Stan.

---

## 3. Expert knowledge elicitation

14. ★ O'Hagan, A. (2019). Expert knowledge elicitation: subjective but scientific. *The American Statistician*, 73(sup1), 69–81.
15. ★ Gosling, J. P. (2018). SHELF: the Sheffield elicitation framework. In Dias, L. C., Morton, A., & Quigley, J. (Eds.), *Elicitation* (pp. 61–93). Springer. **Code:** `SHELF` (Oakley). It fits distributions to elicited judgements, which you then pass as priors to JAGS, NIMBLE, or Stan.
16. Mikkola, P., Martin, O. A., Chandramouli, S., et al. (2024). Prior knowledge elicitation: the past, present, and future. *Bayesian Analysis*, 19(4), 1129–1161.
17. Johnson, S. R., Tomlinson, G. A., Hawker, G. A., Granton, J. T., & Feldman, B. M. (2010). Methods to elicit beliefs for Bayesian priors: a systematic review. *J. Clin. Epidemiol.*, 63(4), 355–369.
18. ★ Dallow, N., Best, N., & Montague, T. H. (2018). Better decision making in drug development through adoption of formal prior elicitation. *Pharmaceutical Statistics*, 17(4), 301–316. *(An industry case study linking elicitation to trial design)*
19. Morris, D. E., Oakley, J. E., & Crowe, J. A. (2014). A web-based tool for eliciting probability distributions from experts. *Environmental Modelling & Software*, 52, 1–4. **Tool:** MATCH, a browser-based version of SHELF

**Book:** O'Hagan, A., Buck, C. E., Daneshkhah, A., et al. (2006). *Uncertain Judgements: Eliciting Experts' Probabilities*. Wiley.

---

## 4. N-of-1 trials

20. ★ Zucker, D. R., Schmid, C. H., McIntosh, M. W., D'Agostino, R. B., Selker, H. P., & Lau, J. (1997). Combining single patient (N-of-1) trials to estimate population treatment effects and to evaluate individual patient responses to treatment. *J. Clin. Epidemiol.*, 50(4), 401–410. *(The original hierarchical Bayesian model; BUGS-style)*
21. Zucker, D. R., Ruthazer, R., & Schmid, C. H. (2010). Individual (N-of-1) trials can be combined to give population comparative treatment effect estimates: methodologic considerations. *J. Clin. Epidemiol.*, 63(12), 1312–1323.
22. ★ Kravitz, R. L., Duan, N., & the DEcIDE Methods Center N-of-1 Guidance Panel (2014). *Design and Implementation of N-of-1 Trials: A User's Guide*. AHRQ Publication No. 13(14)-EHC122-EF. In particular, see the chapter by Schmid & Duan on statistical design and analysis, including Bayesian models. Free online.
23. Duan, N., Kravitz, R. L., & Schmid, C. H. (2013). Single-patient (n-of-1) trials: a pragmatic clinical decision methodology for patient-centered comparative effectiveness research. *J. Clin. Epidemiol.*, 66(8 Suppl), S21–S28.
24. Stunnenberg, B. C., Raaphorst, J., Groenewoud, H. M., et al. (2018). Effect of mexiletine on muscle stiffness in patients with nondystrophic myotonia evaluated using aggregated N-of-1 trials. *JAMA*, 320(22), 2344–2353. *(Applied aggregated Bayesian N-of-1 trial)*
25. Araujo, A., Julious, S., & Senn, S. (2016). Understanding variation in sets of N-of-1 trials. *PLoS One*, 11(12), e0167167.
26. Senn, S. (2019). Sample size considerations for n-of-1 trials. *Stat. Methods Med. Res.*, 28(2), 372–383. *(Frequentist, but essential for design)*

**Code:** github.com/HIAlab/gait_nof1trials is a worked JAGS pipeline that analyses population-level trials as N-of-1 trials, with MCMC diagnostics and model comparison.

---

## Timetable

These papers are scheduled in the combined one-month timetable in *Biostat_Refresh_Plan.md*, where they appear as `B#` references.

## Setup

```r
install.packages(c("rjags", "R2jags", "runjags", "nimble", "brms",
                   "RBesT", "OncoBayes2", "SHELF", "JMbayes", "bayesplot", "loo"))
# cmdstanr: install.packages("cmdstanr", repos = c("https://stan-dev.r-universe.dev", getOption("repos")))
# then run cmdstanr::install_cmdstan()
# JAGS itself must be installed separately: mcmc-jags.sourceforge.io
```
