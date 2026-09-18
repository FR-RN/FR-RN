---
layout: page
title: Wébinaires
permalink: /webinars/
list_title: Wébinaires
n_posts: 500
siteNav: false
---
Voici le programme des wébinaires organisés par le réseau dans le cadre des activités du [collège Animation](https://www.recherche-reproductible.fr/colleges/c_anim). Si vous souhaitez voir aborder un sujet, n'hésitez pas à nous contacter par [mail](contact@recherche-reproductible.fr) !

Nous relayons également des wébinaires sur des sujets connexes qui peuvent inétresser certains d'entre vous !

### Wébinaires du réseau

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

#### Agenda 
Notez dès à présent sur vos agendas les évènements à venir :

* 8 Octobre, 14h : 1/2 journées des doctorants
* 6 Novembre : visio avec les membres du réseau : bilan et projets
* 20 Novembre : webinaire de présentation des activités du réseau suisse, Fabio Molo 
* 12 Mars 2027 : Go with the (Work)Flow! Creating Reusable and Replicable Workflows for Digital Humanities Research, Anne Baillot

Plus d'infomration très prochainement !

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

### Wébinaires connexes
#### Les wébinaires du gt-notebooks

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.past-webinaires-notebooks limit:page.n_posts -%}
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