# 📊 Resumen Teórico de Probabilidad

## 1. Conceptos básicos
- **Espacio muestral (\(\Omega\))**: conjunto de todos los resultados posibles.  
- **Evento (A)**: subconjunto de \(\Omega\).  
- **Probabilidad clásica**:  
\[
P(A) = \frac{\text{casos favorables}}{\text{casos posibles}}
\]
*(si todos los casos son igualmente probables).*

---

## 2. Reglas fundamentales

### 🔹 Regla del producto
Intersección de eventos:
\[
P(A \cap B) = P(A) \cdot P(B \mid A)
\]

- Si \(A, B\) son **independientes**:
\[
P(A \cap B) = P(A)\cdot P(B)
\]

---

### 🔹 Regla de la adición
Unión de eventos:
\[
P(A \cup B) = P(A) + P(B) - P(A \cap B)
\]

- Si \(A, B\) son **mutuamente excluyentes**:
\[
P(A \cup B) = P(A) + P(B)
\]

---

### 🔹 Regla del complemento
\[
P(A^c) = 1 - P(A)
\]

---

## 3. Enfoques de resolución
- **Combinatorio**: usamos combinaciones \(\binom{n}{k}\) para contar casos favorables y totales.  
- **Directo (probabilidades condicionadas)**: aplicamos la regla del producto paso a paso según el proceso.  

Ambos enfoques son equivalentes.

---

## 4. Probabilidades compuestas
- **Eventos excluyentes**: no pueden ocurrir a la vez.  
- **Eventos no excluyentes**: pueden coincidir.  
- **Eventos independientes**: el resultado de uno no afecta al otro.  
- **Eventos dependientes**: el resultado de uno modifica la probabilidad del otro.  

---

## 5. Variable de Bernoulli
Variable aleatoria con dos resultados:  

\[
X =
\begin{cases}
1 & \text{con prob. } p \\
0 & \text{con prob. } 1-p
\end{cases}
\]

- **Función de probabilidad (pmf):**  
\[
P(X=x) = p^x (1-p)^{1-x}, \quad x \in \{0,1\}
\]

- **Esperanza:**  
\[
E[X] = p
\]

- **Varianza:**  
\[
Var(X) = p(1-p)
\]

---

## 6. Distribución binomial
La suma de \(n\) Bernoullis independientes con probabilidad \(p\):

\[
X \sim Binomial(n,p)
\]

- **Función de probabilidad (pmf):**
\[
P(X=k) = \binom{n}{k} p^k (1-p)^{n-k}, \quad k=0,1,\dots,n
\]

- **Esperanza:**
\[
E[X] = np
\]

- **Varianza:**
\[
Var(X) = np(1-p)
\]

---

## 7. Función de distribución acumulada (CDF)
\[
F_X(k) = P(X \leq k) = \sum_{i=0}^k P(X=i)
\]

- Permite calcular “probabilidad de obtener **como mucho k éxitos**”.  
- Su complemento:  
\[
P(X \geq k) = 1 - F_X(k-1)
\]

---

# ✅ Conclusión
- La **regla del producto** y la **regla de la adición** son la base de los cálculos de probabilidad.  
- Hay dos enfoques equivalentes: **combinatorio** y **directo** (condicional).  
- La **variable Bernoulli** es el bloque básico; su suma genera la **binomial**.  
- El análisis de **eventos excluyentes, no excluyentes, dependientes e independientes** guía qué fórmula usar.  
- La **CDF** extiende los cálculos a rangos (*“menos de”*, *“al menos”*).

---
