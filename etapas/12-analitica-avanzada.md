---
etapa: 12
titulo: Analítica avanzada
duracion: 4-6 semanas
estado: pendiente
---

# 🟫 Etapa 12 — Analítica avanzada

⏱️ **4–6 semanas** · [[../progreso|← Progreso]]

> Una vez dominadas las bases, avanzá hacia regresión y forecasting.

---

## 📐 Linear Regression

$$ Y = \beta_0 + \beta_1 X + \epsilon $$

Comprender:

- [ ] **Coeficientes** — "por cada unidad extra de X, Y cambia en β₁, *manteniendo todo lo demás constante*"
- [ ] **R²** — proporción de varianza explicada (y por qué un R² alto no significa buen modelo)
- [ ] **Residuales** — el diagnóstico real del modelo
- [ ] **Significancia** — p-value de cada coeficiente
- [ ] **Supuestos**:
  - Linealidad
  - Independencia de errores
  - Homocedasticidad
  - Normalidad de residuos
  - Ausencia de multicolinealidad
- [ ] Regresión múltiple
- [ ] Variables dummy / one-hot

⚠️ Un coeficiente de regresión **no es una relación causal** salvo que el diseño lo garantice.

---

## 🎯 Logistic Regression

Para problemas de clasificación binaria como:

> ¿Este cliente va a abandonar?

- [ ] Función logística / sigmoide
- [ ] Odds y odds ratio
- [ ] Interpretación de coeficientes (en log-odds)
- [ ] Umbral de decisión (y por qué 0.5 casi nunca es el correcto)
- [ ] Matriz de confusión

---

## 🔮 Forecasting

Introducción a:

- [ ] Series temporales
- [ ] **Trend**
- [ ] **Seasonality**
- [ ] Ciclo vs estacionalidad
- [ ] Descomposición (aditiva vs multiplicativa)
- [ ] Moving averages
- [ ] Exponential smoothing (SES, Holt, Holt-Winters)
- [ ] ARIMA / SARIMA
- [ ] Estacionariedad y diferenciación
- [ ] Forecast intervals

**Ejemplo:** Predecir las ventas de los próximos seis meses.

### Validación en series temporales
⚠️ **Nunca hagas un train/test split aleatorio en series temporales.** Usá split cronológico o walk-forward validation — si no, estás entrenando con el futuro.

### Métricas
- MAE, RMSE, **MAPE** (la que entiende el negocio)
- Baseline obligatorio: *naive forecast* (el valor de ayer / del mismo mes del año pasado). **Si tu modelo no le gana al baseline, no sirve.**

---

## ✅ Criterio de dominio

1. Ajustá una regresión y explicá cada coeficiente **en lenguaje de negocio**.
2. Tu R² es 0.92 pero los residuos tienen forma de embudo. ¿Qué está pasando y qué hacés?
3. Descomponé una serie de ventas en trend + estacionalidad + residuo.
4. Generá un forecast a 6 meses **con intervalo de predicción** y compará contra el naive.
5. ¿Por qué un intervalo de predicción es mucho más ancho que un intervalo de confianza?
