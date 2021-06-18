---
layout: post
title:  "[Dissertation] Anomaly detection in the open financial market: A Case for the Bitcoin Market"
date:   2020-03-30
excerpt: "Masters dissertation by Monamo, Faculty of Engineering and Electronics, University of Johannesburg"
image: "https://github.com/dsfsi/dsfsi.github.io/raw/master/images/patrickImg.png"
---
## Members
Patrick Monamo,  
### Supervisor(s)
Prof Bhekisipho Twala,
 Dr VN Marivate
## Abstract

In the Bitcoin network, lack of class labels tend to cause obscurities in anomalous financial behaviour interpretation. To understand fraud in the latest development of the financial sector, a multifaceted approach is proposed. In this research work, Bitcoin fraud is described from both global and local perspectives using trimmed k-means and kd-trees under the assumption of the existence of a maximum 1% of anomalies. The results of the two spheres are welded together based on agreements of detected anomalies to obtain a dataset with 0.2% belonging to the anomaly class and 99.8% normal class. The study further investigate the Bitcoin dataset from the class imbalance problem viewpoint by focusing on two levels of class imbalance severity. Most counter strategies proven to be effective include the re-sampling methods, instance weighting and cost-sensitive learning with CART as the base learner. Despite effectiveness, re-sampling methods require vector representation for instance propagation. On the one hand, cost-sensitive learning contains cost errors which are often unknown in advance while on the other hand instance-weighting techniques find it difficult to keep track of global objectives.

Supervised learning algorithms are employed across three datasets preprocessing strate-
gies with the quest to assess the appropriateness of the extracted features in this study.
This study proposes data preprocessing using z-score, chord distance and Hellinger
distance with CART as well as its bagging and boosted versions to study the dataset
in comparison to SMOTE.

Although kd-trees provided a good performance than trimmed k-means in relation to
the 30 known criminal incidents, it remains difficult to derive a meaningful conclu-
sion given the unsupervised nature of the work. Characterization of the established
anomalous class from the spheres bears evidence that outlier activity emanate from
highly active users given attribute values. Results based on the class imbalance
shows that z-score is resistant to severely imbalance class distribution with CART.
The datasets preprocessed with both chord and Hellinger distances showed only an
average performance at 0.2% level with performance picking up with improvements
on class imbalance severity to 1%. Although SMOTE outperforms all algorithms in
terms of detecting the minority group, the false positive rate bursts, making it less
favourable to bagging and boosting. Based on Gini impurity, it was established that
the extracted features can be duped to be appropriate in terms of describing the
dataset under study irrespective of preprocessing strategy.

## Publications
* Twala, B. and Marivate, V., 2018. Anomaly detection in the open financial markets: a case for the bitcoin network. [[Link](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Unsupervised+Learning+for+Robust+Bitcoin+Fraud+Detection.+ISSA.+Patrick+Monamo%2C+Vukosi+Marivate+and+Bhekisipho+Twala+%5B2016%5D&btnG=)].
* Monamo, P.M., Marivate, V. and Twala, B., 2016, December. A multifaceted approach to Bitcoin fraud detection: Global and local outliers. In 2016 15th IEEE International Conference on Machine Learning and Applications (ICMLA) (pp. 188-194). IEEE. [[Link](https://ieeexplore.ieee.org/abstract/document/7838143?casa_token=bouNXb4PYO4AAAAA:gv53w2X5pscr0LnbkPYfbT2OwAJiU3Je1-hx4jJ7wQ-5R1zBSWc-7xHDu8xRDP1xBjZGU2Z04iU)].
