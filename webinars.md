---
layout: page
title: Wébinaires
permalink: /webinars/
list_title: Wébinaires
n_posts: 500
siteNav: false
---
Voici le programme des wébinaires organisés par le réseau dans le cadre des activités du [collège Animation](https://www.recherche-reproductible.fr/colleges/c_anim). Si vous souhaitez voir aborder un sujet, n'hésitez pas à nous contacter par [mail](contact@recherche-reproductible.fr) !

## Wébinaires

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.webinaires limit:page.n_posts -%}
    <li> A venir ➔
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
    </li>
 {%- endfor -%}
</ul>


#### Wébinaires passés
Vous pourrez retrouver les vidéos et les présentations associées aux wébinaires en cliquant sur le titre.
<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.past-webinaires limit:page.n_posts -%}
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
