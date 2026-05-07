[Home](index.md) | [Research](research.md) | [Projects](projects.md) | [Resume](resume.pdf) | [LinkedIn](https://www.linkedin.com/in/huyle1625) | [GitHub](https://github.com/lehuypitt)
# Research

## Dissertation

**Differentially Methylated Regions in Longitudinal, Multivariate, and Heterogeneous DNA Methylation Data**  
PhD in Statistics, University of Pittsburgh  
Advisor: Christopher McKennan, PhD  
Defended April 2026

My dissertation develops Bayesian and empirical Bayes methods for identifying differentially methylated regions (DMRs) in high-dimensional DNA methylation data. The main statistical challenge is that methylation data are noisy, high-dimensional, and spatially dependent: nearby CpG sites often carry related biological signal, but the strength and structure of that dependence can vary across genomic regions.

Rather than testing CpG sites independently and then post-processing them into regions, my work builds probabilistic region-level models that account for spatial dependence, temporal or multivariate structure, and uncertainty. The goal is to produce DMR calls that are statistically calibrated, biologically interpretable, and accompanied by posterior summaries such as local false discovery rates.

**Status:** Dissertation defended; manuscript in preparation. Public code examples will be added after manuscript finalization and advisor/coauthor approval.

---

## Bayesian Spatiotemporal Modeling for Longitudinal High-Dimensional Data

This project develops a Bayesian spatiotemporal model for longitudinal and multivariate DNA methylation summary statistics. The model combines spike-and-slab priors, latent Gaussian fields, covariance estimation, and posterior inference to identify genomic regions where methylation effects are persistent or time-varying.

A key part of the method is defining DMRs directly through posterior probabilities at the region level, rather than relying only on site-wise tests or smoothed p-values. This allows the model to distinguish between conserved regions, where effects persist across time points, and discordant regions, where the association pattern changes across time.

The framework was evaluated through simulation studies and applied to longitudinal cohort data with more than 750,000 ordered genomic features. The work emphasizes calibrated region-level inference, false discovery control, and interpretable summaries of high-dimensional correlated data.

**Methods:** Bayesian hierarchical modeling, spike-and-slab priors, latent Gaussian fields, covariance estimation, posterior inference, false discovery rate control, simulation studies.

**Status:** Manuscript in preparation; code repository forthcoming after manuscript finalization.

---

## Spatial Empirical Bayes Modeling for Heterogeneous Correlated Data

This project extends the region-level inference framework to settings where spatial dependence varies across genomic regions. Many existing DMR methods use a fixed smoothing rule or a single genome-wide dependence structure, which can over-smooth some regions and under-smooth others. This project instead uses a spatial empirical Bayes model that allows different regions to adapt to different dependence regimes.

The method uses a grid of spatial covariance structures and estimates mixture weights across regimes. For each candidate region, posterior quantities are computed using scalable approximations, including expectation propagation, importance sampling, pseudo-likelihood estimation, and mixture optimization. These posterior summaries are then used to guide DMR discovery and quantify uncertainty.

The project was evaluated through simulation studies and real-data analyses, with a focus on calibration, localization, posterior uncertainty quantification, and comparison against standard DMR detection tools.

**Methods:** Empirical Bayes, spatial modeling, expectation propagation, importance sampling, pseudo-likelihood, mixture optimization, posterior uncertainty quantification.

**Status:** Manuscript in preparation; code repository forthcoming after manuscript finalization.

---

## Research Interests

- Bayesian inference and empirical Bayes methods
- High-dimensional statistical modeling
- Spatial and temporal dependence
- Gaussian processes and latent variable models
- Simulation-based model evaluation
- False discovery rate control and uncertainty quantification
- Applied statistical computing in R and Python
