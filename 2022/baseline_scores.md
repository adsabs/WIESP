---
layout: simple-page
title: DEAL Shared Task - Baseline Scores
permalink: /2022/SharedTask_BaselineScores
---

# Baseline Scores 

|                  | Random |  BERT  | SciBERT | astroBERT |
|:---------------- |:------:|:------:|:-------:|:---------:|
|    MCC score     | 0.1089 | 0.7405 | 0.8016  |**0.8104** |
|    overall f1    | 0.0166 | 0.4738 | 0.5595  |**0.5781** |
|overall precision | 0.0119 | 0.4779 | 0.5457  |**0.5511** |
|  overall recall  | 0.0274 | 0.4697 | 0.5741  |**0.6080** |
|     accuracy     | 0.7061 | 0.9188 | 0.9365  |**0.9389** |

## Explanations

- Random: a model that makes random label predictions matching the training set distribution.  
- BERT: Google's BERT model finetuned to the task ([arXiv](https://arxiv.org/abs/1810.04805)).  
- SciBERT: AllenAI's SciBERT model finetuned to the task ([arXiv](https://arxiv.org/abs/1810.04805)).  
- **astroBERT**: NASA ADS' astroBERT model finetuned to the task ([arXiv](https://arxiv.org/abs/2112.00590)).  

## In depth comparison
Absolute precision and recall improvement per label class, from the astroBERT model over SciBERT.
![precision / recall improvement for astroBERT over SciBERT](/WIESP/assets/astroBERT_vs_SciBERT.png)
