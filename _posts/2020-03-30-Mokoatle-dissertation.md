---
layout: post
title:  "[Dissertation] Road Traffic Accident Analysis Using Machine Learning Techniques for Soshanguve, Pretoria"
date:   2020-03-30
excerpt: "Masters dissertation by Mokoatle,  North West University"
image: "https://github.com/dsfsi/dsfsi.github.io/raw/master/images/mokoatleImg.png"
---
## Members
Mpho Mokoatle, Masters Computer Science

| Supervisor     | Co-supervisor   | Co-supervisor |
|--------------- |:---------------:|:---------------:|
|Prof BM Esiefarienrhe| Dr VN Marivate| Mrs TL Letlonkane|

## Abstract
Road traffic accidents (RTAs) in South Africa reached the highest road death toll in 2017, in  spite of road safety campaigns and initiatives. “ Ongoing campaigns are simply not sufficient’’, 
said a representative from the South African Automobile Association (AA). RTA data is usually
collected at accident scenes and those who collect this data lack sufficient knowledge and skill to 
translate the data into knowledge that can be used to gain a better understanding of the root 
causes and factors associated with the occurrence of an accident. The South African literature on 
RTAs has shown a limitation in using advanced methods such as machine learning, to extract 
insight from RTA data or trace patterns and trends that are associated with the occurrence of an 
accident. In this work, machine learning methods were deployed to study the relationships that 
exist in data that is captured on South African Accident Report (AR) forms. An AR form is a 
form that is completed for all RTAs that occur on a public road where a motor vehicle was 
involved [1]. In order to increase the data, distances to the nearest places of interest such as bars, 
malls, schools, restaurants, and buildings were extracted through a geospatial database and added 
to the AR data. The reason behind this was to determine if distances to the nearest places of 
interest have an impact on the injury severity of drivers in RTAs. First, the main characteristics 
in the data were summarized by performing the exploratory data analysis. Upon completion of 
the exploratory data analysis, it was found that truck license holders particularly code C1, used 
light vehicles such as motor cars, in comparison to heavy motor vehicles. The results from the 
exploratory data analysis also revealed that these drivers sustained the most severe injuries in 
RTAs, different from light motor vehicle drivers. In South Africa, duty licenses are granted with 
various codes that indicate the kind of vehicle that may be used with that duty license; the codes 
are shown in Appendix A. It should also be noted that the tests for each license code are
conducted differently using different vehicles. For example, when testing for a heavy duty 
license code C1, the test is conducted on a vehicle with a Gross vehicle mass (GVM) of 3500 kg 
and less than 16000 kg, and when testing for a light motor vehicle duty license code B, the test is 
conducted on a vehicle with a GVM of ≤ 3500 kg. To determine if truck licenses code C1 and
the distances to the nearest places of interests such as malls, bars, schools, restaurants, and 
buildings have a high importance on the injury severity of drivers in RTA, three classifiers were 
created by using parametric and non-parametric machine learning algorithms namely; v
Multivariate Logistic Regression (MLR) and the Extreme Gradient Boosting Tree (XGBoost), 
where XGBoost outran MLR. The first classifier was created using the extracted distance 
features and the target class (injury severity), the second classifier was created using the initial 
data that is collected on AR forms and the third classifier was created by integrating engineered 
distance features and data that is collected on AR forms. This model achieved an accuracy of 
83.14%±3.34 %, and a precision, recall, and an F1 score of 82.83%±3.18 %, 82.66 %±3.16 %, 
and 82.35%±3.25 %, respectively. Also, the most significant predictors of injury severity of 
drivers in RTAs were found to be truck licenses code C1, light motor duty license code EB, 
vehicle type (motor car or station wagon), single vehicle: overturned accident type, vehicle 
maneuver and the distance to the closest building. There are several mitigation strategies that can 
arise as a result of confirming whether or not the distances to the nearest places of interest, or if 
the kind of duty license that a motorist has have a high importance on injury severity. For 
example, if the type of duty license and the distances to the nearest places of interest have a 
significant impact on the level of injury in RTAs, than it may be useful to explore how adjusting 
the current status quo will improve safety on the road which states that motorists with heavy duty 
licenses are allowed to use light motor vehicles. Moreover, if closest places of interests also play 
a role in the injury severity of drivers in RTAs, this information can direct policymakers to areas 
of high accident occurrences and proactive measures can then be taken such as to create a road 
safety awareness down the affected line i.e, N1, N14; allocate more funds to improve the road, 
ensure that medical services are close by to provide optimal treatment of rehabilitation following 
the injury such as effective first aid and appropriate care, and also increase traffic personnel in 
the affected area.
The study also searched for frequent attributes that co-exist in the incidence of a RTA by 
applying the association rule mining technique. Before searching for frequent items that co-exist 
in the data, the clustering was performed as a preliminary step. This resulted into having two 
clusters and the support, confidence, and lift of the rules found in the first cluster were 0.21, 0.71 
and 2.05 respectively. Similary, the support, confidence, and lift of the rules found in the second 
cluster were 0.22, 0.71 and 2.35 respectively
## Publications
* Mokoatle, M., Vukosi Marivate, D. and Michael Esiefarienrhe Bukohwo, P., 2019, June. Predicting road traffic accident severity using accident report data in South Africa. In Proceedings of the 20th Annual International Conference on Digital Government Research (pp. 11-17). [[Link](https://dl.acm.org/doi/abs/10.1145/3325112.3325211)].
* Mokoatle, M. and Marivate, V., 2018, August. Collision Course: Challenges with Road Traffic Accident Data in South Africa. In 2018 International Conference on Advances in Big Data, Computing and Data Communication Systems (icABCD) (pp. 1-6). IEEE.[[Link](https://ieeexplore.ieee.org/abstract/document/8465419)].
