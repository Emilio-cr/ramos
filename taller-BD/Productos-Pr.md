# Comparación de Productos de Precipitación Satelital y Reanálisis

Este documento resume las características principales de cuatro productos usados ampliamente en climatología, hidrología y ciencias atmosféricas: **IMERG (GPM)**, **CHIRPS**, **ERA5** y la familia **PERSIANN** (incluyendo sus variantes en tiempo real e histórico).  
El objetivo es contar con una referencia clara y práctica para análisis comparativos y selección de datasets en estudios aplicados a Sudamérica y Chile continental.

---

## 📌 Resumen comparativo

| Producto   | Tipo de datos | Alcance temporal | Resolución espacial | Resolución temporal | Acceso | Gestor de precipitación actual | Data histórica de Pr | Disponible en GEE |
|------------|---------------|------------------|---------------------|---------------------|--------|-------------------------------|----------------------|-------------------|
| **IMERG (GPM)** | Satelital (microondas + infrarrojo, calibrado con pluviómetros) | 2000 – presente | ~0.1° (~10 km) | 30 min / diario / mensual | [NASA GPM](https://gpm.nasa.gov/data) | ✅ (versión *Early Run* disponible a pocas horas) | ✅ (20+ años) | ✅ (IMERG Early/Final) |
| **CHIRPS** | Fusión satélite (infrarrojo) + pluviómetros interpolados | 1981 – presente | 0.05° (~5 km) | Diario / mensual | [Climate Hazards Center](https://www.chc.ucsb.edu/data/chirps) | ❌ (no en tiempo real, con rezago de semanas) | ✅ (40+ años) | ✅ (CHIRPS Daily/Monthly) |
| **ERA5** | Reanálisis atmosférico (ECMWF, modelo + asimilación de observaciones) | 1950 – presente (back extension desde 1940) | 0.25° (~31 km) | 1 hora / diario / mensual | [Copernicus CDS](https://cds.climate.copernicus.eu/) | ✅ (se actualiza con rezago ~5 días) | ✅ (70+ años) | ✅ (ERA5 Monthly/Hourly) |
| **PERSIANN (iRain)** | Satelital (infrarrojo + ANN, calibrado con microondas) | 2000 – presente | 0.25° (~25 km) | 1 h / diario | [iRain](https://irain.eng.uci.edu/) | ✅ (tiempo real, latencia ~1 h) | ❌ (no tiene serie climática larga) | ❌ (no en GEE) |
| **PERSIANN-CDR** | Satelital (infrarrojo geoestacionario, ANN calibrado) | 1983 – presente | 0.25° (~25 km) | Diario | [CHRS Data Portal](https://chrsdata.eng.uci.edu/) | ❌ (no en tiempo real, actualiza con meses de rezago) | ✅ (40+ años) | ✅ (PERSIANN-CDR Daily) |

---

## 📖 Descripción breve

### 🌧️ IMERG (Integrated Multi-satellitE Retrievals for GPM)
- Basado en la misión **GPM (NASA-JAXA)**.  
- Tres versiones: *Early* (tiempo casi real), *Late* (ajustada), *Final* (reprocesada con calibración completa).  

### 🌧️ CHIRPS (Climate Hazards Group InfraRed Precipitation with Station data)
- Combina satélite infrarrojo con estaciones locales interpoladas.  
- Diseñado para zonas con baja densidad de pluviómetros (ej. África, Sudamérica).  
- Útil para sequías y agricultura.  

### 🌧️ ERA5 (Reanalysis v5 – ECMWF)
- Reanálisis climático global del **ECMWF**.  
- Integra observaciones diversas en un modelo atmosférico.  
- Ofrece múltiples variables además de precipitación.  

### 🌧️ PERSIANN
- **PERSIANN (iRain):** versión en **tiempo real** (resolución horaria, latencia ~1h). Ideal para monitoreo de eventos actuales.  
- **PERSIANN-CDR:** versión **climática histórica** (1983–presente, diaria, homogénea). Ideal para estudios de tendencias y balance hídrico.  

---

## 🔑 Observaciones para Chile / Andes
- **IMERG:** útil para monitoreo de tormentas y eventos intensos, pero con sesgo en cordillera.  
- **CHIRPS:** buena cobertura histórica y espacial, valiosa en sequías.  
- **ERA5:** robusto para análisis climáticos multivariables de largo plazo.  
- **PERSIANN (iRain):** opción para monitoreo en tiempo real.  
- **PERSIANN-CDR:** opción para análisis climático e hidrológico de largo plazo.  

---

## 📂 Enlaces de acceso directo
- **IMERG (NASA GPM):** https://gpm.nasa.gov/data  
- **CHIRPS (UCSB):** https://www.chc.ucsb.edu/data/chirps  
- **ERA5 (Copernicus):** https://cds.climate.copernicus.eu/  
- **PERSIANN (iRain – tiempo real):** https://irain.eng.uci.edu/  
- **PERSIANN-CDR (histórico):** https://chrsdata.eng.uci.edu/  

---
