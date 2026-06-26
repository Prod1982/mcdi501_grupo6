# mcdi501_grupo6
Proyecto de Estadística Computacional - MCDI501 - Grupo 6

Este repositorio contiene el desarrollo del proyecto de la asignatura MCDI501 – Estadística Computacional para la Toma de Decisiones.

El objetivo del proyecto es aplicar técnicas de estadística descriptiva e inferencial para analizar un conjunto de datos de un contexto real, documentando el proceso completo de exploración, análisis e interpretación de resultados mediante herramientas computacionales en Python.

Durante la Formativa 1 se trabaja con el conjunto de datos Framingham Heart Study, orientado al estudio de factores de riesgo asociados al desarrollo de enfermedad coronaria.

Integrantes
Pablo Rodríguez
Luiskar Espinoza
Dataset utilizado

Framingham Heart Study

El conjunto de datos contiene información clínica y demográfica de pacientes, incluyendo variables relacionadas con:

Edad
Sexo
Educación
Tabaquismo
Presión arterial
Colesterol
Índice de masa corporal
Glucosa
Riesgo de enfermedad coronaria a diez años

Variable objetivo del análisis:

TenYearCHD
Objetivo del análisis

Evaluar si existe evidencia estadística que permita determinar si las personas que desarrollan enfermedad coronaria a diez años presentan una presión arterial sistólica promedio superior a aquellas que no desarrollan la enfermedad.

Hipótesis de investigación

Hipótesis nula (H₀)

La presión arterial sistólica promedio es igual en ambos grupos.

Hipótesis alternativa (H₁)

La presión arterial sistólica promedio es diferente entre ambos grupos.

Contenido desarrollado

Durante esta actividad se implementaron los siguientes procedimientos:

Carga y exploración inicial del conjunto de datos.
Identificación y clasificación de las variables.
Estadística descriptiva mediante medidas de tendencia central y dispersión.
Representaciones gráficas para caracterizar la variable de interés.
Estimación puntual de la media.
Construcción de un intervalo de confianza para la media poblacional.
Aplicación de una prueba t de Student para muestras independientes.
Interpretación estadística de los resultados obtenidos.
Elaboración de conclusiones preliminares.
Estructura del repositorio
mcdi501_grupo6/
│
├── datos/
│   └── framingham.csv
│
├── notebooks/
│   └── F1_Analisis_Exploratorio.ipynb
│
├── documentos/
│
├── resultados/
│
├── README.md
└── requirements.txt
Herramientas utilizadas
Python 3
Jupyter Notebook
Pandas
NumPy
Matplotlib
SciPy
Git
GitHub
Ejecución
Clonar el repositorio.
Instalar las dependencias indicadas en requirements.txt.
Abrir el notebook F1_Analisis_Exploratorio.ipynb.
Ejecutar todas las celdas en orden para reproducir completamente el análisis.
Resultados preliminares

El análisis estadístico evidenció diferencias significativas en la presión arterial sistólica entre los pacientes que desarrollaron enfermedad coronaria y aquellos que no la desarrollaron durante el período de seguimiento. La prueba t de Student permitió rechazar la hipótesis nula con un nivel de significancia de α = 0.05, respaldando la hipótesis de investigación planteada.

