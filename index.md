---
layout: page
list_title: Dernières nouvelles
n_posts: 8
n_news: 1
n_actus: 2
---

# Bienvenue sur le réseau de la recherche reproductible

> Pour un chercheur, il n’y a rien de plus frustrant que l’impossibilité de reproduire des résultats majeurs obtenus quelques mois auparavant. Les causes de ce type de déconvenues sont multiples et parfois pernicieuses. Ce phénomène participe à ce que certains identifient comme une “crise de la reproductibilité de la recherche”. --- Vers une recherche reproductible, Desquilbet et al., 2019.

<!--
![Actions reseau](../assets/images/banniere_web.png){: style="width: 50%; display:block; margin-right: auto; margin-left:auto;" }
-->
Le Réseau Français de la Recherche Reproductible est une initiative nationale informelle rassemblant des scientifiques engagés dans l’étude des facteurs favorisant la reproductibilité de la recherche. Bien que les enjeux de la reproductibilité varient selon les disciplines, ils concernent l’ensemble des domaines scientifiques. Le réseau s’attache ainsi à représenter une diversité disciplinaire riche et équilibrée.
[Plus d'information dans ce document !](assets/pdfs/presentation.pdf)

## News !

<div class="news">
<h6>  Wébinaires </h6>
  <ul class="post-list">
   {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
     {%- for post in site.categories.webinaires limit:page.n_news -%}
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


<h6>Conférences </h6>
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

<h6>Actualités du réseau</h6>

{% if site.paginate %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.news limit:page.n_actus -%}
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

<h6>Divers</h6>

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.newsletter limit:page.n_news -%}
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


La prochaine newsletter est en préparation, n'hésitez pas à nous faire part des contenus que vous voudriez partager avec la communauté !

<div class="news2"> Retrouvez l'intégralité des actualités <a href="{{activities | relative_url}}/activities/">sur cette page</a> !</div>
</div>


<br>


## Objectifs du réseau

![Objectifs réseau](../assets/images/objectifs_recherche-repro-fr.png){: style="width: 55%; display:block; margin-right: auto; margin-left:auto;" }

Le réseau compte environ 260 membres inscrits à sa liste de diffusion, l’abonnement à celle-ci constituant actuellement le principal critère d’adhésion. Les membres occupent des fonctions variées et sont issus de nombreuses institutions réparties à travers le territoire français. Ainsi, au moins 30 disciplines différentes sont représentées. Cette diversité est un élément fondamental du réseau qui vise à promouvoir l'échange de bonnes pratiques et créer des discussions autour de procédures communes dans des disciplines différentes (voir la page [Membres](/community/) pour plus de détails).

## Actions en cours

![Actions reseau](../assets/images/activites_recherche-repro.png){: style="width: 60%; display:block; margin-right: auto; margin-left:auto;" }

## Structure

Pour atteindre ces objectifs, le réseau s'est doté d'une [structure](/steering/) avec 3 types de composantes : un copil qui définit les axes prioritaires et coordonne les différentes actions, des collèges transverses ([animation](/colleges/c_anim), [relations européennes](/colleges/c_europe), relations institutionnelles) et enfin des groupes de travail sur des sujets spécifiques ([formation](/gtravail/gt_formation), [notebooks](https://gt-notebook.gitpages.huma-num.fr/site_quarto/), [logiciel et environnements](/gtravail/gt_logiciel)).


## Activités

### Journées annuelles

  * [Journées 2023](/rr-days/), Paris
  * [Journées 2024](/rr-days-2024/), Grenoble
  * [Journées 2025](https://jrfrr-2025.sciencesconf.org/), Lyon

### Wébinaires

Le collège "Animation" organise des wébinaires réguliers sur des thèmes variés autour de la recherche reproductible. Vous pouvez retrouver la liste des wébinaires sur la [page du collège animation](/colleges/c_anim).


### Implication au niveau européen
* Participation au groupe de travail sur la pérennisation de la Fédération Globale de Réseaux de Reproductibilité
* Organisation de webinaires consacré aux réseaux européens
* Implication dans le projet TRUSTparency
* Représentation du réseau dans des événements internationaux


<br/>
<a href="https://groupes.renater.fr/sympa/info/recherche-reproductible" target="_blank">![Actions reseau](../assets/images/Contacts.png){: style="width: 65%; display:block; margin-right: auto; margin-left:auto;" }</a>
