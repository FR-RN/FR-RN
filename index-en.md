---
layout: page
list_title: Dernières nouvelles
n_posts: 8
---

# Welcome to the French Network for Reproducible Research

> "For a researcher, there is nothing more frustrating than the inability to reproduce major results obtained just a few months earlier. The causes of such setbacks are numerous and sometimes insidious. This phenomenon contributes to what some describe as a "reproducibility crisis in research.". --- Vers une recherche reproductible, Desquilbet et al., 2019.


The French Network for Reproducible Research is an informal national initiative bringing together scientists involved in the study of factors that promote the reproducibility of research. Although the challenges of reproducibility vary from one discipline to another, they concern all scientific fields. The network is committed to broad and balanced disciplinary diversity.

![Actions reseau](../assets/images/Titre.png){: style="width: 70%; display:block; margin-right: auto; margin-left:auto;" }

With around 260 members on its mailing list, subscription is currently the main criterion for membership. The members occupy a variety of positions and come from numerous institutions across France. At least 30 different disciplines are represented within the network. This diversity is a fundamental element of the network, which aims to promote the exchange of good practice and create discussion around common procedures in different disciplines (see the [Members](/community/) page for more details).


## Network Objectives

![Network Objectives](../assets/images/objectifs_recherche-repro.png){: style="width: 70%; display:block; margin-right: auto; margin-left:auto;" }

## Ongoing Actions

![Ongoing Actions](../assets/images/activites_recherche-repro.png){: style="width: 75%; display:block; margin-right: auto; margin-left:auto;" }

## Network Structure

To achieve these goals, the network has adopted a [structure](/steering/) with three types of components: a steering committee that defines priority areas and coordinates the various actions, cross-functional groups (animation, european relations, institutional relations, communication), and finally, working groups on specific topics (training, notebooks, software environment management).


## Activities

#### Annual Meetings
* [2023](/rr-days/), Paris
* [2024](/rr-days-2024/), Grenoble
* [2025](https://jrfrr-2025.sciencesconf.org/), Lyon

#### Webinars

{% if site.paginate %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.webinaires limit:page.n_posts -%}
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

#### Other Activities

* Attendance at meetings jointly organised with other international networks.
* Setting up training activities such as hackathons, replication games, ANF, etc.
* Drafting of practical sheets to improve the reproducibility of software environments.
* Collaboration with other work groups with common interests (e.g. Notebook WG).
* etc.

## How can you get involved?
![Nextwork Actions](../assets/images/Flyer_contacts-1.png){: style="width: 75%; display:block; margin-right: auto; margin-left:auto;" }
