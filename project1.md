---
layout: default
title: "1. Bolometric Dimming"
parent: "🔬 Research Projects"
nav_order: 1
description: "Hardcoded parameterizations of non-spectral solar constant reductions."
---

# Bolometric Dimming and Climatic Response produced by a space-based Sunshade
{: .fs-8 }

* **Framework:** CESM GCM with the Community Atmospheric Model (CAM).
* **Implementation:** Hardcoded parameterization of uniform, non-spectral solar constant reductions (bolometric dimming) for baseline climate sensitivity testing.
* **Analytics Workflow:** Statistical analysis comparing bolometric forcing mechanisms on global stratospheric and surface temperature anomalies, as well as Arctic sea ice preservation.
* **Data Architecture:** Optimized the low-level Fortran I/O pipeline to ingest NetCDF4 parameters directly into the GCM core, maximizing computational efficiency to perform global sensitivity experiments, and ensuring seamless memory mapping between physical disk storage and the model’s numerical kernels.

<p style="font-size: 0.9em; color: #666; font-style: italic; margin-bottom: 8px; display: flex; align-items: center; gap: 6px;">
  ↗️ <span>Press the pop-up icon on the top right corner to see the slides in full screen:</span>
</p>

<iframe src="https://drive.google.com/file/d/1DHWkINHpbSsCgRyBI2aMFD9SVofIwm5_/preview" width="100%" height="500" allowfullscreen style="border: 1px solid #eee; border-radius: 6px; margin-top: 20px;"></iframe>
