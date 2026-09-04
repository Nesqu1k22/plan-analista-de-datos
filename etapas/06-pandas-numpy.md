---
etapa: 6
titulo: Pandas + análisis de datos
duracion: 4-6 semanas
estado: pendiente
---

# 🐼 Etapa 6 — Pandas + NumPy

⏱️ **4–6 semanas** · [[../progreso|← Progreso]]

> Pandas es **la herramienta central** del analista en Python.

---

## Carga de datos
- [ ] `read_csv()`
- [ ] `read_excel()`
- [ ] Parámetros clave: `sep`, `encoding`, `parse_dates`, `dtype`, `usecols`

## Inspección
- [ ] `head()`
- [ ] `info()`
- [ ] `describe()`
- [ ] `shape`
- [ ] `columns`
- [ ] `dtypes`
- [ ] `value_counts()`
- [ ] `nunique()`

## Selección
- [ ] `loc[]`
- [ ] `iloc[]`
- [ ] Filtrado booleano
- [ ] `query()`
- [ ] `isin()`
- [ ] `between()`

## Agregación
- [ ] `groupby()`
- [ ] `agg()` con múltiples funciones
- [ ] `pivot_table()`
- [ ] `crosstab()`
- [ ] `transform()` (¡subestimado y potentísimo!)

## Combinación
- [ ] `merge()`
- [ ] `join()`
- [ ] `concat()`
- [ ] Entender `how=` (`inner`, `left`, `outer`) y validar con `validate=`

## Transformación
- [ ] `sort_values()`
- [ ] `drop()`
- [ ] `rename()`
- [ ] `fillna()`
- [ ] `dropna()`
- [ ] `apply()` / `map()`
- [ ] `astype()`
- [ ] `assign()`

## Series temporales
- [ ] `to_datetime()`
- [ ] `.dt` accessor
- [ ] `set_index()` con fechas
- [ ] `resample()`
- [ ] `rolling()`
- [ ] `shift()` / `diff()` / `pct_change()`

---

## 🔁 Equivalencias SQL ↔ Pandas

| SQL | Pandas |
|---|---|
| `SELECT a, b` | `df[['a','b']]` |
| `WHERE x > 5` | `df[df.x > 5]` |
| `GROUP BY` | `df.groupby()` |
| `HAVING` | filtro después del `groupby` |
| `JOIN` | `df.merge()` |
| `ORDER BY` | `df.sort_values()` |
| `COUNT DISTINCT` | `df.nunique()` |
| `LAG()` | `df.groupby(...).shift(1)` |
| `SUM() OVER()` | `df.groupby(...).transform('sum')` |

---

## ✅ Criterio de dominio

1. Traducí a pandas la query de "top 3 productos por región" de la [[04-sql|Etapa 4]].
2. Calculá el **% que cada producto representa dentro de su categoría** usando `transform`, sin merge.
3. Tenés ventas diarias. Devolvé el promedio móvil de 7 días por sucursal.
4. Un `merge` te devolvió más filas de las esperadas. ¿Cómo lo diagnosticás? (Pista: `validate=`)
