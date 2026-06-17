---
layout: default
title: "🔬 Research Projects"
nav_order: 2
has_children: true
permalink: /projects/
---

# 🔬 GCM Numerical Implementations, Simulations, and Analysis
{: .fs-9 }

Technical overview of multi-terabyte data architecture, computational physics, and advanced climate engineering simulations within the **Community Earth System Model** (CESM GCM) framework.
{: .fs-5 .fw-300 .text-grey-dk-000 }
---

## 🔬 Scientific Overview
This suite of projects serves as a technical showcase of my research at **Cornell University**, focusing on large-scale data architecture and numerical modifications within the **CESM GCM** framework. The core objective is to simulate the spectral and bolometric impacts of space-based solar radiation management (SRM) strategies.

> **HPC Infrastructure:** All simulations and data pipelines were architected and executed on the [**NCAR Derecho**](https://www.cisl.ucar.edu/capabilities/derecho){:target="_blank"} High-Performance Computing (HPC) cluster, utilizing [**NetCDF4**](https://docs.unidata.ucar.edu/netcdf-c/current/){:target="_blank"} standards for high-throughput I/O of **60 TB+** datasets.
{: .block-tip }

### 📁 Data Standards: Why NetCDF?
The projects documented here utilize **NetCDF (Network Common Data Form)**, the industry standard for array-oriented scientific data:
* **Multidimensional:** Storage of high-resolution atmospheric variables (temperature, pressure, irradiance) across 4D spatiotemporal coordinates **(x, y, z, t)**.
* **Self-Describing:** Every generated file embeds strict metadata (units, coordinate variables), ensuring data integrity across long-term runs.
* **Performance:** Optimized for large-scale parallel I/O architectures on the **NCAR Derecho** supercomputer.

---

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
