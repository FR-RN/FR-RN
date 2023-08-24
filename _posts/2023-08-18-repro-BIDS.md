---
layout: post
title:  "A reproducible and generalizable software workflow for analysis of large-scale neuroimaging data collections using BIDS Apps"
date:   2023-01-09 08:00 +0100
categories: publication
tags: computational science
lang: english
---

Neuroimaging research faces a crisis of reproducibility. With massive sample sizes and greater data complexity, this problem becomes more acute. Software that operates on imaging data defined using the Brain Imaging Data Structure (BIDS) – BIDS Apps – have provided a substantial advance. However, even using BIDS Apps, a full audit trail of data processing is a necessary prerequisite for fully reproducible research. Obtaining a faithful record of the audit trail is challenging – especially for large datasets. Recently, the FAIRly big framework was introduced as a way to facilitate reproducible processing of large-scale data by leveraging DataLad – a version control system for data management. However, the current implementation of this framework was more of a proof of concept, and could not be immediately reused by other investigators for different use cases. Here we introduce the BIDS App Bootstrap (BABS), a user-friendly and generalizable Python package for reproducible image processing at scale. BABS facilitates the reproducible application of BIDS Apps to large-scale datasets. Leveraging DataLad and the FAIRly big framework, BABS tracks the full audit trail of data processing in a scalable way by automatically preparing all scripts necessary for data processing and version tracking on high performance computing (HPC) systems. Currently, BABS supports jobs submissions and audits on Sun Grid Engine (SGE) and Slurm HPCs with a parsimonious set of programs. To demonstrate its scalability, we applied BABS to data from the Healthy Brain Network (HBN; n=2,565). Taken together, BABS allows reproducible and scalable image processing and is broadly extensible via an open-source development model.


[{% reference Zhao2023 --file references.bib %}](https://www.biorxiv.org/content/10.1101/2023.08.16.552472v1?rss=1)
