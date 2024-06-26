---
layout: page
title: Réseaux internationaux
permalink: /international/
siteNav: false
---

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
    <b>{{ node.country }}</b>: 
    <a href="{{ node.url }}">{{ node.url }}</a>
  </li>
{% endfor %}
</ul>
