---
title: Data Provenance
keypoints:
learning objectives:
questions:
---

# Data Provenance

## Week 3 Welcome:
This week's topic is to understand the life cycle of data and how that impacts work as data scientists.

We will aim to answer key questions about where data comes from and the ethical questions around the early stated of its lifespan. This will begin with readings about the origins of data as a concept and object of study itself, a translation of practices from archives for machine learning, and a look at how data has been used in statistics education.  After developing an understanding of the wide variety of ways that data is treated and understood outside of tech, we will discuss some of the ethical questions that arise when we consider data in context. Finally, we'll look more deeply at how data is documented and maintained, considering how these practices can serve as interventions to help mitigate averse impacts of data and avoid ethical missteps in data use.

Before you start the readings, take a 5-10 minutes to note how you think about data. Do you build on the definition that was given in class one, or do you have a different definition? What is the structure of data? Its source? What do you know about data and how do you know that? How is data cared for?

data (iso)
reinterpretable representation of information in a formalized manner suitable for communication, interpretation, or processing

information (iso)
(for information processing) knowledge concerning objects, such as facts, events, things, processes, or ideas, including concepts, that within a certain context has a particular meaning

Data _processing_ and therefore much of data _science_ is taught often taught from the perspective of math and computer science. Data are numbers, points in a space, elements of a set, that exist at the beginning of the process.  This week is meant to challenge these ideas, but it's ok if that's where you begin.

## Week 3 Readings

Required:

note: these are ordered in order of complexity below.

Introduction of "Raw Data is an Oxymoron" editor: Lisa Gitelman. [excerpt here](http://raley.english.ucsb.edu/wp-content/Engl800/RawData-excerpts.pdf) also available in the DSI Library

Note the varying ways data is described/defined
The timeline of data as a concept


Eun Seo Jo and Timnit Gebru. 2020. Lessons from archives: strategies for collecting sociocultural data in machine learning. In Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency (FAT* ’20). Association for Computing Machinery, New York, NY, USA, 306–316. [DOI: https://doi.org/10.1145/3351095.3372829](https://doi.org/10.1145/3351095.3372829)

In particular focus on:

Table 1
Section 3
Section 6
Section 8


Stigler, S. M. (2019). Data Have a Limited Shelf Life. Harvard Data Science Review, 1(2). [doi: https://doi.org/10.1162/99608f92.f9a1e510](https://doi.org/10.1162/99608f92.f9a1e510)

Focus on:

sections 2 and 3
the questions asked about the conditions of the data collection.


Additional Resources (not required reading):

We will look at these in class, but reading the full papers in advance is not required.

- [Data Sheets for Data Sets](https://arxiv.org/pdf/1803.09010.pdf)
  - [Recipe QA](https://hucvl.github.io/recipeqa/recipeqa-datasheet.pdf)
  - [QuAC](http://quac.ai/datasheet.pdf), [paper](https://arxiv.org/pdf/1808.07036.pdf)
  - [Cerema AWP](https://arxiv.org/pdf/1806.04016.pdf)
- [Dataset Nutrition Labels](http://datanutrition.media.mit.edu/abstract.pdf)
  - [Propublica Dollars for Docs](https://ahmedhosny.github.io/datanutrition/)
- [Factsheets for data](https://arxiv.org/pdf/1808.07261.pdf)
- [MithraLabel](https://dl.acm.org/doi/pdf/10.1145/3357384.3357853?download=true)
  - [live instance](http://ec2-18-219-199-72.us-east-2.compute.amazonaws.com/)
  - [info](http://mithra.eecs.umich.edu/demo/label/)


# Assignment: Data Records Memo


TLDR; Write a brief data management proposal that could be submitted to a capstone project sponsor, proposing for a particular data documentation workflow and resource set to be adopted by the data sponsor and your capstone team.


## Details

Write a memo to for a capstone project sponsor, proposing for a particular data documentation workflow and resource set to be adopted by your (hypothetical Capstone) team. The capstone project sponsor is the person or organization who defines the problem and provides data for your project, this is typically a lab at Brown or a company. where you complete an internship.  Your proposal should be applicable for all of the data that your team works with, so your proposal should describe the documentation that would help you get started on the data that you receive and what documentation your team will produce for any processed data or aggregated that you produce.

The data from your project will be used again by the project sponsor and that the data context will help future people understand the results of your project after you are no longer working with the project sponsor. Your data will be released either publicly or for broader use within the organization (as indicated per scenario).

Assume project sponsor (who you are writing your proposal for) understands the dataset itself and the potential ethical considerations associated with the data.  However, the sponsor has not been in class and is not familiar with the readings. Your proposal should state your recommendation(s) (datasheet, nutrition label, mirtha label, OAIS standard, license etc), describe what that entails, define the criteria on which you made this decision, and justify your choice. Be clear about what advantages or protections the recommended steps you provide give your sponsor.


You will submit:
  - a proposal of 1-2 pages (350-700 words)
  - a cover page describing any additional context you are assuming your recipient would have of the scenario.

Here [example template](https://docs.google.com/document/d/1nM6hh75gifsmYBtI7mtw8IPFlnqc85MtJVNOCYZV_c0/edit#) that you may copy for use.

## Evaluation

Writing and Style
- appropriate style and tone for your audience
- correct grammar and concise writing

Factual Content
- description of the proposed data documentation is correct
- appropriate criteria selected for the scenario
- evaluation of the documentation tool is appropriate
-


## Sample Scenarios

The scenarios below are derived from real capstone projects that were completed by the previous cohort of Brown DSI MS students. You may choose any one of these or write your own, by choosing the last option.


If you want to see the full reports for more detail, e-mail Dr. Brown, some of them are available. Some aspects of the scenarios are supplemented to provide more context than was in the project reports.

### Data Driven Marketing

#### Sponsor: Citizens Bank


Citizens Bank is a rapidly growing commercial bank based in New England. The bank's current expansion makes it crucial to reach all of its customers in its 11-state footprint as efficiently as possible. At Citizens Bank, with inspiration from Chairman and CEO Bruce Van Saun and directions outlined by Panickos Palettas, the team focuses on the fact that the bank's niche is ‘customer-based relationship marketing’. This team works under the leadership of the head of marketing analytics and is mostly people with statistical backgrounds. Some members of the team have been working in this domain since they ran surveys to determine marketing strategy and where to place ads in the physical world.


#### Project

The objective of this project is to improve marketing specification and personalization of ads shown on websites with respect to key marketing metrics. The dataset is very large and all calculations must be done in batch. The project will require merging datasets whose unique identifiers have a multiple-to-multiple correspondence (that is, the same identification code may appear multiple times in each individual dataset). Each component dataset will have missing data. The data provided include: finance-related information on all the people in the U.S. with a credit record as of February of 2019; information on the targeted users and labeling treatment groups and control groups; clicks on the online advertisements by person; all users’ navigation on the Citizens bank’s website and classifies them if they were directed from an online campaign or organic visits directly to Citizens; and information on applications and their approval status on different products by users with zip-code information to be used as an outcome variable. Some of the data is collected by the bank, some is purchased, and some is public information.


After your project, the data you've merged and the scripts you developed to merge the various sources will remain in use across the bank. The data will be used to develop alternative models and will be updated as new data is received.


### Optimizing Paide Search Marketing

#### Sponsor: Citizens Bank, Customer Data and Analytics Team


Citizens Financial Group, Inc. is an American bank headquartered in Johnston, Rhode Island. The Customer Data and Analytics team within Citizens Bank out of the CAP Center in Providence, Rhode Island. This team includes people with backgrounds in marketing and the statistical methods associated with online marketing.



#### Project

The objective of this capstone project is to improve Citizen Bank’s search engine marketing approach to more effectively and efficiently market products to both current and prospective customers. This is a step towards a more personalized model for paid search ads, this will be done using both individual’s personal and regional information to determine whether or not to display a paid search ad and how much the bank should pay for a given click. Success is defined as improving conversion, the process of a consumer searching for a particular product online, clicking on a paid search ad, and successfully booking said product.

You will be given large data sources to merge together to build your predictions: web browsing activity on Citizens Bank’s website after clicking on a paid search ad on either Google or Bing, information about account application and bookings for only Citizen's Bank products, a large csv file containing information about almost every individual adult consumer in the United States, Zip5 and Zip9 Bureau Data, Digital Spending Data: the total amount spent on paid search for each keyword per day, information about the number outcomes of paid marketing for each of the 6 products. Some of the data is collected by the bank, some is purchased, and some is public information.


After your project, the data you've merged and the scripts you developed to merge the various sources will remain in use across the bank. The data will be used to develop alternative models and will be updated as new data is received.


### Summarizing Clinical Notes

#### Sponsor: Carsten Eickhof
Professor Carsten Eickhof leads the AI Lab at Brown's Center for Biomedical Informatics. His lab specializes in mining, representation and retrieval of large-scale natural language resources.

#### Project

The objective of this project is to apply natural language processing techniques to Electronic Health Records (EHR) and shorten lengthy notes using a combination of extractive (extract phrases from the source) and abstractive (using meaning to make phrasing more concise) summarization. The lab has a set access to the Medical Information Mart for Intensive Care III (MIMIC-III) database. This database consists of recorded health data from over 40,000 intensive care unit patients at the Beth Israel Deaconess Medical Center between 2001 and 2012. All incoming patient information was documented from the moment the patient was admitted to the moment they were released. The data used consisted of 2,083,180 rows of unstructured clinical notes, where notes may be short or several paragraphs long and include both complete English text and medical shorthand. The data is provided in two files: notes and summary, where the summary is defined by one of the notes.

After your project you will release your summarization framework for others to use.

### Predictive power of Local Field Potentials in Primary visual cortex

#### Sponsor: Paradiso Lab
The Paradiso Lab at Brown explores the neural basis of visual perception. Professor Paradiso is a professor of neuroscience at Brown and holds a BA and PhD in physics. He has postdoctoral training in neurophysiology and visual psychophysics.  He has worked a a number of research lab during his postdoctoral training. His lab collects data from both humans and animals.

#### Project: Local feild potentials

a large amount of neural data for the purpose of understanding
the dynamics of eye movements and fixations. The neural data consists of Local Field Potentials (LFPs) from electrodes placed in the macaque – a group of species of Old World monkeys – primary visual cortex (V1). There are lots of useful predictions that can be made from this data; predicting the onset of new eye fixations, predicting future LFPs, predicting directions of eye movements, predicting the timing of neural spikes, and decoding types of eye fixations are among them. The goal of this project is to improve prior predictions made with SVMs and autoregressive methods recurrent neural networks.

The data will come from two datasets, each from experiments. One dataset is
LFPs from 16 simultaneous electrode recordings of a primate over time. There will also be a detailed description of the experimental protocol and its timing. This dataset will be lowpass filtered and downsampled. The second dataset contains, among other fields, LFPs from 15 simultaneous electrode recordings of a primate. A different experimental protocol was used for this and details of that timing is also included. The second dataset is lowpass filtered but not downsampled.

After your project you will produce a paper and release the data to encourage others to reproduce your results.

#### Sponsor

A customer of a scientific consulting firm wants to test the feasibily of having a feature in their app where consumers can test out changes to their facial hair in a realistic way. The consultant firm is lead by statisticians and a variety of scientists.  The customer is unknown, only that they do not yet have the technical capabilities on staff. The sponsor cares that all people who are concerned with their facial hair are able to use this feature of their app.

#### Project

This project is to develop techniques for removing or adding facial hair from images of faces. The CelebA dataset is used for this project, consisting of 203K images of roughly 10K subjects, all of which are celebrities across a variety of professions. The images are accompanied by 40 binary attribute annotations covering various facial characteristics such as expression, hair color, and gender

After your project the consultant's customer will evaluate your results to determine if they can deploy a similar product or how to proceed further in developing their own system. They will want to be able to determine if they need to collect data and, if so,  what types of additional data they should collect.


### Your actual/ ideal capstone project

On your cover page write a scenario description similar in structure and level of detail to the ones above for the actual capstone project that you are interested in or the ideal project that you would like to do. If you choose this option you should visit office hours to have an instructor or TA confirm that your scenario description is complete.

#### Sponsor:

Describe the background of the project sponsor enough so that we can evaluate if you are using inappropriate jargon for the sponsor

#### Project:

Describe the context, goals, and data for the project enough so that we can evaluate if you have made an appropriate choice of data documentation.


# Class Welcome

Where does data come from and why does that matter?
How does data preparation impact values held by a Data Science product?
What are good data practices?

## warmup

How did the readings change how you think about data?

def: data

## interdisciplinary

Data science is inherently interdisciplinary.

Working across and in between disciplines is hard not only because of the breadth of actual information, but because of the way that information is cataloged and ideas are mapped to terms.

Data.
Data Provenance, Data lineage

Definitions of data and framing of data

Timeline of data and its history




## Review:

Given our discussion of ethical frameworks the past two weeks:
- what initial ethical questions around data do you have
- what ethical frameworks came up in the reading

# Reading Reflection, Review

-




## Metadata



# Data sheets for datasets



# Nutrition Labels



#



# Library

- lineage wrt rights
- iso standard 14.7.21 oais
- archival, digital
- repository manager, programmer, preservation, (metadata head)
- rights of data creator, copyrights

- eg embedding cc0 in pdf, xml in
- mods- metadata schema from library of congress
- shoe
- darwin core 4 (another standard)
- geo coded 11914 (grant at Brown);
  - curation grant
  -

- fixety, md5 hash, bit rot, data quality over copying
  - oais track events and changes in the data
  - a bit stream might capture processing
- versioning,
  - time stamps, who did what at what time
  - both for reproduction, lineage/Provenance

- data collected via scraping breaks these policies eg
- Provenance data in social media

- kolbaishi @ RI hospital
  - alert fatigue, drs ignore alarms because of false positives
  - clinical re-label events
  - (popular dataset)
  - first uses: manufactures of competitor equipment
- role of librarians in data curation, data quality
- end user license

- replicability
- data collection
  - experimental
  - social surveying

- meta analyses:
  - mutliple datasets
  - one creation
  -

- data reference interview
- collection: scientific vs web
  - instruments vs browsers
  - okcupid
  - netflix
  - reuseing for an alternative purpose

- how to check large datasets of images
- images might have geolocation
- document headers
- preservation
- ocr retaining all deriviatives

- DICOM standard
- biomedical largest growth area

- activity
- cleaning IP address

- gender
