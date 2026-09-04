---
etapa: 8
titulo: Exploratory Data Analysis
duracion: 2-3 semanas
estado: pendiente
---

# 🔍 Etapa 8 — Exploratory Data Analysis (EDA)

⏱️ **2–3 semanas** · [[../progreso|← Progreso]]

> Tenés que desarrollar la capacidad de mirar un dataset y preguntarte:
> ## *¿Qué está pasando acá?*

---

## El proceso de 6 pasos

### 1. Understand
**¿Qué representan los datos?**
Granularidad (¿una fila = una venta, un ítem, un día?), período cubierto, origen, definición de cada columna.

### 2. Clean
**¿Son confiables?**
→ [[07-data-cleaning|Etapa 7]]

### 3. Explore
**¿Qué patrones aparecen?**
Distribuciones, correlaciones, tendencias temporales, concentración (¿el 80% del revenue viene del 5% de clientes?).

### 4. Segment
**¿Cambian según grupo?**
Por región, canal, producto, cohorte, tipo de cliente. Un promedio global casi siempre esconde dos historias opuestas.

### 5. Investigate
**¿Por qué ocurre?**
Acá formulás hipótesis y las testeás. No te quedes en el "qué".

### 6. Communicate
**¿Cómo lo explico?**
→ [[09-visualizacion|Etapa 9]]

---

## 🔬 Análisis univariado
- [ ] Histogramas y densidad
- [ ] Box plots
- [ ] `value_counts()` para categóricas
- [ ] Detección de asimetría

## 🔬 Análisis bivariado
- [ ] Scatter plots
- [ ] Correlación (Pearson vs Spearman)
- [ ] Box plot por categoría
- [ ] Tablas de contingencia

## 🔬 Análisis multivariado
- [ ] Heatmap de correlaciones
- [ ] Pair plots
- [ ] Segmentación cruzada

---

## ⚠️ Trampas del EDA

| Trampa | Antídoto |
|---|---|
| Paradoja de Simpson | Siempre segmentá antes de concluir |
| Correlación ≠ causalidad | Buscá la variable de confusión |
| p-hacking (buscar hasta encontrar) | Definí la hipótesis **antes** |
| Confiar en el promedio | Mirá la distribución completa |
| Ignorar la estacionalidad | Compará contra el mismo período del año anterior |
| Survivorship bias | ¿Qué filas *no* están en el dataset? |

---

## ✅ Criterio de dominio

1. Te dan un dataset nuevo sin documentación. Listá las primeras 10 cosas que hacés, en orden.
2. El revenue total subió 5% pero el margen cayó. ¿Qué segmentaciones investigás?
3. Mostrá un caso donde el promedio global sube pero baja en **todos** los segmentos (Simpson).
4. ¿Cuándo usás Spearman en vez de Pearson?
