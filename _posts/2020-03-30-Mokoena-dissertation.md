---
layout: post
title:  "[Dissertation] Why is this an Anomaly? Explaining Anomalies using Sequential Explanations "
date:   2020-03-30
excerpt: "Masters dissertation by Mokoena, Faculty of Science, University of the Witwatersrand, Johannesburg."
image: "https://github.com/dsfsi/dsfsi.github.io/raw/master/images/Tshepiso.png"
---
## Members
Tshepiso Mokoena, Masters Computer Science
| Supervisor     | Co-supervisor   | 
|--------------- |:---------------:|
|Prof. Turgay Celik| Dr VN Marivate| 

## Abstract
Anomaly detection has received much attention throughout the years. Currently, human analysts in real-world applications use anomaly detectors to assist them in identifying
potential anomalous data points. Unfortunately, most anomaly detectors do not provide
the analysts with explanations about what makes a data point anomalous, resulting
in the analysts to consider the information related to the entire feature space of each
detected data point to decide whether they are truly anomalous or not. This process can
be time-consuming and costly in most domains, especially if the feature space is large,
and feature interactions are critical to the analyst’s judgement. To assist the analyst
and minimise the number of features that they must analyse to identify true anomalies
confidently, we introduce an explanation called a Sequential Explanation(SE). A SE
for a detected data point contains subsets of features that explain why the detected
data point could be anomalous to the analyst. The first subset in the SE contains only
one feature; the second subset contains two features; the third subset contains three
features, and so on. The subsets of features explain to the analyst why the detected
data point could be anomalous. The subsets of features in the SE are incrementally
presented to the analyst one at a time, in order, until the analyst has acquired enough
information to decide whether the data point is an anomaly or not. In this thesis, we
introduce two novel methods of generating SEs that will work alongside any anomaly
detector. The first method is the outlier-based method that adds features in the SE
by using an anomaly detector’s outlier scoring measure guided by a search algorithm.
The sample-based method uses sampling to turn the problem into a classical feature
selection problem such that any feature selection algorithm can be used to generate
the SE. In our experiments we (i) analyse the performance and complexity of different
anomaly detectors’ outlier scoring measures and search algorithms in the outlier-based
SEs, (ii) analyse the performance and complexity of different feature selection methods
in the sample-based SEs and (iii) compare the outlier and sample-based SEs based on
their performance and complexity. In addition we also introduced a new and improved
method of evaluating explanations called the area under the curve of the analyst certainty
curve (AUCC). Our results show that both the outlier and sample-based methods can
generate SEs which significantly outperform randomly presenting features to the analyst.
In conclusion, we found that our SEs were able to identify the features that explain the
anomalies and that our new evaluation method is an improvement on the previous
evaluation method used to evaluate explanations.
## Publications
* Mokoena, T., 2019. Why is this an anomaly? Explaining anomalies using sequential explanations (Doctoral dissertation). [[Link](https://ieeexplore.ieee.org/abstract/document/7838143?casa_token=bouNXb4PYO4AAAAA:gv53w2X5pscr0LnbkPYfbT2OwAJiU3Je1-hx4jJ7wQ-5R1zBSWc-7xHDu8xRDP1xBjZGU2Z04iU)]. 
