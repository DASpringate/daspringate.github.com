---
layout: post
title: "Survival analysis in R"
date: 2014-03-25 11:04:22 +0100
comments: true
categories: [rstats, statistics]
external-url: http://rpubs.com/daspringate/survival
---

I recently gave a talk at the Manchester University Faculty of Life Sciences R user group on Survival Analysis in R.  Survival analysis is hugely important for modelling longditudinal data like cohort studies.  However, people still find it tricky to understand and even a recent paper I reviewed did a logistic regression when they should have done survival analysis. Beyond epidemiology and health research, survival analysis is a really useful addition to ecologists and biologists toolkits when they might want to model the time taken for some event to occur. For example:

* Germination timing
* Arrival of a migrant or parasite
* Seed or offspring dispersal
* Response to some stimulus

In the presentation, I discussed censoring (dealing with missing data of various kinds) and the survival function before introducing the Cox proportional hazards model. This is the most commonly used survival model because it is a semi-parametric model where you can look model the multiplicative effects of your covariates of interest (e.g. drug therapy on survival) without having to explicitly model the shape of the survival curve itself.

I then give a run through of a typical survival analysis in R before providing some links for further reading.
