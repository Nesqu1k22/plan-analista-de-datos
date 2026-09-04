---
etapa: 3
titulo: Estadística y probabilidad
duracion: 6-8 semanas
estado: pendiente
---

# 🟥 Etapa 3 — Estadística

⏱️ **6–8 semanas** · [[../progreso|← Progreso]]

> Esta es probablemente **la parte más importante conceptualmente**.
> Un analista que sabe SQL pero no entiende estadística puede producir conclusiones completamente equivocadas.

---

## 📐 Estadística descriptiva

### Medidas de tendencia central
- [ ] Media
- [ ] Mediana
- [ ] Moda
- [ ] *Cuándo la media miente (distribuciones asimétricas, outliers)*

### Medidas de dispersión
- [ ] Rango
- [ ] Varianza
- [ ] Desviación estándar
- [ ] Coeficiente de variación
- [ ] Percentiles
- [ ] Cuartiles
- [ ] IQR

---

## 📉 Distribuciones

- [ ] Normal
- [ ] Uniforme
- [ ] Binomial
- [ ] Poisson
- [ ] Exponencial

> No solamente memorizar sus fórmulas. **Tenés que entender cuándo aparecen y qué representan.**

| Distribución | Aparece cuando... |
|---|---|
| Normal | Suma de muchos efectos pequeños (alturas, errores) |
| Binomial | Cuentas de éxitos en n intentos (conversiones) |
| Poisson | Eventos raros por unidad de tiempo (visitas/hora, fallas) |
| Exponencial | Tiempo entre eventos (tiempo hasta la próxima compra) |
| Uniforme | Todos los resultados igual de probables |

---

## 🎲 Probabilidad

- [ ] Experimentos aleatorios
- [ ] Eventos
- [ ] Probabilidad condicional
- [ ] Independencia
- [ ] Teorema de Bayes
- [ ] Variables aleatorias
- [ ] Esperanza
- [ ] Varianza

**Ejemplo:** Si un cliente compra A, ¿qué probabilidad existe de que también compre B?

$$ P(B|A) = \frac{P(A \cap B)}{P(A)} $$

> Eso lleva directamente al análisis de comportamiento de clientes (market basket analysis).

---

## 📊 Inferencia estadística

> Acá empieza el análisis profesional.

- [ ] Muestreo
- [ ] Población
- [ ] Muestra
- [ ] Sesgo
- [ ] Representatividad
- [ ] Error de muestreo
- [ ] Distribuciones muestrales
- [ ] Media muestral
- [ ] Teorema Central del Límite
- [ ] Intervalos de confianza

**Ejemplo:**
> "El promedio estimado es $52.000, con un IC 95% de $49.000–$55.000."

Tenés que saber **qué significa realmente** ese intervalo.
(Pista: *no* significa "hay 95% de probabilidad de que la media esté ahí".)

---

## 🧪 Tests de hipótesis

- [ ] Hipótesis nula ($H_0$)
- [ ] Hipótesis alternativa ($H_1$)
- [ ] p-value
- [ ] Nivel de significancia ($\alpha$)
- [ ] Error tipo I (falso positivo)
- [ ] Error tipo II (falso negativo)
- [ ] Poder estadístico

### Tests
- [ ] t-test
- [ ] chi-square
- [ ] ANOVA
- [ ] Mann-Whitney
- [ ] Wilcoxon

| Test | Usalo cuando |
|---|---|
| t-test | Comparar medias de 2 grupos, datos ~normales |
| ANOVA | Comparar medias de 3+ grupos |
| Chi-square | Asociación entre 2 variables categóricas |
| Mann-Whitney | Como t-test pero sin supuesto de normalidad |
| Wilcoxon | Como Mann-Whitney pero con muestras apareadas |

---

## 🧬 A/B Testing

> Fundamental para productos digitales.

- [ ] Control
- [ ] Tratamiento
- [ ] Randomización
- [ ] Métrica primaria
- [ ] Significancia
- [ ] Power
- [ ] Sample size
- [ ] Multiple testing
- [ ] Efecto mínimo detectable (MDE)

**Ejemplo:**
Landing A convierte 8,1% · Landing B convierte 8,8%

No podés simplemente decir **"B es mejor"**.

Tenés que determinar:
1. Si la diferencia es **estadísticamente significativa**
2. Si además es **prácticamente relevante**

---

## ✅ Criterio de dominio

1. Explicá qué es un p-value **sin usar la palabra "probabilidad de que la hipótesis sea verdadera"**.
2. Un test dio p = 0.03 con n = 2.000.000. ¿Deberías actuar? ¿Por qué el tamaño de muestra cambia la conversación?
3. Corriste 20 tests A/B y uno dio significativo al 5%. ¿Qué problema tenés?
4. ¿Por qué el intervalo de confianza suele ser más útil que el p-value para el negocio?
5. Diseñá un A/B test: métrica primaria, MDE, sample size necesario, duración.
