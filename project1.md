---
layout: default
title: "1. Bolometric Dimming"
parent: "🔬 Research Projects"
nav_order: 1
description: "Bolometric dimming implementation of the solar irradiance to balance the greenhouse gas emissions SSP2-4.5 scenario."
---
<style>
  .site-title {
    font-size: 1.3em !important; 
    font-weight: 500 !important;
    letter-spacing: 0.5px !important;
  }
  .side-bar {
    width: 290px !important; /* Ajustado a los 290px que unificamos */
    min-width: 290px !important;
  }
</style>

# Bolometric dimming and climatic response produced by a space-based sunshade
{: .fs-8 }

* **Framework:** CESM GCM with the Community Atmospheric Model (CAM).
* **Implementation:** Hardcoded parameterization of uniform, bolometric dimming of the solar irradiance for baseline climate sensitivity testing.
* **Analytics Workflow:** Statistical analysis comparing bolometric forcing mechanisms during the period (2035,2060) on stratospheric temperatures, ozone concentration, surface temperature, and precipitation anomalies, as well as Arctic sea ice preservation with respect to the baseline period (2025,2035).
* **Data Architecture:** Optimized the low-level Fortran I/O pipeline to ingest NetCDF4 parameters directly into the GCM core, maximizing computational efficiency to perform global sensitivity experiments.

<p style="font-size: 0.9em; color: #666; font-style: italic; margin-bottom: 8px; display: flex; align-items: center; gap: 6px;">
  ↗️ <span>Press the pop-up icon on the top right corner to see the slides in full screen:</span>
</p>

<iframe src="https://drive.google.com/file/d/1DHWkINHpbSsCgRyBI2aMFD9SVofIwm5_/preview" width="100%" height="500" allowfullscreen style="border: 1px solid #eee; border-radius: 6px; margin-top: 20px;"></iframe>
