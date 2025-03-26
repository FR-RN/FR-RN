---
layout: page
title: Communauté
permalink: /community/
cities: ["Annecy", "Bobigny", "Bordeaux", "Bron", "Chelles", "Clermont-Ferrand", "Corte", "Dijon", "Évry",  "Gif-Sur-Yvette", "Grenoble", "Limoges", "Lyon", "Marseille", "Montpellier", "Nantes", "Nice", "Orléans", "Orsay", "Palaiseau", "Paris", "Rennes", "Rungis", "Saclay", "Strasbourg", "Tarbes", "Toulouse", "Villetaneuse", "Villeurbanne"]
siteNav: true
childPages: ["Structure du réseau", "Réseaux internationaux", "Initiatives nationales", "Initiatives internationales"]
---
# Cartographie des membres

Suite à l'envoi d'une enquête aux abonnés de la liste, l'analyse de la centaine de réponses reçues nous a permis d'établir les documents ci-dessous.
L'ensemble des informations peut être consultés sur [ce rapport](../assets/pdf/composition_et_distribution_du_RFRR.pdf).
## Répartition géographique des Membres

![répartition géographique](../assets/images/carte_france.png){: style="border: 1px solid black; width: 30%; fl
oat: center; margin-right: 1em;" }

## Répartition par thématiques
![répartition géographique](../assets/images/heatmap_region_discipline_FR.png){: style="border: 1px solid black; width: 30%; fl
oat: center; margin-right: 1em;" }



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
