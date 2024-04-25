---
layout: page
title: Activités
permalink: /activities/
list_title: Dernières nouvelles
n_posts: 500
siteNav: true
---

Voilà les dernières nouvelles ainsi que les événements à venir en lien
avec la recherche reproductible. Si vous souhaitez ajouter une
nouvelle ou annoncer un évènement, allez
[ici](https://github.com/FR-RN/FR-RN/tree/source/_posts) puis cliquez
sur "Add file". Vous pouvez regarder les
[nouvelles](https://raw.githubusercontent.com/FR-RN/FR-RN/source/_posts/2022-01-08-french-reproducibility-network-creation.md)
déjà postées pour copier le format (nommage du fichier et entête).


## Prochains évènements

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


## Nouvelles publications

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.publication limit:10 -%}
    <li>
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
          {% if post.lang == "english" %}
          [en]
          {% endif %}
        </a>
      </h3>
    </li>
 {%- endfor -%}
</ul>

## Évènements passés

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.past-event limit:page.n_posts -%}
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
