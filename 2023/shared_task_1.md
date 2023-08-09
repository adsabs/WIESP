---
layout: simple-page
title: WIESP 2023 FOCAL Shared Task
permalink: /2023/shared_task_1
---

First of the shared tasks at WIESP-2023.  
All info not present to be added in as soon as possible.

## FOCAL: Function Of Citation in Astrophysics Literature

### Description
The citation graph is an essential tool for helping researchers find relevant literature. To further empower discovery, we aim to label the edges of the graph with the function of the citation: e.g. is the cited work necessary background knowledge, or is it used as a comparison, to the citing work? To start this process, we propose a shared task of automatically labeling citations with a function based on the textual context of the citation. 

### Task
More precisely, given a paragraph of text from the astrophysics literature, and the start and end position of a citation in the paragraph, the participants should build a model that outputs why it was cited (the function) and the associated span of text in the paragraph. 

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

### Dataset
We provide a dataset of full-text fragments from the [NASA ADS](https://ui.adsabs.harvard.edu/) annotated by a human expert with the location of citations and their associated functions. 

The dataset is available on [Huggingface](https://huggingface.co/datasets/adsabs/FOCAL).

A list of citation function labels and their definitions is available [here](https://github.com/adsabs/WIESP/blob/gh-pages/2023/LabelDefinitions.md).

### Evaluation & Baseline
(coming soon)

### Challenge
Can a different model/architecture/approach be more successful at recognizing astronomical citation functions?  

Participants will have the opportunity to present their findings during the workshop and write a short paper. The best performant or interesting approaches might be invited to further collaborate with the [NASA Astrophysical Data System](https://ui.adsabs.harvard.edu/).

### Instructions for Participants
Participants should create accounts on [Huggingface](https://huggingface.co/) to access the data. Instructions on how to format your predictions and compute your scores on the training set will be available in the Huggingface repository.

Participants should also create accounts on [Codalab](https://codalab.lisn.upsaclay.fr/), register for the competition (link coming soon) and follow the instructions on how to submit their predictions for scoring.

### Registration

### Timeline
