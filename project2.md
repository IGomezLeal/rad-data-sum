---
layout: default
title: "2. Spectral Dimming"
nav_order: 3
---

# Filter Analysis, Spectral Dimming and Climatic Response
{: .fs-8 }

* **Framework:** CESM con el Whole Atmosphere Community Climate Model (WACCM).
* **Implementation:** Integración numérica del efecto de atenuación de un filtro espectral en el punto de Lagrange L1 dentro del núcleo de transferencia radiativa del GCM.
* **Analytics Workflow:** Desarrollo de pipelines de análisis espectral para evaluar la atenuación de radiación en bandas de longitud de onda del infrarrojo cercano. Diagnósticos de anomalías climáticas multidimensionales bajo el escenario futuro **SSP2-4.5**.
* **Big Data Scale:** Pipelines de E/S de alto rendimiento para el manejo de outputs de modelos climáticos de **60 TB**. Análisis estadístico posterior mediante flujos de trabajo en Python (Xarray/NumPy) paralelizados en el clúster HPC NCAR Derecho.

<iframe src="https://drive.google.com/file/d/1sqeUj7riu_lpyHYPxMysEleNBYZb2ZbS/preview" width="100%" height="500" allowfullscreen style="border: 1px solid #eee; border-radius: 6px; margin-top: 20px;"></iframe>
