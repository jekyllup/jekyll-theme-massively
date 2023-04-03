---
layout: post
title:  "From Data Engineering to Natural Language Corpora - The DSFSI 2022/2023 Summer Internship"
date:   2023-03-31
excerpt: "Richard Lastrucci and Isheanesu Dzingirai - The main focus was collection, processing and creation of parallel corpora in the 11 official languages of South Africa. We collected multilingual data by building web scrapers, we processed and cleaned this and other extracted data before performing sentence alignment to produce the parallel corpora. We also improved and documented Masakhane Web."
image: /images/2023-03-31-Summer-Internship-post.png
---

## Summary and Introduction to the research

For the recess period we worked on a variety of tasks that mostly involved the lower end of the data science pipeline, as well as some software development, documentation and research work. The main focus was collection, processing and outputting parallel corpora in the 11 official languages of South Africa. We collected multilingual data by building web scrapers, we processed and cleaned this and other extracted data before performing sentence alignment to produce the parallel corpora. For software development, we improved and documented Masakhane Web. Documentation was also created on how to instantiate and use GCP spot instances, and finally we collaborated on the compilation and editing of research papers for submission to journals.

## Why is it important?

Why each task is important is listed below.  The 1st point discusses the web scrapers created. The 2nd point discusses the importance of parallel corpora. The 3rd point discusses the development of Masakhane Web. The 4th point discusses the documentation for GCP.  Finally, the 5th point discusses the research work conducted.

1. We collected multilingual data for the 11 official languages of South Africa and several of these languages are categorised as low resource. Most NLP and AI tasks require data so it is crucial that data be sourced for these tasks to be successful.
2. Parallel corpora are vital for many downstream NLP tasks. However, lack of such corpora hinders research and development of NLP in Africa. We worked to create parallel corpora from raw text data to be used in whatever task it might be useful for.
3. Masakhane Web is a platform to host MT models for many african languages that also allows users to provide feedback on the quality of translations. However the platform can be quite unreliable at times. We worked to improve the service so that it can come closer to delivering on its goal of providing a translation service for speakers of low resource languages.
4. The research group uses GCP instances to develop and train AI models - however this can be quite expensive to maintain in the long term. Thus we looked into the usage of Spot Instances which use non-priority resources on GCP to decrease the cost.
5. From exposure to Tasks 2 and 3, we collaboratively edited a paper regarding Masakhane web, as well as creating a paper detailing the parallel corpora that was created. These papers were important as it will draw other researchers to Masakhane Web, which is part of the participatory project Masakhane, and it will also bring attention to the newly created corpora which could be used for a range of NLP tasks.

## Information about the Summer experience program

The research experience program was started within the DSFSi research group in Winter (June-July 2022) to expose students to research through working with DSFSI group members on different research projects. With the Summer edition, we successfully concluded the first year of the program. This blog post goes into the technical details of the research of one of the student teams. We acknowledge the support of NVIDIA (Hardware grant for GPUs), ABSA (through the ABSA UP Data Science Chair funding for remuneration of the students), Tensorflow for funding for research costs. If you would like to support the sustainability of this program and expansion for the future, please get in touch with Prof Vukosi Marivate vukosi.marivate@cs.up.ac.za

## Research details

The technical details of each task are as follows, The task are omitted as they weren’t technical in nature:

1. Several web scrapers were created:
    * The gov_cab_statements scraper was created using Python, it compiles links of all available cab_statments and extracts the raw text from each individual link. The web scraper was also automated by scraping the date off each link and only scraping past the last saved date. The raw data was saved into a json file for further processing.
    * The UKZN term bank was created using Python with Selenium and Pandas to extract the term banks for all 11 official languages in South Africa while the.  OERTB term bank from the University of Pretoria was created using Python and beautiful soup. The extracted data was stored in their respective csv files for further processing and use.
2. Parallel corpora were constructed from the raw text data of the gov_cab_statment data and Vukuzenzele. The corpora construction was done with the use of Python, we cleaned and sentence tokenized the raw text data before feeding it to a LASER encoded which output a vector representation of the sentences. Thereafter comparing the vectors using a cosine score and writing aligned sentences to csv.
3. Masakhane Web was written with Python using a Flask API and a PostgreSQL database. We collected  all available models and made them available on Zenodo, thereafter migrating the process of downloading models from Google Drive and Github to Zenodo. We also found a solution to loading a default language on service startup. Finally, extensive documentation was created for the backend involving code comments, API and server documentation, debugging information, and project structure.

## Significant Results

The most significant result we achieved was the sentence alignment of the government cabinet speeches on the github repo [https://github.com/dsfsi/gov-za-multilingual](https://github.com/dsfsi/gov-za-multilingual),  Vukuzenzele dataset on the github repo [https://github.com/dsfsi/vukuzenzele-nlp](https://github.com/dsfsi/vukuzenzele-nlp) as well a paper that is now in review. The paper preprint is available “Preparing the Vuk'uzenzele and ZA-gov-multilingual South African multilingual corpora” - [https://arxiv.org/abs/2303.03750](https://arxiv.org/abs/2303.03750). The paper has been accepted for presentation at the [Fourth workshop on Resources for African Indigenous Languages (RAIL)](https://sadilar.org/index.php/en/2/374).

## Personal Takeaways from the Summer Research program

### Isheanesu Dzingirai

My time with the Data Science for Social Impact Research group was nothing short of exceptional. Through my various interactions with the group members, I was able to expand my knowledge in NLP. I also enhanced my skill on how to write a research report which will truly benefit me with my honours research. I also learnt through the summer research program to always give back to the community and to do things that make a positive impact on people’s lives.I hope to work with them again in the future.

### Richard Lastrucci

I enjoyed my time working for the research group. I learnt many new things, technical and otherwise. I really liked web scraping - it is a task that involves some critical thinking and bare logic programming which I enjoyed thoroughly. I came into the group with a very narrow view of data science and have since developed a strong appreciation for language and language processing. I hope to have contributed in a meaningful way and am very grateful to have been given the opportunity.

## Why would you suggest others apply for this position in the future?

### Isheanesu Dzingirai

Yes I would suggest others interested in data science to apply for this position as it provides the opportunity to work with a team of experts in the field, collaborate with people in academia, industry and non profit organisations while gaining experience in data analysis and machine learning.

### Richard Lastrucci

I would suggest others to apply for the position as a means to grow yourself and your skills while also contributing to — and collaborating with — a research group looking to positively impact the space it works in.

## Author Bios

### Isheanesu Dzingirai

I am a well-presented, highly focused, and intelligent computer science graduate and software engineer passionate about data science and machine learning with the aspiration of one day becoming a machine learning engineer. I am also proficient in a range of modern programming languages and technologies including Python, C++, and Java.

### Richard Lastrucci

I am a 3rd year Computer Science student with a keen interest in programming and statistics. I hope to become a Data Scientist one day because I have a strong curiosity about the world around me and I appreciate data science as a tool to ask and answer questions relating to almost any topic.

*You can read more about the other student team experience* <> [DSFSI Summer Research Experience: Fine-tuning Multilingual Pre-trained African Language Models](https://dsfsi.github.io/blog/Fiskani-Rozina-internship/)
