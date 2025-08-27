# Comparación de Productos de Precipitación Satelital y Reanálisis

Este documento resume las características principales de cuatro productos usados ampliamente en climatología, hidrología y ciencias atmosféricas: **IMERG (GPM)**, **CHIRPS**, **ERA5** y **PERSIANN**.  
El objetivo es contar con una referencia clara y práctica para análisis comparativos y selección de datasets en estudios aplicados a Sudamérica y Chile continental.

---

## 📌 Resumen comparativo

| Producto   | Tipo de datos | Alcance temporal | Resolución espacial | Resolución temporal | Acceso | Disponible en GEE |
|------------|---------------|------------------|---------------------|---------------------|--------|-------------------|
| **IMERG (GPM)** | Satelital (microondas + infrarrojo, calibrado con pluviómetros) | 2000 – presente | ~0.1° (~10 km) | 30 min / diario / mensual | [NASA GPM](https://gpm.nasa.gov/data) | ✅ (GPM IMERG Final/ Early) |
| **CHIRPS** | Fusión satélite (infrarrojo) + pluviómetros interpolados | 1981 – presente | 0.05° (~5 km) | Diario / mensual | [Climate Hazards Center](https://www.chc.ucsb.edu/data/chirps) | ✅ (CHIRPS Daily / Monthly) |
| **ERA5** | Reanálisis atmosférico (ECMWF, modelo + asimilación de observaciones) | 1950 – presente (ERA5 back extension desde 1940) | 0.25° (~31 km) | 1 hora / diario / mensual | [Copernicus CDS](https://cds.climate.copernicus.eu/) | ✅ (ERA5 Monthly / Hourly) |
| **PERSIANN-CDR** | Satelital (infrarrojo geoestacionario, calibrado con microondas, NN) | 1983 – presente | 0.25° (~25 km) | Diario | [CHRS Data Portal](https://chrsdata.eng.uci.edu/) | ✅ (PERSIANN-CDR Daily) |

---

## 📖 Descripción breve

### 🌧️ IMERG (Integrated Multi-satellitE Retrievals for GPM)
- Basado en la misión **Global Precipitation Measurement (GPM)** de NASA-JAXA.  
- Usa microondas pasivos, infrarrojos y calibración con pluviómetros globales.  
- Ideal para precipitación extrema, tormentas convectivas y estudios de alta resolución temporal.  
- **Fortaleza:** cobertura cuasi-global con 30 min de resolución.  
- **Limitación:** menor confiabilidad en zonas montañosas (Andes).  

### 🌧️ CHIRPS (Climate Hazards Group InfraRed Precipitation with Station data)
- Combina datos de satélite infrarrojo con interpolación de estaciones terrestres.  
- Diseñado para zonas con baja densidad de pluviómetros (ej. África, Sudamérica).  
- Muy usado en **hidrología y sequías**.  
- **Fortaleza:** largo periodo (1981–presente), buena resolución espacial (5 km).  
- **Limitación:** dependencia de la calidad de estaciones locales.  

### 🌧️ ERA5 (Reanalysis v5 – ECMWF)
- Reanálisis climático global del **ECMWF**.  
- Integra observaciones satelitales, radiosondas, estaciones y datos oceánicos en un modelo numérico.  
- Disponible en múltiples variables atmosféricas y de superficie.  
- **Fortaleza:** consistente y multivariable (ideal para estudios climáticos integrales).  
- **Limitación:** puede subestimar precipitación extrema puntual.  

### 🌧️ PERSIANN-CDR (Precipitation Estimation from Remotely Sensed Information using Artificial Neural Networks – Climate Data Record)
- Algoritmo satelital con redes neuronales que usa imágenes infrarrojas geoestacionarias calibradas con microondas.  
- Disponible desde 1983, con cobertura global.  
- **Fortaleza:** continuidad temporal extensa.  
- **Limitación:** menor resolución temporal (diaria).  

---

## 🔑 Observaciones para Chile / Andes
- **IMERG:** buena para tormentas intensas en tiempo casi real, pero con sesgo en cordillera.  
- **CHIRPS:** muy útil para estudios de sequías y balance hídrico (resolución 5 km).  
- **ERA5:** robusto para estudios climáticos de largo plazo, análisis multivariable (temperatura, viento, humedad).  
- **PERSIANN:** valioso por su extensión histórica, aunque menos usado en validaciones locales recientes.  

---

## 📂 Enlaces de acceso directo
- **IMERG (NASA GPM):** https://gpm.nasa.gov/data  
- **CHIRPS (UCSB):** https://www.chc.ucsb.edu/data/chirps  
- **ERA5 (Copernicus):** https://cds.climate.copernicus.eu/  
- **PERSIANN (UCI/CHRS):** https://chrsdata.eng.uci.edu/  

---
