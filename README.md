<p align="center">
  <img src="assets/chunga-malaje-consulting.png" width="420">
</p>

# Brecha de género en empleo HRST en Europa

![Tableau](https://img.shields.io/badge/Tableau-Data%20Visualization-blue)
![Eurostat](https://img.shields.io/badge/Data-Eurostat-orange)
![EDA](https://img.shields.io/badge/Analysis-EDA-purple)
![Dashboard](https://img.shields.io/badge/Dashboard-Interactive-blueviolet)

**Pregunta**: ¿Cómo varía la brecha de género en empleo HRST entre países y a lo largo del tiempo en Europa?

**Objetivo**: visualizar patrones territoriales y temporales para priorizar intervenciones y políticas de impulso STEM/HRST.

**Datos**: Eurostat (indicadores HRST) + preparación y análisis para visualización.

**Entregable**: dashboard interactivo en Tableau Public.

**Uso**: comparar países, detectar tendencias y apoyar decisiones basadas en evidencia.

**Ver dashboard** (Tableau Public):
https://public.tableau.com/views/Brecha_genero_HRST_Europa_Marina-Ruth/BrechadegneroenempleoHRSTenEuropa

## Autoras  
*por la igualdad de género y el cierre de la brecha digital*

<p align="center">

**Marina Martín Díaz**  
✦  

**Ruth Pérez Segovia**

</p>
---

# Objetivo del análisis

El objetivo de este proyecto es analizar la **brecha de género en el empleo HRST (Human Resources in Science and Technology)** en Europa y explorar cómo se distribuye en función de:

- el **sexo**
- la **evolución temporal**
- el **país**
- la **edad**

El análisis se materializa en un **dashboard interactivo** que permite explorar diferencias territoriales, tendencias temporales y patrones demográficos en el empleo científico-tecnológico.

---

# Preguntas analíticas

El dashboard está diseñado para responder tres preguntas principales:

**1️⃣ ¿Cómo evoluciona el empleo HRST por sexo a lo largo del tiempo?**

**2️⃣ ¿Qué países presentan mayor o menor brecha de género relativa?**

**3️⃣ ¿Cómo se distribuye el desempleo HRST según grupo de edad?**

---

# Dashboard preview

El dashboard interactivo integra análisis temporal, territorial y demográfico de la brecha de género en empleo HRST.

<p align="center">
  <img src="assets/dashboard-preview.png" width="900">
</p>

---

# Key Insights

### Participación femenina cercana al equilibrio

El porcentaje medio de mujeres en empleo HRST se sitúa aproximadamente en torno al **50 %**, lo que indica un nivel de participación cercano al equilibrio global entre hombres y mujeres.

Sin embargo, este equilibrio agregado oculta **importantes diferencias entre países**.

---

### Desigualdad territorial significativa

El análisis geográfico muestra que la brecha de género **no se distribuye de forma homogénea en Europa**.

Algunos países presentan niveles de participación femenina relativamente altos, mientras que otros muestran **brechas negativas persistentes**, lo que sugiere diferencias estructurales en políticas educativas, mercado laboral o cultura tecnológica.

---

### Persistencia de la brecha relativa

Aunque la participación femenina ha mejorado en términos absolutos, el análisis comparativo indica que **la brecha relativa sigue presente en muchos contextos**, especialmente en determinados sistemas productivos.

Esto sugiere que el crecimiento del empleo HRST no necesariamente implica una reducción automática de la desigualdad.

---

### Diferencias demográficas en el desempleo HRST

El análisis por grupos de edad muestra que el desempleo en el sector no afecta de forma uniforme a todos los perfiles demográficos.

Esto sugiere que las dinámicas de entrada y permanencia en el sector tecnológico pueden estar influidas por factores como experiencia laboral, formación o ciclos de carrera.

---

# KPIs incluidos

El panel superior del dashboard resume la situación mediante tres indicadores clave:

- **% medio de mujeres en empleo HRST**
- **Brecha media relativa**
- **Número de países con datos disponibles**

Estos indicadores proporcionan una visión rápida del estado general antes de explorar las visualizaciones en detalle.

---

# Visualizaciones del dashboard

### Evolución del empleo HRST por sexo

Gráfico de líneas que muestra la evolución temporal de la presencia de mujeres y hombres en el empleo HRST.

Permite identificar tendencias y posibles convergencias o divergencias entre ambos grupos.

---

### Brecha relativa por país

Mapa coroplético que representa la brecha de género relativa en empleo HRST para cada país europeo.

Facilita detectar patrones geográficos y diferencias territoriales.

---

### Países con mayor y menor brecha

Ranking de países que muestra los extremos en la distribución de la brecha de género relativa.

Permite comparar rápidamente qué países presentan mayor desigualdad relativa.

---

### Desempleo HRST por edad

Gráfico de barras que muestra la distribución del desempleo en HRST por grupos de edad.

Introduce una dimensión demográfica que complementa el análisis de género.

---

# Interactividad

El dashboard incluye varios elementos interactivos que permiten explorar el dataset de forma dinámica.

### Filtros

- Año
- País

### Interacciones entre visualizaciones

- Selección en el mapa filtra el ranking de países
- Selección en el mapa actualiza el resto de visualizaciones

Esto permite analizar patrones específicos dentro de cada país o periodo temporal.

---

# Fuentes de datos

Los datos proceden de **Eurostat**, utilizando tres datasets principales:

- `hrst_st_nsecsex2`  
Empleo en ciencia y tecnología por categoría HRST, actividad económica y sexo.

- `hrst_st_nunesex`  
Personas desempleadas en ciencia y tecnología por categoría y sexo.

- `hrst_st_nuneage`  
Personas desempleadas en ciencia y tecnología por categoría y grupo de edad.

Los datos se descargaron en formato **TSV**.

---

# Preparación y transformación de datos

Durante el proceso de preparación se realizaron varias tareas:

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
- Top/Bottom 10 de brecha de género

---

# Tecnologías utilizadas

- Tableau Desktop Public Edition
- Eurostat datasets
- Git
- GitHub

---

# Estructura del repositorio

Proyecto-4
│
├── README.md
│
├── assets
│   ├── chunga-malaje-consulting.png
│   └── dashboard-preview.png
│
├── data
│   ├── estat_hrst_st_nsecsex2.tsv
│   ├── estat_hrst_st_nunesex.tsv
│   └── estat_hrst_st_nuneage.tsv
│
└── Brecha_genero_HRST_Europa_Marina_Ruth.twbx



---

# Equipo del proyecto

Consultoras de datos especializadas en análisis de desigualdades estructurales y visualización de datos.

<p align="center">
  <img src="assets/Chunga_malaje_2-removebg-preview.png" width="450">
</p>


**Marina Martín Díaz**  
Data Analyst  

**Ruth Pérez Segovia**  
Data Analyst  



---

# Conclusión

El análisis muestra que, aunque la participación femenina en el empleo HRST ha aumentado en Europa, persisten diferencias significativas entre países.

El dashboard permite explorar estas diferencias desde múltiples perspectivas, combinando análisis temporal, territorial y demográfico.

Este enfoque facilita la identificación de patrones estructurales en la brecha de género dentro de los sectores científicos y tecnológicos.
