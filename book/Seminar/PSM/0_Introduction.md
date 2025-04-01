---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Propensity Score Matching (PSM)

Dear students, 

In the previous session we introduced `EffectLiteR` as a powerful statistical tool to investigate treatment effects decomposition from the perspective of individual differences. You learned that this package can be used to investigate relationships between manifest and latent variables after accounting for the effects of one or several covariates.

This tutorial will introduce **propensity score matching (PSM)**. This methodology permits observational studies to mimic one of the most important features of randomized controlled trials (RCTs): **Normal distribution of covariates** within all treatment groups achieved by random allocation of units. This characteristic drastically reduces potential effects of confounders and observational-unit selection bias, thereby strengthening the explanatory power of a given independent variable and increasing the internal validity of an experimental setting. 

Here is the outline for today:

* A working example

* Propensity Score Matching