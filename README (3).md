
# 📊 Proyecto de Análisis de Emisiones de CO₂  

**Autora**: *Sara Peguero Santos*  
**Herramientas**: Python (Jupyter Notebook), Pandas, Matplotlib, Plotly, Power BI  

---

## 🧾 Descripción del Proyecto  

Este proyecto tiene como objetivo analizar las **emisiones de CO₂ a nivel global**, explorando su evolución histórica, diferencias entre países y continentes, así como la relación con variables económicas y poblacionales.  

El trabajo se ha dividido en dos grandes fases:  
1. **Transformación, limpieza y análisis exploratorio de datos (EDA)** en **Python**.  
2. **Visualización interactiva y dashboard operativo** en **Power BI**.  

---

## 📁 Dataset  

El dataset utilizado procede de **Our World in Data (OWID)** sobre emisiones globales de CO₂, disponible públicamente.  

Variables principales:  
- `country`: País.  
- `year`: Año.  
- `population`: Población.  
- `gdp`: PIB en dólares constantes.  
- `co2`: Emisiones absolutas de CO₂ (millones de toneladas).  
- `co2_per_capita`: Emisiones per cápita (toneladas/persona).  
- `coal_co2`, `oil_co2`, `gas_co2`, `cement_co2`, `flaring_co2`: Fuentes de emisiones.  
- `continent`: Continente correspondiente a cada país.  

Tras la limpieza, el dataset quedó con **164 países**, con datos desde **1950 hasta 2022**.  

---

## 🔧 Transformación y Limpieza de Datos  

En **Python (Jupyter)** se realizaron los siguientes pasos:  
1. Eliminación de valores nulos en población, PIB y emisiones per cápita.  
2. Creación de la columna **continent** para agrupar países.  
3. Exportación de un dataset limpio `emisiones_co2_limpio.csv` para su uso en Power BI.  

---

## 📊 Análisis Descriptivo y Estadístico  

### KPIs principales  
- 🌍 **Total de países analizados**: 164  
- 📅 **Último año con datos**: 2022  
- 📈 **Emisiones globales en 2022**: 36.190 millones de toneladas  
- 🧮 **Emisiones acumuladas históricas**: 1.674.112 millones de toneladas  
- 👤 **Emisión media global per cápita**: 3,73 toneladas/persona  

### Principales hallazgos (EDA en Python)  
- Tendencia global creciente de emisiones desde 1950, con caídas notables en **2008 (crisis financiera)** y **2020 (COVID-19)**.  
- Los países con mayores emisiones absolutas en 2022: **China, EE.UU., India, Rusia, Japón, Alemania, Reino Unido, Francia, Canadá, Italia**.  
- Los países con mayores emisiones **per cápita** en 2022: **Qatar, Emiratos Árabes Unidos, Kuwait, Luxemburgo, Bahréin, Estonia, Arabia Saudí, Trinidad y Tobago, Chequia y Kazajistán**.  
- El análisis de reducción histórica reveló países que han logrado reducir más de un **60% sus emisiones desde su pico histórico** (ej. Moldavia, Ucrania, Kuwait, países bálticos).  

---

## 📉 Visualizaciones en Python  

- 📈 Evolución histórica de emisiones globales (línea).  
- 📊 Top 10 países por emisiones absolutas.  
- 📊 Top 10 países por emisiones per cápita.  
- 🌎 Evolución de emisiones por continente.  
- 🔍 Scatter interactivo (PIB per cápita vs CO₂ per cápita, con Plotly).  

---

## 📊 Dashboard en Power BI  

El dashboard operativo incluye:  

1. **KPIs globales** (número de países, emisiones totales, acumuladas, per cápita).  
2. **Evolución global de emisiones** (línea).  
3. **Evolución por continente** (línea comparativa).  
4. **Top 10 países en emisiones absolutas** (barra horizontal).  
5. **Top 10 países en emisiones per cápita** (barra horizontal).  
6. **Top 10 histórico per cápita** (media histórica por país).  
7. **Dispersión PIB per cápita vs CO₂ per cápita** (scatter con filtro por año).  
8. **Evolución comparativa de los Top 10 absolutos** (línea).  

📌 Se han incluido slicers para **año, continente y país**, así como navegación entre páginas.  

---

## 📑 Conclusiones  

- Las emisiones globales de CO₂ han seguido una tendencia creciente, impulsadas principalmente por Asia.  
- Aunque los países con más emisiones absolutas son potencias económicas e industriales, los mayores emisores **per cápita** son principalmente países del Golfo y pequeños estados ricos en recursos fósiles.  
- Existen ejemplos positivos de países que han reducido drásticamente sus emisiones tras su pico histórico, lo que demuestra que las políticas energéticas y tecnológicas pueden tener un impacto real.  
- El análisis combina **una visión macro global** con comparaciones detalladas por país y continente.  

---

## 📂 Archivos del proyecto  

- `EDA_emisiones.ipynb` → Notebook con el análisis exploratorio.  
- `emisiones_co2_limpio.csv` → Dataset limpio y transformado.  
- `Dashboard_CO2.pbix` → Dashboard interactivo en Power BI.  
- `README.md` → Este documento.  
