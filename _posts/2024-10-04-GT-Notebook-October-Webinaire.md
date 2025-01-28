---
layout: post
title:  "GT Notebook Webinaire #7 Jupyter Notebook dans un environnement HPC"
date:   2024-10-04 12:30 +0100
categories: past-webinaires
---

Pour cette **septième édition du webinaire du GT Notebook (Vendredi 04 octobre 12h30-14h00)**, nous avons décidé de faire un focus sur **l'execution des Notebooks dans un environnement HPC**.

Ces dernières  années, avec -entre autres-  le développement rapide et soutenu du Machine Learning et de la Data Science dans de multiples disciplines, de nouvelles communautées avec de nouveaux besoins se sont manifestés auprès des équipes d'ingénieur·e·s dans les centres de calculs.

Ces usages s'appuient sur le format Notebook (Jupyter, etc.), or celui n'est pas/n'était pas historiquement conçu pour un usage sur des clusters. C'est ce qui a poussé **plusieurs équipes d'ingénieur·e·s à développer des solutions pour déléguer les calculs réalisé dans les Notebooks**, en intervenant soit au niveau de la cellule, soit au niveau du Notebook lui-même.

Nous aurons la chance d'écouter et de discuter avec des ingénieurs spécialistes de ces questions au sein de différents [mésocentres](https://www.mesonet.fr/) régionaux, chacun sur 15/20 minutes :

- **Bernard CHAMBON** est ingénieur en développement logiciel au Centre de Calcul de l'IN2P3 (CC-IN2P3, UAR6402 rattachée à l’IN2P3). Il a mis en place et est responsable de la plateforme des notebooks Jupyter. Il présentera une solution avec Dask dans un environnement Slurm.
- **Benoist Gaston** est ingénieur HPC au sein de l'équipe calcul du CRIANN (Centre Régional Informatique et d'Application Numériques de Normandie).Il est rattaché au CCFR (Centre de Compétence HPC, HPDA et IA) du projet EuroCC qui accompagne les entreprises et le secteur public dans l'usage du HPC. Il nous présentera le service Jupyter mis en place sur le nouveau supercalculateur (Austral) du CRIANN.
- **Pierre-Antoine Bouttier** est ingénieur de recherche CNRS en ingéniérie logicielle, actuellement directeur adjoint de l'UAR GRICAD. Sa présentation détaillera comment GRICAD, à travers des services dédiés ou via l'usage des supercalculateurs, offre des possibilités pour travailler avec les bloc-notes Jupyter.
- **Ludovic Courtès** est ingénieur de recherche à Inria Bordeaux. Il a fondé Guix il y a plus de 10 ans et travaille sur l'usage de Guix au sein d'environnement de calcul haute performance via le projet [Guix HPC](https://hpc.guix.info/). Il présentera [Guix-Jupyter](https://gitlab.inria.fr/guix-hpc/guix-kernel), un noyau Jupyter basé sur Guix qui vise à fournir un environnement d'exécution contrôlé et réellement reproductible pour les blocs-notes Jupyter.

Vous trouverez plus de détails sur chaque présentation à l'adresse suivante : https://hackmd.io/@gtnotebook/SJ3ahvHaR/edit

*N'hésitez pas à relayer l'information dans vos réseaux !*

---

Pour vous inscrire, merci d'indiquer vos coordonnées (nom, prénom, courriel) dans ce [formulaire](https://enquetes-ng.univ-rouen.fr/index.php/719751)

La séance a lieu en ligne sur BBB, en simultanée un chat sur le rocket-chat d'Esup (https://rocket.esup-portail.org/) Vous recevrez les différentes informations la veille du webinaire.

Pour prendre connaissance des activités et des futurs du gt notebook, c'est ici ([humanum gitlab page work in progress](https://gt-notebook.gitpages.huma-num.fr/site_quarto/)) ou là ([groupe humanum gitlab](https://gitlab.huma-num.fr/gt-notebook)).

Pour rappel, le gt Notebook à le plaisir de vous proposer une série de webinaires pour 2024, l'objectif est d'explorer cet objet complexe que sont les notebooks, et cela au travers de ces différentes facettes : histoire, épistémologie, écriture, reproductibilité, plateformes, avantages et limites pédagogiques, interactivité, etc. Les vidéos des précédentes sessions sont  disponibles au fil de l'eau sur  la [chaîne Canal-U TV du GT notebook](https://www.canal-u.tv/chaines/gt-notebook/).
