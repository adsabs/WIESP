---
layout: simple-page
title: DEAL Shared Task
permalink: /2022/SharedTasks
---

### DEAL: Detecting Entities in the Astrophysics Literature
# Shared Task

A good amount of astrophysics research makes use of data coming from missions and facilities such as ground observatories in remote locations or space telescopes, as well as digital archives that hold large amounts of observed and simulated data. These missions and facilities are frequently named after historical figures or use some ingenious acronym which, unfortunately, can be easily confused when searching for them in the literature via simple string matching. For instance, `Planck` can refer to the person, the mission, the constant, or several institutions. Automatically recognizing entities (i.e., Named Entity Recognition or NER) such as missions or facilities would help tackle this word sense disambiguation problem.

# Task

The task consists on building a system (any strategy is valid as long as it is automatic and does not require human intervention) that is capable of identifying Named Entities in a dataset composed by full-text fragments and acknowledgements from the astrophysics literature.

# Dataset

We provide a [dataset with acknowledgements and full-text fragments](https://huggingface.co/datasets/fgrezes/WIESP2022-NER) from the [NASA ADS](https://ui.adsabs.harvard.edu/) with manually tagged astronomical facilities and other entities of interest (e.g., celestial objects), as well as a baseline metric obtained with the [astroBERT model](https://ui.adsabs.harvard.edu/abs/2021arXiv211200590G/abstract).

# Evaluation & Baseline

Submissions will be scored using both the CoNLL-2000 shared task [seqeval](https://github.com/chakki-works/seqeval) F1-Score at the entity level and [scikit-learn's Matthews correlation coefficient method](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.matthews_corrcoef.html) at the token level. We also encourage authors to propose their own evaluation metrics. The baseline is computed using the [astroBERT](https://ui.adsabs.harvard.edu/abs/2021arXiv211200590G/abstract) trained for this NER task (see [the detailed baseline scores](SharedTask_BaselineScores)). The submissions will be scored on [Codalab](https://codalab.lisn.upsaclay.fr/competitions/5062).  


# Challenge

Can a different model/architecture/approach be more successful at recognizing astronomical named entities?

Participants will have the opportunity to present their findings during the workshop and write a short paper. The best performant or interesting approaches might be invited to further collaborate with the [NASA Astrophysical Data System](https://ui.adsabs.harvard.edu/).

# Instructions for Participants

Participants should create accounts on [Huggingface](https://huggingface.co/datasets) to access the data. Instructions on how to format your predictions and compute your scores on the training set are available in the [Huggingface repository](https://huggingface.co/datasets/fgrezes/WIESP2022-NER) 

Participants should also create accounts on [Codalab](https://codalab.lisn.upsaclay.fr/competitions/5062) and follow the instructions on how to submit their predictions for scoring. 

# Registration

***Please fill in this form to report your intention to participate in the shared task*** 

[https://forms.office.com/r/KKpeKJBLy3](https://forms.office.com/r/KKpeKJBLy3)

# Timeline

- Training+Validation Data Release: June 1, 2022
- Validation Phase: June 1 - July 31, 2022
- Test Data Release: August 1, 2022
- Final Scoring Period: August 1 - August 26, 2022
- System Report Submission: September 2, 2022
- Notification: September 25, 2022
- Camera-ready Submission Deadline: October 10, 2022
- Event Date: November 20, 2022 (online)

# Contact

You can contact us at `WIESP_AACL2022 [at] softconf.com`.

