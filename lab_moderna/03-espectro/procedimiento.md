# Procedimiento Experimental  
## Experimento 03: Análisis Espectral

El experimento se divide en dos partes: **uso del espectrómetro convencional** y **uso del espectrómetro computarizado (PASCO)**.  

---

### 1. Espectrómetro Convencional
1. Verificar que la **red de difracción** esté montada perpendicular al haz de luz de la lámpara de descarga.  
2. Ajustar el espectroscopio para determinar la posición del **máximo central (orden cero)**.  
3. Para el **primer orden ($n=1$)**:  
   - Medir los ángulos $\theta_{\text{izq}}$ y $\theta_{\text{der}}$ respecto al orden cero.  
   - Calcular el valor promedio:  
     $$ \theta_{\text{prom}} = \frac{\theta_{\text{izq}} + \theta_{\text{der}}}{2} $$
4. Repetir el procedimiento para el **segundo orden ($n=2$)** si las líneas espectrales son visibles.  
5. Usar la ecuación de difracción para calcular la longitud de onda:  
   $$ \lambda = \frac{d \, \sin \theta}{n} $$
6. Registrar resultados en una tabla con las columnas:  
   **Orden – Ángulo Izq – Ángulo Der – Ángulo Prom – Longitud de Onda – Color**.  
7. Comparar los valores experimentales de $\lambda$ con valores de referencia en la literatura.

---

### 2. Espectrómetro Computarizado (PASCO)
1. Conectar el **sensor de movimiento rotatorio** y el **sensor de luz de alta sensibilidad** al sistema PASCO.  
2. Calibrar el sensor de ángulo:  
   - Girar el brazo del espectrómetro 180°.  
   - Verificar que el sistema dé un factor de corrección cercano a 30 (relación 60:1).  
3. Activar el software de adquisición de datos:  
   - Configurar registro de **ángulo vs intensidad**.  
   - Presionar “tare” para fijar el cero antes de medir.  
4. Barrer lentamente con el brazo del espectrómetro para registrar el espectro completo de **primer orden** a ambos lados del orden cero.  
5. Identificar en el software los **máximos de intensidad** correspondientes a cada línea espectral.  
6. Calcular las longitudes de onda con la relación:  
   $$ \lambda = \frac{d \, \sin \theta}{n} $$  
   (donde $n=1$ para el primer orden).  
7. Comparar con tablas de referencia y con los resultados obtenidos en el espectrómetro convencional.

---

### 3. Análisis y Comparación
- Contrastar las longitudes de onda medidas con valores de la literatura.  
- Analizar posibles fuentes de error: alineación de la red, precisión en lectura de ángulos, sensibilidad del detector.  
- Discusión sobre diferencias entre **observación directa** y **detección computarizada**.  

---
