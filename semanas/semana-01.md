---
tipo: plan-semanal
etapa: 1
semana: 1
inicio: 2026-09-04
---

# 🚀 Semana 1 — Fundamentos matemáticos

**Etapa:** [[../etapas/01-fundamentos-matematicos|Etapa 1]] · **Objetivo de la semana:** álgebra operativa + porcentajes al nivel que necesita un analista.

> ⚠️ **Nota de calendario:** arrancás viernes 4. Como la [[../rutina-semanal|rutina]] está armada de lunes a sábado, el viernes y sábado son un **arranque anticipado** (setup + porcentajes), y la semana completa corre del **lunes 7 al sábado 12**.

---

## 📅 Viernes 4/9 — Setup + arranque *(2 h)*

### Bloque 1 — Herramientas (45 min)

Dejá el entorno listo de una vez para no perder tiempo después:

- [ ] Instalar **Python** (o Anaconda) + **VS Code**
- [ ] Instalar **Power BI Desktop** (es gratis, pero lo vas a usar recién en la etapa 10 — instalalo igual)
- [ ] Verificar que tenés **Excel** con Power Query (pestaña *Datos → Obtener datos*)
- [ ] Crear carpeta de trabajo: `Documentos/analista-datos/` con subcarpetas `ejercicios/` y `datasets/`
- [ ] Confirmar acceso al repo: https://github.com/Nesqu1k22/plan-analista-de-datos

### Bloque 2 — Definir el punto de partida (15 min)

- [ ] Abrir [[../progreso]] y confirmar la fecha de inicio
- [ ] Leer completa la [[../rutina-semanal]] y la [[../metodologia]]
- [ ] Bloquear los horarios de estudio en tu calendario **como si fueran clases**. Esto no es opcional: lo que no está agendado no pasa.

### Bloque 3 — Álgebra: diagnóstico (1 h)

Resolvé los **Ejercicios A** (abajo). No los estudies antes: la idea es ver qué sabés y qué no.

- [ ] Ejercicios A1–A6
- [ ] Anotar en [[../bitacora]] cuáles te costaron

---

## 📅 Sábado 5/9 — Porcentajes *(3 h)*

El tema más importante de toda la etapa 1. Un analista usa porcentajes todos los días.

### Bloque 1 — Teoría (45 min)
- [ ] Variación porcentual
- [ ] Porcentaje sobre total y acumulado
- [ ] Diferencia entre **margen** y **markup**
- [ ] Puntos porcentuales vs porcentaje (¡no son lo mismo!)

### Bloque 2 — Práctica (2 h 15)
- [ ] Ejercicios B1–B8
- [ ] Rehacer B5 y B6 **en Excel**, con fórmulas (no a mano)

---

## 📅 Domingo 6/9 — Descanso

Descanso real. No "leo algo liviano". Descanso.

---

## 📅 Lunes 7/9 — Teoría: potencias, raíces y logaritmos *(2 h)*

- [ ] Potencias y sus propiedades
- [ ] Raíces como potencias fraccionarias
- [ ] Logaritmos: qué son y **por qué existen**
- [ ] Propiedades: $\log(ab) = \log a + \log b$, $\log(a^n) = n\log a$
- [ ] Por qué una escala logarítmica convierte el crecimiento exponencial en una recta

**Recurso:** buscá "logarithms" en 3Blue1Brown o Khan Academy en español.

**Pregunta guía:** *¿por qué los gráficos de crecimiento de startups y de casos de una epidemia se muestran en escala log?*

---

## 📅 Martes 8/9 — Ejercicios: logaritmos y exponenciales *(2 h)*

- [ ] Ejercicios C1–C5
- [ ] Regla del 72 y su comparación con el cálculo exacto (C4)

---

## 📅 Miércoles 9/9 — Herramienta: Excel *(2 h)*

Primer contacto real con la herramienta. Armá una planilla llamada `semana-01-porcentajes.xlsx`:

- [ ] Tabla con 12 meses de ventas inventadas
- [ ] Columna de **variación mensual %** (MoM)
- [ ] Columna de **variación acumulada** desde enero
- [ ] Columna de **% sobre el total anual**
- [ ] Columna de **% acumulado** (Pareto)
- [ ] Formato de celda como porcentaje (no multipliques por 100 a mano)
- [ ] Usar **referencias absolutas** (`$B$15`) para el total — practicá el `F4`
- [ ] Un gráfico de líneas de la evolución y uno de barras de la variación

> 🎯 El objetivo no es Excel todavía. Es que los porcentajes te salgan sin pensar.

---

## 📅 Jueves 10/9 — Matemática aplicada a métricas *(2 h)*

> En la rutina el jueves es "estadística", pero todavía no llegaste. En la etapa 1 lo reemplazamos por **matemática de métricas de negocio**, que es la que vas a usar en la etapa 11.

- [ ] **CAGR** — fórmula, cuándo se usa y por qué no es lo mismo que el promedio de las variaciones
- [ ] **Growth rate** vs **run rate**
- [ ] **Margen bruto / neto**
- [ ] Ejercicios D1–D4

---

## 📅 Viernes 11/9 — Caso práctico *(2 h)*

Primera vez que aplicás la [[../metodologia|metodología]]. Todavía sin datos reales: sólo el razonamiento.

### El encargo

> *"El año pasado facturamos $11.000.000. Este año $11.550.000. El dueño dice que crecimos y está contento. ¿Vos qué le decís?"*

- [ ] Calculá el crecimiento nominal
- [ ] **Pregunta clave:** ¿cuánto fue la inflación del período? ¿Crecieron **en términos reales**?
- [ ] Si la inflación fue del 12%, ¿cuál fue el crecimiento real?
- [ ] Escribí una respuesta de **5 líneas** dirigida al dueño, sin jerga técnica
- [ ] Listá 3 datos adicionales que pedirías antes de dar una conclusión firme

📄 Guardalo en `notas/01-caso-crecimiento-real.md`

> Este ejercicio es el más importante de la semana. Es literalmente lo que hace un analista.

---

## 📅 Sábado 12/9 — Consolidación *(3 h)*

- [ ] Rehacer sin mirar los ejercicios que fallaste
- [ ] Responder por escrito las **4 preguntas del [[../etapas/01-fundamentos-matematicos#✅ Criterio de dominio|Criterio de dominio]]** de la etapa 1
- [ ] Escribir una nota en `notas/` explicando **con tus palabras** qué es un logaritmo
- [ ] Actualizar [[../progreso]] (horas + estado)
- [ ] Cerrar la semana en [[../bitacora]]
- [ ] `git add -A && git commit -m "semana 1" && git push`

---

# 📝 Ejercicios

> Resolvé **a mano o en papel** primero. Las soluciones están en [[semana-01-soluciones]] — no las mires antes de intentarlo.

## A — Álgebra (viernes)

**A1.** Resolvé: $3x + 12 = 5x - 8$

**A2.** Despejá $q$: $I = p \cdot q - CF$

**A3.** Una empresa tiene costos fijos de $450.000 y un costo variable de $320 por unidad. Vende cada unidad a $500. ¿Cuántas unidades necesita vender para no perder plata (punto de equilibrio)?

**A4.** Vendiste 340 unidades entre dos productos y facturaste $212.000. El producto A sale $500 y el B $800. ¿Cuántas vendiste de cada uno?

**A5.** Simplificá: $\dfrac{x^5 \cdot x^{-2}}{x^{4}}$

**A6.** La utilidad es $U(q) = 180q - 450.000$. ¿Cuál es la pendiente y qué significa **en lenguaje de negocio**?

---

## B — Porcentajes (sábado) ⭐

**B1.** Las ventas de enero fueron $1.250.000 y las de febrero $1.437.500. ¿Cuál fue la variación porcentual?

**B2.** En marzo cayeron a $1.322.500. ¿Cuál fue la variación de febrero a marzo?

**B3.** ¿Cuál fue la variación **acumulada** de enero a marzo? ¿Por qué **no** es la suma de B1 y B2?

**B4.** Las ventas cayeron 20% en un mes y subieron 20% al siguiente. ¿Volvieron al valor original? Demostralo.

**B5.** Estos son los ingresos por producto:

| Producto | Ingresos |
|---|---|
| A | 4.200.000 |
| B | 2.800.000 |
| C | 1.900.000 |
| D | 1.100.000 |
| E | 600.000 |
| F | 400.000 |

Calculá el **% sobre el total** y el **% acumulado** de cada uno (ordenados de mayor a menor). ¿Cuántos productos explican el 80% de los ingresos?

**B6.** Un producto se vende a $8.500 y cuesta $5.950. Calculá el **margen** y el **markup**. ¿Por qué dan distinto?

**B7.** El precio final con IVA (21%) es $12.100. ¿Cuál es el precio sin IVA? *(Ojo: no es restarle el 21%.)*

**B8.** La tasa de conversión pasó del 4% al 5%. Un compañero dice "subió 1%". Otro dice "subió 25%". ¿Quién tiene razón?

---

## C — Logaritmos y exponenciales (martes)

**C1.** Resolvé: $2^x = 64$

**C2.** Resolvé: $\log_{10}(1000) = ?$ y $\ln(e^3) = ?$

**C3.** Aplicá propiedades: $\log(50 \cdot 4) - \log(2)$

**C4.** Si tus ventas crecen 3% por mes, ¿en cuántos meses se duplican? Resolvelo con logaritmos y después compará con la **regla del 72**.

**C5.** Tenés una serie: 100, 200, 400, 800, 1600. Graficala en escala lineal y en escala logarítmica (Excel o papel). ¿Qué forma tiene en cada una y por qué?

---

## D — Métricas de negocio (jueves)

**D1.** Una inversión pasó de $100.000 a $180.000 en 4 años. ¿Cuál es el CAGR?

$$ CAGR = \left(\frac{V_f}{V_i}\right)^{\frac{1}{n}} - 1 $$

**D2.** Los crecimientos anuales fueron +30%, −10% y +20%. ¿Cuál fue el crecimiento total del período? ¿Cuál es el CAGR? ¿Por qué **no** es el promedio simple (13,3%)?

**D3.** Facturaste $2.400.000 en el primer trimestre. ¿Cuál es tu **run rate** anual? Listá 2 razones por las que ese número puede ser engañoso.

**D4.** Vendés a $8.500, el costo del producto es $5.950 y tenés gastos operativos de $1.200 por unidad. Calculá margen bruto y margen neto.

---

## ✅ Checklist de cierre de semana

- [ ] 13 h de estudio registradas
- [ ] Ejercicios A, B, C y D resueltos
- [ ] Planilla de Excel armada
- [ ] Caso práctico escrito en `notas/`
- [ ] Criterio de dominio de la etapa 1 respondido
- [ ] [[../progreso]] y [[../bitacora]] actualizados
- [ ] Cambios pusheados a GitHub
