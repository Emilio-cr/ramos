# Comparación de Productos de Precipitación (PR) según Clasificación

Este documento presenta una comparación de los principales productos de precipitación organizados en **cuatro categorías**:  
1. Observacionales/fusión satelital  
2. Reanálisis  
3. Modelos de pronóstico  
4. Plataformas regionales/locales  

Cada grupo se compara con criterios distintos, acordes a su naturaleza.

---

## 🌍 1. Productos Satelitales / Fusión

| Producto   | Tipo de datos | Alcance temporal | Resolución espacial | Resolución temporal | Acceso | Tiempo real | Data histórica | Disponible en GEE |
|------------|---------------|------------------|---------------------|---------------------|--------|-------------|----------------|-------------------|
| **IMERG (GPM, NASA-JAXA)** | Satélite (microondas + IR, calibrado con pluviómetros) | 2000 – presente | ~0.1° (~10 km) | 30 min / diario / mensual | [NASA GPM](https://gpm.nasa.gov/data) | ✅ (versión Early Run) | ✅ (20+ años) | ✅ |
| **CHIRPS (UCSB)** | Satélite (IR) + interpolación de pluviómetros | 1981 – presente | 0.05° (~5 km) | Diario / mensual | [CHC UCSB](https://www.chc.ucsb.edu/data/chirps) | ❌ (rezago de semanas) | ✅ (40+ años) | ✅ |
| **PERSIANN (iRain)** | Satélite IR + ANN calibrado con microondas | 2000 – presente | 0.25° (~25 km) | 1 h / diario | [iRain](https://irain.eng.uci.edu/) | ✅ (latencia ~1 h) | ❌ (sin serie climática larga) | ❌ |
| **PERSIANN-CDR** | Satélite IR + ANN (homogéneo para clima) | 1983 – presente | 0.25° (~25 km) | Diario | [CHRS Data](https://chrsdata.eng.uci.edu/) | ❌ (rezago de meses) | ✅ (40+ años) | ✅ |
| **CMORPH (NOAA)** | Satélite (microondas + IR morfología) | 1998 – presente | 0.07° (~8 km) | 30 min / diario | [NOAA CPC](https://www.cpc.ncep.noaa.gov/products/janowiak/cmorph_description.html) | ✅ (near real time) | ✅ (25+ años) | ✅ |
| **GSMaP (JAXA)** | Satélite (microondas + IR) | 2000 – presente | 0.1° (~10 km) | 1 h | [JAXA GPM](https://sharaku.eorc.jaxa.jp/GSMaP/) | ✅ (near real time) | ✅ (20+ años) | ✅ |

---

## 🌎 2. Reanálisis (Modelo + Asimilación de Observaciones)

| Producto   | Institución | Alcance temporal | Resolución espacial | Resolución temporal | Acceso | Tiempo real | Variables multiclima | Disponible en GEE |
|------------|-------------|------------------|---------------------|---------------------|--------|-------------|----------------------|-------------------|
| **ERA5** | ECMWF (Europa) | 1950 – presente (back ext. desde 1940) | 0.25° (~31 km) | 1 h / diario / mensual | [Copernicus CDS](https://cds.climate.copernicus.eu/) | ❌ (rezago ~5 días) | ✅ (atmósfera completa, superficie y océano) | ✅ |
| **MERRA-2** | NASA (EE.UU.) | 1980 – presente | 0.5° × 0.625° (~50 km) | 1 h | [NASA GES DISC](https://gmao.gsfc.nasa.gov/reanalysis/MERRA-2/) | ❌ (rezago semanas) | ✅ (énfasis en aerosoles y balance radiativo) | ❌ (no directo) |
| **JRA-55** | JMA (Japón) | 1958 – presente | ~55 km | 3 h | [JMA Reanalysis](https://jra.kishou.go.jp/JRA-55/index_en.html) | ❌ | ✅ (larga serie climática) | ❌ |

👉 **Características clave de los reanálisis:**
- Consistencia física multivariable.  
- Buenas para balances climáticos globales.  
- Limitaciones en eventos extremos locales debido a suavizado del modelo.  

---

## 🌐 3. Modelos de Pronóstico Operacional

| Modelo | Institución | Resolución | Horizonte temporal | Frecuencia de corrida | Acceso |
|--------|-------------|------------|--------------------|------------------------|--------|
| **GFS** | NOAA/NCEP (EE.UU.) | ~13 km (0–10 días), ~25 km (11–16 días) | 0–16 días | 4 veces al día | [NOAA NOMADS](https://nomads.ncep.noaa.gov/) |
| **ECMWF-HRES (IFS)** | ECMWF (Europa) | ~9 km | 0–10 días | 2 veces al día | [ECMWF](https://www.ecmwf.int/en/forecasts/datasets) |
| **ICON** | DWD (Alemania) | ~13 km | 0–7 días | 4 veces al día | [DWD ICON](https://www.dwd.de/EN/ourservices/nwp_forecast_data/nwp_forecast_data.html) |

👉 **Características clave de los modelos operacionales:**
- Diseñados para pronóstico a corto y mediano plazo.  
- Proveen salidas de precipitación junto con muchas otras variables atmosféricas.  
- No recomendados para estudios climáticos de largo plazo (para eso se usan reanálisis).  

---

## 🇨🇱 4. Plataformas Regionales / Productos Locales

Estas herramientas están diseñadas para **Chile y Sudamérica**, y no generan datasets globales nuevos, sino que **compilan, homogenizan y distribuyen** datos de precipitación a nivel regional.  

### Mawün: Explorador de Productos de Precipitaciones para Chile

- **Nombre:** Mawün: Explorador de Productos de Precipitaciones para Chile  
- **Descripción:** Mawün, cuyo nombre significa lluvia en mapudungún, es una plataforma online creada por el Observatorio de Recursos Hídricos de la Universidad de la Frontera y apoyada por el Centro de Ciencia del Clima y la Resiliencia (CR)2. Diseñada para simplificar la exploración y análisis de las Estimaciones Espacialmente Distribuidas de Precipitación (EEDP) en Chile continental, esta herramienta es especialmente útil para visualizar y analizar de manera sencilla datos de precipitación, particularmente valiosa en áreas con escasas mediciones tradicionales como la cordillera de los Andes, el Desierto de Atacama y la Patagonia.  
- **Bajada:** Comparación de productos de precipitación con observaciones (1980/98 - 2022) en Chile continental. Permite una fácil visualización y análisis preliminar de estimaciones de precipitación distribuidas espacialmente.  
- **URL:** [https://mawun.cr2.cl](https://mawun.cr2.cl)  
- **Tipo:** Análisis comparativo y herramientas especializadas  
- **Palabras claves:** Precipitación, Comparación, Productos Satelitales, CR2MET  
- **Implementada en:** 2020  
- **Investigador responsable:** *(no especificado)*  
- **Variables:** Precipitación (Pr)  
- **Tipo de dato:** Observaciones de superficie, Reanálisis, Datos satelitales  
- **Resolución:** Diaria, Mensual, Anual  
- **Periodo histórico:** Histórico, Presente, Actualización reciente  
- **Fuentes de datos:**  
  - Datos generados por CR2 (CR2)  
  - Dirección General de Aguas (DGA)  
  - Dirección Meteorológica de Chile (DMC)  
  - Climate Hazards Group InfraRed Precipitation with Station data (CHIRPS)  
  - ECMWF reanalysis (ERA5)  
  - NASA productos de precipitación grillados  
- **Organizaciones responsables:**  
  - Centro de Ciencia del Clima y la Resiliencia (CR2)  
  - Universidad de la Frontera (UFRO)  
- **Dominio geográfico:** Chile, Regiones de Chile, Cordillera de los Andes  
- **Unidades espaciales:** Datos grillados, Ubicaciones de estaciones  


### Otros ejemplos regionales
- **DataClima (CR2):** base de datos de series observadas y homogenizadas en Chile.  
- **SACA&D (South American Climate Assessment & Dataset):** recopilación de datos climáticos diarios en Sudamérica.  

---

## 📌 Resumen
- **Satelitales/fusión:** estimaciones directas desde sensores espaciales.  
- **Reanálisis:** reconstrucción atmosférica global con modelos + observaciones.  
- **Pronóstico:** predicción numérica en tiempo real, no diseñada para clima histórico.  
- **Plataformas regionales/locales:** integran y adaptan datasets globales para aplicaciones en Chile y Sudamérica (ej. Mawün).  

---
