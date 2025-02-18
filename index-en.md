---
layout: page
list_title: Dernières nouvelles
n_posts: 8
---

# Welcome to the French Network for Reproducible Research

> "For a researcher, there is nothing more frustrating than the inability to reproduce major results obtained just a few months earlier. The causes of such setbacks are numerous and sometimes insidious. This phenomenon contributes to what some describe as a "reproducibility crisis in research.". --- Vers une recherche reproductible, Desquilbet et al., 2019.


![Actions reseau](../assets/images/bandeau-web.png){: style="width: 50%; display:block; margin-right: auto; margin-left:auto;" }

The French Network for Reproducible Research is an informal national initiative bringing together scientists involved in the study of factors that promote the reproducibility of research. Although the challenges of reproducibility vary from one discipline to another, they concern all scientific fields. The network is committed to broad and balanced disciplinary diversity.

## Last news !

<div class="news">
<h6>  Webinar </h6>
  <ul class="post-list">
   {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
     {%- for post in site.categories.past-webinaires limit:page.n_news -%}
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
<h6>Conference </h6>
<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.event limit:page.n_news -%}
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

<h6>News</h6>

{% if site.paginate %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.news limit:page.n_news -%}
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

<h6>Further information</h6>
The next newsletter is in preparation, so don't hesitate to let us know what content you'd like to share with the community!

<div class="news2"> Read all the news <a href="{{activities | relative_url}}/activities/">on this page</a> !</div>
</div>

## Network Objectives

![Network Objectives](../assets/images/aims.png){: style="width: 45%; display:block; margin-right: auto; margin-left:auto;" }

With around 260 members on its mailing list, subscription is currently the main criterion for membership. The members occupy a variety of positions and come from numerous institutions across France. At least 30 different disciplines are represented within the network. This diversity is a fundamental element of the network, which aims to promote the exchange of good practice and create discussion around common procedures in different disciplines (see the [Members](/community/) page for more details).

## Ongoing Actions

![Ongoing Actions](../assets/images/actions.png){: style="width: 60%; display:block; margin-right: auto; margin-left:auto;" }

## Network Structure

To achieve these goals, the network has adopted a [structure](/steering/) with three types of components: a steering committee that defines priority areas and coordinates the various actions, cross-functional groups (animation, european relations, institutional relations, communication), and finally, working groups on specific topics (training, notebooks, software environment management).


## Activities

#### Annual Meetings
* [2023](/rr-days/), Paris
* [2024](/rr-days-2024/), Grenoble
* [2025](https://jrfrr-2025.sciencesconf.org/), Lyon

#### Webinars
The network organises regular webinars on a variety of topics relating to reproducible research. You can find [the list of seminars on this page](/activities/).


<br />

<a href="https://groupes.renater.fr/sympa/info/recherche-reproductible" target="_blank">![Actions reseau](../assets/images/Contacts-en.png){: style="width: 65%; display:block; margin-right: auto; margin-left:auto;" }</a>
