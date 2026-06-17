## 🚀 Explore Core Implementations
Use the sidebar menu or click directly below to explore the detailed numerical setups, workflows, and visualization panels for each research project:

<<<<<<< HEAD
<<<<<<< HEAD
{% for child in site.pages %}
  {% if child.parent == page.title %}
1. [**{{ child.title }}**]({{ child.url | relative_url }}) — {{ child.description }}
  {% endif %}
{% endfor %}

<style>
  .child_nav_list, #table-of-contents, .text-delta + ul, .has_children + ul {
    display: none !important;
  }
</style>
=======
1. [**1. Bolometric Dimming**](../projects/project1) — Hardcoded parameterizations of non-spectral solar constant reductions.
2. [**2. Spectral Dimming**](../projects/project2) — Radiative transfer integrations of Lagrangian L1 space filters.
3. [**3. 4D Matrix Simulation**](../projects/project3) — 4D numerical array embedding for time-space-wavelength dynamic forcing.
=======
{% for child in site.pages %}
  {% if child.parent == page.title %}
1. [**{{ child.title }}**]({{ child.url | relative_url }}) — {{ child.description }}
  {% endif %}
{% endfor %}
>>>>>>> f0e41c5f5e79b581c05a4e21afef6829347a5660

<style>
  .child_nav_list, #table-of-contents, .text-delta + ul, .has_children + ul {
    display: none !important;
  }
</style>

>>>>>>> 2d2cd38cef56bcb680f1895ea20eac339ba99aba