---
layout: post
title:  " BioFlow-Insight: facilitating reuse of Nextflow workflows with structure reconstruction and visualization "
date:   2024-09-01 15:00 +0100
categories: publication
tags: bioinformatics
lang: english
---

Bioinformatics workflows are increasingly used for sharing analyses, serving as a cornerstone for enhancing the reproducibility and shareability of bioinformatics analyses. In particular, Nextflow is a commonly used workflow system, permitting the creation of large workflows while offering substantial flexibility. An increasing number of Nextflow workflows are being shared on repositories such as GitHub. However, this tremendous opportunity to reuse existing code remains largely underutilized. In cause, the increasing complexity of workflows constitute a major obstacle to code reuse. Consequently, there is a rising need for tools that can help bioinformaticians extract valuable information from their own and others’ workflows. To facilitate workflow inspection and reuse, we developed BioFlow-Insight to automatically analyze the code of Nextflow workflows and generate useful information, particularly in the form of visual graphs depicting the workflow’s structure and representing its individual analysis steps. BioFlow-Insight is an open-source tool, available as both a command-line interface and a web service. It is accessible at https://pypi.org/project/bioflow-insight/ and https://bioflow-insight.pasteur.cloud/.


[{% reference Marchment:2024 --file references.bib %}](https://doi.org/10.1093/nargab/lqae092)
