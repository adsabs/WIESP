---
layout: single
title: Shared Task Labels<br> WASP @ IJCNLP-AACL 2026
permalink: /2025/shared_task_labels
sidebar:
  nav: "sidebar2026"
---

## Description of the Labels for TRACS @ WASP @ IJCNLP-AACL 2025
The TRACS dataset consists of papers associated with a telescope and three categories likely to be of interest to bibliographers. We have drawn the categories from a simplification of those discussed by the [Observatory Bibliographers Collaboration (2024)](https://scixplorer.org/abs/2024OJAp....7E..85O/abstract).  

Papers can be categorized as one of `science`, `instrumentation`, `mention`, or `not_telescope`.

### `science`
New science papers use data from the designated telescope to obtain new results. The authors may be using new observations, using archival observations, or reanalyzing previous results. However, papers that merely refer to previous results for comparison or suggest what might be possible with future observations are Mentions, rather than Science papers.  
Science papers may use observations directly or indirectly, such as through a published source catalog. Indirect use must be substantive. Papers that overlay new data over images from the designated telescope without discussing the underlying image are Mentions, rather than Science papers. Papers that use catalog data, such as positions or measurements, without further discussion are Mentions, rather than Science papers.  
Papers that reference a grant associated with the designated telescope but provide no evidence of using data from it are Not Telescope papers, rather than Science papers or Mentions.  

### `instrumentation`
Instrumentation papers describe the technical aspects of the telescope, its calibration activities, its data processing pipeline, or its archival procedures. These papers can discuss hardware, software, or methodologies.  
A paper that includes new science facilitated by use of the hardware, software, or methodology described in the paper may be both a Science and an Instrumentation paper. A paper that describes a novel technique or software to achieve its scientific conclusions may be a Science and an Instrumentation paper. A paper that uses calibration, alignment, or engineering data to produce new results may be a Science and an Instrumentation paper.

### `mention`
Mentions are papers that do reference the designated telescope but do not produce new scientific results (Science) or contribute to understanding it (Instrumentation). If a paper meets the criteria for a Science paper or an Instrumentation paper anywhere, then the paper is a Science paper, even if it also contains statements that would otherwise be considered a Mention.  
Papers that discuss the designated telescope as part of their introductory overview of the issue, of the history of a problem, or their survey of current relevant research are Mentions.  Papers that discuss the designated telescope and its scientific contributions as part of an in-depth review of a research topic are Mentions.  
Papers that merely refer to previous results for comparison or suggest what might be possible with future observations are Mentions, rather than Science papers. Papers that overlay new data over images from the designated telescope without discussing the underlying image are Mentions, rather than Science papers. Papers that use catalog data, such as positions or measurements without further discussion are Mentions, rather than Science papers.  
Papers that use a secondary catalog that incorporates data from a catalog produced directly by the designated telescope are Mentions, even if that paper acknowledges the telescope.    
Papers that reference a grant associated with the designated telescope but provide no evidence of using data from it are Not Telescope papers, rather than Science papers or Mentions.

### `not_telescope`
Not Telescope papers are papers that include a reference that might otherwise be confused with one or more designations used for the telescope of interest. An telescope may share part of their name with a historical figure for which several things are named. An telescope may share an acronym with an unrelated program.  
Papers that reference a grant associated with the designatedtelescope but provide no evidence of using data from it are Not Telescope papers, rather than Science papers or Mentions.  
If a paper meets the criteria for a Science paper, an Instrumentation paper, or Mention anywhere, then the paper belongs to that category, even if it also contains references to other items that share names in common with the designated telescope or instrument. 

