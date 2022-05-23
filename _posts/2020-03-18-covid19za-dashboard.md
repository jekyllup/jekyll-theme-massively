---
layout: post
title:  "A repo and dashboard for COVID-19 in South Africa"
date:   2020-03-18
excerpt: "How and why we built the dashboard. Dr. Vukosi Marivate - Dept. Computer Science"
image: ""
---

**TLDR:** *We collected and collated data from the South African Department of Health [DoH] and National Institute for Communicable Diseases [NICD] statements and alerts. From there we built a dashboard that you can access at [https://bitly.com/covid19za-dash](https://bitly.com/covid19za-dash). In this post, we will go over some design decisions we made so that you can understand how we thought about the project.*

## What is this about?
In this post, I talk a little about how a few volunteers started a repo to consolidate the numbers that are released by the South African Department of Health [DoH]. The National Institute for Communicable Diseases [NICD] is the source of our COVID-19 [Corona virus] case data. First, let’s give you some background for context and clarity.

### What is COVID-19?
As per [http://www.sacoronavirus.co.za](http://www.sacoronavirus.co.za): *“On 31 December 2019, the World Health Organization (WHO) reported a cluster of pneumonia cases in Wuhan City, China. ‘Severe Acute Respiratory Syndrome Coronavirus 2’ (SARS-CoV-2) was confirmed as the causative agent of what we now know as ‘Coronavirus Disease 2019’ (COVID-19). Since then, the virus has spread to more than 100 countries, including South Africa”*

### Who is the NICD?
As per [http://www.nicd.ac.za](http://www.nicd.ac.za): *"The National Institute for Communicable Diseases is a national public health institute of South Africa, providing reference microbiology, virology, epidemiology, surveillance and public health research to support the government’s response to communicable disease threats. The NICD serves as a resource of knowledge and expertise of communicable diseases to the South African Government, Southern African Development Community countries and the African continent. The institution assists in the planning of policies and programmes to support and respond to communicable diseases."*

They are the experts we rely on for our confirmed case data. 

## We collect the data
From the first confirmed case by the Minister of the DoH in early March, there was a feeling that we should have a place to easily see the numbers so we can understand the full picture in South Africa. First, it meant we had to collect data from the statements. Initially, this was done manually meaning that the statements had to be read and then the data input into a CSV file. Now, one of the contributors [We have a great set of volunteers] has created a script that scrapes the NICD releases and creates an output that can be put in a CSV file. This means then that we go from this

![raw_file](https://lh6.googleusercontent.com/PFwZDcGtJdM08eWUsrpTD_AipGzey0k4P8rkSsStsaYsmeto1l5PBgY4TnLSC2F5-DTijP-I9570zVUIRVCIcp7zcvKDyCS8_xxgKXJ8YloqrRRjc5yuoPEUuhE2zXPPbEDeTZt_)

**to this**
![processed](https://lh5.googleusercontent.com/_thHo063uSxBvGsjmd_6IXCzAmsUPMnZEtnIxfvAj_hFPq6I1s8V22PLE3KAABOOKN3S6xJM3bzvmEvIUBhY6U0y6AYy9FAgnaf_qWjxe-cbef1jHS5aO6uWVNgDt5zCh_hoCx8S)

This is much easier to handle and the data is stored in the data folder

## Why don’t we consider other sources of case data?
There have been queries about using news reports as a source of data, why are we not using these? We, as a group, acknowledge that we are not health professionals and believe it will be irresponsible to assume that role. It is a tense time and we believe in keeping people informed about the current state of things, as it is shared from the public health experts. DoH and NICD have also noted these challenges about putting correct numbers out. We, as a nation, have already had to remove 1 case from the data because of misreporting. 

## The Dashboard
The dashboard is built on Google Data Studio and ONLY presents data that is confirmed from accredited public sources. We are not reporting on any information about predictions, as again (you will notice a pattern), we would like to leave this to the public health experts and researchers that have dedicated their time and expertise to focus on this. You can see the design of the dashboard below:
![dashboard](https://lh5.googleusercontent.com/8QfAkBtYFrfSrOQ9nH_N4LCIxXSofM_38HYy4r1fstGzY_FiDWXmTdGLoufR87kmjOzFkc1k0AVaYTakJa0-sBGbPp15nWuhTBRLvhIY1DA-0IlIyLc-MwPTmW7S1eWlP1MOJdHy)

## What are the open questions and analytics?
* Is the health system coping? -> Live ICU and COVID-19 prepped bed capacity
* Is social distancing working? -> Some way to see the slow down of movement and if the social distance is working? What data can we use? Traffic, daily sales etc.

## Where to from here?
We have ideas coming along and you can see some of the open issues on the repo. We now also have API capability that was added by one of the volunteers. 

## Acknowledgements
Thank you to

* Alta De Waal [Analysis Notebooks]
* Herkulaas Combrinkb[Hospital Data
* Nompumelelo Mtsweni [Hospital Data]
* Ofentswe Lebogo [Analysis Notebooks]
* Shivan Moodley [Automated Scraper]
* Vutlhari Rikhotso [API framework]
