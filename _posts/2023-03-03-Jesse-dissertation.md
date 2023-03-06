---
layout: post
title: "[Dissertation] BantuBERTa: Using Language Family Grouping in Multilingual Language Modeling for Bantu Languages"
date: 2023-03-03
excerpt: "Masters dissertation by Jesse Parvess, Faculty of Engineering, Built Environment and Information Technology University of Pretoria, Pretoria"
image: ""
---
## Members
Jesse Parvess, MITC Big Data Science
### Supervisor(s)
Prof. Vukosi Marivate, Dr Verrah Akinyi
## Abstract
It was researched whether a multilingual Bantu pretraining corpus could be created from freely available data. Here, to create the dataset, Bantu text extracted from datasets that are freely available online (mainly from Huggingface) were used. The resulting multilingual language model (BantuBERTa) from this pretraining data proved to be predictive across multiple Bantu languages on a higher-order NLP task (NER) and in a simpler NLP task (classification). This proves that this dataset can be used for Bantu multilingual pretraining and transfer to multiple Bantu languages. Additionally, it was researched whether using this Bantu dataset could benefit transfer learning in downstream NLP tasks. BantuBERTa under-performed with respect to other models (XlM-R, mBERT, and AfriBERTa) bench-marked on MasakhaNER’s Bantu language tests (Swahili, Luganda, and Kinyarwanda). Additionally, it produced state of the art results for the Bantu language benchmarks (Zulu, and Lingala) in the African News Topic Classification dataset. 
It was surmised that the pretraining dataset size (which was 30% smaller than AfriBERTa’s) and dataset quality were the main cause for the poor performance in the NER test. We believe this is a case-specific failure due to poor data quality resulting from a pretraining dataset consisting mainly of web-scraped pages. Here, the resulting dataset consisted mainly of MC4 and CC100 Bantu text. However, on lower-order NLP tasks, like classification, pretraining on languages solely within the language family seemed to benefit transfer to other similar languages within the family. This potentially opens a method for effectively including low-resourced languages in low-level NLP tasks.
## Publications