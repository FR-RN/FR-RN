---
layout: page
title: Collège Animation scientifique
---

# Organisation actuelle

Les membres du collège organisent des wébinaires en lien avec la reproductibilité.

## Wébinaires organisés par le réseau
#### Programme des prochains séminaires
* **28 Mars 2025, 14h** : Reproductibilité et géomatique, *Thimotée Giraud, Nicolas Roelandt*
* **6 Mai 2025, 14h** : Présentation du réseau anglais de reproducbilité (UKRN), organisation, fonctionnement et initiatives, *Etienne Roesch*
* **23 Mai 2025, 14h** : Reproductibilité en calcul scientifique, *Pol Dellaiera* (date à confirmer)
* **13 Juin 2025, 16h** :{rix}, un paquet R qui s'appuie sur Nix ,*Bruno Rodriguez*.


<ul class="post-list">
 {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
   {%- for post in site.categories.webinaires limit:page.n_posts -%}
   #### Prochains séminaires
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
