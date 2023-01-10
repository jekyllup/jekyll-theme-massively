---
layout: post
title:  "Mapping the South African health facility landscape in response to COVID-19"
date:   2020-05-25
excerpt: "N Mtsweni, H Combrink, A Van der Walt, V Marivate"
image: "https://github.com/dsfsi/dsfsi.github.io/raw/master/images/flourish.png"
---

As we now move to the next phase of our country's experience of COVID-19 and its responses, we continue to look back at what the covid19za project has been busy with over the last 2 months. Our focus for this write up is on understanding our health system capacity. The lack of updated openly available health system data (data about hospitals, clinics and health resources) was identified early on in the project as a challenge. Little did project members know how much work would have to go into getting data and making it accessible. In this post, we discuss these challenges, present what has been achieved so far and propose the next steps. 

## Where we were
Initially, we wanted information on the public healthcare system related to the South African COVID-19 response for four primary reasons. We wanted to be able to identify: 
where the COVID-19 hospitals were going to be in the country; 
what the current situation in the country is related to the COVID-19 response;
when the shortages were going to arise within the public healthcare system related to the COVID-19 response; and 
how to assist the public in understanding which healthcare facilities were used for what specific response amidst the COVID-19 pandemic.

Up until this point, the questions were in their infancy and fairly descriptive in nature. No one could fathom at that point in time the challenges that lay ahead related to the available South African hospital data. Initially, a few members in the COVID-19 volunteer group started posting unique issues on Github related to the healthcare system, but as time continued, an informal working group was established where these issues were discussed and addressed. The informal working group consisted of: .

* *Nompumelelo*,  a self-employed web developer and an independent researcher;
* *Herkulaas*, a medical scientist, member of the DSFSI research group, and a Research Coordinator at the University of the Free State;
* *Anelda*,  founder of Talarify, a company that supports the implementation of open science and reproducible research practices in universities; and
* *Vukosi*, the UP ABSA Chair of Data Science and the principal investigator for DSFSI. Vukosi works on topics in Data Science for Society and Natural Language processing. 

What follows is a dive into what it actually takes to bring together information about the South African health system in order to be able to support communication and decision making. 

## Data, Data, Data

### Where did we source the data

Nompumelelo was looking for an opportunity to contribute her skills to the COVID0-19 response and came across the request for  assistance with finding accurate data about hospitals across the country, The issue was posted on the [covid19za repository](https://github.com/dsfsi/covid19za) from where the project is managed. In contributing to this issue,  she added a pivoted dataset (in a CSV format) containing geo-coordinates of the locations of hospitals in the public sector and some hospitals in the private sector. The dataset Nompumelelo contributed is a subset of a much bigger dataset from the [National Department of Health’s Data Dictionary](https://dd.dhmis.org/). This Data Dictionary is said to provide a reference point for selected health information standards to support healthcare activities within South Africa. 

Although the DoH Data Dictionary listed a large number of facilities, it did not represent the current realities of some hospitals. One example that we found was that some hospital names had changed and had not been updated. The dataset also had a large number of missing data points including, for example, physical addresses and contact details. The facilities listed did not include attributes such as capacity (number of beds, number of ICU beds), services available, and infrastructure (ambulances, ventilators, etc) that could inform the COVID-19 response. Despite the fact that the dataset contains great details about the administrative division within which a facility resorts, it lacks information about health districts and clusters. More information about the health district approach in South Africa can be found at the [Health Systems Trust](https://www.hst.org.za/publications/HST%20Publications/lg_dhs.pdf). 

The [Gauteng Cluster Policy](https://drive.google.com/file/d/1AhafV1DoTGwNRIx26J12_ICh-3vSVnyt/view) describes the concept of health clusters. The Gauteng Cluster Policy did not only have details about health facilities in each cluster in Gauteng but also provided some details about the number of hospital beds in each cluster. It should be noted that, in this report, some hospitals were duplicated (meaning one hospital could be in two different clusters) making the accounting of hospital beds per cluster questionable.  

Anelda responded to the request for assistance by recommending [a relevant study](http://www.samj.org.za/index.php/samj/article/view/12143) found via a Google search. The study looked at the geographical mal-distribution of surgical resources in South Africa. It formed part of the [PhD dissertation](https://open.uct.ac.za/handle/11427/22796) of Dr Angela Dell that was published in 2016. We reached out to Dr Dell and asked if the data underpinning the study was available. Dr Dell was incredibly helpful and published the data in [Excel format in Figshare](https://figshare.com/articles/SURGICAL_RSurgical%20resources%20in%20South%20Africa%20according%20to%20province%20(2016)ESOURCES_latestmarch2016_xlsx/12066711) (an open data repository) to allow re-use under an open license, upon our request. The dataset describes, amongst other things, the number of beds per hospital for over 500 hosptials across all provinces in both private and public sector. Despite the fact that Dr Dell’s dataset dates back to 2016, this dataset has been most useful in filling the gaps from the data dictionary.

### You don't have good data, without a good cleaning

Combining various health facility lists to create a single, complete view of a country’s health system is no trivial task. Lists cannot be merged simply by using facility names, for example. As mentioned before, facility names change over time and lists are often not updated. Furthermore, facilities may be listed under their full names, short names, and/or common names. Typos, capitalisation, mis-spelling, and varying naming conventions all contribute to the challenge of merging health facility lists by facility name.

To understand some of the real-world challenges experienced in the analysis and merging of health facility lists and identify steps that can be streamlined for others wanting to do the same, Anelda set out to assist with collating the South African data. Some aspects of the datasets and challenges experienced are discussed in this [blog post](http://www.afrimapr.org/blog/2020/merging-health-facility-lists-part1/) with supporting [R Markdown file](https://github.com/anelda/merge_open_hospital_data/blob/master/reports/merge_open_hospital_data_part1.Rmd) and [full report](https://htmlpreview.github.io/?https://github.com/anelda/merge_open_hospital_data/blob/master/reports/merge_open_hospital_data_part1.html) available from Github. 

This work is also feeding into the [_afrimapr_ project](http://afrimapr.org), a Wellcome Open Research Fund project hosted at the Liverpool School of Tropical Medicine, of which Anelda is part. The overarching aim of _afrimapr_ is to develop reusable open-source R building blocks to make open African health data more accessible. One of the focus areas at this stage is the [_afrihealthsites_ package](https://andysouth.shinyapps.io/healthsites_viewer/) that currently provides easy access to two continental open health facility datasets - one developed by the [KEMRI Wellcome Trust Research Programme](https://www.nature.com/articles/s41597-019-0142-2) and hosted by WHO, and a second collated by [healthsites.io](https://healthsites.io/). Ongoing work includes adding functionality to include self-defined health facility lists (such as the ones described in this blog post) for visualisation and analysis. 

Since data is being collected from a wide variety of sources published under a variety of licenses (or even without obvious licenses), we had to figure out a way to keep track of data sources and ensure proper credit is given. The [README file](https://github.com/dsfsi/covid19za/blob/master/data/README_hospital_data.md) summarises data sources and provides links to the original raw data. Gaps still exist and are being addressed.

What we have identified as challenges with open health facility data in South Africa is incomplete, fragmented, and outdated data [in some cases]. This then provides challenges for responding in realtime to a disaster by those who need the data.  Why is openly available, updated, complete health facility data important? The [Master Facility List Resource Package](https://www.who.int/healthinfo/MFL_Resource_Package_Jan2018.pdf?ua=1) developed in 2018 by the WHO recommends that countries make their master health facility list openly available. According to this guide, and in line with open science and open government philosophy, data’s value lies in the ability of people to access it. Open health facility data can be used by various government departments, donors, development partners, civic society, and more. Open data can enhance transparency, lead to improved quality (more eyes on the data), and increased efficiency (duplicated out of sync lists can be replaced by a single open data source).

We have made progress with getting data but it is still not enough. Over the next few weeks we will attempt to find clear hospital descriptions, operational functions, contact details, and most importantly the COVID-19 status of health facilities. We will also combine the population estimates for local municipalities and districts with the facility data. Current bed numbers in hospitals have not been verified. We’d also like to add the locations of recently developed field hospitals and add information about hospitals (both in the public and the private sector) that are being upgraded, as it becomes available.

## Inspiration

A project that has been inspirational to us, specifically in terms of sharing the number of beds available, is [this volunteer project](https://coronavis.dbvis.de/en/) that allows for the visualisation of intensive care unit bed capacities of German hospitals. 

![](https://github.com/dsfsi/dsfsi.github.io/raw/master/images/testingmap.png)


Some of the outputs from the healthcare facilities data collected by the team so far include:
![](https://github.com/dsfsi/dsfsi.github.io/raw/master/images/germanicu.png)


-a [COVID-19 testing map](https://www.ineff.ch/cov19testmap/) developed by a Switzerland based entrepreneur with more explanations in [this article](https://www.ineff.ch/2020-04-03-The-COVID-19-Testing-Facility-Map/); and 

-a collection of South Africa’s healthcare facilities visualizations developed by us (Nompumelelo with the input from Anelda, Vukosi and Herkulaas).


## Where to next

Our next goal is to complete other missing parts and update the health facility dataset with current developments made by the government and others. Developments such as upgrading of public hospitals, addition of beds in some hospitals and development of field hospitals for triage. We hope to populate the dataset with data related to these current developments in preparation for the anticipated surge of COVID-19 cases over the next few months. Nompumelelo will also continue to work on the visualisations and incorporate feedback from the community to make these more useful. We invite collaboration and input from the community and welcome collaboration.

### Tools for healthcare workers

We are planning to develop a Progressive Web Application that will enhance accessibility of the complete dataset available from the covid19za repository as well as the data visualisations to people living in remote, low-bandwidth areas.
