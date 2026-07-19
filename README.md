# Sistema de Análisis y Gestión de Riesgo Bancario

Este proyecto implementa un sistema académico de **análisis y gestión de riesgo bancario** enfocado en **observabilidad moderna**, **monitoreo proactivo**, **detección de anomalías**, **data drift**, **SLO**, **error budgets** y **simulación de incidentes**.

La solución fue desarrollada en Python y está pensada para ejecutarse en un **notebook de Visual Studio Code**, evitando la dependencia de múltiples archivos externos. El sistema utiliza **datos sintéticos**, por lo que no requiere información real de clientes ni datos confidenciales.

---

## Objetivo

Diseñar e implementar un prototipo que permita:

- entrenar un modelo de riesgo de crédito,
- monitorear su comportamiento en tiempo de ejecución,
- detectar degradación del servicio o cambios en los datos,
- generar alertas inteligentes,
- simular incidentes operativos,
- y documentar respuestas automáticas como reentrenamiento, rollback o escalamiento.

---

## Características principales

- Generación de **datos sintéticos** para riesgo crediticio.
- Entrenamiento de un modelo de clasificación para probabilidad de incumplimiento.
- Evaluación con métricas como:
  - ROC-AUC
  - Precision
  - Recall
  - F1-score
  - Log Loss
- Registro opcional de experimentos con **MLflow**.
- API de predicción preparada con **FastAPI**.
- Visualizaciones interactivas con **Plotly** e ինտերfaz en notebook.
- Monitoreo de:
  - latencia,
  - tasa de error,
  - disponibilidad,
  - drift de datos,
  - drift de predicciones.
- Definición de **SLO** y **error budgets**.
- Motor de alertas con severidad y reglas de priorización.
- Simulación de incidentes:
  - data drift,
  - incremento de latencia,
  - degradación del modelo,
  - errores de servicio.
- Ejecución de runbooks automatizados:
  - reentrenamiento,
  - rollback,
  - mitigación,
  - escalamiento.

---

## Tecnologías utilizadas

- Python 3.11+
- Jupyter Notebook
- NumPy
- Pandas
- Scikit-learn
- Plotly
- IPyWidgets
- FastAPI
- Pydantic
- Prometheus Client
- MLflow
- Joblib

---

## Estructura del proyecto

El proyecto se encuentra organizado en un único notebook principal:

- `Sistema_Riesgo_Bancario_Observabilidad.ipynb`

Este notebook contiene:

- generación de datos,
- entrenamiento,
- inferencia,
- monitoreo,
- alertas,
- simulación de incidentes,
- runbooks,
- y dashboard interactivo.

---

## Requisitos

Antes de ejecutar el notebook, asegúrate de tener instalado:

- Python 3.11 o superior
- Visual Studio Code
- Extensión de Jupyter en VS Code

---

## Instalación

Puedes instalar las dependencias desde una terminal:

```bash
pip install numpy pandas scikit-learn plotly ipywidgets fastapi uvicorn pydantic prometheus-client mlflow joblib
