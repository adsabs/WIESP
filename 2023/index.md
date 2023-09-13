---
layout: simple-page
title: 2023
permalink: /2023/
---

## The 2nd [WIESP](https://ui.adsabs.harvard.edu/WIESP/) @ IJCNLP-AACL 2023 

The 2nd Workshop on Information Extraction from Scientific Publications will be held online at the [IJCNLP-AACL 2023](http://www.ijcnlp-aacl2023.org/) on November 1, 2023 and it will feature:

- Paper Presentations
- Keynote talks
- Panel discussion on "LLMs for Science"
- A virtual social cum poster presentation

## Call for Papers

Building on the success of the [First WIESP at AACL-IJCNLP 2022](2022), the [Second Workshop on Information Extraction from Scientific Publications (WIESP)](2023) will provide a platform for researchers to foster discussion and research on information extraction, mining, generation, and knowledge discovery from scientific publications using Natural Language Processing and Machine Learning techniques. Much technological change happened in one year (since the 1st WIESP), especially with Generative Artificial Intelligence research. We are incorporating a few additional topics to stay abreast with the latest developments and research in the community. The 2nd iteration of WIESP would focus on the following topics  (but not limited to):

## Topics

- <b>Large Language Models (LLMs) for Science</b>
- <b>Application of LLMs on information extraction, generation, mining and knowledge discovery from scientific publications</b>
- <b>Probing LLMs for scientific fact-checking and misinformation</b>
- Scientific document parsing
- Scientific named-entity recognition
- Scientific article summarization
- Question-answering on scientific articles
- Citation context/span extraction
- Structured information extraction from full-text, tables, figures, bibliography
- <b>Novel datasets</b> curated from scientific publications
- Argument extraction and mining
- Challenges in information extraction from scientific articles
- Building knowledge graphs via mining scientific literature; querying scientific knowledge graphs
- Novel tools for IE on scientific literature and interaction with users
- Mathematical information extraction
- Scientific concepts, facts extraction
- Visualizing scientific knowledge
- Bibliometric and Altmetric studies via information extraction from scientific articles and metadata

We especially welcome participation from academic and research institutions, government and industry labs, publishers, and information service providers. Projects and organizations using NLP/ML techniques in their text mining and enrichment efforts are also welcome to participate. We strongly encourage the participation of students, researchers, and science practitioners from diverse backgrounds, especially from underrepresented groups and communities, to be a part of WIESP events, and proactively make the workshop a diverse and inclusive one.

We invite papers of the following categories:

***Long papers*** must describe substantial, original, completed, and unpublished work. Wherever appropriate, concrete evaluation and analysis should be included. Papers must not exceed eight (8) pages of content, plus unlimited pages of references. The final versions of long papers will be given one additional page of content (up to 9 pages) so that reviewers' comments can be taken into account.

***Short papers*** must describe original and unpublished work. Please note that a short paper is not a shortened long paper. Instead, short papers should have a point that can be made in a few pages, such as a small, focused contribution, a negative result, or an interesting application nugget. Short papers must not exceed four (4) pages, plus unlimited pages of references. The final versions of short papers will be given one additional page of content (up to 5 pages) so that reviewers' comments can be taken into account.

In addition to papers, WIESP will also host a shared task.  Details on the WIESP shared tasks are available below. Also, we will publish a separate CfP on the shared task. Shared task authors will be invited to write their system descriptions and those will be subjected to peer review.

All accepted papers will be published in the WIESP proceedings as part of IJCNLP-AACL 2023 and indexed in the ACL Anthology.

***Shared Task: [Function of Citation in Astrophysics Literature (FOCAL)](shared_task_1))***

The citation graph is an essential tool for helping researchers find relevant literature. To further empower discovery, we aim to label the edges of the graph with the function of the citation: e.g. is the cited work necessary background knowledge, or is it used as a comparison, to the citing work? To start this process, we propose a shared task of automatically labeling citations with a function based on the textual context of the citation. 

More precisely, given a paragraph of text from the astrophysics literature, and the start and end position of a citation in the paragraph, can the competitors build a model that outputs why it was cited (the function) and the associated span of text in the paragraph . 

For example, given the following paragraph:  
```
In some cases, when the pulse broadening time is a significant fraction of the pulse period (30 per cent or more) one can see a
relatively sharp pulse, but at the same time the extended scattering tail may obscure the real baseline level, which leads to an
underestimation of the pulsar flux. For pulsars with DMs in 200–300 pc cm−3 range this usually happens between 300 and 600 MHz
(Lewandowski et al. 2013, 2015a). This leads to a somewhat pseudo-correlation between high DM and GPS pulsars (Kijak et al. 2007,
2011b) where serious underestimation of the flux at lower frequencies for high DM pulsars may give rise to an inverted spectra. The
interferometric imaging technique provide a more robust measurement of the pulsar flux owing to the baseline lying at zero level
thereby reducing errors made during the baseline subtraction. 
```
and the following citation `Kijak et al. 2007` with `start = 495` and `end = 511`.  
The model should output:  
`prediction['Function Labels'] = [Uses, Uses]` and `predictions['Functions Start End'] = [(418,492), (521,640)]`  
which corresponds to the text `predictions['Function Text'] = ['This leads to a somewhat pseudo-correlation between high DM and GPS pulsars', 'where serious underestimation of the flux at lower frequencies for high DM pulsars may give rise to an inverted spectra.']`.

Instructions can be found [here](shared_task_1)

The shared task papers/system descriptions would be published with the 2nd WIESP proceedings in ACL Anthology. Please register in this [link](https://forms.office.com/g/cUyC00LnWB) to participate.

## Important Dates 

- Paper/Abstract Submission Deadline: <s>August 25, 2023</s> <s>September 4, 2023</s> September 11, 2023 (Final)
- Deadline for FOCAL shared task: extended to September 17
- Notification of workshop paper/abstract acceptance: October 5, 2023
- Camera-ready Submission Deadline: October 12, 2023
- Workshop: November 1, 2023 (online, final date TBD)

*All submission deadlines are 11.59 pm UTC -12h (“Anywhere on Earth”)*

## Submission Site

Submission Link: [SoftConf](https://softconf.com/ijcnlp2023/WorkshopWIESP2023/)

## Submissions

Submission will be via softconf. Submissions should follow the [ACLPUB formatting guidelines](https://acl-org.github.io/ACLPUB/formatting.html) and [template files](https://github.com/acl-org/acl-style-files/tree/master). 

Submissions (Long and Short Papers) will be subject to a double-blind peer-review process.  We follow the same policies as IJCNLP-AACL 2023 regarding anonymity, preprints and double submissions.

## Organizers

- [Tirthankar Ghosal](https://elitr.eu/tirthankar-ghosal), National Center for Computational Sciences \| Oak Ridge National Laboratory, USA
- [Felix Grezes](https://ui.adsabs.harvard.edu/about/team/team/fgrezes.html), Center for Astrophysics \| Harvard & Smithsonian, USA
- [Thomas Allen](https://ui.adsabs.harvard.edu/about/team/team/tallen.html), Center for Astrophysics \| Harvard & Smithsonian, USA
- [Kelly Lockhart](https://ui.adsabs.harvard.edu/about/team/team/klockhart.html) , Center for Astrophysics \| Harvard & Smithsonian, USA
- [Alberto Accomazzi](https://ui.adsabs.harvard.edu/about/team/team/aaccomazzi.html), Center for Astrophysics \| Harvard & Smithsonian, USA
- [Sergi Blanco-Cuaresma](https://blancocuaresma.com/s/), Center for Astrophysics \| Harvard & Smithsonian, USA


## Contact

`wiesp_ijcnlp-aacl-2023 [at] softconf.com`
