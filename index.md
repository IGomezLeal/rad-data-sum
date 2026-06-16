---
layout: page
title: "Portfolio | HPC & Climate Analytics"
sidebar:
  nav: index-sidebar
---

<article class="md-content">

<p class="teaser">
  Technical summary focused on multi-terabyte data architecture, computational physics, and advanced climate engineering simulations within the <a href="https://www.cesm.ucar.edu/models" target="_blank"><strong>Community Earth System Model</strong></a> (CESM GCM) framework.
</p>

## 🔬 Project Overview

This repository serves as a technical showcase of my research at **Cornell University**, focusing on large-scale data architecture and numerical modifications within the **CESM GCM** framework. The core objective is to simulate the spectral and bolometric impacts of space-based solar radiation management (SRM) strategies.

<blockquote>
  <p>🖥️ <strong>HPC Infrastructure:</strong> All simulations and data pipelines were architected and executed on the <a href="https://www.cisl.ucar.edu/capabilities/derecho" target="_blank"><strong>NCAR Derecho</strong></a> High-Performance Computing (HPC) cluster, utilizing <a href="https://docs.unidata.ucar.edu/netcdf-c/current/" target="_blank"><strong>NetCDF4</strong></a> standards for high-throughput I/O of <strong>60 TB+</strong> datasets.</p>
</blockquote>

### 📁 Data Standards: Why NetCDF?

The projects in this repository utilize <a href="https://docs.unidata.ucar.edu/netcdf-c/current/" target="_blank"><strong>NetCDF (Network Common Data Form)</strong></a>, the industry standard for array-oriented scientific data:

* **Multidimensional:** It allows for the storage of variables (temperature, pressure, solar irradiance) across 4D space-time coordinates ($x, y, z, t$).
* **Self-Describing:** Each file includes metadata (units, standard names, and coordinates), ensuring data integrity during high-throughput I/O.
* **Performance:** Optimized for large-scale parallel reads/writes on HPC clusters like <a href="https://www.cisl.ucar.edu/capabilities/derecho" target="_blank"><strong>NCAR Derecho</strong></a>, facilitating the management of the <strong>60 TB</strong> dataset created and analyzed in this work.

---

## 🚀 GCM Numerical Implementations & Core Projects

### 1. Bolometric Dimming and Climatic Response produced by a space-based Sunshade
* **Framework:** CESM GCM with the Community Atmospheric Model (CAM).
* **Implementation:** Hardcoded parameterization of uniform, non-spectral solar constant reductions (bolometric dimming) for baseline climate sensitivity testing.
* **Analytics Workflow:** Statistical analysis comparing bolometric forcing mechanisms on global stratospheric and surface temperature anomalies, as well as Arctic sea ice preservation.
* **Data Architecture:** Optimized the low-level Fortran I/O pipeline to ingest NetCDF4 parameters directly into the GCM core, maximizing computational efficiency to perform global sensitivity experiments, and ensuring seamless memory mapping between physical disk storage and the model’s numerical kernels.

<div class="embed-video" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; margin: 20px 0 40px 0; border: 1px solid var(--border-color); border-radius: 6px;">
  <iframe src="https://drive.google.com/file/d/1DHWkINHpbSsCgRyBI2aMFD9SVofIwm5_/preview" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none;" allowfullscreen></iframe>
</div>

### 2. Filter Analysis, Spectral Dimming and Climatic Response produced by a space-based Sunshade
* **Framework:** CESM with the Whole Atmosphere Community Climate Model (WACCM).
* **Implementation:** Numerical integration of a space-based (Lagrangian point L1) spectral filter sunshade dimming effect into the GCM radiative transfer core.
* **Analytics Workflow:** Developed spectral analysis pipelines to evaluate different wavelength bands radiation attenuations on the near infrared, focusing on different climate responses. Computed multidimensional climate anomaly diagnostics under the Shared Socioeconomic Pathways (SSP) framework **SSP2-4.5** future scenario.
* **Big Data Scale:** High-throughput I/O pipelines for 60 TB of climate dataset output. Developed routines to ingest and transform NetCDF4 structures into multidimensional arrays within the Fortran model core on the NCAR Derecho HPC cluster, with subsequent statistical analysis via parallelized Python (Xarray/NumPy) workflows.

<div class="embed-video" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; margin: 20px 0 40px 0; border: 1px solid var(--border-color); border-radius: 6px;">
  <iframe src="https://drive.google.com/file/d/1sqeUj7riu_lpyHYPxMysEleNBYZb2ZbS/preview" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none;" allowfullscreen></iframe>
</div>

### 3. 4D Spatio-temporal Matrix Implementation and Simulations
* **Framework:** Modification of the solar forcing arrays inside the CESM GCM radiative transfer and the chemical modules.
* **Implementation:** Architected and embedded <strong>4D numerical matrices</strong> into the model's core to simulate the solar forcing dimming produced by a space-based sunshade located at the first Lagrangian point (L1). The dimming has a variability in time, latitude, longitude, and wavelength.
* **Analytics Workflow:** Implemented dynamic spatiotemporal distributions of dimming factors that scale the solar irradiance at the top of the atmosphere. Analysis of multi-variable climate responses to the localized radiative forcing over a long-term 30-year timeline [2035, 2065].
* **Core Skills:** Advanced Fortran modifications, NetCDF data creation and implementation on the global climate model, multidimensional coordinate mapping, and high-resolution 3D visualization.

---

<p style="font-size: 0.9em; opacity: 0.8; line-height: 1.6;">
  📝 <strong>Note:</strong> This repository showcases specific technical implementations in <strong>HPC and Climate Analytics</strong>. For inquiries regarding my broader research in <strong>Astrophysics and Climate Science</strong>, please contact me via my ResearchGate profile or the email provided in my CV.<br><br>
  🔒 <strong>Privacy Note:</strong> Full source code and configuration files are hosted in private repositories. Specific code samples (e.g., Python data pipelines or Fortran core modifications) are available upon request.
</p>

</article>
