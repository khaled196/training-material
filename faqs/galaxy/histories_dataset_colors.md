---
title: Dataset colors
description: Explains meaning of dataset colors in Galaxy's history
area: histories
box_type: tip
layout: faq
contributors: [nekrut]
---

There are several different "states" a dataset can be in. These states are indicated by colors:

![Colors indicating states of Galaxy datasets]({% link shared/images/galactic_colors.svg %})

- **ok**: everything is fine, life is good;
- **new**: the dataset was just created. Galaxy does not yet know when it is available;
- **queued**: indicates that the job generating this dataset is scheduled for execution but not running yet;
- **running**: job generating this dataset is running;
- **setting metadata**: when a new dataset is uploaded Galaxy examines it to understand what kind of data it is (e.g., BAM, FASTQ, fasta, BED, etc.). This is called "setting metadata";
- **deferred**: sometimes it does not make sense to upload the dataset until it is needed for an analysis. Galaxy will download deferred datasets later during the job execution. Those datasets do not count toward your quota;
- **paused**: in some cases, workflow executions or upstream errors can prevent subsequent jobs from starting to create datasets in "paused" state. Rerun the errored tool with the option ***Resume dependencies from this job?*** to resume paused jobs; 
- **discarded**: something went wrong. For example, a job producing this dataset might have been cancelled;
- **error**: everything is not fine; life is bad! Click on the information **i** button to know more about what happened;
- **placeholder**: similar to "new"; we know something will be there, but are not yet sure what;
- **failed populated state**: this refers to collections (not individual datasets). Here, a collection has failed to be populated with datasets;
- **new populated state**: this refers to collections (not individual datasets). A collection was created but not populated yet.

<!-- original editable image = https://docs.google.com/drawings/d/1F2Lq1m3cMIckvCexXMzug-dqwgifkoMOzoyH4VcoVX0/edit?usp=sharing -->

<!-- TO DO 
Needs to be linked to FAQs on:
- how to report errors
- explaining collections 
-->
