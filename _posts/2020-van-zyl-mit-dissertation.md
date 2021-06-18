---
layout: post
title:  "[Dissertation] USE OF MACHINE LEARNING TECHNIQUES TO BETTER UTILISE MULTIPLE UNDERWRITING FACTORS IN MORTALITY PRICING AND RESERVING OF LIFE INSURANCE RISK PRODUCTS"
date:   2020-03-30
excerpt: "Masters dissertation by Collin, Faculty of Engineering, Built Environment and Information Technology University of Pretoria, Pretoria"
image: 
---
## Members
Colin van Zyl, MITC Big Data Science
## Supervisor(s)
Dr. Conrad Beyers,
Dr. Vukosi Marivate

## Abstract
Actuaries need to graduate or adjust standard tables for the expected experience of the insured popu-
lation and then make further adjustments for the various selected underwriting factors when pricing and calculating liabilities (reserving) for life insurance benefits. This is a time-consuming process that requires actuarial judgement at various steps. Automating portions of the process and introducing statistical tests to assess fit would allow more accurate pricing, inclusion of more rating factors and more regular review of pricing bases.

This research explores the use of statistical and machine learning approaches to pricing the mortality
cost of life insurance benefits (for use in pricing and reserving). In particular, the research explores
how generalised linear models and tree-based machine learning models can be used used to develop
entity specific mortality tables that account for a large number of underwriting factors.

To allow for regular review and the application of actuarial judgement at various stages, the methodology
allows for the following discrete steps:

* Derivation of a population specific standard table by adjusting an industry standard table using approaches described by Gschlössl et al. (2011) and Tomas & Planchet (2014).
* Adjustment to the standard table for common underwriting factors. For this step both generalised linear models as well as tree-based models (Model-Based Recursive Partitioning and Gradient Boosting Machines) are used.
* Adjustment to the standard table using additional underwriting factors only present in a smaller
subset of the data using similar models.

The research also aims to assess whether tree-based models can improve on simpler generalised linear models.

The results of the research illustrate the relative ease and effectiveness of the approach to derive a standard table and / or test the current tables used for an insured population for their fit, which is useful when assessing the need to make assumption or basis changes as part of the actuarial control cycle.

The results further demonstrate the effective allowance for more traditional underwriting factors such as income, smoking status and education levels for all models tested.

Results using more underwriting factors were less intuitive or suitable for use in practice despite apparent better performance of the models using criteria such as mean square error. This highlights the need for actuarial judgement and explains the lower use of such rating factors in the industry other than for initial underwriting. Options for including such factors in pricing models is discussed.

In all cases, the tree-based machine learning models (despite extensive parameter tuning) did not
meaningfully outperform generalised linear models suggesting that generalised linear models are better
suited given their easier application and interpretation.

## Publications

