---
layout: page
title: Publications
permalink: /publications/
list_title: Publications
n_posts: 500
siteNav: false
---
Voici une liste de publications identifiées autour de la recherche reproductible. Vous pouvez trouver plus de références sur l'archive de publication du réseau : [zotero](https://www.zotero.org/groups/5860361/french_reproducible_research_network/), qui contient beaucoup de références !

## Publications

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
