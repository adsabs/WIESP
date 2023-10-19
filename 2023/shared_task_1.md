---
layout: simple-page
title: WIESP 2023 FOCAL Shared Task
permalink: /2023/shared_task_1
---

Shared task for WIESP-2023.  

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

The competition will be run on [Codalab](https://codalab.lisn.upsaclay.fr/competitions/15292).

### Dataset
We provide a dataset of full-text fragments from the [NASA ADS](https://ui.adsabs.harvard.edu/) annotated by a human expert with the location of citations and their associated functions. 

The dataset is available on [Huggingface](https://huggingface.co/datasets/adsabs/FOCAL).

### Dataset Description
Datasets are in JSON Lines format (each line is a json dictionary).  

Each entry consists of a dictionary with the following keys:
- `"Identifier"`: unique string to identify the entry
- `"Paragraph"`: text string from an astrophysics paper 
- `"Citation Text"`: list of strings forming the citation (most often a single string, but sometimes the citation text is split up)

The keys below are only present in the Training dataset.  
Participants should format their submissions to the challenge in this format.
- `"Citation Start End"`: list of integer pairs denoting where the citation starts and end in `"Paragraph"` (most often a single pair, sometimes the citation text is split up, if so follows the order in `"Citation Text"`)
- `"Functions Text"`: list of strings highlighting parts of the paragraph that explain the function of the citation
- `"Functions Label"`: list of strings with the label for each text element in `"Functions Text"` (in same order)
- `"Functions Start End"`: list of integer pairs denoting where the elements in `"Functions Text"` start and end in `"Paragraph"`(in same order)
  
`start` and `end` are defined by the character position in the `"Paragraph"` string.

A list of citation function labels and their definitions is available [here](LabelDefinitions).

### Evaluation & Baseline
#### Evaluation
Submissions will be evaluated using two scripts found [here](https://huggingface.co/datasets/adsabs/FOCAL/tree/main/scoring_scripts). The submissions will be scored by three metrics:

- The full seqeval score and main evaluation metric: `evaluate_FOCAL_seqeval(references_jsonl, predictions_jsonl)[0]['micro avg']['f1-score']`. This metrics check that you placed the functions of the citation correctly in the paragraph along with the correct function labels.
- A seqeval score with a generic label instead of functions: `evaluate_FOCAL_seqeval(references_jsonl, predictions_jsonl)[1]['micro avg']['f1-score']`. This metric checks that you correctly found the parts of the paragraph that explain the functions of the citation, without checking if you correctly predicted the reason(s) a given citation was made (the function labels)
- An f1-score on the function labels only: `evaluate_FOCAL_labels(references_jsonl, predictions_jsonl)['micro avg']['f1-score']`. This metric checks that you correctly predicted the reason(s) a given citation was made, without checking if you correctly find the parts of the paragraph that explain the function of the citation.

We also encourage authors to propose their own evaluation metrics. 

### Baseline
Baseline scores from a simple model are provided as benchmark for the participants.  This model is defined as follows:  
- the function of the citation is the majority class (i.e. `Background`).
- the start and end of the function is the sentence that includes citation, as defined by [pySBD](https://github.com/nipunsadvilkar/pySBD).  
 The baseline scores (all micro-averaged f1-scores) are as follows:

| seqeval_full | seqeval_generic | score_labels_only |
| :----------: | :-------------: | :---------------: |
| 0.2368       | 0.5986          | 0.4287            |
 

### Challenge
Can a different model/architecture/approach be more successful at recognizing astronomical citation functions?  

Participants will have the opportunity to present their findings during the workshop and write a short paper. The best performant or interesting approaches might be invited to further collaborate with the [NASA Astrophysical Data System](https://ui.adsabs.harvard.edu/).

### Registration for FOCAL

Please register in this [link](https://forms.office.com/g/cUyC00LnWB) to participate.

### Instructions for Participants
Participants should create accounts on [Huggingface](https://huggingface.co/) to access the data. Instructions on how to format your predictions and compute your scores on the training set will be available in the Huggingface repository.

Participants should also create accounts on [Codalab](https://codalab.lisn.upsaclay.fr/), register for the competition here [https://codalab.lisn.upsaclay.fr/competitions/15292](https://codalab.lisn.upsaclay.fr/competitions/15292), and follow the instructions on how to submit their predictions for scoring.

Participants should format their submissions the challenge in the same format as the training dataset.  
I.E. each submission should be in JSON Lines format (each line is a json dictionary), with each entry consisting of a dictionary with the following keys: `["Identifier", "Paragraph", "Citation Text", "Citation Start End", "Functions Text", "Functions Label", "Functions Start End"]` (note: for the first three of those keys, the values are provided by the validation/test set, while the last five are the participants' work). Submit your predictions as a .zip file.

### Registration

## Timeline

| Timeline                                              | Date          |
| ----------------------------------------------------- | ------------- |
| 1st CfP + Registration starts                         | Aug 10        |
| Train and Validation Data Release                     | Aug 10        |
| Test Set Release + 2nd CfP                            | Sep 17        |
| Shared Task Period                                    | Sep 17-Oct 2  |
| Registration Ends                                     | Oct 2         |
| System Paper Submisison                               | Oct 2         |
| Evaluation & Review Period                            | Oct 3-Oct 7   |
| Notification                                          | Oct 8         |
| Camera Ready Submission                               | Oct 13        |

