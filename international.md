---
layout: page
title: Réseaux internationaux
permalink: /international/
siteNav: false
---

Le réseau français s'inscrit dans un écosystème la Fédération Globale des Réseaux de Reproductibilité [GFRN](https://reproducibility.global/).
Cette fédération rassemble des réseaux nationaux composés d'universitaires qui visent
à promouvoir et à garantir des pratiques de recherche rigoureuses en
mettant en place des activités de formation appropriées, en concevant
et en évaluant les efforts d'amélioration de la recherche, en
diffusant les meilleures pratiques et en travaillant avec les parties
prenantes pour coordonner les efforts dans tout le secteur. Ces réseaux
nationaux visent une large représentation disciplinaire et un dialogue
interdisciplinaire intensif (par exemple, avec les organismes de
financement, les éditeurs, les sociétés savantes et d'autres
organisations sectorielles, ainsi que des chercheurs de toutes les
disciplines et à tous les stades de leur carrière).

<img src="../assets/images/New-world-map-smaller-key2.png" alt="Structure" usemap="#workmap" width="600" height="350" style="display:block; margin-right: auto; margin-left:auto;">


<ul>
{% for node in site.data.nodes %}
  <li>
    <b>{{ node.country }}</b>:
    <a href="{{ node.url }}">{{ node.url }}</a>
  </li>
{% endfor %}
</ul>
