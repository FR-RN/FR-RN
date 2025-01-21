---
layout: page
list_title: Dernières nouvelles
n_posts: 10
---

# Bienvenue sur le réseau de la recherche reproductible

> Pour un chercheur, il n’y a rien de plus frustrant que l’impossibilité de reproduire des résultats majeurs obtenus quelques mois auparavant. Les causes de ce type de déconvenues sont multiples et parfois pernicieuses. Ce phénomène participe à ce que certains identifient comme une “crise de la reproductibilité de la recherche”. --- Vers une recherche reproductible, Desquilbet et al., 2019.

Le Réseau Français de la Recherche Reproductible est une initiative nationale informelle rassemblant des scientifiques engagés dans l’étude des facteurs favorisant la reproductibilité de la recherche. Bien que les enjeux de la reproductibilité varient selon les disciplines, ils concernent l’ensemble des domaines scientifiques. Le réseau s’attache ainsi à représenter une diversité disciplinaire riche et équilibrée.

Le réseau compte environ 260 membres inscrits à sa liste de diffusion, l’abonnement à celle-ci constituant actuellement le principal critère d’adhésion. Les membres occupent des fonctions variées et sont issus de nombreuses institutions réparties à travers le territoire français. Ainsi, au moins 30 disciplines différentes sont représentées. Cette diversité est un élément fondamental du réseau qui vise à promouvoir l'échange de bonnes pratiques et créer des discussions autour de procédures communes dans des disciplines différentes (voir la page [Membres](/members/) pour plus de détails).

## Objectifs du réseau

![Objectifs réseau](../assets/images/objectifs_recherche-repro.png){: style="width: 60%; display:block; margin-right: auto; margin-left:auto;" }

## Actions en cours

![Actions reseau](../assets/images/activites_recherche-repro.png){: style="width: 60%; display:block; margin-right: auto; margin-left:auto;" }

## Structure

Pour atteindre ces objectifs, le réseau s'est doté d'une structure avec 3 types de composantes : un copil qui définit les axes prioritaires et coordonne les différentes actions, des collèges transverses (animation, relations européennes, relations institutionnelles) et enfin des groupes de travail sur des sujets spécifiques (formation, notebooks, gestion des environnements logiciels).


## Activités

### Journées annuelles
* Journées 2023
* Journées 2024
* Journées 2025

### Wébinaires

{% if site.paginate %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.news limit:page.n_posts -%}
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



### Autres activités

* Participation aux réunions organisées avec les autres réseaux internationaux.
* Mises en place d'actions de formation de type hackathon, replication games, ANF
* Rédaction de fiches pratiques pour améliorer la reproductibilité des environnements logiciels
* Collaboration avec d'autres groupes de travail ayant des intérêts communs (GT notebooks par exemple)
* ...

## Comment participer ?

![Actions reseau](../assets/images/participer_recherche-repro.png){: style="width: 60%; display:block; margin-right: auto; margin-left:auto;" }
