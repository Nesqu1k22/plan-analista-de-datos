---
etapa: 4
titulo: SQL y bases de datos
duracion: 6-8 semanas
estado: pendiente
---

# 🟨 Etapa 4 — SQL

⏱️ **6–8 semanas** · [[../progreso|← Progreso]]

> Esta debería ser **una de tus mayores prioridades**.
> Un analista profesional debe sentirse cómodo consultando bases de datos.

---

## Nivel básico

- [ ] `SELECT`
- [ ] `FROM`
- [ ] `WHERE`
- [ ] `ORDER BY`
- [ ] `GROUP BY`
- [ ] `HAVING`
- [ ] `LIMIT`

Después:

- [ ] `CASE`
- [ ] `COALESCE`
- [ ] `NULLIF`
- [ ] `DISTINCT`

---

## 🔗 JOINs

- [ ] `INNER JOIN`
- [ ] `LEFT JOIN`
- [ ] `RIGHT JOIN`
- [ ] `FULL OUTER JOIN`
- [ ] `CROSS JOIN`

Y sobre todo:

> **Entender qué está pasando con las filas después del JOIN.**

⚠️ El error #1 del analista junior: hacer un JOIN que duplica filas y reportar un revenue inflado. **Siempre chequeá el `COUNT(*)` antes y después de un JOIN.**

---

## 📈 Agregaciones

- [ ] `SUM`
- [ ] `AVG`
- [ ] `COUNT`
- [ ] `MIN`
- [ ] `MAX`
- [ ] `COUNT DISTINCT`

```sql
SELECT
    customer_id,
    SUM(amount) AS revenue
FROM sales
GROUP BY customer_id;
```

---

## 🧠 SQL avanzado

### CTEs
- [ ] `WITH ... AS (...)`
- [ ] CTEs encadenadas
- [ ] Cuándo una CTE es más legible que una subquery

```sql
WITH customer_sales AS (
    SELECT customer_id, SUM(amount) AS revenue
    FROM sales
    GROUP BY customer_id
)
SELECT * FROM customer_sales WHERE revenue > 100000;
```

### Subqueries
- [ ] En `SELECT`
- [ ] En `FROM`
- [ ] En `WHERE` (`IN`, `EXISTS`)
- [ ] Correlacionadas

### Window Functions ⭐⭐

- [ ] `ROW_NUMBER()`
- [ ] `RANK()`
- [ ] `DENSE_RANK()`
- [ ] `LAG()`
- [ ] `LEAD()`
- [ ] `SUM() OVER()`
- [ ] `AVG() OVER()`
- [ ] `PARTITION BY` + `ORDER BY` dentro del `OVER()`

> **Esto es muy importante.**

**Ejemplo:**
> ¿Cuál fue la venta de cada cliente comparada con su compra anterior?

```sql
SELECT
    customer_id,
    order_date,
    amount,
    LAG(amount) OVER (PARTITION BY customer_id ORDER BY order_date) AS compra_anterior,
    amount - LAG(amount) OVER (PARTITION BY customer_id ORDER BY order_date) AS delta
FROM sales;
```

> Eso requiere **pensar analíticamente**, no solamente escribir SQL.

---

## 🗄️ Bases de datos

- [ ] Tablas
- [ ] Primary keys
- [ ] Foreign keys
- [ ] Relaciones
- [ ] Normalización
- [ ] Índices
- [ ] Constraints
- [ ] Views
- [ ] Fact tables
- [ ] Dimension tables

Y conceptos básicos de:

- [ ] Data Warehouse / OLAP
- [ ] Diferencia OLTP vs OLAP

---

## ✅ Criterio de dominio

1. Escribí una query que devuelva el **top 3 de productos por revenue dentro de cada región**. (Necesitás window functions.)
2. Después de un `LEFT JOIN` tu revenue total subió. ¿Qué pasó y cómo lo detectás?
3. Diferencia entre `WHERE` y `HAVING`, con un ejemplo donde intercambiarlos rompe la query.
4. Calculá la **retención mes a mes** (cohortes) sólo con SQL.
5. `ROW_NUMBER()` vs `RANK()` vs `DENSE_RANK()` sobre un caso con empates.
