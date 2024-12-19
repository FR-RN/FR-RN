---
layout: page
list_title: Dernières nouvelles
n_posts: 3
---

# Bienvenue sur le réseau de la recherche reproductible

> Pour un chercheur, il n’y a rien de plus frustrant que l’impossibilité de reproduire des résultats majeurs obtenus quelques mois auparavant. Les causes de ce type de déconvenues sont multiples et parfois pernicieuses. Ce phénomène participe à ce que certains identifient comme une “crise de la reproductibilité de la recherche”. --- Vers une recherche reproductible, Desquilbet et al., 2019.


Le réseau français de la recherche reproductible est un réseau
national composé de scientifiques intéressés par l'étude des facteurs
qui contribuent à la robustesse de la recherche, la promotion des
activités de formation et la diffusion des bonnes pratiques ainsi que
des recommandations. Les questions de reproductibilité touchent toutes
les disciplines et le réseau vise une large représentation
disciplinaire.

Si vous êtes intéressé :
- envoyez-nous un [courriel](mailto:contact@recherche-reproductible.fr)

- rejoignez la [mailing list](https://groupes.renater.fr/sympa/info/recherche-reproductible) !

## Prochains évenements

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.event limit:page.n_posts -%}
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

## Dernières nouvelles

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


## Dernières publications

{% if site.paginate %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.publication limit:page.n_posts -%}
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
