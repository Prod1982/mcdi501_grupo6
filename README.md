# mcdi501_grupo6
Proyecto de Estadística Computacional

MCDI501 – Estadística Computacional para la Toma de Decisiones
Grupo 6

Descripción del proyecto

Este repositorio contiene el desarrollo del proyecto de la asignatura MCDI501 – Estadística Computacional para la Toma de Decisiones, cuyo propósito es aplicar técnicas de estadística descriptiva e inferencial sobre un conjunto de datos real para apoyar la toma de decisiones basada en evidencia.

Durante la Sumativa 1 (Fase 2) se desarrolló un análisis exploratorio completo del conjunto de datos Framingham Heart Study, incorporando procedimientos de preparación de datos, estadística descriptiva, estimación de parámetros, intervalos de confianza, pruebas de hipótesis e interpretación de resultados.

El proyecto ha sido diseñado de forma progresiva, permitiendo que los resultados obtenidos en esta etapa sirvan como base para las siguientes fases del curso, orientadas a la validación estadística mediante técnicas de remuestreo y al desarrollo de modelos predictivos.

Integrantes
Pablo Rodríguez
Luiskar Espinoza
Dataset utilizado

Framingham Heart Study

El conjunto de datos contiene información clínica y demográfica utilizada para estudiar factores asociados al desarrollo de enfermedad coronaria a diez años.

Entre las principales variables se incluyen:

Edad
Sexo
Nivel educacional
Consumo de tabaco
Colesterol total
Presión arterial sistólica y diastólica
Índice de masa corporal (BMI)
Frecuencia cardíaca
Glucosa
Diabetes
Hipertensión
Riesgo de enfermedad coronaria a diez años

Variable objetivo:

TenYearCHD
Objetivo del análisis

Analizar los principales factores de riesgo cardiovascular presentes en el conjunto de datos mediante técnicas de estadística descriptiva e inferencial, con el propósito de obtener evidencia estadística que contribuya a comprender las diferencias observadas entre distintos grupos de pacientes.

Hipótesis evaluadas

Durante esta etapa del proyecto se analizaron dos hipótesis de investigación.

Hipótesis 1

H₀: La presión arterial sistólica promedio es igual entre personas que desarrollan enfermedad coronaria y aquellas que no la desarrollan.

H₁: La presión arterial sistólica promedio es diferente entre ambos grupos.

Hipótesis 2

H₀: El nivel promedio de glucosa es igual entre personas con y sin diabetes.

H₁: El nivel promedio de glucosa es diferente entre ambos grupos.

Contenido desarrollado

Durante esta etapa se implementaron los siguientes procedimientos estadísticos:

Carga y exploración inicial del conjunto de datos.
Evaluación de la calidad de los datos.
Identificación de valores faltantes y registros duplicados.
Clasificación de variables numéricas y categóricas.
Estadística descriptiva mediante medidas de tendencia central y dispersión.
Cálculo de asimetría y curtosis.
Análisis descriptivo de variables categóricas mediante frecuencias absolutas y relativas.
Construcción de histogramas, boxplots, gráficos de barras y gráficos de dispersión.
Análisis bivariado mediante correlaciones y mapa de calor.
Estimación puntual de parámetros poblacionales.
Construcción de intervalos de confianza del 95 % para variables clínicas relevantes.
Aplicación de dos pruebas de hipótesis utilizando la prueba t de Welch.
Verificación de supuestos mediante pruebas de Shapiro-Wilk y Levene.
Interpretación estadística de resultados.
Elaboración de conclusiones, limitaciones y proyección del proyecto.
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
Seaborn
SciPy
Git
GitHub
Reproducibilidad

Para reproducir completamente el análisis:

Clonar el repositorio.
Instalar las dependencias indicadas en requirements.txt.
Abrir el notebook F1_Analisis_Exploratorio.ipynb.
Ejecutar todas las celdas en orden mediante Restart & Run All.
Resultados preliminares

El análisis permitió caracterizar estadísticamente el conjunto de datos Framingham Heart Study mediante técnicas descriptivas e inferenciales.

Los resultados evidenciaron diferencias estadísticamente significativas tanto en la presión arterial sistólica entre personas con y sin enfermedad coronaria como en los niveles de glucosa entre personas con y sin diabetes. Asimismo, el análisis de correlaciones y las estimaciones mediante intervalos de confianza aportaron evidencia complementaria sobre el comportamiento de las principales variables clínicas.
Esta caracterización establece el fundamento metodológico para las siguientes etapas, enfocadas en validar la estabilidad de las estimaciones mediante remuestreo (bootstrapping / cross-validation) antes de proceder con el desarrollo de los modelos predictivos de riesgo cardiovascular.
Estos resultados constituyen la base metodológica para las siguientes etapas del proyecto, donde se validará la estabilidad de las estimaciones mediante técnicas de remuestreo y se desarrollarán modelos predictivos para el análisis del riesgo cardiovascular.
