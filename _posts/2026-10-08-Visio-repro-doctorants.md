---
layout: post
title:  "La reproductibilité vue par de jeunes chercheur.e.s"
date:   2026-10-08 14:00 +0100
categories: webinaires
tags: slides
---

Un *webinaire* est organisé le Jeudi 08 octobre de 14h à 16h autour
 de les *enjeux de la reproductibilité* présentés par 3
 jeunes scientifiques.

Ce webinaire sera diffusé sur le lien : [https://visio.numerique.gouv.fr/qns-tvbg-iny](https://visio.numerique.gouv.fr/qns-tvbg-iny).

### Programme 

 **Jey Pujet-Gill**

*Titre* : **Rejouer une expérience, 6 mois plus tard : les compromis de la reproductibilité**

*Résumé* :
La reproductibilité d'une expérience computationnelle se dégrade sans que personne n'intervienne.
Parmi les composantes d'une expérience, l'environnement d'exécution est celle que l'on décrit le moins, alors qu'il se reconstruit à partir de dépendances dont les versions évoluent en amont.
Cette présentation est un retour d'expérience sur les dispositifs mis en place durant une thèse en informatique pour contenir cette dérive, et sur ce qu'ils ont coûté.
Le cas d'étude est un benchmark portant sur l'interrogation de graphes de connaissances versionnés.
Le plan croise quatre facteurs à quatre modalités chacun : le nombre de versions du graphe ; le volume de données de la version initiale ; la croissance du graphe entre deux versions successives ; et les systèmes évalués. Le produit cartésien compte 256 exécutions.
La grandeur mesurée étant une durée, l'exigence n'était pas d'obtenir des valeurs identiques, mais de pouvoir rejouer la procédure complète plusieurs mois plus tard, sans réinstallation ni reprise manuelle.
Quatre niveaux d'outillage sont présentés : la conteneurisation de l'environnement, son exécution sur une infrastructure partagée, l'explicitation du plan d'expérience sous forme de programme, puis l'archivage et l'identification pérenne de l'artefact logiciel.
Le troisième niveau est détaillé : un modèle de workflow unique et paramétré est instancié une fois par sélection du produit cartésien, les 256 branches s'exécutant en parallèle avant une étape d'agrégation qui attend leur achèvement.
Changer une liste de paramètres suffit alors à définir une autre campagne.
Chaque niveau est discuté au regard de sa nécessité réelle selon l'échelle des expériences, l'ensemble représentant environ deux mois de travail cumulés.
La première partie de l'exposé ne suppose aucun prérequis technique.
La communication se conclut par une gradation d'actions selon le temps disponible, d'une journée à un mois et plus, en soutenant que le rapport entre bénéfice et effort est le plus favorable au premier échelon.


**Maxime Dieudonné**, post-doctorant au [Centre de Recherche en Psychologie et Neurosciences](https://crpn.univ-amu.fr/fr)

*Titre* : **Du notebook au code reproductible : retour d’expérience sur la structuration d’une pipeline de prétraitement d’IRM fonctionnelle**

*Résumé* :
Dans le cadre d'une étude portant sur le prétraitement et le débruitage d'images IRM fonctionnelles de la moelle épinière, j'ai été amené à reprendre une base de code déjà existante. Ma mission a consisté à réorganiser et améliorer des scripts, majoritairement développés sous Jupyter Notebook, afin de les faire évoluer vers une structure plus robuste, reproductible et plus facile à maintenir. Je partage avec vous mon retour d'expérience sur cette démarche, ainsi que les choix et les difficultés rencontrés au cours de cette démarche.


**Romain Caneill**, post-doctorant à l'[Intitut des Géosciences et de l'Environnement](https://www.ige-grenoble.fr/) à Grenoble

*Titre* : **Reproductibilité, science ouverte et logiciels libres**

*Résumé* :
Depuis plusieurs années, la mention de reproductibilité des articles scientifiques est de plus en plus discutée.
Un nombre croissant de revues demandent à ce que le code et les données utilisées pour produire les articles soient fournies publiquement.
Cette action avance dans la bonne direction, mais n’est pas suffisante pour garantir la reproductibilité d’une étude.
Nous verrons comment le logiciel libre et les publications en accès libre s’incrivent comme éléments essentiels dans cette démarche.
Dans cette présentation, je raconterai mon point de vue de chercheur en début de carrière sur les difficultés associées à l’analyse de données d’observations (de l’océan et la banquise dans mon cas).
Je présenterai aussi rapidement quelques solutions que j’utilise qui participent à la production de science plus reproductible.

