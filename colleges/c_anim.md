---
layout: page
title: Collège Animation scientifique
---

# Organisation actuelle
Le collège animation se réunit une fois par mois avec pour objectifs de proposer des wébinaires et des animations
en lien avec la reproductibilité.
Les thèmes traités se veulent variés afin de représenter aux mieux les préoccupations des membres du réseau.

Si vous souhaitez participer à ce collège, il vous suffit de nous rejoindre en vous abonnant à la [liste de diffusion](https://groupes.renater.fr/sympa/info/recherche-reproductible-animation)
Pour voir un thème particulier abordé, n'hésitez pas à nous contacter :  [recherche-reproductible-animation](mailto:recherche-reproductible-animation@groupes.renater.fr).

## Wébinaires organisés par le réseau

<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.webinaires limit:page.n_posts -%}
   #### Prochains wébinaires
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

#### Programme des séminaires à venir
* **6 Mai 2025, 14h** : Présentation du réseau anglais (UKRN), organisation, fonctionnement et initiatives, *Etienne Roesch*
* **23 Mai 2025, 14h** : Reproductibilité et environnements de développement, *Pol Dellaiera*
* **13 Juin 2025, 16h** :{rix}, un paquet R qui s'appuie sur Nix ,*Bruno Rodriguez*.


#### Séminaires passés
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
