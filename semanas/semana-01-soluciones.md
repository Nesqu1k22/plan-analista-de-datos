---
tipo: soluciones
semana: 1
---

# ✅ Soluciones — Semana 1

> ⚠️ **Intentá los ejercicios antes de mirar esto.** Mirar la solución sin haber luchado con el problema no genera aprendizaje.
>
> Lo importante no es el número final: es **el razonamiento** y, sobre todo, **la interpretación de negocio**.

---

## A — Álgebra

### A1. $3x + 12 = 5x - 8$
$$12 + 8 = 5x - 3x \Rightarrow 20 = 2x \Rightarrow \boxed{x = 10}$$

### A2. Despejar $q$ en $I = p \cdot q - CF$
$$I + CF = p \cdot q \Rightarrow \boxed{q = \frac{I + CF}{p}}$$

### A3. Punto de equilibrio
Margen de contribución por unidad: $500 - 320 = 180$

$$q = \frac{450.000}{180} = \boxed{2.500 \text{ unidades}}$$

> 💡 **Interpretación:** cada unidad vendida aporta $180 a cubrir los costos fijos. Recién a partir de la unidad 2.501 la empresa gana plata. Este es uno de los cálculos más usados en análisis comercial.

### A4. Sistema de ecuaciones
$$\begin{cases} a + b = 340 \\ 500a + 800b = 212.000 \end{cases}$$

Sustituyendo $a = 340 - b$:
$$500(340 - b) + 800b = 212.000$$
$$170.000 + 300b = 212.000 \Rightarrow b = 140$$

$$\boxed{a = 200 \text{ (producto A)},\quad b = 140 \text{ (producto B)}}$$

### A5. $\dfrac{x^5 \cdot x^{-2}}{x^{4}}$
$$\frac{x^{5-2}}{x^4} = \frac{x^3}{x^4} = x^{-1} = \boxed{\frac{1}{x}}$$

### A6. $U(q) = 180q - 450.000$
**Pendiente = 180.**

> 💡 **En lenguaje de negocio:** *"Cada unidad adicional que vendemos aumenta la utilidad en $180."*
> Eso es el **margen de contribución unitario**. La ordenada al origen (−450.000) son los costos fijos: lo que perdés si no vendés nada.

---

## B — Porcentajes ⭐

### B1. Enero → Febrero
$$\frac{1.437.500 - 1.250.000}{1.250.000} = \frac{187.500}{1.250.000} = \boxed{+15\%}$$

### B2. Febrero → Marzo
$$\frac{1.322.500 - 1.437.500}{1.437.500} = \frac{-115.000}{1.437.500} = \boxed{-8\%}$$

### B3. Acumulada enero → marzo
$$\frac{1.322.500 - 1.250.000}{1.250.000} = \boxed{+5,8\%}$$

**¿Por qué no es 15% − 8% = 7%?**

Porque los porcentajes **se multiplican, no se suman**. Cada variación se calcula sobre una base distinta:

$$1{,}15 \times 0{,}92 = 1{,}058 \Rightarrow +5{,}8\%$$

> 🔑 **Este es el concepto más importante de la semana.** Sumar porcentajes de períodos consecutivos es uno de los errores más frecuentes en reportes de negocio.

### B4. −20% y después +20%
$$1{,}00 \times 0{,}80 \times 1{,}20 = 0{,}96$$

**No.** Quedaste **4% por debajo** del valor original.

> 💡 La caída del 20% se calcula sobre 100, pero la suba del 20% se calcula sobre 80. Por eso nunca se compensan. Para volver de una caída del 20% necesitás subir 25%.

### B5. Pareto

Total: **$11.000.000**

| Producto | Ingresos | % del total | % acumulado |
|---|---:|---:|---:|
| A | 4.200.000 | 38,18% | 38,18% |
| B | 2.800.000 | 25,45% | 63,64% |
| **C** | 1.900.000 | 17,27% | **80,91%** ← |
| D | 1.100.000 | 10,00% | 90,91% |
| E | 600.000 | 5,45% | 96,36% |
| F | 400.000 | 3,64% | 100,00% |

**3 productos (A, B y C) explican el 80% de los ingresos.**

> 💡 Esto es el **principio de Pareto (80/20)** y vas a encontrarlo en todos lados: clientes, productos, regiones, causas de reclamos. Es la base del análisis ABC de inventario y de la priorización comercial.

### B6. Margen vs Markup

Ganancia: $8.500 − 5.950 = 2.550$

$$\text{Margen} = \frac{2.550}{8.500} = \boxed{30\%} \quad \text{(sobre el precio de venta)}$$

$$\text{Markup} = \frac{2.550}{5.950} = \boxed{42,86\%} \quad \text{(sobre el costo)}$$

> ⚠️ **Dan distinto porque la base es distinta.** Confundirlos es un error clásico y caro: si el dueño quiere "30% de ganancia" y vos aplicás 30% de markup sobre el costo, el margen real te da 23%. Siempre preguntá **sobre qué base** está definido el porcentaje.

### B7. Precio sin IVA
$$\frac{12.100}{1{,}21} = \boxed{\$10.000}$$

> ⚠️ **Restarle 21% da $9.559 — está mal.** El IVA se calcula *sobre el precio neto*, así que para volver atrás hay que **dividir**, no restar. Mismo principio que B4.

### B8. ¿4% → 5%?

**Los dos tienen razón, pero están diciendo cosas distintas:**

| Afirmación | Correcta | Nombre |
|---|---|---|
| "Subió 1%" | Sí, pero mal dicho | Es **1 punto porcentual** |
| "Subió 25%" | Sí | Es la **variación relativa**: $\frac{5-4}{4} = 25\%$ |

> 🔑 **Regla profesional:** cuando compares dos porcentajes, decí siempre *"subió 1 punto porcentual (+25%)"*. Es la forma inequívoca. Confundir puntos porcentuales con porcentaje es una de las manipulaciones más comunes en presentaciones.

---

## C — Logaritmos y exponenciales

### C1. $2^x = 64$
$$64 = 2^6 \Rightarrow \boxed{x = 6}$$

### C2.
$$\log_{10}(1000) = \boxed{3} \qquad \ln(e^3) = \boxed{3}$$

### C3. $\log(50 \cdot 4) - \log(2)$
$$\log(200) - \log(2) = \log\left(\frac{200}{2}\right) = \log(100) = \boxed{2}$$

### C4. Duplicación al 3% mensual

$$1{,}03^n = 2 \Rightarrow n = \frac{\ln 2}{\ln 1{,}03} = \frac{0{,}6931}{0{,}02956} = \boxed{23,4 \text{ meses}}$$

**Regla del 72:** $72 / 3 = 24$ meses.

> 💡 La regla del 72 es una aproximación mental muy buena (se equivoca en menos de un mes acá). Sirve para hacer cuentas rápidas en una reunión sin calculadora.

### C5. Escala lineal vs logarítmica

| Escala | Forma |
|---|---|
| **Lineal** | Curva que se dispara hacia arriba (exponencial) |
| **Logarítmica** | **Línea recta** |

**Por qué:** la serie duplica en cada paso (×2 constante). El logaritmo convierte multiplicación en suma, así que un crecimiento porcentual constante se ve como una recta.

> 🔑 **Utilidad práctica:** en escala log, **la pendiente es la tasa de crecimiento**. Si dos series son paralelas, crecen al mismo ritmo aunque una esté 100 veces más arriba. Por eso se usa para comparar crecimiento de empresas de tamaños muy distintos, o curvas epidémicas.

---

## D — Métricas de negocio

### D1. CAGR
$$CAGR = \left(\frac{180.000}{100.000}\right)^{\frac{1}{4}} - 1 = 1{,}8^{0{,}25} - 1 = \boxed{15,83\%}$$

**Verificación:** $100.000 \times 1{,}1583^4 = 180.000$ ✓

### D2. +30%, −10%, +20%

**Crecimiento total:**
$$1{,}30 \times 0{,}90 \times 1{,}20 = 1{,}404 \Rightarrow \boxed{+40,4\%}$$

**CAGR:**
$$1{,}404^{\frac{1}{3}} - 1 = \boxed{11,98\%}$$

**¿Por qué no es el promedio simple (13,3%)?**

Porque el crecimiento es **multiplicativo**. El promedio aritmético de tasas de crecimiento **siempre sobreestima** el crecimiento real (desigualdad entre media aritmética y geométrica). Cuanto más volátiles las tasas, mayor la sobreestimación.

Comprobalo: $1{,}133^3 = 1{,}455 \neq 1{,}404$. El promedio simple te haría reportar un crecimiento que no existió.

> 🔑 **Para tasas de crecimiento siempre usá media geométrica (CAGR), nunca media aritmética.**

### D3. Run rate
$$2.400.000 \times 4 = \boxed{\$9.600.000}$$

**Por qué puede ser engañoso:**

1. **Estacionalidad.** Si el Q1 incluye una temporada alta (o baja), extrapolarlo distorsiona todo. Un negocio de indumentaria o turismo tiene trimestres radicalmente distintos.
2. **Operaciones excepcionales.** Un contrato grande y único, una promoción agresiva o un cliente que se va inflan o deprimen el trimestre y no se repiten.

> *(Otras válidas: cambios de precio previstos, inflación, capacidad limitada, ramp-up de un producto nuevo.)*

### D4. Márgenes

$$\text{Margen bruto} = \frac{8.500 - 5.950}{8.500} = \frac{2.550}{8.500} = \boxed{30\%}$$

$$\text{Margen neto} = \frac{8.500 - 5.950 - 1.200}{8.500} = \frac{1.350}{8.500} = \boxed{15,88\%}$$

> 💡 La diferencia entre bruto y neto es donde se esconden los problemas de rentabilidad. Un negocio puede tener margen bruto excelente y estar perdiendo plata por gastos operativos.

---

## 🎯 Los 5 conceptos que te tenés que llevar

1. **Los porcentajes se multiplican, no se suman** (B3, B4)
2. **Margen ≠ Markup** — siempre preguntá sobre qué base (B6)
3. **Puntos porcentuales ≠ porcentaje** (B8)
4. **CAGR ≠ promedio de crecimientos** (D2)
5. **Escala log = crecimiento porcentual constante se ve recto** (C5)

Si estos cinco te quedaron claros, la semana fue un éxito.
