---
title: 'shinyssdtools: A web application for fitting Species Sensitivity Distributions (SSDs)'
date: '2020-06-02'
authors:
- affiliation: 1
  name: Seb Dalgarno
  orcid: 0000-0002-3658-4517
affiliations:
  index: 1
  name: Poisson Consulting, Nelson, British Columbia
bibliography: paper.bib
tags:
   - R
   - Shiny
   - ssdtools
   - species sensitivity distributions
---

# Summary

`shinyssdtools` is a Shiny [@shiny] web application for fitting Species Sensitivity Distributions (SSDs).
The application provides a Graphical User Interface (GUI) to the `ssdtools` R package [@ssdtools].

SSDs are used to estimate the concentration of a chemical that affects a certain percentage (typically 5%) of the species considered [@posthuma_species_2001]. 
The `ssdtools` R package allows model averaging using information-theoretic criteria and the construction of confidence intervals using bootstrapping [@ssdtools].

### Graphical User Interface

The `shinyssdtools` web app, which is available in French or English, provides access to the core functionality of `ssdtools` via five navigational tabs. 

1. Data
   - Upload a dataset or enter data manually.
1. Fit
   - Select distributions.
   - Calculate information-theoretic criteria.
1. Predict
   - Estimate the concentration that affects a specific percentage of the species.
   - Calculate confidence limits using bootstrapping.
1. R code
   - Copy the R code required to reproduce the results.
1. User guide
   - Step-by-step guide to proper use of the application.
   
The app also allows the user to download plots and tables, calculate goodness-of-fit criteria, and estimate the percentage of species affected by a specific concentration.

![shinyssdtools user interface](shinyssdtools_ui.png)

# Installation

The `shinyssdtools` application is available at https://bcgov-env.shinyapps.io/ssdtools/.
`shinyssdtools` is bundled as an R package [@r] to allow the user to install and run locally using just three lines of R code:

```r
install.packages('remotes')
remotes::install_github('bcgov/shinyssdtools')
shinyssdtools::run_ssdtools_app()
```

# Contribution

The similarly named `shinyssd` is an alternative open source Shiny web application to fit SSDs that is also bundled as an R package [@dandrea_shinyssd_2019].
`shinyssdtools` contributes by being bilingual; providing additonal distributions including the gamma, Gompertz and log-Gumbel; by allowing the user to model average and by providing the R code to replicate the analysis.

# Acknowledgements

We acknowledge contributions from Angeline Tillmanns, Marianne Métivier, Andy Teucher, David Fox, Carl Schwarz and Joe Thorley.
Development of `shinyssdtools` was funded by the Ministry of Environment and Climate Change Strategy, British Columbia.

## References