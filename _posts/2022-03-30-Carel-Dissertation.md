---
layout: post
title: "[Dissertation] Using NER and Doc2Vec to cluster South African criminal cases"
date: 2022-03-30
excerpt: "Masters dissertation by Carel Kagiso Nchachi, Faculty of Engineering, Built Environment and Information Technology University of Pretoria, Pretoria"
image: "https://github.com/dsfsi/dsfsi.github.io/raw/master/images/Carel.PNG"
---
## Members
Carel Kagiso Nchachi, MITC Big Data Science
### Supervisor(s)
Prof. Vukosi Marivate
## Abstract
The judicial system is the central pillar of law and order across the world. It is responsible for
maintaining order amongst citizens and also solving litigations that arise. Although this system has worked quite well, there still exists several challenges, such as racial biases in cases, shortage of legal professionals and inconsistencies with regards to rulings in cases. These challenges need to be addressed in order to maintain law and order in society and to help strengthen the criminal justice system. Researchers have incorporated Natural Language Processing (NLP) techniques to help address some of these challenges. Focusing primarily on three legal applications, which are Legal Judgment Prediction (LJP), Similar Case Matching (SCM) and Legal Question Answering (LQA)[28].

SCM focuses on identifying the relationships among cases using the available information. In other words, SCM is focused on segmenting or grouping legal cases. This is especially useful for Common Law judicial systems, where judicial decisions are based on similar and representative cases that have happened in the past. South Africa uses this type of judicial system.

Although good progress has been made in SCM applications, there currently exists several challenges found in the these models. These challenges include using entities found in a legal document to improve the matching of similar cases and the interpretability of these models.

In this research we will focus on applying the SCM application on South African criminal cases, by creating a model that will be able to match similar crime cases together. This model will also solve the two challenges currently faced in SCM applications.

We found that using a Named Entity Recognizer (NER) with a Paragraph Vector-Distributed memory (PV-DM) model produced better results than using conventional PV-DM or TFIDF model. This model also overcomes the current SCM challenges as it uses the entities found in cases as the main variables for the model (using the NER model). Since the entities help explain how the model mapped similar case, this makes the model also interpretable.Based on the accuracy (similarity score) of the model, we can use this model as tool to segment criminal cases in real life.
## Publications

