---
layout: post
title:  "[Dissertation] THE DESIGN AND IMPLEMENTATION OF A DOMAIN-ADAPTIVE DEEP REINFORCEMENT LEARNING TEXT CLASSIFICATION ARCHITECTURE"
date:   2021-03-30
excerpt: "Masters dissertation by Andreas Bayer, Faculty of Engineering, Built Environment and Information Technology(Big Data Science) University of Pretoria, Pretoria"
image: "https://github.com/dsfsi/dsfsi.github.io/raw/master/images/Andreas.png"
---
## Members
Andreas Bayer, MITC Big Data Science
### Supervisor(s)
Dr. Vukosi Marivate , Abiodun Modupe

## Abstract
Breakthroughs in text classification and other machine learning tasks in the domain of natural language processing have made headlines in the past decade. A significant contribution to this success has been made by progress in the development of language models. However, this progress comes at a cost: model sizes of state-of-the-art architectures, such as Embeddings from Language Models (ELMo) or Bidirectional Encoder Representations from Transformers (BERT) have grown significantly in parameter size, thus rendering the training of such models increasingly expensive. Moreover, practical problem settings have advanced, with many of them in security-related fields. An example is the discrimination of the surge of fake and deceiving information flow from legitimate information. The performance in such problem settings may not be limited by the sophistication of the utilised language and classification model architecture for one particular task but by the value which can be derived from available data of limited volume and mixed quality as well as the ability to derive insight from classification models which were trained for different, but potentially related, targets. Imperfections in labelled data for supervised text classification tasks include scarce data or data whose
labels might be biased, unavailable or applicable to a different problem setting. Untreated, they might lead to biased, unfair models with poor generalisation properties on unseen data and insufficient knowledge transfer properties. Different, but potentially related targets, may include models in different application contexts, such as different geographies. One approach is to design models in a way to mimic transferable skills, rather than task-specific skills. This can then be applied to derive new tasks with minimal additional training effort.

This research proposes a deep reinforcement learning architecture with favourable domain adaptation characteristics and quantifies the performance in a series of experiments. Firstly, three datasets are chosen, three separate text classification tasks are defined and three models are pre-trained. Thereafter measures are taken to quantify how the deep-reinforcement-learning-based architecture adapts to changing tasks, either by influencing the reward received for individual classes of data records on the same datasets on which the models have been trained, or by training the three models with the records of the remaining two datasets and problem definitions. Secondly, it is demonstrated how the architecture can be utilised in settings with scarce labelled data. Concretely, pseudo-labelling, a semi-supervised learning approach, is incorporated into the proposed architecture. Lastly, the architecture is utilised in a multi-task-learning problem setting, to demonstrate its usage in comparison to a grid-search in order to find model weights for models in ensembles.

## Publications

