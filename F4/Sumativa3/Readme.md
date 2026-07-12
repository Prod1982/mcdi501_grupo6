# Evaluación Sumativa 3 – Proyecto Final Integrado

## Curso

MCDI501 - Estadística Computacional para la Toma de Decisiones

Universidad Andrés Bello

---

## Integrantes

- Pablo Andrés Rodríguez López
- (Completar con el resto del grupo)

---

# Objetivo

Desarrollar el proyecto final integrado del curso mediante la implementación de modelos de regresión lineal y regresión logística, incorporando los resultados obtenidos en las Sumativas 1 y 2 para fundamentar todas las decisiones metodológicas relacionadas con el tratamiento de datos, selección de variables, validación de modelos y evaluación del desempeño predictivo.

---

# Descripción del proyecto

El proyecto utiliza el conjunto de datos **Framingham Heart Study**, cuyo objetivo consiste en predecir la probabilidad de desarrollar enfermedad coronaria a diez años (TenYearCHD).

Durante esta etapa se integran los resultados obtenidos previamente en las Sumativas 1 y 2 para construir un flujo completo de análisis que incluye:

- manejo inteligente de datos faltantes;
- imputación mediante regresión lineal;
- comparación de estrategias de imputación;
- construcción de modelos de regresión logística;
- selección de variables mediante Stepwise y criterio AIC;
- evaluación del desempeño predictivo;
- validación mediante bootstrap;
- diagnóstico del modelo final;
- análisis comparativo del impacto de las estrategias de imputación.

---

# Estructura del proyecto

```
Sumativa3/

│

├── notebooks/

│ └── S3_Proyecto_Final_Integrado.ipynb

│

├── figures/

│ ├── roc_modelo_final.png

│ └── ...

│

├── results/

│ ├── comparacion_modelos.csv

│ ├── comparacion_imputacion.csv

│ ├── bootstrap_coeficientes.csv

│ └── bootstrap_odds_ratio.csv

│

└── README.md
```

---

# Flujo metodológico

El desarrollo del proyecto sigue la secuencia:

**Sumativa 1**

- análisis exploratorio;
- estadística descriptiva;
- estadística inferencial;
- correlaciones;
- detección de valores faltantes y outliers.

↓

**Sumativa 2**

- bootstrap;
- pruebas de permutación;
- simulación Monte Carlo;
- análisis de robustez.

↓

**Sumativa 3**

- imputación de datos faltantes;
- construcción de tres modelos logísticos;
- selección del modelo final;
- bootstrap de coeficientes;
- diagnóstico del modelo;
- comparación de estrategias de imputación.

---

# Principales librerías utilizadas

- pandas
- numpy
- matplotlib
- scipy
- scikit-learn
- statsmodels

---

# Reproducibilidad

El notebook fue desarrollado utilizando semillas aleatorias (`random_state = 42`) para garantizar la reproducibilidad de los resultados.

Todos los resultados exportados automáticamente se almacenan en la carpeta **results/**.

Las figuras utilizadas en el informe final se almacenan en la carpeta **figures/**.

---

# Productos entregados

La Sumativa 3 contempla la entrega de los siguientes productos:

- Notebook ejecutable.
- Informe técnico integrado (PDF).
- Presentación del proyecto.
- Repositorio GitHub completo.

---

# Conclusiones

El proyecto integra de forma coherente los resultados obtenidos durante las tres evaluaciones del curso, demostrando la aplicación de técnicas de análisis exploratorio, inferencia estadística, simulación, remuestreo y modelamiento predictivo para apoyar la toma de decisiones basada en datos.

La integración metodológica entre S1, S2 y S3 permitió construir un modelo predictivo robusto, validado mediante bootstrap y sustentado en evidencia estadística obtenida durante todas las etapas del proyecto.