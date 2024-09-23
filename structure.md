---
layout: page
title: Structure du réseau
permalink: /steering/
cities: ["Annecy", "Bobigny", "Bordeaux", "Bron", "Chelles", "Clermont-Ferrand", "Corte", "Dijon", "Évry",  "Gif-Sur-Yvette", "Grenoble", "Limoges", "Lyon", "Marseille", "Montpellier", "Nantes", "Nice", "Orléans", "Orsay", "Palaiseau", "Paris", "Rennes", "Rungis", "Saclay", "Strasbourg", "Tarbes", "Toulouse", "Villetaneuse", "Villeurbanne"]
---

# Organisation actuelle

![Structure réseau](../assets/images/frrn-structure_v2.png){: style="width: 60%; display:block; margin-right: auto; margin-left:auto;" }


# Comité de pilotage

Le comité de pilotage actuel est composé des membres suivants:

  <ul style="list-style-type: none;">
  {% for person in site.data.members %}
       {%if person.steering == true %}
       <li>
       {%if person.image %}
       <img alt="{{ person.name }} image" src="{{ person.image }}" style="width: 100px; display:block;"/>
       {%endif%}
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

# Collèges

Les collèges transverses sont articulés autour de 4 thématiques :

* Relations européennes : liens et organisations d'évènements communs avec les autres réseaux européens
* <b><a href="/colleges/c_anim">Animation scientifique</a></b> : organisation de séminaires et wébinaires autour de la reproductibilité
* Relations institutionnelles et administratives : lien avec les différentes institutions de recherche françaises
* Veille bibliographique et évènementielle : assurer la veille bibliographique mais également des conférences en lien avec la reproductibilité


# Groupes de travail

Les groupes de travail, sont organisés autour d'une thématique précise et ont pour but de définir et diffuser les bonnes pratiques pour une science reproductible dans leur périmètre :

* GT Formation
* GT Notebooks
* GT Reproductibilité des environnements logiciels : vous puovez rejoindre ce groupe en vous abonnant à la liste de diffusion [mailing list](https://groupes.renater.fr/sympa/info/gt-env-logiciel).
* GT Contrôle qualité des échantillons biologiques
