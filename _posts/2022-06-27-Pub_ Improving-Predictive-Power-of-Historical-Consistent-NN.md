---
layout: post
title: "[Publication] Improving the Predictive Power of Historical Consistent Neural Networks"
date: 2022-06-27
image: "https://github.com/dsfsi/dsfsi.github.io/raw/master/images/2022-06-27-vanilla-HCNN-ensemble-comp.PNG"
excerpt: "Paper by Rockefeller Rockefeller, Bubacarr Bah, Vukosi Marivate, and Hans-Georg Zimmermann , *African Institute for Mathematical Sciences, Cape Town, South Africa; 
*Department of Mathematical Sciences, Stellenbosch University, Cape Town, South Africa;
Department of Computer Sciences, University of Pretoria, Pretoria, South Africa;
Fraunhofer Society, 200703 Munich, Germany, Germany"
---
## Members
Rockefeller Rockefeller, Bubacarr Bah, Vukosi Marivate, Hans-Georg Zimmermann 

## Abstract
The Historical Consistent Neural Networks (HCNN) are an extension of the standard Recurrent Neural Networks (RNN): they allow the modeling of highly-interacting dynamical systems across multiple time scales. HCNN do not draw any distinction between inputs and outputs, but model observables embedded in the dynamics of a large state space. In this paper, we propose to improve the predictive power of the (Vanilla) HCNN using three methods: (1) HCNN with Partial Teacher Forcing, (2) HCNN with Sparse State Transition Matrix, and (3) a Long Short Term Memory Formulation of HCNN. We investigated the effect of those long memory improvement methods on three chaotic time-series mathematically generated from the Rabinovich–Fabrikant, the Rossler System and the Lorenz system. To complement our study, we compared the accuracy of the different HCNN variants with well-known recurrent neural networks methods such as Vanilla RNN and LSTM for the same prediction tasks. Overall, our results show that the Vanilla HCNN is superior to RNN and LSTM. This is even more the case if you include the above long memory extensions (1), (2) and (3). We demonstrate that (1) and (3) are superior for the modeling of our chaotic dynamical systems. We show that for these deterministic systems, the ensembles are narrowed.
## Publications
* R. Rockefeller, B. Bah, V. Marivate, and H.G. Zimmermann. **Improving the Predictive Power of Historical Consistent Neural Networks**, *  Engineering Proceedings, 2022. [ML]  <> [[Paper URL](https://www.mdpi.com/2673-4591/18/1/36)] **DOI:** [10.1145/3543434.3543484](https://doi.org/10.3390/engproc2022018036) 