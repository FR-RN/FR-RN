---
layout: post
title:  "# Newsletter N°1 : Mai 2024"
date:   2024-03-26 13:00 +0100
categories: newsletter
---

--------------------------------------------------------------------
## Manifestations

* [2ième journées](href="https://jrfrr-2024.sciencesconf.org/") du réseau [Recherche Reproductible](https://www.recherche-reproductible.fr/), 26-28 Mars 2024, Grenoble : #DF0174" News : les vidéos sont en ligne !
* [52e forum ORAP](https://orap52.sciencesconf.org/) : "HPC et reproductibilité", 15 Mars 2024, siège du CNRS, 3 rue Michel Ange, Paris. Retrouvez les enregistrements sur ce [lien](http://orap.irisa.fr/52ieme-forum-reproductibilite/).

**A venir** :

* [META-REP 2024](https://www.conference2024.meta-rep.uni-muenchen.de/index.html) – the Conference on Meta-Science and Replicability in the social, behavioral, and cognitive sciences. 28-31 Octobre, Munich.
* [ACM conference on Replicability and Reproducibility](https://acm-rep.github.io/2024/), 18-20 Juin 2024, Rennes.


## Formations
* MOOC "Recherche reproductible : principes méthodologiques pour une science transparente", partie II  : bientôt en ligne !!
* [MOOC "Recherche reproductible : principes méthodologiques pour une science transparente"](https://www.fun-mooc.fr/fr/cours/recherche-reproductible-principes-methodologiques-pour-une-science-transparente/), partie I : toujours d'actualité !

## Publications

* [High replicability of newly discovered social-behavioural findings is achievable](https://www.nature.com/articles/s41562-023-01749-9), Protzko, J., Krosnick, J., Nelson, L. et al.
* [NLP Reproducibility For All: Understanding Experiences of Beginners](https://aclanthology.org/2023.acl-long.568/), Shane Storks, Keunwoo Yu, Ziqiao Ma, Joyce Chai.
* [A guide to reproducible research papers](https://hpc.guix.info/blog/2023/06/a-guide-to-reproducible-research-papers/), Ludovic Courtès, Marek Felšöci, Konrad Hinsen, Philippe Swartvagher.
* [Reproducibility and Research Integrity – Report Summary](https://publications.parliament.uk/pa/cm5803/cmselect/cmsctech/101/summary.html), UK parliament.



  *Le réseau français de la recherche reproductible est un réseau national composé de scientifiques intéressés par l’étude des facteurs qui contribuent à la robustesse de la recherche, la promotion des activités de formation et la diffusion des bonnes pratiques ainsi que des recommandations. Les questions de reproductibilité touchent toutes les disciplines et le réseau vise une large représentation disciplinaire.*


    *Vous trouverez plus d'information sur le site du réseau [Recherche Reproductible](https://recherche-reproductible.fr/)
     Si vous souhaitez vous impliquer, envoyez-nous un courriel et rejoignez le réseau : mailto:contact@recherche-reproductible.fr.*

## Archives

Vous pouvez retrouver les lettres plus anciennes sur la page Archive.

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for newsl in site.categories.newsletter -%}
    <li>
      <span class="post-meta">{{ newsletter.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ newsletter.url | relative_url }}">
          {{ newsletter.title | escape }}
        </a>
      </h3>
    </li>
 {%- endfor -%}
</ul>

---
