# Fase 3 – Simulación y Métodos Computacionales

Proyecto de la asignatura **MCDI501 – Estadística Computacional para la Toma de Decisiones**

## Objetivo

Esta fase del proyecto tiene como propósito validar y fortalecer los resultados obtenidos durante la Sumativa 1 mediante técnicas computacionales de remuestreo, simulación y análisis de sensibilidad.

Se implementan métodos estadísticos no paramétricos y simulaciones para evaluar la estabilidad de los parámetros estimados y la robustez de las conclusiones obtenidas previamente, proporcionando evidencia metodológica para la toma de decisiones y preparando los insumos necesarios para la Sumativa 3.

## Integrantes

- Pablo Rodríguez
- Luiskar Espinoza

## Dataset utilizado

**Framingham Heart Study**

El conjunto de datos corresponde al estudio Framingham Heart Study y contiene información clínica y demográfica de pacientes utilizada para analizar factores de riesgo asociados al desarrollo de enfermedad coronaria a diez años.

Entre las principales variables analizadas se encuentran:

- Edad
- Sexo
- Nivel educacional
- Tabaquismo
- Colesterol total
- Presión arterial sistólica
- Presión arterial diastólica
- Índice de masa corporal (BMI)
- Frecuencia cardíaca
- Glucosa
- Diabetes
- Riesgo de enfermedad coronaria a diez años

**Variable objetivo del proyecto:**

**TenYearCHD**

## Contenido desarrollado

Durante esta fase del proyecto se implementaron y validaron los siguientes procedimientos estadísticos y computacionales:

### Validación bootstrap

- Bootstrap no paramétrico con 10.000 remuestras.
- Construcción de intervalos de confianza mediante los métodos:
  - Clásico (t de Student)
  - Bootstrap Percentil
  - Bootstrap BCa
- Comparación de los intervalos de confianza obtenidos para las variables:
  - Presión arterial sistólica (sysBP)
  - Índice de masa corporal (BMI)
  - Glucosa (glucose)

### Validación de pruebas de hipótesis

- Implementación de un test de permutación con 10.000 permutaciones.
- Comparación entre el valor p obtenido mediante la prueba t de Welch (Sumativa 1) y el valor p obtenido mediante permutación.
- Interpretación de la robustez de los resultados.

### Estabilidad de correlaciones

Se evaluó la estabilidad mediante bootstrap de las principales correlaciones clínicas:

- Edad – Presión arterial sistólica.
- Presión arterial sistólica – Presión arterial diastólica.
- Índice de masa corporal – Glucosa.
- Colesterol total – Presión arterial sistólica.

### Simulación Monte Carlo

- Simulación basada en los parámetros estimados durante la Sumativa 1.
- Generación de 10.000 escenarios simulados.
- Evaluación de convergencia.
- Comparación entre datos reales y datos sintéticos.

### Análisis de sensibilidad y robustez

- Identificación de valores atípicos mediante el criterio IQR.
- Comparación entre el conjunto de datos original y el conjunto sin valores atípicos.
- Evaluación de la estabilidad de las estimaciones obtenidas.

### Preparación para la Sumativa 3

- Exportación de resultados validados.
- Generación de archivos de apoyo para la siguiente fase del proyecto.

## Estructura de la carpeta

```text
F3/
│
├── notebooks/
│   └── F3_simulacion_metodos_computacionales.ipynb
│
├── results/
│   ├── resumen_bootstrap_sysBP.csv
│   ├── comparacion_intervalos_bootstrap.csv
│   ├── correlaciones_bootstrap.csv
│   ├── resumen_montecarlo_sysBP.csv
│   ├── comparacion_datos_reales_sinteticos.csv
│   ├── analisis_sensibilidad_sysBP.csv
│   ├── datos_sinteticos_fase3.csv
│   └── (gráficos exportados)
│
└── README.md
```

## Herramientas utilizadas

- Python 3
- Jupyter Notebook
- Pandas
- NumPy
- SciPy
- Matplotlib
- Git
- GitHub

## Ejecución

Para reproducir completamente el análisis desarrollado durante esta fase se recomienda seguir los siguientes pasos:

1. Clonar el repositorio del proyecto.
2. Instalar las dependencias indicadas en el archivo `requirements.txt`.
3. Acceder a la carpeta `F3/notebooks/`.
4. Abrir el notebook `F3_simulacion_metodos_computacionales.ipynb`.
5. Ejecutar todas las celdas en orden, sin omitir ninguna.

Al finalizar la ejecución, el notebook genera automáticamente los archivos de resultados en la carpeta `results`, incluyendo tablas resumen, datos sintéticos, análisis de sensibilidad y demás evidencias utilizadas en el informe técnico.

## Principales resultados

Los métodos implementados durante esta fase permitieron validar los principales resultados obtenidos en la Sumativa 1 mediante técnicas de remuestreo y simulación computacional.

Los principales hallazgos fueron:

- Los intervalos de confianza obtenidos mediante bootstrap mostraron una alta concordancia con los intervalos clásicos calculados en la Sumativa 1.
- El test de permutación confirmó las conclusiones obtenidas mediante la prueba t de Welch, reforzando la evidencia estadística sobre la diferencia en la presión arterial sistólica entre los grupos analizados.
- Las correlaciones clínicas evaluadas presentaron intervalos de confianza bootstrap que no incluyeron el valor cero, indicando asociaciones estables dentro del conjunto de datos.
- La simulación Monte Carlo reprodujo adecuadamente el comportamiento observado de la presión arterial sistólica, mostrando convergencia y resultados consistentes con los datos originales.
- El análisis de sensibilidad evidenció que la eliminación de valores atípicos produjo cambios reducidos en las estimaciones, indicando que las conclusiones obtenidas son robustas frente a la presencia de observaciones extremas.

## Próxima etapa

Los resultados obtenidos durante esta fase constituyen la base metodológica para el desarrollo de la Sumativa 3 del proyecto.

En la siguiente etapa se abordará la construcción y evaluación de modelos de regresión logística, el tratamiento de datos faltantes mediante distintas estrategias de imputación y la validación de la estabilidad de los modelos utilizando técnicas de bootstrap, dando continuidad al proceso de análisis iniciado en las fases anteriores.