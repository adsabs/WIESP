---
layout: single
title: Shared Task <br> WASP @ IJCNLP-AACL 2026
permalink: /2026/shared_task
sidebar:
  nav: "sidebar2026"
---

# AstroCLIMB:  
## Astronomy Citation Linking from Illustrations: a Multimodal Benchmark

### Motivation
Scientists rely on figures to share their discoveries, but this makes the information contained in the figures hard to parse, archive, and search. Recent multimodal neural-network models promise to extract this information, but have not yet been widely tested and adopted by the astronomy community.  
In partnership with [astroexplorer.org](https://www.astroexplorer.org/), we propose a novel dataset and an associated task as a benchmark to evaluate a model’s multimodal capabilities.  The task is to partially reconstruct the citation graph of astronomy papers from their figures and captions.

![AstroCLIMB image: these figures come from the same astronomy paper. Courtesy of astroexplorer.org](AstroCLIMB_001.png)



### Task Description
The goal of the task is single-class classification.  
The inputs are pairs of figures, a figure and a caption, or a pair of captions.  
The possible classes are:
- `"same paper"`
- `"different paper but related"` (cited/citing)
- `"unrelated"` 
- `"same figure"` (only for figure+caption pairs)


### Dataset
The dataset consists of over 100K figure+caption pairs from the [astroexplorer.org](https://www.astroexplorer.org/) from recent open access astronomy papers. More details to come.

### Evaluation
Models will be evaluated on [Kaggle.com](https://www.kaggle.com/). More details to come.

## Instructions for Participants
1. Participants should register for ICNLP-AACL [here] (TBD).
2. Participants should join the competition on Kaggle [here] (TBD), where they can find the latest version of the dataset, and score their submissions.
3. Participants should format their papers using the ACL LaTeX template on Github [here](https://github.com/acl-org/acl-style-files/tree/master?tab=readme-ov-file), and submit them to OpenReview [here] (TBD).


## Timeline 
(subject to changes)
| Timeline                          | Date                |
|-----------------------------------|---------------------|
| 1st CfP + Registration starts     | TBD                 |
| Train and Validation Data Release | TBD                 |
| Test Set Release                  | TBD                 |
| Registration Ends                 | TBD                 |
| System Run and Output Submission  | TBD                 |
| System Paper Submisison           | ~September 14, 2026 |
| Result Announcement               | ~October 1, 2026    |
| Notification                      | TBD                 |
| Camera Ready Submission           | ~October 12, 2026   |
| Workshop                          | November 9-10, 2026 |

*All deadlines are 11.59 pm UTC-12h ("Anywhere on Earth").*

### Contact
For inquiries, contact Felix Grezes at [felix.grezes@cfa.harvard.edu](mailto:felix.grezes@cfa.harvard.edu)
