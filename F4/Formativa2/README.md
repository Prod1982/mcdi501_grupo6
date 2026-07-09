# Formativa 2 – Modelamiento Predictivo mediante Regresión Logística

## MCDI501 – Estadística Computacional para la Toma de Decisiones

**Magíster en Ciencia de Datos e Inteligencia Artificial**

**Universidad Andrés Bello**

---

## Descripción

Este directorio contiene el desarrollo de la **Formativa 2** correspondiente a la Fase 4 del proyecto de la asignatura **MCDI501 – Estadística Computacional para la Toma de Decisiones**.

En esta etapa se construye el primer modelo predictivo mediante **regresión logística**, utilizando el conjunto de datos **Framingham Heart Study** e integrando explícitamente los resultados obtenidos durante la Sumativa 1 y la Sumativa 2.

El notebook fue desarrollado siguiendo criterios de reproducibilidad, trazabilidad metodológica y documentación, preparando la base para la Evaluación Sumativa 3.

---

## Objetivo

Desarrollar un modelo de regresión logística para predecir el riesgo de enfermedad coronaria a diez años, utilizando variables clínicas previamente validadas mediante análisis estadísticos, bootstrap, pruebas de permutación y simulaciones desarrolladas en las fases anteriores del proyecto.

---

## Integración con las fases anteriores

### Sumativa 1

Se utilizaron los principales resultados obtenidos durante el análisis exploratorio de datos:

- Estadística descriptiva.
- Estimación puntual.
- Intervalos de confianza.
- Pruebas de hipótesis.
- Identificación de valores faltantes.
- Identificación de valores atípicos.
- Correlaciones entre variables clínicas.

### Sumativa 2

Se incorporaron los resultados obtenidos mediante técnicas de remuestreo y simulación:

- Bootstrap de intervalos de confianza.
- Test de permutación.
- Bootstrap de correlaciones.
- Simulación Monte Carlo.
- Análisis de robustez.
- Validación de parámetros estadísticos.

Toda esta información fue utilizada para justificar la selección de variables predictoras y la construcción del modelo de clasificación.

---

## Variables utilizadas

El modelo fue construido utilizando las siguientes variables predictoras:

- age
- sysBP
- BMI
- glucose
- male

Variable objetivo:

- TenYearCHD

La selección de variables se fundamentó en la evidencia estadística obtenida durante las Sumativas 1 y 2, considerando además el análisis de multicolinealidad mediante el Factor de Inflación de la Varianza (VIF).

---

## Modelo desarrollado

Durante esta actividad se implementaron las siguientes etapas:

- Preparación del conjunto de datos.
- Tratamiento de valores faltantes mediante eliminación de registros (`dropna`).
- División entrenamiento/prueba (70 % / 30 %).
- Estandarización de variables numéricas.
- Diagnóstico de multicolinealidad mediante VIF.
- Ajuste del modelo de regresión logística.
- Interpretación de coeficientes.
- Cálculo de Odds Ratios.
- Evaluación mediante matriz de confusión.
- Cálculo de Accuracy, Precision, Recall y F1-score.
- Evaluación mediante Curva ROC y Área Bajo la Curva (AUC).
- Exportación automática de resultados y figuras.

---

## Resultados obtenidos

El modelo presentó un desempeño predictivo aceptable, alcanzando un **AUC de 0.7468**, lo que indica una adecuada capacidad para discriminar entre pacientes que desarrollan y no desarrollan enfermedad coronaria a diez años.

El análisis mostró que las variables **age**, **sysBP**, **glucose** y **male** fueron estadísticamente significativas, mientras que **BMI** no presentó evidencia suficiente para considerarse un predictor significativo en este primer modelo.

La evaluación del desempeño evidenció además que el conjunto de datos presenta un importante desbalance entre clases, reflejado en un valor bajo de Recall, situación que será abordada en la siguiente etapa del proyecto.

---

## Estructura del directorio

```text
Formativa2/
│
├── notebooks/
│   └── F2_Modelamiento_Predictivo.ipynb
│
├── figures/
│   ├── curva_roc.png
│   └── matriz_confusion.png
│
├── results/
│   ├── metricas_modelo.csv
│   ├── odds_ratio.csv
│   ├── predicciones_modelo.csv
│   ├── resumen_modelo.csv
│   └── vif.csv
│
└── README.md
```

---

## Requisitos

El notebook fue desarrollado utilizando Python y las siguientes librerías principales:

- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Statsmodels

---

## Ejecución

1. Clonar el repositorio.
2. Instalar las dependencias del proyecto.
3. Abrir el notebook ubicado en:

```
Formativa2/notebooks/F2_Modelamiento_Predictivo.ipynb
```

4. Ejecutar todas las celdas en orden.

El notebook genera automáticamente las figuras y archivos CSV dentro de las carpetas **figures** y **results**.

---

## Trabajo futuro

La Formativa 2 constituye la base para la **Evaluación Sumativa 3**, donde se implementarán:

- Estrategias de imputación de datos faltantes.
- Comparación entre distintos modelos de regresión logística.
- Bootstrap para evaluar la estabilidad de coeficientes y Odds Ratios.
- Comparación del impacto de las estrategias de imputación sobre el desempeño predictivo.
- Construcción del modelo final del proyecto.