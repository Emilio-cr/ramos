# Procedimiento Experimental: Relación Carga/Masa del Electrón

## Ajuste del haz de electrones

1. Aplique una **tensión de calefacción** de aproximadamente **7.5 V**.  
2. Ajuste la **tensión anódica** a **300 V** (el haz de electrones es inicialmente horizontal y se hace visible como una luz azul tenue).  
3. Seleccione la **tensión de Wehnelt** de manera que, en lo posible, se observe un haz de rayos delgado y nítido.  
4. Optimice la **nitidez y claridad** del haz de rayos variando la tensión de calefacción.  
5. Aumente la **corriente $I$** que circula por las bobinas de Helmholtz y compruebe si el haz de electrones se curva hacia arriba.  
   - Si **no se observa curvatura**, invierta la polaridad de una de las bobinas de modo que la corriente circule en el mismo sentido en ambas.  
   - Si la curvatura es hacia abajo, invierta la corriente de las bobinas intercambiando los cables.  
6. Si aún no se observa inversión, cambie la **polaridad de la alimentación DC de 12 V**.  
7. Ajuste la tensión de Wehnelt para que el **haz de electrones forme un círculo definido**.  
8. Optimice el diámetro del círculo variando la corriente de las bobinas.  

---

## Registro de los valores de medición

1. Seleccione la corriente de la bobina de manera que el radio de la órbita circular sea de **5 cm** y el haz de electrones quede sobre la marca correspondiente.  
2. Anote los valores de la **tensión anódica $U$** y la **corriente de la bobina $I$**.  
3. Disminuya la tensión anódica en pasos de **20 V**, hasta llegar a **200 V**.  
   - En cada paso, ajuste la corriente de la bobina para que el radio se mantenga constante.  
   - Registre los valores medidos.  
4. Repita el procedimiento para radios de órbita de **4 cm** y **3 cm**.  

---

## Ejemplo de tabla de medición

| $U$ (V) | $I$ con $r=3$ cm | $I$ con $r=4$ cm | $I$ con $r=5$ cm |
|---------|------------------|------------------|------------------|
| 300     |                  |                  |                  |
| 280     |                  |                  |                  |
| 260     |                  |                  |                  |
| 240     |                  |                  |                  |
| 220     |                  |                  |                  |
| 200     |                  |                  |                  |

---

## Evaluación

El campo magnético generado por el par de bobinas de Helmholtz es proporcional a la corriente:

$$
B = k \cdot I_b
$$

donde:

$$
k = \left( \frac{4}{5} \right)^{3/2} \cdot \frac{\mu_0 \, N}{R}
= 0.756 \, \frac{\text{mT}}{\text{A}}
$$

con:

- $R = 147.5 \, \text{mm}$ (radio de la bobina)  
- $N = 124$ (número de espiras por bobina)  
- $\mu_0 = 4 \pi \times 10^{-7} \, \text{T·m/A}$  

Con esta expresión se calculan los valores de $B$ y, junto con los datos experimentales, se determina la relación carga/masa del electrón:

$$
\frac{e}{m} = \frac{2 V}{B^2 r^2}
$$
