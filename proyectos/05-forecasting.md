---
proyecto: 5
titulo: Forecasting
stack: Python + Power BI
estado: pendiente
---

# 🔮 Proyecto 5 — Forecasting

**Stack:** Python + Power BI

---

## 🎯 Pregunta de negocio

> ¿Cuánto vamos a vender en los próximos 6 meses y con qué nivel de incertidumbre?

---

## 🔁 Pipeline

```
Raw Data
   ↓
Cleaning
   ↓
EDA
   ↓
Time Series
   ↓
Forecast
   ↓
Dashboard
```

---

## 🔧 Pasos

### 1. Raw Data
- [ ] Serie de ventas con al menos 3 años (para captar estacionalidad)
- [ ] Frecuencia definida (diaria / semanal / mensual)

### 2. Cleaning
- [ ] Fechas faltantes completadas
- [ ] Outliers evaluados (¿promoción puntual? ¿error?)
- [ ] Serie continua sin huecos

### 3. EDA
- [ ] Gráfico de la serie
- [ ] Descomposición: trend + seasonality + residuo
- [ ] Test de estacionariedad (ADF)
- [ ] ACF / PACF

### 4. Time Series
- [ ] **Baseline naive** (obligatorio)
- [ ] Moving average
- [ ] Exponential smoothing (Holt-Winters)
- [ ] ARIMA / SARIMA
- [ ] Validación **cronológica** (nunca aleatoria)
- [ ] Comparación con MAE / RMSE / MAPE

### 5. Forecast
- [ ] Predicción a 6 meses
- [ ] **Intervalos de predicción**
- [ ] Escenarios (optimista / base / pesimista)

### 6. Dashboard
- [ ] Histórico + forecast en un solo gráfico
- [ ] Banda de incertidumbre visible
- [ ] Métricas de error del modelo mostradas

---

## ⚠️ Reglas

1. **Si no le ganás al naive forecast, el modelo no sirve.** Reportá siempre la comparación.
2. Nunca entregues un forecast sin intervalo. Un número solo es una promesa que no podés cumplir.
3. El MAPE es la métrica que el negocio entiende. Traducila: "nos equivocamos en promedio un 8%".

---

## 💡 Insights

1.
2.
3.

## 🎬 Recomendaciones

1.
2.
3.

---

## 📝 Bitácora

| Fecha | Qué hice | Bloqueos |
|---|---|---|
| | | |
