---
etapa: 14
titulo: Data Engineering básica
duracion: 2-3 semanas
estado: pendiente
---

# 🟦 Etapa 14 — Data Engineering básica

⏱️ **2–3 semanas** · [[../progreso|← Progreso]]

> Un analista moderno debería entender **cómo llegan los datos**.
> No necesitás convertirte en Data Engineer. Pero sí conocer el recorrido.

---

## 🔁 El pipeline

```
Fuente
 ↓
Database
 ↓
ETL/ELT
 ↓
Data Warehouse
 ↓
BI
 ↓
Dashboard
 ↓
Business Decision
```

---

## Conceptos

- [ ] **APIs** — REST, autenticación, paginación, rate limits
- [ ] **CSV** — encoding, delimitadores, escapes
- [ ] **JSON** — anidamiento, normalización a tabla
- [ ] **ETL** vs **ELT** — y por qué el mundo se movió a ELT
- [ ] **Data pipelines** — orquestación, dependencias, reintentos
- [ ] **Data warehouse** — estructurado, esquema al escribir
- [ ] **Data lake** — crudo, esquema al leer
- [ ] **Cloud** — BigQuery, Snowflake, Redshift, Databricks
- [ ] **Batch processing** — corridas programadas
- [ ] **Streaming** — tiempo real

---

## 🧠 Lo que realmente te sirve como analista

| Concepto | Por qué te importa |
|---|---|
| Freshness | "¿Este dato de cuándo es?" — antes de reportar |
| Granularidad | Define qué preguntas podés responder |
| Idempotencia | Que reprocesar no duplique |
| Slowly Changing Dimensions | El cliente cambió de región: ¿histórico o actual? |
| Data lineage | De dónde viene cada columna cuando algo no cierra |
| Data contracts | Qué pasa cuando alguien renombra una columna aguas arriba |

---

## 🛠️ Práctica mínima

- [ ] Consumí una API pública con `requests` y armá un DataFrame
- [ ] Normalizá un JSON anidado con `json_normalize`
- [ ] Escribí un script que corra todos los días y actualice un CSV/base
- [ ] Conocé qué es dbt (aunque no lo uses todavía)
- [ ] Cargá datos a SQLite/Postgres desde Python

---

## ✅ Criterio de dominio

1. Explicá la diferencia entre ETL y ELT y cuándo conviene cada uno.
2. Tu dashboard muestra un número raro. Recorré el lineage hacia atrás: ¿qué chequeás y en qué orden?
3. ¿Qué es una slowly changing dimension tipo 2 y por qué te cambia el análisis histórico?
4. Escribí un pipeline simple: API → limpieza → base → query de verificación.
