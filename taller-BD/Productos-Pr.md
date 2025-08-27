# Comparación de Productos de Precipitación Satelital y Reanálisis

Este documento resume las características principales de cuatro productos usados ampliamente en climatología, hidrología y ciencias atmosféricas: **IMERG (GPM)**, **CHIRPS**, **ERA5** y **PERSIANN**.  
El objetivo es contar con una referencia clara y práctica para análisis comparativos y selección de datasets en estudios aplicados a Sudamérica y Chile continental.

---

## 📌 Resumen comparativo

| Producto   | Tipo de datos | Alcance temporal | Resolución espacial | Resolución temporal | Acceso | Gestor de precipitación actual | Data histórica de Pr | Disponible en GEE |
|------------|---------------|------------------|---------------------|---------------------|--------|-------------------------------|----------------------|-------------------|
| **IMERG (GPM)** | Satelital (microondas + infrarrojo, calibrado con pluviómetros) | 2000 – presente | ~0.1° (~10 km) | 30 min / diario / mensual | [NASA GPM](https://gpm.nasa.gov/data) | ✅ (versión *Early Run* disponible a pocas horas) | ✅ (20+ años) | ✅ (IMERG Early/Final) |
| **CHIRPS** | Fusión satélite (infrarrojo) + pluviómetros interpolados | 1981 – presente | 0.05° (~5 km) | Diario / mensual | [Climate Hazards Center](https://www.chc.ucsb.edu/data/chirps) | ❌ (no en tiempo real, con rezago de semanas) | ✅ (40+ años) | ✅ (CHIRPS Daily/Monthly) |
| **ERA5** | Reanálisis atmosférico (ECMWF, modelo + asimilación de observaciones) | 1950 – presente (back extension desde 1940) | 0.25° (~31 km) | 1 hora / diario / mensual | [Copernicus CDS](https://cds.climate.copernicus.eu/) | ✅ (se actualiza con rezago ~5 días) | ✅ (70+ años) | ✅ (ERA5 Monthly/Hourly) |
| **PERSIANN-CDR** | Satelital (infrarrojo geoestacionario, calibrado con microondas, ANN) | 1983 – presente | 0.25° (~25 km) | Diario | [CHRS Data Portal](https://chrsdata.eng.uci.edu/) | ❌ (no en tiempo real, se actualiza con meses de rezago) | ✅ (40+ años) | ✅ (PERSIANN-CDR Daily) |

---

## 📖 Descripción breve

### 🌧️ IMERG (Integrated Multi-satellitE Retrievals for GPM)
- Basado en la misión **Global Precipitation Measurement (GPM)** de NASA-JAXA.  
- Usa microondas pasivos, infrarrojos y calibración con pluviómetros globales.  
- Ofrece tres versiones: *Early* (casi tiempo real), *Late* (corregida), *Final* (con calibración completa).  

### 🌧️ CHIRPS (Climate Hazards Group InfraRed Precipitation with Station data)
- Combina datos de satélite infrarrojo con interpolación de estaciones terrestres.  
- Diseñado para zonas con baja densidad de pluviómetros.  
- Ideal para análisis de sequías y agricultura.  

### 🌧️ ERA5 (Reanalysis v5 – ECMWF)
- Reanálisis climático global del **ECMWF**.  
- Integra observaciones satelitales, radiosondas, estaciones y datos oceánicos en un modelo numérico.  
- Entrega múltiples variables (no solo precipitación).  

### 🌧️ PERSIANN-CDR
- Algoritmo satelital con redes neuronales que usa imágenes infrarrojas geoestacionarias.  
- Focalizado en generar un **registro climático homogéneo** desde 1983.  
- Muy útil para estudios de tendencias a largo plazo.  

---

## 🔑 Observaciones para Chile / Andes
- **IMERG:** buena para tormentas intensas en tiempo casi real, pero con sesgo en cordillera.  
- **CHIRPS:** muy útil para estudios de sequías y balance hídrico (resolución 5 km, larga serie).  
- **ERA5:** robusto para estudios climáticos de largo plazo, análisis multivariable.  
- **PERSIANN:** valioso por su extensión histórica, aunque menos usado en validaciones locales recientes.  

---

## 📂 Enlaces de acceso directo
- **IMERG (NASA GPM):** https://gpm.nasa.gov/data  
- **CHIRPS (UCSB):** https://www.chc.ucsb.edu/data/chirps  
- **ERA5 (Copernicus):** https://cds.climate.copernicus.eu/  
- **PERSIANN (UCI/CHRS):** https://chrsdata.eng.uci.edu/  

---
