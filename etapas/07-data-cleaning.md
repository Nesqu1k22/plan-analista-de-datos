---
etapa: 7
titulo: Data Cleaning
duracion: 2-3 semanas
estado: pendiente
---

# 🧹 Etapa 7 — Data Cleaning

⏱️ **2–3 semanas** · [[../progreso|← Progreso]]

> Acá empieza **una gran parte del trabajo real**. En un trabajo de verdad, esto se lleva el 60–80% del tiempo.

---

## Qué tenés que aprender a detectar

- [ ] **Missing values** — y decidir: ¿eliminar, imputar, o dejar?
- [ ] **Duplicados** — exactos y parciales (mismo cliente, distinta grafía)
- [ ] **Outliers** — ¿error de carga o dato real extremo?
- [ ] **Errores de tipeo**
- [ ] **Categorías inconsistentes**
- [ ] **Fechas inválidas** — futuras, imposibles, formatos mezclados (DD/MM vs MM/DD)
- [ ] **Unidades incorrectas** — pesos vs miles de pesos, kg vs g
- [ ] **Datos imposibles** — edad 250, precio negativo, fecha de baja anterior al alta

---

## El ejemplo canónico

```
Argentina
ARG
Argentina 
argentina
AR
```

Para una persona son lo mismo.
**Para una computadora pueden ser cinco categorías diferentes.**

---

## 🧰 Técnicas

### Missing values
| Estrategia | Cuándo |
|---|---|
| Eliminar filas | Pocos nulos, MCAR |
| Eliminar columna | >50% nulos y poco valor |
| Imputar media/mediana | Numérica, distribución conocida |
| Imputar moda | Categórica |
| Categoría "Desconocido" | El nulo *significa* algo |
| Forward/backward fill | Series temporales |

⚠️ **Siempre documentá qué imputaste.** Un nulo imputado que después se reporta como dato real es fraude involuntario.

### Outliers
- [ ] Método IQR: fuera de $[Q1 - 1.5 \cdot IQR,\ Q3 + 1.5 \cdot IQR]$
- [ ] Z-score: $|z| > 3$
- [ ] Percentiles (winsorizing)
- [ ] **Criterio de negocio** ← el más importante

### Normalización de texto
- [ ] `.str.strip()`, `.str.lower()`, `.str.title()`
- [ ] Quitar acentos
- [ ] Regex para patrones
- [ ] Diccionario de mapeo explícito
- [ ] Fuzzy matching (`rapidfuzz`) para casos difíciles

---

## 📋 Checklist de limpieza (usá esto siempre)

- [ ] `df.info()` — tipos correctos?
- [ ] `df.isna().sum()` — nulos por columna
- [ ] `df.duplicated().sum()` — duplicados exactos
- [ ] Duplicados por clave de negocio
- [ ] `describe()` — mínimos/máximos imposibles
- [ ] `value_counts()` en cada categórica
- [ ] Rango de fechas razonable
- [ ] Totales contrastados contra fuente oficial
- [ ] **Registro escrito de cada decisión de limpieza**

---

## ✅ Criterio de dominio

1. Te dan un CSV de 200k filas de ventas. Escribí el reporte de calidad de datos antes de analizar nada.
2. Tenés `cliente` con 4.000 valores únicos pero sabés que hay ~2.500 clientes reales. ¿Cómo los consolidás?
3. Encontraste 30 ventas con importe negativo. ¿Las borrás? Justificá.
4. ¿Por qué imputar con la media puede arruinar tu análisis de dispersión?
