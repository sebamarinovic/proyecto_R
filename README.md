# Análisis Térmico y Gestión de Mantenimiento EP-110

Este repositorio contiene el análisis realizado sobre el desempeño térmico de los enfriadores EP-110 en las plantas de limpieza de gases GCP-2 y GCP-4. El análisis se enfoca en evaluar el rendimiento térmico, identificar equipos críticos, detectar ciclos de mantenimiento y analizar la correlación entre la temperatura de los gases y el diferencial de temperatura del agua (ΔT Agua).

## Descripción del Proyecto

El objetivo principal de este análisis es optimizar el control térmico y la gestión del mantenimiento de los enfriadores EP-110. Se utilizaron datos simulados desde 2015 hasta 2025 para investigar el comportamiento térmico de estos enfriadores, lo cual es crucial para optimizar los procesos de limpieza de gases.

**Pregunta de investigación:**

> ¿Qué equipos EP-110 presentan bajo desempeño térmico (ΔT Agua < 4°C), cuántos ciclos completos de mantenimiento se han realizado por año, y qué correlación existe entre la temperatura de gases de salida (GCP) y ΔT Agua?

## Estructura del Repositorio

El repositorio está organizado de la siguiente manera:

* `README.md`: Este archivo, que proporciona una descripción general del proyecto.
* `Informe_Catedra1_Final.Rmd`: El documento RMarkdown que contiene el código del análisis y la narrativa del informe.
* `data_extrapolated.csv`: Conjunto de datos con registros horarios de los enfriadores EP-110.
* `temp_gcp_data_extrapolated.csv`: Conjunto de datos con registros diarios de la temperatura de los gases GCP.

## Contenido del Documento RMarkdown (Informe\_Catedra1\_Final.Rmd)

El documento RMarkdown incluye las siguientes secciones:

1.  **Definición del Problema / Objetivo:** Descripción del problema y la pregunta de investigación.
2.  **Introducción:** Contexto del análisis, descripción de los datos y las variables.
    * **Irregularidades de los datos:** Detalle de los problemas encontrados en los datos.
3.  **Pre-procesamiento de Datos:** Pasos realizados para limpiar y preparar los datos para el análisis.
4.  **Análisis Exploratorio de Datos (EDA):** Visualizaciones y análisis descriptivo de los datos.
    * Distribución de ΔT Agua por Equipo (Boxplots)
    * Histograma de ΔT Agua
    * Correlación entre ΔT Agua y Temperatura Gas Salida GCP´s
    * Comparación Temperatura de Salida Gas Trenes y ΔT Agua EP-110
5.  **Planificación del Proyecto:** Marco teórico, metodología y entregables del proyecto.
6.  **Interpretación de Resultados:** Análisis de los resultados del EDA y los ciclos de mantenimiento.
    * Equipos Críticos (GCP-2 y GCP-4)
    * Ciclos de Mantenimiento
7.  **Conclusiones:** Resumen de los hallazgos principales y respuestas a la pregunta de investigación.
8.  **Propuesta de Función Modular para el Examen:** Descripción de la función `analisis_ep110()` y propuesta de un dashboard de Shiny para el monitoreo y gestión del mantenimiento.

## Datos y Complementos

Los datos necesarios para ejecutar el análisis se encuentran en los archivos `data_extrapolated.csv` y `temp_gcp_data_extrapolated.csv`.

**Dependencias de R:**

El análisis requiere las siguientes librerías de R:

* `tidyverse`
* `lubridate`
* `hexbin`
* `scales`

## Visualizaciones

Algunas de las visualizaciones clave incluidas en el análisis son:

* Boxplots de la distribución de ΔT Agua por equipo y planta.
* Histogramas de ΔT Agua por planta.
* Gráficos de dispersión para la correlación entre ΔT Agua y la temperatura de los gases.
* Gráficos de series temporales comparando la temperatura de salida de los gases y el ΔT Agua.

## Uso

Para replicar el análisis:

1.  Clona el repositorio a tu máquina local.
2.  Asegúrate de tener R y RStudio instalados.
3.  Instala las librerías de R necesarias.
4.  Abre el archivo `Informe_Catedra1_Final.Rmd` en RStudio y ejecútalo.

## Autor

Sebastián Marinovic
