---
layout: default
title: "1. Bolometric Dimming"
nav_order: 2
---

# Bolometric Dimming and Climatic Response produced by a space-based Sunshade
{: .fs-8 }

* **Framework:** CESM GCM con el Community Atmospheric Model (CAM).
* **Implementation:** Parametrización en código de reducciones uniformes y no espectrales de la constante solar (bolometric dimming) para baseline climate sensitivity testing.
* **Analytics Workflow:** Análisis estadístico comparando los mecanismos de forzamiento bolométrico sobre anomalías de temperatura global (estratosférica y superficial), así como la preservación del hielo marino en el Ártico.
* **Data Architecture:** Optimización del pipeline de E/S en Fortran de bajo nivel para ingerir parámetros NetCDF4 directamente en el núcleo del GCM, maximizando la eficiencia computacional en experimentos de sensibilidad global.

<iframe src="https://drive.google.com/file/d/1DHWkINHpbSsCgRyBI2aMFD9SVofIwm5_/preview" width="100%" height="500" allowfullscreen style="border: 1px solid #eee; border-radius: 6px; margin-top: 20px;"></iframe>
