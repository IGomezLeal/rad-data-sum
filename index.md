---
layout: default
title: "Home"
nav_order: 1
permalink: /
---

# Illeana Gomez-Leal, PhD.
{: .fs-9 }
Physics · Data Science · Numerical Modeling · HPC
{: .fs-6 .fw-300 .text-delta }

---

<div class="main-wrapper" style="display: flex; flex-wrap: wrap; gap: 40px; margin-top: 30px; align-items: flex-start;">

  <div class="sidebar-profile" style="flex: 1; min-width: 260px; background: #fafafa; padding: 20px; border-radius: 8px; border: 1px solid #eee;">
    
    <img src="/rad-data-sum/assets/fig/fpro.png" alt="Illeana Gomez-Leal, PhD." style="width: 110px; height: 110px; border-radius: 50%; object-fit: cover; border: 3px solid #fff; box-shadow: 0 2px 8px rgba(0,0,0,0.1); margin-bottom: 15px; display: block;">
    
    <h3 style="margin-top: 0; color: #272d33;">👤 Contact & Profiles</h3>
    <ul style="list-style: none; padding-left: 0; margin-bottom: 20px; font-size: 0.85em; line-height: 1.5;">
      <li style="margin-bottom: 6px;">🏫 Postdoctoral Associate at <br><strong>Cornell University</strong></li>
      <li style="margin-bottom: 6px;">🎓 <strong>PhD. in Astrophysics</strong></li>
      <li style="margin-bottom: 6px;">🔗 <a href="https://orcid.org/0000-0003-2254-5936" target="_blank">ORCID Profile</a></li>
      <li style="margin-bottom: 6px;">🔗 <a href="https://www.researchgate.net/profile/Illeana-Gomez-Leal-2" target="_blank">ResearchGate Profile</a></li>
      <li style="margin-top: 10px;"><a href="/rad-data-sum/cv_graphics.pdf" target="_blank" style="display: inline-block; padding: 6px 12px; background: #0056b3; color: #fff; border-radius: 4px; text-decoration: none; font-weight: bold; font-size: 0.9em;">Download CV (PDF)</a></li>
    </ul>

    <h3 style="color: #272d33;">🛠️ Production Stack</h3>
    <ul style="list-style: none; padding-left: 0; margin-bottom: 20px; font-size: 0.82em; line-height: 1.4; color: #555;">
      <li style="margin-bottom: 5px;"><strong>Languages:</strong> Python (Xarray, NumPy, Pandas), Fortran, Bash, SQL, IDL.</li>
      <li style="margin-bottom: 5px;"><strong>Data:</strong> NetCDF4, HDF5.</li>
      <li style="margin-bottom: 5px;"><strong>Infra:</strong> HPC (SLURM/PBS), Linux, Git, LaTeX.</li>
    </ul>

    <h3 style="color: #272d33;">🤝 Collaborations</h3>
    <ul style="list-style: none; padding-left: 0; margin-bottom: 0; font-size: 0.82em; line-height: 1.4; color: #555;">
      <li style="margin-bottom: 5px;"><strong>NCAR:</strong> Prof. Simone Tilmes.</li>
      <li style="margin-bottom: 5px;"><strong>PSI:</strong> Morgan Goodwin, CEO.</li>
      <li style="margin-bottom: 5px;"><strong>Nottingham:</strong> Prof. Cappelletti, Prof. Pushparaj, A. Sanchez.</li>
    </ul>
  </div>

  <div class="content-body" style="flex: 2.5; min-width: 350px;">
    
    <div style="background-color: #f4f6f8; border-left: 4px solid #0056b3; padding: 15px; margin-bottom: 25px; border-radius: 0 4px 4px 0; font-size: 0.95em;">
      Technical summary focused on multi-terabyte data architecture, computational physics, and advanced climate engineering simulations within the <strong>Community Earth System Model</strong> (CESM GCM) framework.
    </div>

    <h2>🔬 Project Overview</h2>
    <p>This repository serves as a technical showcase of my research at <strong>Cornell University</strong>, focusing on large-scale data architecture and numerical modifications within the <strong>CESM GCM</strong> framework. The core objective is to simulate the spectral and bolometric impacts of space-based solar radiation management (SRM) strategies.</p>

    <div style="background-color: #e6f4ea; border-left: 4px solid #137333; padding: 15px; margin-bottom: 25px; border-radius: 0 4px 4px 0; font-size: 0.95em;">
      🖥️ <strong>HPC Infrastructure:</strong> All simulations and data pipelines were architected and executed on the <a href="https://www.cisl.ucar.edu/capabilities/derecho" target="_blank"><strong>NCAR Derecho</strong></a> High-Performance Computing (HPC) cluster, utilizing <a href="https://docs.unidata.ucar.edu/netcdf-c/current/" target="_blank"><strong>NetCDF4</strong></a> standards for high-throughput I/O of <strong>60 TB+</strong> datasets.
    </div>

    <h3>📁 Data Standards: Why NetCDF?</h3>
    <p>The projects in this repository utilize <strong>NetCDF (Network Common Data Form)</strong>, the industry standard for array-oriented scientific data:</p>
    <ul>
      <li><strong>Multidimensional:</strong> Almacenamiento de variables (temperatura, presión, irradiancia) en coordenadas espacio-temporales 4D ($x, y, z, t$).</li>
      <li><strong>Self-Describing:</strong> Cada archivo incluye metadatos (unidades, coordenadas), asegurando la integridad de los datos.</li>
      <li><strong>Performance:</strong> Optimizado para lectura/escritura paralela a gran escala en el supercomputador <strong>NCAR Derecho</strong>.</li>
    </ul>

    <hr style="border: 0; border-top: 1px solid #eee; margin: 30px 0;">

    <h2>🚀 GCM Numerical Implementations & Core Projects</h2>

    ### 1. Bolometric Dimming and Climatic Response produced by a space-based Sunshade
    * **Framework:** CESM GCM con el Community Atmospheric Model (CAM).
    * **Implementation:** Parametrización en código de reducciones uniformes y no espectrales de la constante solar (bolometric dimming).
    * **Data Architecture:** Optimización del pipeline de E/S en Fortran de bajo nivel para ingerir parámetros NetCDF4 directamente en el núcleo del GCM.

    <iframe src="https://drive.google.com/file/d/1DHWkINHpbSsCgRyBI2aMFD9SVofIwm5_/preview" width="100%" height="450" allowfullscreen style="border: 1px solid #eee; border-radius: 6px; margin: 20px 0;"></iframe>

    ### 2. Filter Analysis, Spectral Dimming and Climatic Response produced by a space-based Sunshade
    * **Framework:** CESM con el Whole Atmosphere Community Climate Model (WACCM).
    * **Implementation:** Integración numérica del efecto de atenuación de un filtro espectral en el punto de Lagrange L1 dentro del núcleo de transferencia radiativa.
    * **Analytics Workflow:** Diagnósticos de anomalías climáticas multidimensionales bajo el escenario futuro **SSP2-4.5**.

    <iframe src="https://drive.google.com/file/d/1sqeUj7riu_lpyHYPxMysEleNBYZb2ZbS/preview" width="100%" height="450" allowfullscreen style="border: 1px solid #eee; border-radius: 6px; margin: 20px 0;"></iframe>

    ### 3. 4D Spatio-temporal Matrix Implementation and Simulations
    * **Framework:** Modificación de las matrices de forzamiento solar dentro de los módulos químicos y de transferencia radiativa de CESM GCM.
    * **Implementation:** Inserción de **matrices numéricas 4D** para simular la variabilidad en tiempo, latitud, longitud y longitud de onda del apantallamiento solar.
    * **Timeline:** Análisis de respuestas climáticas a largo plazo en una línea temporal de 30 años [2035, 2055].

    <hr style="border: 0; border-top: 1px solid #eee; margin: 30px 0;">

    <p style="font-size: 0.85em; color: #666;">
      📝 <strong>Note:</strong> This repository showcases specific technical implementations in <strong>HPC and Climate Analytics</strong>.<br>
      🔒 <strong>Privacy Note:** Full source code and configuration files are hosted in private repositories. Specific code samples are available upon request.
    </p>
  </div>
</div>lable upon request.
{: .fs-2 .text-grey-dk-000 }
