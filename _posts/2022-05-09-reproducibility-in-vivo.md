---
layout: post
title:  "Reproducibility of in-vivo electrophysiological measurements in mice"
date:   2022-05-09 15:00 +0100
categories: publication
tags: neuroscience
lang: english
---

Understanding whole-brain-scale electrophysiological recordings will rely on the collective work of multiple labs. Because two labs recording from the same brain area often reach different conclusions, it is critical to quantify and control for features that decrease reproducibility. To address these issues, we formed a multi-lab collaboration using a shared, open-source behavioral task and experimental apparatus. We repeatedly inserted Neuropixels multi-electrode probes targeting the same brain locations (including posterior parietal cortex, hippocampus, and thalamus) in mice performing the behavioral task. We gathered data across 9 labs and developed a common histological and data processing pipeline to analyze the resulting large datasets. After applying stringent behavioral, histological, and electrophysiological quality-control criteria, we found that neuronal yield, firing rates, spike amplitudes, and task-modulated neuronal activity were reproducible across laboratories. To quantify variance in neural activity explained by task variables (e.g., stimulus onset time), behavioral variables (timing of licks/paw movements), and other variables (e.g., spatial location in the brain or the lab ID), we developed a multi-task neural network encoding model that extends common, simpler regression approaches by allowing nonlinear interactions between variables. We found that within-lab random effects captured by this model were comparable to between-lab random effects. Taken together, these results demonstrate that across-lab standardization of electrophysiological procedures can lead to reproducible results across labs. Moreover, our protocols to achieve reproducibility, along with our analyses to evaluate it are openly accessible to the scientific community, along with our extensive electrophysiological dataset with corresponding behavior and open-source analysis code.


[{% reference IBL:2022 --file references.bib %}](https://www.biorxiv.org/content/10.1101/2022.05.09.491042v1)
