# Marco Teórico – Radiación Térmica

## 1. Modelo General de Radiación Térmica

La radiación térmica es la energía emitida por un cuerpo debido a su temperatura.  
Todo cuerpo cuya temperatura sea mayor al cero absoluto emite radiación electromagnética en un espectro continuo.  

Los principios fundamentales son:

- **Ley de Stefan–Boltzmann**  
  La potencia radiante total por unidad de área de un cuerpo negro es proporcional a la cuarta potencia de su temperatura absoluta:

  $$Rad = \sigma T^4$$

  donde:  
  - $Rad$ : potencia radiada por unidad de área \([W/m^2]\)  
  - $T$ : temperatura absoluta \([K]\)  
  - $\sigma = 5.6703 \times 10^{-8}\ [W\,m^{-2}\,K^{-4}]$ es la constante de Stefan–Boltzmann  

- **Ley del cuadrado inverso**  
  La intensidad radiante de una fuente puntual se distribuye sobre superficies esféricas concéntricas, por lo que la energía por unidad de área disminuye con el cuadrado de la distancia $r$:

  $$Rad(r) \propto \frac{1}{r^2}$$

Estas leyes constituyen la base del experimento, aplicadas a un **filamento de tungsteno** (ampolleta incandescente), que se comporta aproximadamente como un cuerpo negro.

---

## 2. Primera Parte – Ley de Stefan–Boltzmann

### Fundamentos Teóricos

- El filamento de tungsteno se calienta por efecto Joule al circular corriente eléctrica.  
- Su **temperatura** no se mide directamente, sino a través de su **resistencia eléctrica**, utilizando la relación entre la resistividad del tungsteno y la temperatura.  
- La resistencia del filamento se calcula como:

  $$R = \frac{V}{I}$$

  donde $V$ es la diferencia de potencial aplicada e $I$ la corriente.  

- Conociendo $R$ y la resistencia de referencia $R_{ref}$ a temperatura ambiente $T_{ref}$, se determina la temperatura del filamento a partir de tablas de calibración de tungsteno.  

- Una vez obtenida la temperatura, se aplica la ley de Stefan–Boltzmann:  

  $$Rad \propto T^4$$

### Aplicación Experimental

- Se mide la potencia radiada relativa $Rad$ (lectura de la termopila en mV) para distintos voltajes.  
- Se calcula $T$ a partir de $R$ y $R_{ref}$.  
- Se construye el gráfico **$Rad$ vs $T^4$**, que debe mostrar una relación lineal.

---

## 3. Segunda Parte – Ley del Inverso Cuadrático

### Fundamentos Teóricos

- La radiación emitida por el filamento se propaga en el espacio.  
- Si se considera al filamento como una fuente puntual, la intensidad radiada disminuye con el cuadrado de la distancia $x$ al sensor:

  $$Rad(x) \propto \frac{1}{x^2}$$

- Esta relación se deduce porque la energía total se distribuye sobre una superficie esférica de radio $x$ y área $A = 4 \pi x^2$.  

### Aplicación Experimental

- Se mantiene fija la ampolleta y se desplaza el sensor a distintas distancias $x$.  
- Se mide la radiación $Rad(x)$ en cada posición.  
- Se compara el gráfico de $Rad$ vs $x$ y $Rad$ vs $1/x^2$, siendo este último el que debería mostrar un comportamiento lineal.  

---

## 4. Consideraciones Finales

- El filamento de tungsteno **no es un cuerpo negro ideal**, por lo que pueden existir desviaciones respecto a la ley de Stefan–Boltzmann.  
- Fuentes térmicas externas y el ambiente influyen en las mediciones, generando un **ruido de radiación ambiental** que debe corregirse.  
- La ampolleta no es estrictamente una **fuente puntual**, lo que puede explicar pequeñas desviaciones respecto a la ley del inverso cuadrático.  
