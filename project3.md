---
layout: default
title: "3. 4D Matrix Simulation"
nav_order: 4
---

# 4D Spatio-temporal Matrix Implementation and Simulations
{: .fs-8 }

* **Framework:** Modificación de las matrices de forzamiento solar dentro de los módulos químicos y de transferencia radiativa de CESM GCM.
* **Implementation:** Arquitectura e inserción de **matrices numéricas 4D** en el núcleo del modelo para simular la atenuación del forzamiento solar producido por un parasol en L1 con variabilidad en tiempo, latitud, longitud y longitud de onda.
* **Analytics Workflow:** Implementación de distribuciones espaciotemporales dinámicas de factores de atenuación que escalan la irradiancia solar en la cima de la atmósfera (*Top of the Atmosphere*). Análisis de respuestas climáticas multivariable a lo largo de una línea temporal de 30 años [2035, 2065].
* **Core Skills:** Modificaciones avanzadas en Fortran, generación e implementación de estructuras NetCDF y visualización 3D de alta resolución.
