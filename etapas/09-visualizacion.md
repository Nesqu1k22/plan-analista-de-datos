---
etapa: 9
titulo: Visualización
duracion: 3-4 semanas
estado: pendiente
---

# 📊 Etapa 9 — Visualización

⏱️ **3–4 semanas** · [[../progreso|← Progreso]]

---

## Principios

- [ ] Percepción visual (qué codifica mejor el ojo: posición > longitud > ángulo > área > color)
- [ ] Jerarquía visual
- [ ] Color (paletas secuenciales / divergentes / categóricas · accesibilidad daltónica)
- [ ] Escalas (¿eje Y desde cero? ¿escala log?)
- [ ] Ejes (etiquetas, unidades, formato de número)
- [ ] Storytelling
- [ ] Selección de gráficos

---

## Gráficos a dominar

| Gráfico | Usalo para | Evitalo cuando |
|---|---|---|
| **Bar chart** | Comparar categorías | Hay 50+ categorías |
| **Line chart** | Evolución temporal | El eje X no es continuo |
| **Scatter plot** | Relación entre 2 numéricas | Hay demasiado solapamiento |
| **Histogram** | Distribución de una numérica | Pocos datos |
| **Box plot** | Comparar distribuciones entre grupos | La audiencia no lo sabe leer |
| **Heatmap** | Matriz de valores / correlaciones | Sin escala clara |
| **Area chart** | Composición acumulada en el tiempo | Muchas series apiladas |
| **KPI cards** | Un número clave con contexto | Sin comparación ni tendencia |

---

## 🚫 Y aprendé cuándo NO utilizar un gráfico

- Un solo número → **escribilo**, no lo grafiques.
- 3 filas de datos → **tabla**.
- Torta con más de 4 categorías → **barras**.
- Gráfico 3D → **nunca**.
- Doble eje Y → casi siempre engañoso.
- Gráfico decorativo sin mensaje → sacalo.

---

## 🎨 Herramientas
- [ ] Matplotlib (base, control total)
- [ ] Seaborn (estadístico, rápido)
- [ ] Plotly (interactivo)
- [ ] Excel (para audiencias que viven ahí)

---

## 📖 Data Storytelling

Estructura de una presentación de análisis:

1. **Contexto** — qué estaba pasando
2. **Conflicto** — qué encontramos que no esperábamos
3. **Resolución** — qué recomendamos hacer

Un gráfico por idea. Título del gráfico = **la conclusión**, no la descripción.
❌ "Ventas por región"
✅ "Cuyo cayó 22% mientras el resto creció"

---

## ✅ Criterio de dominio

1. Rehacé un gráfico malo (buscá uno en un diario) y explicá cada cambio.
2. Tenés que mostrar la evolución de 12 productos en el tiempo. ¿Cómo evitás el "spaghetti chart"?
3. ¿Cuándo está justificado cortar el eje Y y cómo lo señalizás?
4. Convertí un análisis de 8 gráficos en una historia de 3 slides.
