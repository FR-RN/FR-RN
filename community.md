---
layout: page
title: Communauté
permalink: /community/
cities: ["Annecy", "Bobigny", "Bordeaux", "Bron", "Chelles", "Clermont-Ferrand", "Corte", "Dijon", "Évry",  "Gif-Sur-Yvette", "Grenoble", "Limoges", "Lyon", "Marseille", "Montpellier", "Nantes", "Nice", "Orléans", "Orsay", "Palaiseau", "Paris", "Rennes", "Rungis", "Saclay", "Strasbourg", "Tarbes", "Toulouse", "Villetaneuse", "Villeurbanne"]
siteNav: true
childPages: ["Structure du réseau", "Réseaux internationaux", "Initiatives nationales", "Initiatives internationales"]
---

# Membres du réseau

Liste des scientifiques ayant exprimé un intérêt ou étant actifs autour des thématiques de la recherche reproductible.

{% for city in page.cities %}
## {{ city }}
  <ul>
  {% for person in site.data.members %}
    {%if person.city == city %}
       <li>
       {%if person.url %}
          <b><a href="{{ person.url }}"> {{ person.name }}</a></b>
       {% else %}
          <b>{{ person.name }}</b>
       {% endif %}  
       — {{ person.lab }}
       </li>
    {% endif %}  
  {% endfor %}
  </ul>
{% endfor %}  
