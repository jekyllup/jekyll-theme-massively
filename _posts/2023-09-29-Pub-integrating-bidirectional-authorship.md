---
layout: post
title: "[Publication] Integrating Bidirectional Long Short-Term Memory with Subword Embedding for Authorship Attribution "
date: 2023-09-29
image: /images/2023-08-16-Pub-Exploring-Covid_19.jpg
excerpt: "Paper by Abiodun Modupe and Vukosi Marivate"
---

## Members
Abiodun Modupe, Vukosi Marivate

## Abstract
The problem of unveiling the author of a given text document from multiple candidate authors is called authorship attribution. Manifold word-based stylistic markers have been successfully used in deep learning methods to deal with the intrinsic problem of authorship attribution. Unfortunately, the performance of word-based authorship attribution systems is limited by the vocabulary of the training corpus. Literature has recommended character-based stylistic markers as an alternative to overcome the hidden word problem. However, character-based methods often fail to capture the sequential relationship of words in texts which is a chasm for further improvement. The question addressed in this paper is whether it is possible to address the ambiguity of hidden words in text documents while preserving the sequential context of words. Consequently, a method based on bidirectional long short-term memory (BLSTM) with a 2-dimensional convolutional neural network (CNN) is proposed to capture sequential writing styles for authorship attribution. The BLSTM was used to obtain the sequential relationship among characteristics using subword information. The 2-dimensional CNN was applied to understand the local syntactical position of the style from unlabeled input text. The proposed method was experimentally evaluated against numerous state-of-the-art methods across the public corporal of CCAT50, IMDb62, Blog50, and Twitter50. Experimental results indicate accuracy improvement of 1.07\%, and 0.96\% on CCAT50 and Twitter, respectively, and produce comparable results on the remaining datasets.

## Publications
* Modupe, A., Celik, T., Marivate, V., & Olugbara, O. O. (2023). **Integrating Bidirectional Long Short-Term Memory with Subword Embedding for Authorship Attribution** *arXiv preprint arXiv:2306.14933* [NLP] <> [[Paper URL](https://arxiv.org/abs/2306.14933)]