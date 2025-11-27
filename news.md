---
layout: page
title: Activités ↓
permalink: /activities/
list_title: Dernières nouvelles
n_posts: 500
n_posts_news: 6
siteNav: true
childPages: ["Collèges et GTs", "Wébinaires", "Publications", "Formations"]
---

Voilà les dernières nouvelles ainsi que les événements à venir en lien
avec la recherche reproductible. Si vous souhaitez ajouter une
nouvelle ou annoncer un évènement, allez
[ici](https://github.com/FR-RN/FR-RN/tree/source/_posts) puis cliquez
sur "Add file". Vous pouvez regarder les
[nouvelles](https://raw.githubusercontent.com/FR-RN/FR-RN/source/_posts/2022-01-08-french-reproducibility-network-creation.md)
déjà postées pour copier le format (nommage du fichier et entête).

## Activités du réseau

Les membres du réseau organise des [wébinaires](/webinars/) via le [collège Animation](/colleges/c_anim), participent à des [formations](/training/) autour de la reproductibilité via le groupe de travail "Formation" et recensent des [publications](/publications/) en lien avec le sujet.

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.event-network limit:page.n_posts -%}
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

{% if site.paginate %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.news-network limit:page.n_posts -%}
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



### Journées annuelles
Le réseau organise des journées annuelles, multidiciplinaires, pour favoriser l'échange d'expériences :
  * [Journées 2023](/rr-days/), Paris
  * [Journées 2024](/rr-days-2024/), Grenoble
  * [Journées 2025](https://jrfrr-2025.sciencesconf.org/), Lyon


### Implication au niveau européen et international

Le réseau s'inscrit dans une dynamique européenne et internationale et participe à plusieurs actions mises en place :

* Participation au groupe de travail sur la pérennisation de la Fédération Globale de Réseaux de Reproductibilité
* Organisation de webinaires consacré aux réseaux européens
* Implication dans le projet TRUSTparency
* Représentation du réseau dans des événements internationaux


## Activités connexes

### Conférences

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

### Dernières nouvelles

{% if site.paginate %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.news limit:page.n_posts_news -%}
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




### Évènements passés

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.past-event limit:page.n_posts_news -%}
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
