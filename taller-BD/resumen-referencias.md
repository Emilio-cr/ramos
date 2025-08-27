# Estado del Arte – Publicaciones sobre Precipitación y Productos Relacionados

---

## 📌 Tabla comparativa

| ID | Título resumido | Qué comparan | Elemento de referencia | Técnicas distintas a obs | PR indirecta | Resultados útiles |
|----|-----------------|--------------|------------------------|--------------------------|--------------|------------------|
| 1 | CORDEX-CORE Subtropical Chile (RCMs) | 3 RCMs (ERA-Interim, GCMs) | Gridded obs + ERA5 | Simulación climática regional | No | RCMs reproducen patrones, sesgos frío/húmedo en altura |
| 2 | SPI vs SPEI en Chile | Índices SPI (lluvia) y SPEI (lluvia+ET) | CR2MET gridded | Correlación con modos climáticos (ENSO, PDO, AAO) | Sí (ET) | Tendencias secas centro-norte, húmedas al sur; utilidad diferencial de SPI y SPEI |
| 3 | Extremos PR y temperatura en Chile | Tendencias Rx1day, Tx, Tn | Estaciones + AgERA5 (ERA5) | Análisis SST, PW, CAPE, ARs, sondeos | Sí (variables atmosféricas) | Patrones regionales de extremos PR; procesos a gran escala involucrados |
| 4 | Comparative analysis Andes (MIMERG) | MERRA-2, ERA5, CHIRPS, MSWEP, IMERG | Estaciones + ETC | Desarrollo producto combinado (MIMERG) | No | IMERG mejor en ETC; MIMERG supera a productos individuales |
| 5 | Sat. PR para sequía en Chile | CHIRPS, PERSIANN-CDR, TRMM | 278 estaciones | SPI, cluster analysis, k-means, SVD | Sí (SPI) | Sobreestimación en norte árido; mejor desempeño en centro-sur; CHIRPS usado para SPI-3 |
| 6 | Sat. PR y extremos en SESA | IMERG, PERSIANN, CCS-CDR, PDIR-NOW | Obs. SESA | Evaluación R95p, R99p, SDII | No | IMERG y CCS-CDR representan mejor extremos; limitaciones en altura y costas |
| 7 | CAMELS-CL dataset | Diferentes PR y PET integrados en dataset | Estaciones, reanálisis, satélite | Construcción dataset hidrometeorológico | Sí (PET, atributos cuenca) | Discrepancias en zonas áridas; subestimación en cabeceras; PET satelital sobreestima |
| 8 | SREs en Latinoamérica | TRMM, CHIRPS, CMORPH, PERSIANN-CDR, MSWEP | Estaciones (Brasil, Colombia, Chile) | Métricas continuas/categóricas; impacto upscaling | No | MSWEP y CHIRPS mejor en distintas cuencas; necesidad validación sitio-específica |
| 9 | DYffCast: Nowcasting con IMERG | Modelos generativos para nowcasting de PR | IMERG satelital | Framework DYffusion, nueva función de pérdida | No | Mejor desempeño en predicción 0–4h; alta estabilidad hasta 2h; código abierto disponible |
| 10 | ET en páramos andinos | Influencia de niebla y lluvia en ET | Datos meteorológicos y balance hídrico | Comparación de condiciones secas, niebla y mixtas | Sí (ET) | Niebla y lluvia reducen ET anual en 77–174 mm; importancia ecohidrológica de entradas de agua |

---

## 📌 Categorías identificadas

1. **Comparación de productos PR (datasets satelitales y reanálisis)**  
   - #4, #5, #6, #8  

2. **Modelado climático regional (RCMs/CMIP-CORDEX)**  
   - #1  

3. **Índices y proxies indirectos de PR**  
   - #2, #3, #10  

4. **Bases de datos integradas / hidrología**  
   - #7  

5. **Nowcasting y nuevas técnicas de IA aplicadas a PR**  
   - #9  

---

## 📌 Dos publicaciones clave a priorizar

- **#4. Comparative analysis Andes (MIMERG):** comparación directa de 5 productos PR + desarrollo de producto combinado → central para tu objetivo.  
- **#2. SPI vs SPEI en Chile:** incorpora precipitación + evapotranspiración → conecta con tu idea de métodos indirectos/ecohidrológicos para caracterizar precipitación.

---


# Resumen de Publicaciones Seleccionadas

## 1. Evaluation of temperature and precipitation from CORDEX-CORE South America and Eta-RCM regional climate simulations over the complex terrain of Subtropical Chile

- **Qué comparan:** Tres Modelos Climáticos Regionales (RCMs), forzados con ERA-Interim y escenarios históricos de GCMs.  
- **Elemento de referencia:** Productos gridded observacionales y reanálisis ERA5.  
- **Técnicas distintas a observaciones:** Simulaciones RCMs, comparación a distintas elevaciones.  
- **PR indirecta:** No se menciona.  
- **Resultados útiles:** Los RCMs reproducen patrones espacio-temporales principales de T y PR; sesgos fríos y húmedos en altura; se enfatiza la necesidad de más observaciones en terreno complejo.

---

## 2. Comparing SPI and SPEI to detect different precipitation and temperature regimes in Chile throughout the last four decades

- **Qué comparan:** Índices de sequía SPI (precipitación) y SPEI (precipitación + evapotranspiración).  
- **Elemento de referencia:** Dataset gridded CR2MET (5 × 5 km, 1979–2019).  
- **Técnicas distintas a observaciones:** Aplicación de índices climáticos; correlación con modos de variabilidad climática (PDO, ENSO, AAO).  
- **PR indirecta:** Sí, SPEI incorpora temperatura (evapotranspiración) además de precipitación.  
- **Resultados útiles:** Tendencias secas en norte y centro, húmedas en el sur; SPI más útil en zonas costeras, SPEI en interiores.

---

## 3. Trends in seasonal precipitation extremes and associated temperatures along continental Chile

- **Qué comparan:** Tendencias en extremos de precipitación (Rx1day) y temperaturas (Tx, Tn) durante días con precipitación.  
- **Elemento de referencia:** Estaciones de superficie y producto gridded AgERA5 (reanálisis ERA5).  
- **Técnicas distintas a observaciones:** Análisis de variables atmosféricas complementarias (SST, PW, CAPE, EKE, ARs, sondeos en altura).  
- **PR indirecta:** Sí, se relacionan variables como CAPE, PW, SST con precipitación extrema.  
- **Resultados útiles:** Tendencias regionales diferenciadas en extremos de PR y temperatura; identificación de posibles mecanismos a gran escala (SST, ARs, dinámica atmosférica).

---
## 4. Comparative analysis of gridded precipitation products and the development of a blended product in the Andes and surrounding regions

- **Qué comparan:** Cinco productos de precipitación gridded (MERRA-2, ERA5, CHIRPS, MSWEP, IMERG).  
- **Elemento de referencia:** Estaciones pluviométricas y método Extended Triple Collocation (ETC).  
- **Técnicas distintas a observaciones:** Desarrollo de un nuevo producto combinado (MIMERG) usando interpolación (algoritmo de Braseth).  
- **PR indirecta:** No se menciona.  
- **Resultados útiles:** IMERG con mejor desempeño en ETC; MERRA-2 con menor error contra estaciones; creación de MIMERG mejora desempeño respecto a productos individuales.

---

## 5. Evaluating satellite-derived long-term historical precipitation datasets for drought monitoring in Chile

- **Qué comparan:** Tres datasets satelitales históricos: TRMM TMPA 3B43 v7, PERSIANN-CDR, CHIRPS 2.0.  
- **Elemento de referencia:** 278 estaciones pluviométricas en Chile (divididas en cinco zonas latitudinales).  
- **Técnicas distintas a observaciones:** Cálculo de SPI; análisis estadístico con nueve métricas; uso de clustering jerárquico, k-means y descomposición en valores singulares.  
- **PR indirecta:** Sí, aplicación de SPI para monitoreo de sequías.  
- **Resultados útiles:** Sobreestimación en el norte árido; mejor desempeño en centro-sur; CHIRPS usado para mapear SPI-3; necesidad de calibración regional y estacional.

---

## 6. Can Satellite Products Recognise Extreme Precipitation Over Southeastern South America?

- **Qué comparan:** Productos satelitales IMERG Final Run V06, PERSIANN, PERSIANN CCS-CDR, PDIR-NOW en detección de extremos de precipitación.  
- **Elemento de referencia:** Datos observacionales en SESA (Sudeste de Sudamérica).  
- **Técnicas distintas a observaciones:** Evaluación de índices extremos: R95p, R99p, SDII; análisis de percentiles (95º y 99º).  
- **PR indirecta:** No se menciona.  
- **Resultados útiles:** IMERG y PERSIANN CCS-CDR representan mejor eventos extremos; PERSIANN y PDIR-NOW menos consistentes; IMERG con menor BIAS y RMSE en percentiles altos.

---

## 7. The CAMELS-CL dataset: catchment attributes and meteorology for large sample studies – Chile dataset

- **Qué comparan:** Diferentes productos de precipitación y PET (nacionales y globales) integrados en un dataset de 516 cuencas en Chile.  
- **Elemento de referencia:** Datos en terreno (streamflow, estaciones), productos satelitales y de reanálisis.  
- **Técnicas distintas a observaciones:** Construcción de un dataset hidrometeorológico integrado (CAMELS-CL), análisis de balances hídricos, índices hidroclimáticos.  
- **PR indirecta:** Sí, se incluye PET (dos productos) y atributos de cuencas (uso humano, topografía, geología, cobertura).  
- **Resultados útiles:** Diferencias grandes entre productos de precipitación en zonas áridas; subestimación sistemática en cabeceras húmedas; sobreestimación de PET satelital; influencia de intervenciones humanas en la respuesta hidrológica.

---

## 8. Temporal and spatial evaluation of satellite rainfall estimates over different regions in Latin-America

- **Qué comparan:** Seis productos satelitales (TRMM 3B42v7, TRMM 3B42RT, CHIRPSv2, CMORPHv1, PERSIANN-CDR, MSWEPv2).  
- **Elemento de referencia:** Estaciones pluviométricas en tres cuencas (Brasil, Colombia, Chile).  
- **Técnicas distintas a observaciones:** Evaluación con métricas continuas (RMSE, KGE’, PBIAS) y categóricas (POD, FAR, FBIAS); prueba de impacto de *upscaling* espacial.  
- **PR indirecta:** No se menciona.  
- **Resultados útiles:** Mejor desempeño de MSWEPv2 y CHIRPSv2 en distintas cuencas y escalas temporales; CMORPH y TRMM útiles en ciertas estaciones; necesidad de validación sitio-específica; el *upscaling* puede afectar desempeño.

---

## 9. Evaluation of temperature and precipitation from CORDEX-CORE South America and Eta-RCM regional climate simulations over the complex terrain of Subtropical Chile

- **Qué comparan:** Tres Modelos Climáticos Regionales (RCMs) forzados con ERA-Interim y GCMs históricos.  
- **Elemento de referencia:** Productos observacionales gridded y reanálisis ERA5.  
- **Técnicas distintas a observaciones:** Simulaciones climáticas RCM, evaluación por subregiones y elevaciones.  
- **PR indirecta:** No se menciona.  
- **Resultados útiles:** Los RCMs reproducen patrones principales de T y PR, pero muestran sesgo frío y húmedo en altura; necesidad de mejores redes de observación para calibración.
