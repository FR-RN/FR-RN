---
layout: page
title: Ressources
permalink: /resources/
siteNav: true
n_posts: 5
---

# Communication

## Liste de diffusion

L'objectif de la liste
**[recherche-reproductible](https://groupes.renater.fr/sympa/info/recherche-reproductible)**
est de confronter les points de vue de différentes disciplines
scientifiques sur la notion de reproductibilité et recenser les
différentes initiatives prises notamment au niveau national. Au-delà
du diagnostic spécifique à chaque discipline, il s'agit d'identifier
certaines problématiques communes et d'évoquer, avec différents
acteurs (chercheurs, éditeurs scientifiques etc.), les solutions qui
peuvent émerger autour notamment du concept de publication exécutable.

## Forum de discussion

Le **[forum](https://forum.recherche-reproductible.fr/)** de la recherche reproductible est le lieu pour discuter librement de la reproductibilité afin d'améliorer notre méthodologie de recherche en échangeant des expériences, des informations et des conseils. Aidez-nous à faire de ce site un lieu de discussion privilégié en essayant toujours d'améliorer la discussion d'une manière ou d'une autre, aussi minime soit-elle.

## Newsletters

Le réseau publie une newsletter tous les deux mois environ afin de partager les dernières actualités avec les membres du réseau.

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.newsletter limit:page.n_posts -%}
    <li>
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
    </li>
 {%- endfor -%}
</ul>

## Syndication

Le flux **[RSS]({{ 'feed.xml' | relative_url }})** donne accès aux dernières nouvelles du réseau ainsi que des événements à venir en relation avec la rechercher reproductible en France et dans le monde.

# Documents de présentation {#documents}

Afin de communiquer sur les objectifs et la actions du réseaux, nous avons rédigés plusieurs documents :

* un document de présentation générale : [quelques pages !](assets/pdfs/presentation.pdf)  qui donnent des informations essentielles sur le réseau.
* un [poster qui peut être librement téléchargé !](assets/pdfs/FRRN_Poster.pdf) et utilisé dans des conférences
* un [flyer au format a4 !](assets/pdfs/FRRN_Flyer.pdf) pour être affiché dans les lieux de convivialité de votre laboratoire ou sur la porte de votre bureau.


# Ressources bibliographiques

Les membres du réseau sont invités à ajouter à la base de données bibliographique zotero :

[base zotero du réseau](https://www.zotero.org/groups/5860361/french_reproducible_research_network/)

toute publication en lien avec la reproductibilité qu'ils jugent d'intérêt pour la communauté.

# Education

## Recherche reproductible : principes méthodologiques pour une science transparente

Ce **[mooc](https://www.fun-mooc.fr/en/courses/reproducible-research-methodological-principles-transparent-scie/)** propose des principes méthodologiques pour une science ouverte et transparente. Il aborde de manière pratique la prise de notes, le document computationnel, la réplicabilité des analyses. Vous prenez des notes et vous voulez vous y retrouver ? Vous faites des calculs sur ordinateur et vos résultats changent d’un jour à l’autre ? Vous aimeriez partager avec vos collègues vos analyses de données et vos derniers travaux et qu’ils puissent les réutiliser ? Ce mooc {%cite mooc:2020 %} est pour vous, doctorant-e-s, chercheur-se-s, étudiant-e-s en master, enseignant-e-s, ingénieur-e-s de toutes disciplines qui souhaitez vous former à des environnements de publication et des outils fiables.


## Vers une recherche reproductible

Pour un chercheur, il n’y a rien de plus frustrant que l’impossibilité de reproduire des résultats majeurs obtenus quelques mois auparavant. Les causes de ce type de déconvenues sont multiples et parfois pernicieuses. Ce phénomène participe à ce que certains identifient comme une “crise de la reproductibilité de la recherche”. Cet ouvrage {%cite book:2019 %} considère un ensemble de situations et de pratiques potentiellement dangereuses afin d’illustrer et de mettre en évidence les symptômes de la non-reproductibilité dans la recherche. À chaque fois, il propose un éventail de solutions allant de bonnes pratiques faciles et rapides à implémenter jusqu’à des outils plus techniques, tous gratuits et mis à l’épreuve par les auteurs eux-mêmes. Dans ce **[livre](https://rr-france.github.io/bookrr/)** rédigé lors d’un book sprint, étudiants, ingénieurs et chercheurs devraient trouver des moyens efficaces et à leur portée pour améliorer leurs pratiques de la recherche reproductible.

# Publications des membres du réseau

{% bibliography --file network.bib %}
