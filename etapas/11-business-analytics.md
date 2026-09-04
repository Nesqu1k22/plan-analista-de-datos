---
etapa: 11
titulo: Business Analytics
duracion: 3-4 semanas
estado: pendiente
---

# 🟧 Etapa 11 — Business Analytics

⏱️ **3–4 semanas** · [[../progreso|← Progreso]]

> Esta parte **separa a un técnico de un analista**.
> Porque la empresa no te contrata para hacer gráficos. Te contrata para responder:
> ## *¿Qué está pasando y qué deberíamos hacer?*

---

## 📌 KPIs

| KPI | Qué mide | Fórmula |
|---|---|---|
| **Revenue** | Ingresos | $\sum precio \times cantidad$ |
| **Gross Profit** | Ganancia bruta | Revenue − COGS |
| **Net Profit** | Ganancia neta | Gross Profit − gastos operativos |
| **Margin** | Rentabilidad % | Profit / Revenue |
| **CAC** | Costo de adquirir un cliente | Gasto marketing / clientes nuevos |
| **LTV** | Valor de vida del cliente | ARPU × margen × vida promedio |
| **Churn** | Tasa de abandono | Clientes perdidos / clientes al inicio |
| **Retention** | Tasa de retención | 1 − churn |
| **Conversion Rate** | Tasa de conversión | Conversiones / visitas |
| **ARPU** | Ingreso promedio por usuario | Revenue / usuarios activos |
| **AOV** | Ticket promedio | Revenue / cantidad de órdenes |

⭐ **Regla clave:** $LTV / CAC \geq 3$ es el umbral de negocio sano.

---

## 📈 Análisis comercial

Aprendé a analizar:

- [ ] Ventas
- [ ] Clientes
- [ ] Productos
- [ ] Marketing
- [ ] Pricing
- [ ] Inventario
- [ ] Rentabilidad
- [ ] Cohortes
- [ ] Retención

### Descomposición de una caída de ventas
```
Revenue = Clientes × Frecuencia × Ticket promedio
```
Cuando el revenue cae, **siempre** descomponé: ¿perdiste clientes, compran menos seguido, o gastan menos por compra? Cada causa tiene una acción distinta.

---

## 👥 Customer Analytics

### Segmentación
- [ ] Demográfica
- [ ] Conductual
- [ ] **RFM** (Recency, Frequency, Monetary)

### RFM
| Dimensión | Pregunta |
|---|---|
| **R**ecency | ¿Hace cuánto compró por última vez? |
| **F**requency | ¿Cuántas veces compró? |
| **M**onetary | ¿Cuánto gastó en total? |

Puntuás cada una 1–5 y obtenés segmentos: *Champions*, *Loyal*, *At Risk*, *Hibernating*, *Lost*.

### Cohort Analysis
- [ ] Cohorte de adquisición
- [ ] Matriz de retención
- [ ] Curva de retención

**Ejemplo:** Clientes adquiridos en enero.

¿De esos clientes cuántos siguen activos en:
- febrero?
- marzo?
- abril?
- mayo?

> El cohort analysis es la herramienta que revela si tu negocio está sano o si estás tapando el churn con adquisición.

---

## ✅ Criterio de dominio

1. Las ventas cayeron 12%. Descomponé la caída en sus 3 factores y decí cuál investigás primero.
2. Tu CAC es $8.000 y tu LTV $18.000. ¿Es un negocio sano? ¿Qué le recomendás a marketing?
3. Construí una matriz de cohortes de retención mensual (SQL o pandas).
4. Segmentá una base de clientes con RFM y proponé **una acción concreta por segmento**.
5. ¿Por qué el churn mensual del 5% no es "95% de retención anual"?
