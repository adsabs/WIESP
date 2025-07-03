---
layout: single
title: Shared Task <br> WASP @ IJCNLP-AACL 2025
permalink: /2025/shared_task
sidebar:
  nav: "sidebar2025"
---

## Telescope Reference and Astronomy Categorization Shared task (TRACS)

### Description
The NASA Science eXplorer (SciX) is literature-based, open digital information system that enriches its content by making relevant data discoverable by researchers. For example in astrophysics, large efforts have been made by human contributors to create a bibliography tracking all papers related to the CHANDRA space telescope.  
To help librarians and archivists with these data discovery efforts, automated text mining tools have been created, however they rely on explicit links either in the citations or the full-text. These automated tools struggle with the additional information that human curators add based on the needs of each project. 
<!---
to add: figuring out what LLMS can do, we offer this challenge
--->


### Task


### Dataset  
We provide a dataset of scientific papers from SciX annotated with their associated telescope, categorization, and metada. 
The TRACS dataset is hosted on Hugginface here (link TBD).  

### Dataset Description  

The dataset entries consists of the following features:  

- `"bibcode"`: unique string that identifies the entry in the SciX database
- `"telescope"`: the telescope referenced in the entry 
- `"science"`, `"mention"`, `"not_telescope"`: boolean labels for the entry
- `"author"`, `"year"`: metadata for the entry
- `"title"`, `"abstract"`, `"body"`, `"acknowledgments"`, `"grants"`: the relevant textual information for the entry.R

### Baseline


### Challenge

### Registration for TRACS
<!---
XXX add registration link
--->
Please register here (link TBD) to participate.

### Instructions for Participants



## Timeline

| Timeline                                              | Date          |
| ----------------------------------------------------- | ------------- |
| 1st CfP + Registration starts                         |         |
| Train and Validation Data Release                     |         |
| Test Set Release + 2nd CfP                            |         |
| Shared Task Period                                    |   |
| Registration Ends                                     |          |
| System Paper Submisison                               |          |
| Evaluation & Review Period                            |    |
| Notification                                          |          |
| Camera Ready Submission                               |         |

