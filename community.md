---
layout: page
title: Communauté
permalink: /community/
cities: ["Bordeaux", "Grenoble", "Orléans", "Rennes", "Orsay"]
---

# Membres du réseau

Voilà la liste des universitaires ayant exprimé un intérêt ou étant actifs autour des thématiques de la recherche reproductible.

{% for city in page.cities %}
## {{ city }}
  <ul>
  {% for person in site.data.people %}
    {%if person.city == city %}
      <li>
        {%if person.url %}
          <a href="{{ person.url }}"> {{ person.name }}</a>
        {% else %}
          {{ person.name }}
        {% endif %}  
        ({{ person.laboratory }}, {{ person.city }})
      </li>
    {% endif %}  
  {% endfor %}
  </ul>
{% endfor %}


# Réseaux internationaux

Le réseau français s'inscrit dans un plus vaste réseau international
regroupant des réseaux nationaux composés d'universitaires qui visent
à promouvoir et à garantir des pratiques de recherche rigoureuses en
mettant en place des activités de formation appropriées, en concevant
et en évaluant les efforts d'amélioration de la recherche, en
diffusant les meilleures pratiques et en travaillant avec les parties
prenantes pour coordonner les efforts dans tout le secteur. Ces rseaux
nationaux visent une large représentation disciplinaire et un dialogue
interdisciplinaire intensif (par exemple, avec les organismes de
financement, les éditeurs, les sociétés savantes et d'autres
organisations sectorielles, ainsi que des chercheurs de toutes les
disciplines et à tous les stades de leur carrière).

<ul>
{% for node in site.data.nodes %}
  <li>
    {{ node.country }}: 
    <a href="{{ node.url }}">{{ node.url }}</a>
  </li>
{% endfor %}
</ul>

# Initiatives nationales corrélées

## Comité pour la Science Ouverte ([ouvrirlascience.fr](https://www.ouvrirlascience.fr/))

Le Comité pour la science ouverte mobilise les acteurs de l’enseignement supérieur et de la recherche pour accompagner de manière dynamique et coordonnée la mise en œuvre de la politique nationale de science ouverte. Il se compose de plusieurs instances qui proposent des orientations, instruisent les dossiers, effectuent des arbitrages, impulsent et accompagnent les actions associées. Il constitue une structure fluide, facilitant l’expression et la remontée des idées, les engagements et les contributions.

## Software Heritage ([softwareheritage.org](https://www.softwareheritage.org))

La mission de Software Heritage est de collecter, préserver et partager tous les logiciels disponibles publiquement sous forme de code source, dans le but de construire une infrastructure commune et partagée au service de l'industrie, de la recherche, de la culture et de la société dans son ensemble. Le code source des logiciels est collecté depuis des plateformes d'hébergement de code, comme GitHub, GitLab.com ou Bitbucket, et des archives de paquets, comme Npm ou Pypi, et est intégré dans une structure de données spécifique, un arbre de Merkle, qui est le cœur des archives de Software Heritage. Les artefacts qui se trouvent dans les archives sont associés à des identifiants appelés SWHID.

## HAL ([hal.archives-ouvertes.fr](https://hal.archives-ouvertes.fr/))

HAL est une plateforme en ligne développée en 2001 par le Centre pour la communication scientifique directe du CNRS, destinée au dépôt et à la diffusion d'articles de chercheurs (publiés ou non), et de thèses, émanant des établissements d'enseignement et de recherche français ou étrangers, des laboratoires publics ou privés. L'accès aux données est libre, mais pas nécessairement leur utilisation ou réutilisation. La plateforme vérifie le contenu scientifique des articles et documents déposés, mais ne procède pas à leur évaluation. Cet outil vient donc en complément de la publication dans des revues à comité de lecture. Les articles scientifiques peuvent y être déposés avant publication (preprint) ou après publication, l'archive fournissant alors, le cas échéant, un accès ouvert. 
