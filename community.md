---
layout: page
title: Communauté ↓
permalink: /community/
cities: ["Annecy", "Aubervilliers", "Aubière", "Avignon", "Bobigny", "Bordeaux", "Bron", "Bruxelles", "Champs-sur-Marne", "Chelles", "Clermont-Ferrand", "Corte", "Créteil", "Dijon", "Évry",  "Gif-Sur-Yvette", "Grenoble", "Limoges", "Lille", "Lyon", "Marseille", "Montpellier", "Nantes","Narbonne", "Nice","Nogent-sur-Marne", "Noisy-le-Grand", "Orléans", "Orsay", "Palaiseau", "Paris","Reading", "Rennes", "Rouen", "Rungis", "Saclay","Stockholm", "Strasbourg", "Tarbes", "Toulouse","Tours", "Villetaneuse", "Villeurbanne"]
siteNav: true
childPages: ["Structure, collèges et GTs", "Réseaux internationaux", "Initiatives nationales", "Initiatives internationales", "Nous rejoindre"]
---
# Cartographie des membres

Suite à l'envoi d'une enquête aux abonnés de la liste, l'analyse de la centaine de réponses reçues nous a permis d'établir les documents ci-dessous.
L'ensemble des informations peut être consultés sur [ce rapport](../assets/pdfs/composition_et_distribution_du_RFRR.pdf).
## Répartition géographique et thématique des Membres

![répartition géographique](../assets/images/Carto1.png){: style="border: 1px solid black; width: 70%; fl
oat: center; margin-right: 1em;margin-left: 10em;" }


# Membres du réseau

Liste des scientifiques ayant exprimé un intérêt ou étant actifs autour des thématiques de la recherche reproductible.
Si vous souhaitez apparaitre sur cette page ou au contraire ne plus apparaitre, merci d'envoyer un mail à contact[@]recherche-reproductible.fr.
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
