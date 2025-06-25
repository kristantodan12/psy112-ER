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

# Individual differences and treatment effect decomposition

Dear students, 

In the previous session we covered several ways in which **latent change score path models (LCS)** can be extended to investigate a wide range of hypotheses, including multiple methods for measuring a construct, multiple groups and multiple measured constructs. I suppose that you are now aware of the advantages associated with the analysis of latent variables. Unfortunately, even the inclusion of latent variables can yield biased results with respect to treatment effects if certain methodological and theoretical issues are ignored. These aspects are addressed in causality theories (e.g., those of Rubin, Pearl, Steyer).

The main goal of this tutorial is to provide an initial insight into a methodology that allows us to investigate unbiased relationships among dependent and independent variables - especially treatment effects. That is, a methodology that reduces the bias in variables' dependency by accounting for observed and/or latent covariates which might directly or indirectly affect both the dependent and independent variables.  

During this session we will:

* Explore a data example suitable for investigating treatment effect decomposition from the perspective of individual differences;
* Become acquainted with the **EffectLiteR** approach, available as an **R Shiny app**; 
* Explore some of the analysis options in **EffectLiteR** to learn how to make use of it in evaluation-related research projects;
* Conduct a full **EffectLiteR analysis**; 
