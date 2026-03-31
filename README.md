<p align="center">
  <img src="assets/chunga-malaje-consulting.png" width="420" alt="Logo proyecto">
</p>

# Brecha de género en empleo HRST en Europa (Eurostat + Tableau)

![Tableau](https://img.shields.io/badge/Tableau-Dashboard-blue)
![Eurostat](https://img.shields.io/badge/Datos-Eurostat-orange)
![Social%20Impact](https://img.shields.io/badge/Enfoque-Impacto%20Social-6f42c1)
![Gender%20Gap](https://img.shields.io/badge/Tema-Brecha%20de%20G%C3%A9nero-ff69b4)

## Resumen ejecutivo (para qué sirve)
**Pregunta:** ¿Cómo varía la brecha de género en empleo HRST (Human Resources in Science and Technology) entre países y a lo largo del tiempo en Europa?

**Objetivo:** identificar patrones territoriales, temporales y demográficos para priorizar intervenciones (políticas públicas y programas STEM/HRST) basadas en evidencia.

**Aplicación (empleabilidad e innovación social):** útil para orientar acciones de atracción, retención y progresión de talento (especialmente femenino) en itinerarios STEM/HRST y programas de empleabilidad.

**Datos:** Eurostat (indicadores HRST) + preparación y modelado para visualización.

**Entregable:** dashboard interactivo en Tableau Public.

**Ver dashboard (Tableau Public):**  
https://public.tableau.com/views/Brecha_genero_HRST_Europa_Marina-Ruth/BrechadegneroenempleoHRSTenEuropa

---

## Acceso rápido
- **Dashboard:** https://public.tableau.com/views/Brecha_genero_HRST_Europa_Marina-Ruth/BrechadegneroenempleoHRSTenEuropa
- **Preview:** ver imagen más abajo
- **Datos:** Eurostat (datasets listados en “Fuentes de datos”)

---

## Autoras
**Marina Martín Díaz**  
**Ruth Pérez Segovia**

---

## Qué preguntas responde el dashboard
1) **Evolución temporal:** ¿Cómo evoluciona el empleo HRST por sexo a lo largo del tiempo?  
2) **Comparativa territorial:** ¿Qué países presentan mayor o menor brecha de género relativa?  
3) **Dimensión demográfica:** ¿Cómo se distribuye el desempleo HRST por grupos de edad?

---

## Dashboard preview
<p align="center">
  <img src="assets/dashboard-preview.png" width="900" alt="Dashboard preview">
</p>

---

## KPIs incluidos
El panel superior resume la situación con:
- **% medio de mujeres en empleo HRST**
- **Brecha media relativa**
- **Número de países con datos disponibles**

---

## Key insights (orientados a decisión)
*Insights cualitativos basados en el dashboard; pueden ampliarse con ejemplos por país.*

- **Equilibrio agregado ≈ 50%**, pero con variabilidad por país → priorizar acciones por contexto nacional/territorial.
- **Desigualdad territorial persistente** → sugiere factores estructurales → útil para identificar “países referencia” y zonas prioritarias.
- **La mejora absoluta no implica cierre automático de brecha** → diseñar medidas específicas de atracción/retención/progresión.
- **Diferencias por edad en desempleo HRST** → diseñar acciones segmentadas por etapa de carrera.

---

## Interactividad (cómo explorar)
### Filtros
- **Año**
- **País**

### Interacciones
- Selección en el **mapa** filtra el ranking y actualiza el resto de visualizaciones.
- Permite analizar patrones específicos por país y periodo temporal.

---

## Visualizaciones incluidas
- **Evolución HRST por sexo:** series temporales para detectar convergencias/divergencias.
- **Mapa de brecha relativa por país:** lectura territorial rápida.
- **Ranking Top/Bottom:** identifica extremos en desigualdad relativa.
- **Desempleo HRST por edad:** dimensión demográfica complementaria.

---

## Fuentes de datos (Eurostat)
Datasets utilizados (TSV):
- `hrst_st_nsecsex2` — Empleo en ciencia y tecnología por categoría HRST, actividad económica y sexo  
- `hrst_st_nunesex` — Personas desempleadas en ciencia y tecnología por categoría y sexo  
- `hrst_st_nuneage` — Personas desempleadas en ciencia y tecnología por categoría y grupo de edad

---

## Preparación y transformación de datos
Tareas realizadas:
- limpieza de valores nulos
- normalización de tipos de dato
- creación de campos calculados
- filtrado de agregados supranacionales
- normalización de nombres de países
- preparación de variables para visualización

Campos calculados principales:
- porcentaje de mujeres
- brecha de género relativa
- número de países con dato
- filtro de países válidos
- Top/Bottom 10 por brecha relativa

---

## Limitaciones
- Datos agregados por país: no capturan diferencias por sector/ocupación/empresa dentro de cada país.
- La disponibilidad y cobertura puede variar por país/año.
- Requiere contexto adicional (políticas educativas, estructura productiva) para interpretar causas.

---

## Tecnologías utilizadas
- Tableau Desktop Public Edition
- Eurostat datasets
- Git / GitHub

---

## Estructura del repositorio
```text
Proyecto-4/
├── README.md
├── assets/
│   ├── chunga-malaje-consulting.png
│   └── dashboard-preview.png
├── data/
│   ├── estat_hrst_st_nsecsex2.tsv
│   ├── estat_hrst_st_nsecsex2.tsv
│   ├── estat_hrst_st_nunesex.tsv
│   └── estat_hrst_st_nuneage.tsv
└── Brecha_genero_HRST_Europa_Marina_Ruth.twbx
