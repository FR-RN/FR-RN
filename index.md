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
## Le réseau

Le Réseau Français de la Recherche Reproductible est une initiative nationale informelle rassemblant des scientifiques engagés dans l’étude des facteurs favorisant la reproductibilité de la recherche. Bien que les enjeux de la reproductibilité varient selon les disciplines, ils concernent l’ensemble des domaines scientifiques. Le réseau s’attache ainsi à représenter une diversité disciplinaire riche et équilibrée.
[Plus d'information dans ce document !](assets/pdfs/presentation.pdf)

Le réseau compte environ 400 membres inscrits à sa liste de diffusion, l’abonnement à celle-ci constituant actuellement le principal critère d’adhésion. Les membres occupent des fonctions variées et sont issus de nombreuses institutions réparties à travers le territoire français. Ainsi, au moins 30 disciplines différentes sont représentées. Cette diversité est un élément fondamental du réseau qui vise à promouvoir l'échange de bonnes pratiques et créer des discussions autour de procédures communes dans des disciplines différentes (voir la page [Membres](/community/) pour plus de détails).
Un rapport d'activité pour l'année 2024 est disponible en [téléchargement](assets/pdfs/rapport-2024.pdf).


## Les objectifs

![Objectifs réseau](../assets/images/objectifs_recherche-repro2b.png){: style="width: 70%; display:block; margin-right: auto; margin-left:auto;" }


La reproductibilité de la recherche vise avant tout à renforcer la transparence, la robustesse, la fiabilité et la réutilisabilité des résultats scientifiques. Pour y parvenir, les actions mises en œuvre par le réseau de recherche reproductible doivent s’inscrire dans une approche pérenne, ancrée à la fois dans les dynamiques européennes et internationales.

Pour répondre à ces enjeux, les objectifs visés par le réseau sont multiples :

* Constituer une communauté multidisciplinaire engagée à promouvoir la reproductibilité des recherches scientifiques;
* Identifier les facteurs limitant la reproductibilité des résultats de recherche et proposer des actions concrètes pour y parvenir notamment la mise en place et la diffusion de bonnes pratiques, la formation, et l’acculturation des chercheur.euse.s;
* Étendre cette dynamique à l’échelle institutionnelle, nationale et internationale, tout en établissant des connexions avec les initiatives liées à la science ouverte et à l’intégrité scientifique.


## Les activités

![Actions reseau](../assets/images/activites_recherche-repro2c.png){: style="width: 70%; display:block; margin-right: auto; margin-left:auto;" }

Les activités du réseau sont multiples et cherchent à toucher différents publics. Le réseau organise des journées annuelles de rencontres multi-disciplinaire autour de la reproductibilité. Le collège animation du réseau organise régulièrement des wébinaires, Des membres du groupe de travail formation participent et/ou organisent des formations sur la reproductibilité. La reproductibilité computationnelle étant une problématique transverse à beaucoup de disciplines scientifiques, un groupe de travail logiciel a été mis en place pour rédiger et promouvoir des fiches de bonnes pratiques sur le sujet.

→ [Plus d’informations sur la page Activités](/activities/).

## Comment contribuer ?

La reproductibilité est un sujet qui vous intéresse ? 

Vous pouvez :
* vous abonner à la [liste de diffusion](https://groupes.renater.fr/sympa/info/recherche-reproductible) pour être informé 
* diffuser des informations dans vos réseaux professionnels : relayer les mails, mettre une [affiche en français](assets/pdfs/flyerA4_rechercherepro_FR.pdf) ou une [affiche en anglais](assets/pdfs/flyerA4_rechercherepro_EN.pdf), …
* animer une [sensibilisation dans votre laboratoire](/training/#ateliers)
* proposer une sensibilisation aux doctorants de votre école doctorale 
* rédiger une fiche de bonnes pratiques spécifiques à votre discipline 
* participer à un [groupe de travail](/steering/#gt)
* proposer un nouveau groupe de travail

N'hésitez pas à nous rejoindre !
<br/>
<a href="https://groupes.renater.fr/sympa/info/recherche-reproductible" target="_blank">![Actions reseau](../assets/images/Contacts.png){: style="width: 65%; display:block; margin-right: auto; margin-left:auto;" }</a>
