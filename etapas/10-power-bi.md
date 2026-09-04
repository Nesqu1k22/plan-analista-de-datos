---
etapa: 10
titulo: Power BI + DAX
duracion: 4-6 semanas
estado: pendiente
---

# 🟪 Etapa 10 — Power BI

⏱️ **4–6 semanas** · [[../progreso|← Progreso]]

> Acá pasás de **"analizar datos"** a **construir productos analíticos**.

---

## Power Query / ETL

- [ ] Power Query
- [ ] ETL
- [ ] Transformaciones
- [ ] Merge
- [ ] Append
- [ ] Limpieza
- [ ] Parámetros y consultas reutilizables

> Es el mismo motor que ya viste en [[02-excel-profesional|Excel]]. Ventaja acumulada.

---

## 🧩 Data Modeling ⭐ *muy importante*

- [ ] Relaciones (1:muchos, muchos:muchos)
- [ ] Dirección del filtro
- [ ] Tabla calendario dedicada
- [ ] **Star Schema**

```
             Dim_Date
                 |
Dim_Product — Fact_Sales — Dim_Customer
                 |
             Dim_Store
```

⚠️ El 80% de los problemas de DAX son en realidad problemas de modelo. Si tu DAX se está volviendo imposible, el modelo está mal.

---

## 🧮 DAX

### Funciones a dominar
- [ ] `SUM()`
- [ ] `CALCULATE()` ⭐ *la función central de DAX*
- [ ] `FILTER()`
- [ ] `ALL()`
- [ ] `ALLEXCEPT()`
- [ ] `DIVIDE()` *(nunca uses `/` — `DIVIDE` maneja el división por cero)*
- [ ] `DISTINCTCOUNT()`
- [ ] `COUNTROWS()`
- [ ] `RELATED()` / `RELATEDTABLE()`
- [ ] `SUMX()` y las funciones iteradoras `X`

### Conceptos ⭐
- [ ] **Row context**
- [ ] **Filter context**
- [ ] **Context transition** *(lo que hace `CALCULATE` cuando hay row context)*
- [ ] Measures vs Calculated columns *(regla: measure por defecto, columna sólo si la necesitás para filtrar/agrupar)*

### Time intelligence
- [ ] YTD
- [ ] MTD
- [ ] YoY
- [ ] MoM
- [ ] Rolling averages
- [ ] `SAMEPERIODLASTYEAR`, `DATEADD`, `DATESYTD`

---

## ✅ Criterio de dominio

1. Explicá **filter context** con un ejemplo concreto de tu modelo.
2. ¿Por qué una medida da distinto valor en una tarjeta que dentro de una tabla?
3. Construí un `% del total` que respete los filtros del usuario pero ignore el de producto.
4. Tu YoY da en blanco para enero. ¿Qué está mal? (Pista: tabla calendario)
5. Publicá un dashboard con 4 páginas, drill-through y navegación entre ellas.
