---
layout: post
title:  "Recherche Reproductible: états des lieux (compte-rendu)"
date:   2023-03-15 08:00 +0100
categories: news
---

Les premières journées du [réseau français de la recherche reproductible](http://www.recherche-reproductible.fr/) se sont déroulées à l’Institut Pasteur les 8 et 9 mars 2023, en mode hybride. L'objectif de ces journées était de dresser un état des lieux de la reproductibilité dans les domaines de la recherche scientifique en France, en tenant compte de la diversité des disciplines et des pratiques. Les 2 jours ont été divisés en 6 sessions, contenant des présentations de 10 minutes, suivies à chaque fois d’une discussion générale. **[[slides]](/assets/rrdays/00-Introduction.pdf)**

## 1. Reproductibilité observationnelle

L’objectif de cette session était d’identifier les sources de non-reproductibilité dans le domaine observationnel, les solutions envisagées, et les nouvelles questions qui en émergent.

**Alexandre Hocquet** a ouvert les journées en nous rappelant que, depuis les années 1980, les historiens des sciences travaillent sur la thématique de la reproductibilité en science, mais que la communauté scientifique ne s'y intéresse que depuis la crise de la reproductibilité. Il a cité les recherches de Sabina Leonelli, qui permettent de mieux cerner les multiples facettes de la reproductibilité *et offre une catégorisation de ces facettes*. La reproductibilité s'envisage de multiples façons, y compris à l'intérieur du même domaine de recherche.

**Timothée Giraud** est ensuite intervenu pour expliquer le point de vue des sciences humaines et sociales, où les traitements numériques sont le quotidien. Les problèmes sont l'utilisation d'outils numériques avec interface graphique, ne permettant pas une bonne traçabilité des étapes des analyses, et l'utilisation de logiciels privateurs qui entrainent des problèmes de formats et de transparence des méthodes d'analyse. Les formations initiales abordent peu les outils et notions de la recherche reproductible, et les personnes se forment par elles-mêmes, sans acquérir les bonnes pratiques de programmation.
**[[slides]](/assets/rrdays/02-Giraud.pdf)**

**Thomas Vuillaume** a présenté [le projet européen ESCAPE](https://projectescape.eu/) (cluster pour la physique des particules et l'astronomie) en mettant notamment en avant les [données FAIR](https://www.ouvrirlascience.fr/fair-principles/), les [logiciels FAIR](https://www.nature.com/articles/s41597-022-01710-x) et [les moyens techniques](https://projectescape.eu/services) pour une recherche reproductible dans les grandes infrastructures de recherche partenaires d'ESCAPE. Il a expliqué que ces moyens techniques ne suffisent pas et que les chercheurs aussi doivent être "FAIR" (c'est-à-dire qui adoptent et appliquent les principes FAIR) et que la reproductibilité ne doit pas être un objectif dès le départ, mais qu'il faut y tendre progressivement, par étapes. **[[slides]](/assets/rrdays/03-Vuillaume.pdf)**
  
## 2. Reproductibilité computationnelle

L'objectif de cette session était d'identifier les sources de non-reproductibilité dans le domaine computationnel, les solutions envisagées, et les nouvelles questions qui en émergent.

À partir d'un exemple en biophysique moléculaire, **Konrad Hinsen** a montré les limites de la reproductibilité computationelle, nous rappelant que la confusion entre un modèle scientifique (défini) et son implémentation informatique (variable) condamne presque tout effort de réplicabilité, et que la négligence dans la gestion des environnement logiciel empêche la reproductibilité. On a fait du progrès au cours des dernières années, mais il reste beaucoup de chemin à faire. **[[slides]](/assets/rrdays/04-Hinsen.pdf)**


**Roberto Di Cosmo** a poursuivi en faisant un historique de la prise de conscience des problèmes de reproductibilité en informatique et les efforts faits pour y pallier. La Digital Library de l'[ACM](https://dl.acm.org/journals) s'efforce de lier article et code, mais le code source n'est pas toujours publié avec l'article, et quand il l'est, il manque l'historique de dévéloppement, essentiel pour le comprendre et le ré-utiliser. La communauté du machine learning est à l'origine de *Papers with Code*, mais le lecteur est renvoyé directement à la plateforme de développement du code source, ce qui ne permet pas d'identifier la version précise utilisée dans l'article et ne garantit pas un accès pérenne. Une solution existe pour préserver sur le long terme les codes sources et identifier précisément les versions associées aux publications : [Software Heritage](https://archive.softwareheritage.org/). Cette méthode permet notamment la conservation du code source, le suivi des versions et un référence plus précis et sûr que des simples DOI. Elle est adoptées par des journaux comme IPOL, eLife ou JTCAM.

**Camille Maumet** nous a présenté les problèmes de reproductibilité en neuro-imagerie, notamment autour de l'analyse des données  - qui même si elle est automatique est soumise à de nombreux choix réalisés par des experts - et donc difficilement reproductible. Un autre problème est la taille de l'études, qui n'est pas toujours suffisante pour conférer une puissance statistique adéquate. Pour y remédier, des consortiums sont mis en place afin de mutualiser les données. Elle a aussi mentionné le nombre d'étapes dans les analyses, entre données brutes et résultats finaux, et la nécessité de travailler de façon collaborative au sein de la communauté pour mettre en place de bonnes pratiques.
**[[slides]](/assets/rrdays/06-Maumet.pdf)**

**Thomas Moreau** a présenté [l'environnement BenchOpt](https://benchopt.github.io/), développé dans le cadre de l'apprentissage automatique. BenchOpt permet d'assurer la création de benchmarks collaboratifs et efficaces, en combinant plusieurs langages dans un même benchmark. BenchOpt permet de comparer et de comprendre la variabilité de traitements de données d'une méthode à l'autre. Le but de benchopt n'est pas d'assurer une reproducibilité bit à bit, mais plutot une reproducibilité statistique des resultats, tout en promouvant une forme de maintenance des benchmarks, pour que les resultats soit mis à jour avec les évolutions des softwares. **[[slides]](/assets/rrdays/07-Moreau.pdf)**


## 3. Reproductibilité statistique

L'objectif de cette session était d'identifier les sources de non-reproductibilité dans le domaine des méthodes statistiques, les solutions envisagées, et les nouvelles questions qui en émergent.

Après avoir rappelé le très faible taux de reproductibilité en économie, **Christophe Hurlin** a présenté [Cascad](https://www.ouvrirlascience.fr/cascad-la-certification-de-la-reproductibilite-de-la-recherche-scientifique/), une UMS de certification de codes et de données qui permet de garantir la reproductibilité des articles. Cette UMS est aujourd'hui sollicitée par des journaux en économie et a déjà certifié une cinquantaine de codes.

**Nelle Varoquaux** a ensuite présenté les problématiques rencontrées en bio-physique, biochimie et évolution où les facteurs de non-reproductibilité sont nombreux : origine des données, annotations des génomes, méthode d'analyses, disponibilité et accessibilité du code, temps de calcul parfois long qui empêche les ré-analyses. La nouvelle revue [SFDS](http://journal-sfds.fr/) tente d'y remédier en publiant des analyses entièrement reproductibles, et ce dans un temps raisonable.

Pour **Isabelle Boutron**, la transparence pour les essais cliniques vient avant même la question de la reproductibilité de ces essais. Sous l'impulsion de Drumond Rennie, le pré-enregistrement des protocoles des essais ainsi que des directives claires pour écrire les rapports sont devenus incontournables, notamment pour éviter le "harking" ou post-hoc analysis.

## 4. Reproductibilité expérimentale

L'objectif de cette session était d'identifier les sources de non-reproductibilité en recherche expérimentale, les solutions envisagées, et les nouvelles questions qui en émergent.

**Fay Betsou** a commencé son intervention en soulignant qu'il existe d'innombrables facteurs de variabilité dans la préparation des échantillons biologiques, avant même de réaliser des expériences à la paillasse. Ces facteurs sont rarement, ou mal, mentionnés dans les méthodes d'un article. Il est donc nécesaire d'avoir de nouveaux standards de rédaction de protocole et la traçabilité des données.

**Florian Naudet** nous a rappelé le cycle hypothetico-déductif et les déviances, telles que le *harking* ou le *p-hacking*. A travers différents exemples, il a insisté sur les conséquences de santé publique des difficultés à reproduire la recherche thérapeutique (e.g. rTMS, antidépresseurs, traitement du paludisme). Les solutions envisagées reposent sur une meilleure conception et l'enregistrement des études, le partage des données, la nécessité d'aligner les incitatifs et de former une nouvelle génération de chercheurs à ces enjeux. Il est important de mettre en oeuvre une approche de métarecherche permettant d'évaluer l'impact de ces solutions.

**François Ric** a présenté un bref historique de la reproductibilité en psychologie et comment la communauté s'est saisie du problème pour se réformer en profondeur, notamment via l'[Open Science Framework](https://osf.io/). Aujourd'hui, le pré-enregistrement des études, le partage des données et la transparence des méthodes ont été adoptés. **[[slides]](/assets/rrdays/12-Ric.pdf)**

**Yoann Lafon** a présenté les problèmes de reproductibilité méthodologique en caractérisation de matériaux biologiques, poussée notamment par les nouvelles réglementations pour la mise sur le marché des dispositifs médicaux autorisant le recours à la simulation numérique. Se posent alors le problème de la certification des données utilisées dans ces simulations. Un consortium international a donc rassemblé 25 équipes pour améliorer la reproductibilité de la caractérisation mécanique de tissus biologiques. Les membres du consortium ont travaillé sur les mêmes données, d'abord avec des protocoles différents, puis en appliquant un protocole unique issu d'un consensus. des travaux sont encore en cours pour réduire les incertitudes expérimentales. L'effet de ces incertitudes sur le comportement des modèles dépend finalement des paramètres de sortie utilisés pour répondre à la Question d'Intérêt.

## 5. Formation et enseignement

La sensibilisation aux notions de reproductibilité dans le domaine de la recherche peut être effectuée en formation initiale, dès le master, ou dans le cadre professionnel. L'objectif de cette session a été de présenter des exemples actuellement mis en place dans certains masters, et des solutions de formation dans le milieu professionnel.

**Frédéric Lemoine** a présenté le *Reprohackathon*, un module d'enseignement mis en place depuis 2020 dans le master AMI2B (Université Paris-Saclay, ~40 étudiants/an) sur la reproductibilité computationnelle. Ce module est composé d'une partie théorique+pratique et d'un projet long, consistant pour les étudiants en un travail de plusieurs mois en semi-autonomie. Les étudiants doivent comprendre la méthode utilisée dans un article pour ensuite la mettre en oeuvre via un workflow afin d'en reproduire les résultats. L'objectif est de comprendre l'intérêt de la reproductibilité et d'en connaître en profondeur les concepts techniques et outils.
**[[slides]](/assets/rrdays/14-Lemoine.pdf)**

[ReproducibiliTea](https://reproducibilitea.org/) est une initiative anglaise reprise [à Bordeaux par **Eduarda Centeno** et **Fjola Hyseni**](https://www.bordeaux-neurocampus.fr/reproducibilitea-in-bordeaux-another-successful-year/). Elles nous ont présenté sa mise en place en 2021 ainsi que son organisation. Après deux ans, elles ont organisé 18 sessions sur une variété de sujets sur la science ouverte et la reproductibilité, y compris des sessions spéciales avec des invités de l'UNESCO, FORRT et d'autres 'ReproductibiliTea's. Le BordeauxTea est devenu une formation doctorale sur l'ADUM, donnant des heures et des certificats aux étudiants participants.
**[[slides]](/assets/rrdays/15-Centeno-Hyseni.pdf)**

**Laurent Oudre** nous a ensuite présenté un nouveau track d'enseignement dans le master MVA (ENS Paris-Saclay) composé d'un cours théorique et d'un cours pratique. Le but pour les étudiants est de pouvoir soumettre un article à la [revue IPOL](https://www.ipol.im/), très exigeante sur les aspects de reproductibilité.  **[[slides]](/assets/rrdays/17-Oudre.pdf)**

**Arnaud Legrand** a terminé la session en expliquant la genèse du MOOC "Recherche Reproductible", qui compte désormais plus de 13 000 participants depuis la troisième édition ouverte en 2020. Une suite de ce MOOC, plus technique, est appelée à se développer avec 3 modules en préparation : gestion des données, contrôle des environnements logiciels et workflow scientifique. Ces modules seront disponibles à la fin de l'automne 2023. Ce retour d'expérience permet aussi de mettre en lumière la problématique de la sensibilisation de communautés variées : comment toucher efficacement des utilisateurs de domaines pouvant se percevoir éloignés de ces questions ? 
 **[[slides]](/assets/rrdays/18-Legrand.pdf)**

## 6. Europe et international

Dans de nombreux pays, il existe des réseaux académiques nationaux dédiés à la question de la reproductibilité. Un des enjeux de ces journées a été de réfléchir à la définition et à la gouvernance d'un tel réseau, à l'échelle nationale française.

**Étienne Roesch** a présenté le United Kingdom Reproducitibility Network ([UKRN](https://www.ukrn.org/)) fondé en 2018 en abordant son organisation, ses financements et son développement. Ce réseau, aujourd'hui composé de 70 noeuds locaux, 25 universités et 50 "stakeholders", permet d'influer sur les politiques. Toutefois, Étienne met en garde contre les risques de dérives : le *reproducibility washing*. **[[slides]](/assets/rrdays/19-Roesch.pdf)**

**Vittorio Iacovella** est le fondateur du réseau italien de reproductibilité ([ITRN](https://www.itrn.org/)) qui a démarré en mars 2021, à la suite de discussions datant de 2017. Le réseau se veut un lieu de formation, de discussion, d'organisation. Le réseau est aussi conçu pour permettre la formation de groupes de travail et est toujours en évolution.

**Isabelle Blanc** a terminé la session en présentant le Comité pour la Science Ouverte ([COSO](https://www.ouvrirlascience.fr/accueil/)) en expliquant notamment ses ambitions, son organisation, ses réalisations et son influence sur le paysage scientifique français, européen et international. Le COSO pourrait être une structure d'accueil pour un futur réseau national français de la recherche reproductible.

## Discussion générale

Ces deux journées se sont terminées par une discussion générale concernant l'avenir de la communauté de recherche reproductible en France.  L'objectif de ces premières journées était de réaliser un état des lieux de la reproductibilité dans divers domaines de la recherche scientifique. Ces journées ont permis aux personnes intéressées de se réunir afin d'échanger sur les objectifs de créer une initiative nationale autours de la recherche reproductible, et les prochaines étapes. Outre le sujet des financements, la question des fonctions support dont le réseau a besoin pour se développer et se structurer a été notamment abordée et va être examinée. 

Les personnes présentes (physiquement ou en ligne) semblent enthousiastes à l'idée de se structurer. Une réunion en ligne sera bientôt organisée afin de poursuivre nos efforts. Un questionnaire va être diffusé afin de recenser, à l'échelle nationale, les initiatives locales de reproductibilité ; et de savoir quelles personnes seraient volontaires pour s'impliquer dans la mise en place d'un projet d'envergure nationale, et dans quelle mesure.
