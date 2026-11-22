---
title: "Projects"
permalink: /projects/
author_profile: true
---

Small open-source projects, mostly in Python, on electrochemical simulation, data analysis and modelling. All code is on [GitHub](https://github.com/deannguyen9xyz).

{% for group in site.data.projects %}
## {{ group.category }}

<div class="project-grid">
{%- for p in group.items %}
<div class="project-card{% unless p.image %} project-card--text{% endunless %}">
{%- if p.image %}
<a class="project-card__image" href="{{ p.url }}"><img src="{{ '/images/projects/' | append: p.image | relative_url }}" alt="{{ p.alt }}" loading="lazy" width="960" height="600"></a>
{%- endif %}
<div class="project-card__body">
<h3 class="project-card__title"><a href="{{ p.url }}">{{ p.name }}</a></h3>
<p>{{ p.description }}</p>
</div>
</div>
{%- endfor %}
</div>
{% endfor %}
