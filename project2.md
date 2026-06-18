---
layout: default
title: "2. Spectral Dimming"
parent: "🔬 Research Projects"
nav_order: 2
description: "Implementation of Spectral Dimming experiments of the Solar Irradiance on a Global Climate model"
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

# Filter Analysis, Spectral Dimming, and Climatic Response produced by a space-based Sunshade
{: .fs-8 }

* **Framework:** CESM with the Whole Atmosphere Community Climate Model (WACCM).
* **Implementation:** Numerical integration into the GCM radiative transfer core of a spectral filter sunshade orbiting at the first Lagrangian point (L<sub>1</sub>) with a spectral dimming effect on the solar irradiance.
* **Analytics Workflow:** Developed spectral analysis pipelines to evaluate different wavelength bands radiation attenuations on the near infrared, focusing on different climate responses (atmospheric water vapor primary and secondary absorptions and NIR atmospheric window). Computed multidimensional climate anomaly diagnostics under the Shared Socioeconomic Pathways (SSP) framework **SSP2-4.5** future scenario.
* **Big Data Scale:** High-throughput I/O pipelines for 60 TB of climate dataset output. Developed routines to ingest and transform NetCDF4 structures into multidimensional arrays within the Fortran model core on the NCAR Derecho HPC cluster, with subsequent statistical analysis via parallelized Python (Xarray/NumPy) workflows.

<p style="font-size: 0.9em; color: #666; font-style: italic; margin-bottom: 8px; display: flex; align-items: center; gap: 6px;">
  ↗️ <span>Press the pop-up icon on the top right corner to see the slides in full screen:</span>
</p>

<iframe src="https://drive.google.com/file/d/1sqeUj7riu_lpyHYPxMysEleNBYZb2ZbS/preview" width="100%" height="500" allowfullscreen style="border: 1px solid #eee; border-radius: 6px; margin-top: 20px;"></iframe>
