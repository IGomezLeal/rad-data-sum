---
layout: default
title: "3. Dimming Field"
nav_title: "3. Dimming Field"
parent: "🔬 Research Projects"
nav_order: 3
description: "4D numerical array code modification for time-space-wavelength dynamic forcing."
---
<style>
  /* Fuerza al navegador a mostrar siempre el espacio del scrollbar para evitar saltos de pantalla */
  html {
    overflow-y: scroll;
  }

  .site-title {
    font-size: 1.3em !important; 
    font-weight: 500 !important;
    letter-spacing: 0.5px !important;
  }
  /* Fuerza a la barra lateral izquierda a mantener un ancho fijo idéntico en todo el sitio */
  .side-bar {
    width: 290px !important; /* Ajusta este número si la quieres un poco más estrecha o ancha */
    min-width: 290px !important;
  }
</style>

# 4D Spatio-temporal Matrix Implementation and Simulations
{: .fs-8 }

* **Framework:** Modification of the solar forcing arrays inside the CESM GCM radiative transfer and the chemical modules.
* **Implementation:** Architected and embedded **4D numerical matrices** into the model's core to simulate the solar forcing dimming produced by a space-based sunshade located at the first Lagrangian point (L1). The dimming has a variability in time, latitude, longitude, and wavelength.
* **Analytics Workflow:** Implemented dynamic spatiotemporal distributions of dimming factors that scale the solar irradiance at the top of the atmosphere. Analysis of multi-variable climate responses to the localized radiative forcing over a long-term 30-year timeline [2035, 2065].
* **Core Skills:** Advanced Fortran modifications, NetCDF data creation and implementation on the global climate model, multidimensional coordinate mapping, and high-resolution 3D visualization.

<!-- ================= PIE DE PÁGINA (HTML LIMPIO PARA ASIMETRÍA) ================= -->
<hr style="border: 0; border-top: 1px solid #eee; margin: 30px 0;">

<div style="font-size: 0.85em; color: #555; line-height: 1.6;">
  <p>📝 <strong>Note:</strong> This repository showcases specific technical implementations in <strong>HPC and Climate Analytics</strong>.</p>
  <p>🔒 <strong>Privacy Note:</strong> Full source code and configuration files are hosted in private repositories. Specific code samples (e.g., Python data pipelines or Fortran core modifications) are available upon request.</p>
</div>
