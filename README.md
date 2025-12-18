# Análisis Descriptivo de Rotación de Talento - Insights y Descubrimientos

## 📋 Descripción General

Este proyecto realiza un **análisis descriptivo profundo** de la rotación de talento en una empresa con **2,534 ejecutivos**, enfocándose en descubrir **insights clave** sobre las causas y consecuencias de la desvinculación voluntaria por dimisión. El análisis se estructura bajo el **marco de las 4 preguntas analíticas** (Descriptivas, Diagnósticas, Predictivas y Prescriptivas) para proporcionar una visión integral del fenómeno.

## 🎯 Objetivos del Proyecto

### Pregunta Descriptiva: "¿Qué está pasando?"
Caracterizar y mapear la rotación de talento en la organización:
- Identificar las **áreas de la empresa con mayor índice de rotación**
- Calcular el **Pareto 80/20** de áreas críticas
- Determinar el porcentaje de personas desvinculadas por **dimisión voluntaria** por departamento

### Pregunta Diagnóstica: "¿Por qué está pasando?"
Entender los factores detrás de la rotación:
- Analizar **variables influyentes** en la desvinculación voluntaria
- Identificar patrones y correlaciones en los departamentos de mayor riesgo
- Determinar la variable con **mayor influencia** en cada área crítica

### Pregunta Predictiva: "¿Qué pasará si no actuamos?"
Cuantificar el impacto financiero:
- Estimar el **costo de pérdida de know-how** por desvinculación
- Calcular los **gastos de re-contratación y onboarding**
- Proyectar el **costo financiero total** para el cierre del año fiscal
- Identificar áreas de mayor impacto económico

### Pregunta Prescriptiva: "¿Qué deberíamos hacer?"
Proponer soluciones optimizadas:
- Analizar el **mix óptimo de incremento salarial vs. beneficios no monetarios**
- Maximizar la **retención del talento joven**
- Minimizar costos de intervención
- Proporcionar recomendaciones accionables por área

## 📊 Datos y Fuentes

### Archivos de Datos Disponibles

| Archivo | Descripción |
|---------|-------------|
| `data_empleados_limpia.csv` | Base de datos maestra de empleados con todas sus características |
| `data_analisis_ventas_total_2534_ejecutivos.csv` | Datos de ventas totales (2,534 ejecutivos) |
| `data_analisis_ventas_quedaron_2534_ejecutivos.csv` | Datos de ventas - empleados que permanecen |
| `data_analisis_ventas_renunciaron_2534_ejecutivos.csv` | Datos de ventas - empleados que se desvincularon |
| `bubble_grafic.csv` | Datos preparados para visualizaciones tipo bubble chart |

### Dimensiones Analíticas

El análisis examina variables como:
- **Departamento/Área** de la empresa
- **Tipo de desvinculación** (dimisión voluntaria vs. otros)
- **Variables de performance** (ventas, productividad)
- **Características demográficas** (experiencia, nivel, edad)
- **Indicadores financieros** (salario, comisiones, incentivos)

## 🔍 Estructura del Análisis

El Jupyter Notebook `analisis_descriptivo_insights.ipynb` está organizado en 4 secciones principales:

### 1️⃣ Análisis Descriptivo
- Carga y exploración de datos
- Estadísticas descriptivas de rotación por área
- Cálculo del **Pareto 80/20** de departamentos críticos
- Visualización de distribuciones y tendencias

### 2️⃣ Análisis Diagnóstico
- Correlación entre variables y desvinculación voluntaria
- Análisis de variables influyentes por departamento
- Identificación de patrones diferenciados
- Segmentación de riesgo

### 3️⃣ Análisis Predictivo
- Estimación de costos por desvinculación
- Proyección de impacto financiero anual
- Cálculo de ROI en retención
- Modelado de escenarios

### 4️⃣ Análisis Prescriptivo
- Recomendaciones de política de compensación
- Optimización del mix salario/beneficios no monetarios
- Estrategias de retención de talento joven
- Plan de acción por área

## 📈 Visualizaciones Principales

El análisis incluye:
- **Gráficos Pareto** de rotación por departamento
- **Bubble charts** para análisis multidimensional
- **Heatmaps** de correlación con desvinculación
- **Barras comparativas** de cost-benefit
- **Proyecciones** de impacto financiero

## 🛠️ Requisitos Técnicos

### Lenguaje y Entorno
- **Lenguaje**: R
- **Entorno**: Jupyter Notebook
- **Formato**: `.ipynb`

### Librerías Utilizadas (R)
```r
# Data manipulation
library(dplyr)
library(tidyr)
library(data.table)

# Visualization
library(ggplot2)
library(plotly)
library(corrplot)

# Analysis
library(psych)
library(car)
library(cluster)
```

## 🚀 Cómo Usar este Proyecto

### 1. Preparación del Entorno

```bash
# Navega al directorio del proyecto
cd /Users/k4t3/Coding/La-Salle/storytelling-ratio-renuncia

# Asegúrate de tener R y Jupyter instalados
# Con conda:
conda create -n storytelling r-essentials jupyter r-tidyverse r-ggplot2
conda activate storytelling
```

### 2. Ejecutar el Análisis

```bash
# Abre el notebook en Jupyter
jupyter notebook analisis_descriptivo_insights.ipynb
```

### 3. Interpretar los Resultados

Cada sección del notebook proporciona:
- **Tablas de resumen** con métricas clave
- **Visualizaciones** interpretables
- **Hallazgos principales** en markdown
- **Recomendaciones** accionables

## 📌 Hallazgos Clave (Esperados)

El análisis responde preguntas críticas como:

1. ¿Cuáles son los **3-5 departamentos** con mayor rotación?
2. ¿Qué porcentaje concentran estos en el total de desvinculaciones?
3. ¿Cuáles son los **factores más influyentes** en la decisión de dimisión?
4. ¿Cuál es el **impacto financiero** anual de esta rotación?
5. ¿Qué **intervenciones** son más costo-efectivas?

## 📊 Métricas Clave

### Rotación
- **Índice de rotación por área** (%)
- **Desvinculaciones voluntarias** (dimisiones)
- **Ratio reemplazo/retención**

### Impacto Financiero
- **Costo de conocimiento perdido**
- **Gastos de re-contratación**
- **Costo de onboarding**
- **Pérdida de productividad**

### Retención
- **Tasa de retención por intervención**
- **ROI de beneficios vs. salario**
- **Costo unitario de retención**

## 📁 Estructura de Archivos

```
storytelling-ratio-renuncia/
├── README.md                                          # Este archivo
├── analisis_descriptivo_insights.ipynb               # Análisis completo
├── data_empleados_limpia.csv                         # Datos maestros
├── data_analisis_ventas_total_2534_ejecutivos.csv    # Ventas totales
├── data_analisis_ventas_quedaron_2534_ejecutivos.csv # Ventas (permanencia)
├── data_analisis_ventas_renunciaron_2534_ejecutivos.csv # Ventas (rotación)
├── bubble_grafic.csv                                 # Datos para visualizaciones
├── Dockerfile.storytelling                           # Configuración Docker
├── LICENSE                                            # Licencia
└── .gitignore                                         # Configuración git
```

## 🔐 Tecnología y Reproducibilidad

### Docker
Para asegurar reproducibilidad del análisis:

```bash
# Construir imagen
docker build -t storytelling:latest -f Dockerfile.storytelling .

# Ejecutar contenedor
docker run -p 8888:8888 storytelling:latest
```

### Versiones de Librerías
Se recomienda usar las versiones especificadas en el Dockerfile para garantizar consistencia en resultados.

## 🎓 Metodología

El proyecto sigue el **framework de Analytics de 4 Preguntas**:

```
DESCRIPTIVA → DIAGNÓSTICA → PREDICTIVA → PRESCRIPTIVA
¿Qué?         ¿Por qué?      ¿Qué pasará?  ¿Qué hacer?
```

Este enfoque garantiza que:
- Los descubrimientos están **basados en datos**
- Las recomendaciones son **respaldadas por evidencia**
- Las intervenciones son **orientadas a resultados**

## 📞 Contacto y Contribuciones

Este proyecto fue desarrollado como análisis de rotación de talento para:
- **Institución**: La Salle
- **Tema**: Storytelling - Análisis de Ratio de Renuncia

Para preguntas o mejoras, contacta al desarrollador del proyecto.

## 📄 Licencia

Este proyecto está bajo licencia (consulta el archivo `LICENSE` para detalles).

---

**Última actualización**: Diciembre 2025

**Estado**: Análisis activo y en revisión

**Proximamente**: 
- [ ] Integración de modelos predictivos avanzados
- [ ] Dashboard interactivo de resultados
- [ ] Reportes automatizados mensuales
- [ ] Análisis de benchmarking sector
