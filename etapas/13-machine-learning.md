---
etapa: 13
titulo: Machine Learning para analistas
duracion: 4-6 semanas
estado: pendiente
---

# 🤖 Etapa 13 — Machine Learning para analistas

⏱️ **4–6 semanas** · [[../progreso|← Progreso]]

> **No necesitás convertirte en ML Engineer.** Pero deberías entender qué hacen estos modelos y, sobre todo, cómo se evalúan.

---

## Supervised Learning

- [ ] Linear Regression
- [ ] Logistic Regression
- [ ] Decision Trees
- [ ] Random Forest
- [ ] Gradient Boosting (XGBoost / LightGBM)

| Modelo | Fuerte en | Débil en |
|---|---|---|
| Regresión lineal | Interpretabilidad | Relaciones no lineales |
| Regresión logística | Interpretabilidad, probabilidades | Interacciones complejas |
| Decision Tree | Explicable, no lineal | Overfitting brutal solo |
| Random Forest | Robusto, poco tuning | Menos interpretable |
| Gradient Boosting | Mejor performance tabular | Tuning, riesgo de overfit |

---

## Unsupervised Learning

- [ ] **K-means** — segmentación de clientes
- [ ] **Hierarchical clustering** — dendrogramas
- [ ] **PCA** — reducción de dimensionalidad

⚠️ En K-means: escalá las variables antes (si no, la de mayor magnitud domina) y elegí *k* con el método del codo + silhouette + **sentido de negocio**.

---

## ⚠️ Muy importante: evaluación

> Esta sección importa más que conocer los modelos.

- [ ] Train / test split
- [ ] Cross-validation (k-fold)
- [ ] **Overfitting**
- [ ] **Underfitting**
- [ ] Trade-off **bias / variance**
- [ ] Feature engineering
- [ ] **Data leakage** ← el error más caro y más frecuente

---

## 📏 Métricas

### Regresión
| Métrica | Interpretación |
|---|---|
| **MAE** | Error promedio, en unidades reales |
| **MSE** | Penaliza fuerte los errores grandes |
| **RMSE** | Como MSE pero en unidades reales |
| **R²** | Varianza explicada |

### Clasificación
| Métrica | Usala cuando |
|---|---|
| **Accuracy** | Clases balanceadas *(casi nunca)* |
| **Precision** | El costo del falso positivo es alto |
| **Recall** | El costo del falso negativo es alto |
| **F1** | Necesitás balance entre ambas |
| **ROC-AUC** | Comparar modelos, ranking de probabilidades |

⚠️ **El clásico:** 99% de accuracy en un dataset con 1% de fraude = un modelo que dice "no hay fraude" siempre. Inútil.

---

## ✅ Criterio de dominio

1. Explicá overfitting a alguien de negocio sin usar jerga.
2. ¿Qué es data leakage? Dame 3 ejemplos reales que se te podrían escapar.
3. Modelo de churn: ¿optimizás precision o recall? Justificá **con el costo del negocio**.
4. Segmentá clientes con K-means y **nombrá cada cluster** en términos de negocio.
5. Tu modelo pasó de 0.85 a 0.87 de AUC. ¿Vale la pena ponerlo en producción?
