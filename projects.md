## 🚀 Explore Core Implementations
Use the sidebar menu or click directly below to explore the detailed numerical setups, workflows, and visualization panels for each research project:

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
