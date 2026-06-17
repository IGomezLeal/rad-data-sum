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

## 🔬 Project Overview

Technical summary focused on multi-terabyte data architecture, computational physics, and advanced climate engineering simulations within the **Community Earth System Model** (CESM GCM) framework.
{: .note }

This repository serves as a technical showcase of my research at **Cornell University**, focusing on large-scale data architecture and numerical modifications within the **CESM GCM** framework. The core objective is to simulate the spectral and bolometric impacts of space-based solar radiation management (SRM) strategies.

> **HPC Infrastructure:** All simulations and data pipelines were architected and executed on the [**NCAR Derecho**](https://www.cisl.ucar.edu/capabilities/derecho){:target="_blank"} High-Performance Computing (HPC) cluster, utilizing [**NetCDF4**](https://docs.unidata.ucar.edu/netcdf-c/current/){:target="_blank"} standards for high-throughput I/O of **60 TB+** datasets.
{: .block-tip }

### 📁 Data Standards: Why NetCDF?

The projects in this repository utilize **NetCDF (Network Common Data Form)**, the industry standard for array-oriented scientific data:

* **Multidimensional:** Almacenamiento de variables (temperatura, presión, irradiancia) en coordenadas espacio-temporales 4D ($x, y, z, t$).
* **Self-Describing:** Cada archivo incluye metadatos (unidades, coordenadas), asegurando la integridad de los datos.
* **Performance:** Optimizado para lectura/escritura paralela a gran escala en el supercomputador **NCAR Derecho**, facilitando el manejo de datasets de **60 TB+**.

---

## 🚀 GCM Numerical Implementations & Core Projects

### 1. Bolometric Dimming and Climatic Response produced by a space-based Sunshade
* **Framework:** CESM GCM con el Community Atmospheric Model (CAM).
* **Implementation:** Parametrización en código de reducciones uniformes y no espectrales de la constante solar (bolometric dimming).
* **Data Architecture:** Optimización del pipeline de E/S en Fortran de bajo nivel para ingerir parámetros NetCDF4 directamente en el núcleo del GCM.

<iframe src="https://drive.google.com/file/d/1DHWkINHpbSsCgRyBI2aMFD9SVofIwm5_/preview" width="100%" height="480" allowfullscreen style="border: 1px solid #eee; border-radius: 6px; margin: 20px 0;"></iframe>

### 2. Filter Analysis, Spectral Dimming and Climatic Response produced by a space-based Sunshade
* **Framework:** CESM con el Whole Atmosphere Community Climate Model (WACCM).
* **Implementation:** Integración numérica del efecto de atenuación de un filtro espectral en el punto de Lagrange L1 dentro del núcleo de transferencia radiativa.
* **Analytics Workflow:** Diagnósticos de anomalías climáticas multidimensionales bajo el escenario futuro **SSP2-4.5**.

<iframe src="https://drive.google.com/file/d/1sqeUj7riu_lpyHYPxMysEleNBYZb2ZbS/preview" width="100%" height="480" allowfullscreen style="border: 1px solid #eee; border-radius: 6px; margin: 20px 0;"></iframe>

### 3. 4D Spatio-temporal Matrix Implementation and Simulations
* **Framework:** Modificación de las matrices de forzamiento solar dentro de los módulos químicos y de transferencia radiativa de CESM GCM.
* **Implementation:** Inserción de **matrices numéricas 4D** para simular la variabilidad en tiempo, latitud, longitud y longitud de onda del apantallamiento solar.
* **Timeline:** Análisis de respuestas climáticas a largo plazo en una línea temporal de 30 años [2035, 2055].

---

📝 **Note:** This repository showcases specific technical implementations in **HPC and Climate Analytics**.  
🔒 **Privacy Note:** Full source code and configuration files are hosted in private repositories. Specific code samples are available upon request.
{: .fs-2 .text-grey-dk-000 }
