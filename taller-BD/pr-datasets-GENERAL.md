# Clasificación de Productos de Precipitación: Satelitales, Reanálisis y Pronóstico

Este documento presenta una clasificación general de los principales productos de precipitación usados en meteorología, hidrología y climatología.  
La organización se divide en **tres categorías principales** según su origen y metodología: **observacionales/fusión satelital**, **reanálisis**, y **modelos de pronóstico**.

---

## 🌍 1. Observacionales / Satelitales / Fusión
- Basados en **sensores satelitales** (infrarrojo, microondas).  
- En algunos casos incluyen **ajuste con pluviómetros**.  
- Representan estimaciones directas de precipitación observada o fusionada.  
- **Ventajas:** buena resolución espacial y temporal, útiles para monitoreo.  
- **Limitaciones:** sesgos en regiones montañosas o con baja cobertura de estaciones.  

**Ejemplos relevantes:**
- **IMERG (GPM, NASA-JAXA)**  
- **CHIRPS (UCSB)**  
- **PERSIANN (iRain, CDR, CHRS-UCI)**  
- **CMORPH (NOAA)**  
- **GSMaP (JAXA)**  
- **TRMM (NASA-JAXA, misión previa a GPM)**  
- **MSWEP (fusión multi-fuente: satélite + reanálisis + estaciones)**  

---

## 🌎 2. Reanálisis (Modelo + Asimilación de Datos)
- Generados a partir de un **modelo numérico atmosférico global**.  
- Incorporan millones de observaciones (satelitales, estaciones, radiosondas, boyas) mediante **asimilación de datos**.  
- Proporcionan un campo atmosférico **consistente en espacio y tiempo**.  
- **Ventajas:** multivariables, coherencia física, series largas.  
- **Limitaciones:** pueden suavizar eventos extremos locales.  

**Ejemplos relevantes:**
- **ERA5 (ECMWF)**  
- **MERRA-2 (NASA)**  
- **JRA-55 (JMA, Japón)**  
- **NCEP/NCAR Reanalysis**  
- **CFSR / CFSv2 (NOAA)**  
- **20CR (NOAA/CIRES, siglo XX)**  

---

## 🌐 3. Modelos de Pronóstico Operacional
- **Modelos numéricos globales** que entregan pronósticos meteorológicos en tiempo real.  
- No incluyen correcciones retrospectivas (no son reanálisis).  
- Diseñados para **predicciones a corto y mediano plazo** (días-semanas).  
- **Ventajas:** información inmediata y operativa.  
- **Limitaciones:** no son datasets climáticos; su calidad depende de la física del modelo.  

**Ejemplos relevantes:**
- **GFS (NOAA/NCEP, EE.UU.)**  
- **ECMWF-HRES (IFS, Europa)**  
- **ICON (DWD, Alemania)**  
- **UKMO (Met Office, Reino Unido)**  

---

## 📌 Resumen visual
- **Observacionales / fusión satelital** → lo que *vemos* desde satélites + estaciones.  
- **Reanálisis** → lo que *reconstruimos* con modelos + observaciones.  
- **Pronóstico** → lo que *proyectamos* con modelos a futuro.

---
