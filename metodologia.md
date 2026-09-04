---
tipo: referencia
plan: data-analyst
---

# 🧑💼 Metodología profesional del analista

> Cuando te den un dataset, **no empieces a hacer gráficos**.

Esto es lo que separa a un técnico de un analista. Usá siempre este proceso.

---

## Los 9 pasos

### 1. Business Question
**¿Qué quiere saber la empresa?**
Escribila textual. Si es vaga ("quiero entender a los clientes"), volvé y preguntá hasta que sea concreta.

### 2. Analytical Question
**¿Qué necesitamos calcular para responderla?**
Traducción de lenguaje de negocio a lenguaje de datos. *"¿Por qué cayeron las ventas?"* → *"¿Cayó el ticket promedio, la cantidad de transacciones, o la cantidad de clientes activos?"*

### 3. Data Requirements
**¿Qué datos necesitamos?** Tablas, columnas, granularidad, período.

### 4. Data Collection
**¿De dónde salen?** Base, API, CSV, export manual. Documentá la fuente y la fecha del extract.

### 5. Data Cleaning
**¿Son confiables?** Nulos, duplicados, outliers, categorías inconsistentes, fechas inválidas.

### 6. Analysis
**¿Qué encontramos?** Acá recién empieza el análisis.

### 7. Validation
**¿El resultado es correcto?** Contrastá totales contra otra fuente. Un número que no cierra con el reporte oficial destruye tu credibilidad más rápido que un error de análisis.

### 8. Communication
**¿Cómo lo presentamos?** Audiencia, formato, nivel de detalle. Un director no quiere ver tu notebook.

### 9. Recommendation
**¿Qué debería hacer la empresa?**
Sin este paso sos un generador de gráficos. Con este paso sos un analista.

---

## 🔁 Pipeline mental completo

```
Pregunta empresarial
        ↓
    SQL / Data
        ↓
     Cleaning
        ↓
       EDA
        ↓
   Estadística
        ↓
   Segmentación
        ↓
   Visualización
        ↓
     Power BI
        ↓
     Insights
        ↓
  Recomendaciones
        ↓
Decisión empresarial
```

---

## ⚠️ Errores clásicos a evitar

| Error | Por qué mata |
|-------|--------------|
| Graficar antes de entender | Encontrás patrones en datos sucios |
| Confundir correlación con causalidad | Recomendaciones desastrosas |
| Reportar una diferencia sin test | "B es mejor" cuando es ruido |
| No validar totales | Perdés credibilidad para siempre |
| Entregar el dashboard sin insight | Nadie lo usa |
| Segmentar hasta encontrar algo (p-hacking) | Hallazgo falso garantizado |
| Ignorar el contexto del negocio | Análisis técnicamente perfecto e inútil |

---

## 📋 Plantilla de arranque de análisis

```markdown
## Pregunta empresarial
## Pregunta analítica
## Datos necesarios
## Fuente y fecha del extract
## Supuestos
## Limitaciones conocidas
## Hallazgos
## Validación (¿contra qué contrasté?)
## Recomendación
```
