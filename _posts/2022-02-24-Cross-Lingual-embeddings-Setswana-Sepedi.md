---
layout: post
title: "[Publication] Training Cross-Lingual embeddings for Setswana and Sepedi"
date: 2022-02-24
image: "https://github.com/dsfsi/dsfsi.github.io/raw/master/images/2022-02-24-Cross-Lingual-embeddings-Setswana-Sepedi.PNG"
excerpt: "Paper by Mack Makgatho, Faculty of Engineering, Built Environment and Information Technology University of Pretoria, Pretoria"
---
## Members
Mack Makgatho, Vukosi Marivate, Tshephisho Sefara, Valencia Wagner

## Abstract
How can we transfer semantic information between two low-resourced African languages? With one language having more resources than the other? The problem is that African languages still lag in the advances of Natural Language Processing techniques, one reason being the lack of representative data, having a technique that can transfer information between languages can help mitigate against the data problem. This paper trains Setswana and Sepedi monolingual word vectors and uses VecMap to create cross-lingual embeddings for Setswana-Sepedi since cross-lingual embeddings can be used as a method of transferring semantic information from rich to low-resourced languages.

Word embeddings are word vectors that represent words as continuous floating numbers where semantically similar words are mapped to nearby points in n-dimensional space. Each point captures the meaning of a word with semantically similar words having similar vector values near the point. The vectors are captured in a manner that, words used in a similar context will be mapped very close to each other on a vector space. The geometric relations between words can be understood by determining the cosine distance between word vectors. The idea of word embeddings is based on the distribution hypothesis that states, semantically similar words are distributed in similar contexts (Harris, 1954). The monolingaul embeddings can be used to do cross-lingaul transfer thus improving one language from another.

Cross-lingual embeddings leverages monolingual embeddings by learning a shared vector space for two separately trained monolingual vectors such that words with similar meaning are represented by similar vectors. In this work we investigate cross-lingual embeddings for Setswana-Sepedi monolingual word vector. We use the unsupervised cross lingual embeddings in VecMap to train the Setswana-Sepedi cross-language word embeddings. We evaluate the quality of the Setswana-Sepedi cross-lingual word representation using a semantic evaluation task. For the semantic similarity task, we translated the WordSim and SimLex tasks into Setswana and Sepedi. We release this dataset as part of this work for other researchers. We evaluate the intrinsic quality of the embeddings to determine if there is improvement in the semantic representation of the word embeddings.
## Publications
* M. Makgatho, V. Marivate, T. Sefara, and V. Wagner. **Training Cross-Lingual embeddings for Setswana and Sepedi**, *Journal of the Digital Humanities Association of Southern Africa *, 2022. [NLP] <> [[Paper URL](https://upjournals.up.ac.za/index.php/dhasa/article/view/3822)] [[Preprint URL](https://arxiv.org/abs/2111.06230)] [[Dataset](https://zenodo.org/record/5673974)] **DOI:** [10.55492/dhasa.v3i03.3822](https://dx.doi.org/10.55492/dhasa.v3i03.3822) 