---
layout: page
title: Community
permalink: /community/
cities: ["Bordeaux", "Grenoble"]
---

# French Reproducibility Network Members

Here are the French academics (or affiliated to a French research entity) that have declared interests and/or are active in reproducibility related topics.

{% for city in page.cities %}
## {{ city }}
  <ul>
  {% for person in site.data.people %}
    {%if person.city == city %}
      <li>
        <a href="{{ person.url }}"> {{ person.name }}</a>
        ({{ person.laboratory }}, {{ person.city }})
      </li>
    {% endif %}  
  {% endfor %}
  </ul>
{% endfor %}


# Network nodes

The Reproducibility Network is made of a number of international nodes whose number is growing each year. Each node is a national, peer-led consortium of researchers that aims to promote and ensure rigorous research practices by establishing appropriate training activities, designing and evaluating research improvement efforts, disseminating best practice and working with stakeholders to coordinate efforts across the sector. RNs aim for broad disciplinary representation and an intensive interdisciplinary dialogue (e.g., with funding agencies, publishers, learned societies and other sectoral organisations, as well as researchers from all disciplines and across all career stages).

<ul>
{% for node in site.data.nodes %}
  <li>
    {{ node.country }}: 
    <a href="{{ node.url }}">{{ node.url }}</a>
  </li>
{% endfor %}
</ul>

# Internationale initiatives

## Center for Open Science ([www.cos.io](https://www.cos.io))

Our mission is to increase openness, integrity, and reproducibility of research.
These are core values of scholarship and practicing them is presumed to increase the efficiency of acquiring knowledge. For COS to achieve our mission, we must drive change in the culture and incentives that drive researchers’ behavior, the infrastructure that supports their research, and the business models that dominate scholarly communication. This culture change requires simultaneous movement by funders, institutions, researchers, and service providers across national and disciplinary boundaries. Despite this, the vision is achievable because openness, integrity, and reproducibility are shared values, the technological capacity is available, and alternative sustainable business models exist.



## Reproducibility tea ([reproducibilitea.org](https://reproducibilitea.org/))

We are a grassroots journal club initiative that helps researchers create local Open Science journal clubs at their universities to discuss diverse issues, papers and ideas about improving science, reproducibility and the Open Science movement. Started in early 2018 at the University of Oxford, ReproducibiliTea has now spread to 137 institutions in 26 different countries. We are completely volunteer run, and provide a unique and supportive community for our members, who are predominantly Early Career Researchers.

## Reprohack ([www.reprohack.org](https://www.reprohack.org/))

During a ReproHack, participants attempt to reproduce published research of their choice from a list of proposed papers with publicly available associated code and data. Participants get to work with other people’s material in a low pressure environment and record their experiences on a number of key aspects, including reproducibility, transparency and reusability of materials. At the end of the day we regroup, share our experiences and give feedback to the authors. It’s imperative to note that ReproHacks are by no means an attempt to criticise or discredit work. We see reproduction as beneficial scientific activity in itself, with useful outcomes for authors and valuable learning experiences for the participants and the research community as a whole.

