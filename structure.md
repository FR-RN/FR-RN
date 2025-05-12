---
layout: page
title: Structure, collèges et GTs
permalink: /steering/
cities: ["Annecy", "Bobigny", "Bordeaux", "Bron", "Chelles", "Clermont-Ferrand", "Corte", "Dijon", "Évry",  "Gif-Sur-Yvette", "Grenoble", "Limoges", "Lyon", "Marseille", "Montpellier", "Nantes", "Nice", "Orléans", "Orsay", "Palaiseau", "Paris", "Rennes", "Rungis", "Saclay", "Strasbourg", "Tarbes", "Toulouse", "Villetaneuse", "Villeurbanne"]
---

# Organisation actuelle
<!--
![Structure réseau](../assets/images/Structure_fr_nologo_links.png){: style="width: 60%; display:block; margin-right: auto; margin-left:auto;" }
-->
<img src="../assets/images/Structure_fr_nologo.png" alt="Structure" usemap="#workmap" width="400" height="400" style="display:block; margin-right: auto; margin-left:auto;">

<map name="workmap">
  <area shape="rect" coords="50,50,120,120" alt="animation" href="/colleges/c_anim">
  <area shape="rect" coords="50,290,200,390" alt="publications" href="/publications/">
  <area shape="rect" coords="350,210,400,350" alt="logiciel" href="/gtravail/gt_logiciel">
  <area shape="rect" coords="10,50,30,250" alt="formation" href="/gtravail/gt_formation">
  <area shape="rect" coords="10,250,30,350" alt="animation" href="https://gt-notebook.gitpages.huma-num.fr/site_quarto/">
  <area shape="rect" coords="150,150,250,250" alt="Steering" href="#steering">
</map>



# Comité de pilotage {#steering}


## Coordination du comité
<table style="list-style-type: none;">
<tr>
{% for person in site.data.members %}
     {%if person.coord == true %}
     <td>
     {%if person.image %}
     <img alt="{{ person.name }} image" src="{{ person.image }}" style="width: 100px; display:block;"/>
     {%endif%}
     {%if person.url %}
        <b><a href="{{ person.url }}"> {{ person.name }}</a></b>
     {% else %}
        <b>{{ person.name }}</b>
     {% endif %}
      <br>  
     {{ person.lab }}
   </td>
     {% endif %}
{% endfor %}
</tr>
</table>

## Membres
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

* [Relations européennes](/colleges/c_europe) : liens et organisations d'évènements communs avec les autres réseaux européens
* <b><a href="/colleges/c_anim">Animation scientifique</a></b> : organisation de séminaires et wébinaires autour de la reproductibilité
* Veille bibliographique et évènementielle : assurer la veille bibliographique mais également des conférences en lien avec la reproductibilité
* Relations institutionnelles et administratives : lien avec les différentes institutions de recherche françaises



# Groupes de travail

Les groupes de travail, sont organisés autour d'une thématique précise et ont pour but de définir et diffuser les bonnes pratiques pour une science reproductible dans leur périmètre :

* [GT Formation](https://www.recherche-reproductible.fr/gtravail/gt_formation): Sujets liés à l’enseignement et à la formation en matière de reproductibilité.
* [GT développement logiciel](/gtravail/gt_logiciel) : n'hésitez pas à rejoindre en vous abonnant à la [**liste de diffusion**](https://groupes.renater.fr/sympa/info/gt-env-logiciel).
* GT Contrôle qualité des échantillons biologiques
* Le [GT notebook](https://gt-notebook.gitpages.huma-num.fr/site_quarto/) est un GT autour les enjeux et problématiques du Notebook, pris comme un objet complexe au sein du cycle des données de la recherche. Il n'est pas directement un GT du réseau mais nous entretenons des collaborations étroites avec ses membres.
