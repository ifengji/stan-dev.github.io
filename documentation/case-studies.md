---
layout: page
title: Case Studies
excerpt: ""
modified:
image:
  feature: feature/wide_ensemble.png
  credit:
  creditlink:
---

{:.center-txt}
open-source methods and models

The case studies on this page are intended to reflect best practices
in Bayesian methodology and Stan programming.  

# Contributing Case Studies

To contribute a case study, please contact us through the [users
group](/community/).  We require 

* a documented, reproducible example with narrative documentation
<span class="note">(preferably coded using knitr or Jupyter)</span> and

* an open-source license <span class="note">(preferably BSD 3
clause)</span>; authors retain all rights, including copyright.


# *Stan Case Studies*, &nbsp; Volume 3 &nbsp; (2016)

<hr style="margin:0.25em 0 0.25em 0;"/>
<hr style="margin:0 0 2em 0;"/>

## Pooling with Hierarchical Models for Repeated Binary Trials

<small>This note illustrates the effects on posterior inference of pooling
data (aka sharing strength) across items for repeated binary trial
data.  It provides Stan models and R code to fit and check predictive
models for three situations: (a) complete pooling, which assumes each
item is the same, (b) no pooling, which assumes the items are
unrelated, and (c) partial pooling, where the similarity among the
items is estimated.  We consider two hierarchical models to estimate
the partial pooling, one with a beta prior on chance of success and
another with a normal prior on the log odds of success.  The note
explains with working examples how to (i) fit models in RStan and plot
the results in R using ggplot2, (ii) estimate event probabilities,
(iii) evaluate posterior predictive densities to evaluate model
predictions on held-out data, (iv) rank items by chance of success,
(v) perform multiple comparisons in several settings, (vi) replicate
new data for posterior p-values, and (vii) perform graphical posterior
predictive checks.</small>

Keywords
: binary trials, pooling, hierarchical models, baseball, epidemiology, prediction, posterior predictive checks

Source Repository
: [example-models/knitr/pool-binary-trials](https://github.com/stan-dev/example-models/tree/master/knitr/pool-binary-trials)
<span class="note">(GitHub)</span>

R Package Dependencies
: <tt style="font-size: 90%">rstan, ggplot2, rmarkdown</tt>

License
:  BSD (3 clause), CC-BY

View
: [HTML](case-studies/pool-binary-trials.html)


# *Stan Case Studies*, &nbsp; Volume 2 &nbsp; (2015)

<hr style="margin:0.25em 0 0.25em 0;"/>
<hr style="margin:0 0 2em 0;"/>


## Multiple Species-Site Occupancy Model

<small>This case study replicates the analysis and output graphs of
Dorazio et al. (2006) noisy-measurement occupancy model for multiple
species abundance of butterflies.  Going beyond the paper, the
supercommunity assumptions are tested to show they are invariant to
sizing, and posterior predictive checks are provided.</small>

Keywords
: ecology, occupancy, species abundance, supercommunity,
posterior predictive check

Source Repository
: [example-models/knitr/dorazio-royle-occupancy](https://github.com/stan-dev/example-models/tree/master/knitr/dorazio-royle-occupancy)
<span class="note">(GitHub)</span>

License
:  BSD (3 clause), CC-BY

R Package Dependencies
: <tt style="font-size: 90%">rstan, ggplot2, rmarkdown</tt>

View
: [HTML](case-studies/dorazio-royle-occupancy.html)


# *Stan Case Studies*, &nbsp; Volume 1 &nbsp; (2014)

<hr style="margin:0.25em 0 0.25em 0;"/>
<hr style="margin:0 0 2em 0;"/>


## Soil Carbon Modeling with RStan

<small>This case study provides ordinary differential equation-based
compartment models of soil carbon flux, with experimental data fitted
with unknown initial compartment balance and noisy CO<sub>2</sub>
measurements.  Results form Sierra and Müller’s (2014) soilR package
are replicated.</small>

Keywords
: biogeochemistry, compartment ODE, soil carbon
respiration, incubation experiment

Source Repository
: [soil-metamodel/stan/soil-knit](https://github.com/soil-metamodel/stan/tree/master/soil-incubation)
<span class="note">(GitHub)</span>

License
:  BSD (3 clause), CC-BY

R Package Dependencies
: <tt style="font-size: 90%">rstan, ggplot2, rmarkdown</tt>

View
: [HTML](case-studies/soil-knit.html)
<span class="note">(GitHub)</span>