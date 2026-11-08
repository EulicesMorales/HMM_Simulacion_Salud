# 🏥 Modelado Probabilístico de la Evolución Clínica de Pacientes (HMM)

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![hmmlearn](https://img.shields.io/badge/hmmlearn-0.2.8-green.svg)
![License](https://img.shields.io/badge/License-MIT-purple.svg)

## 📖 Resumen del Proyecto (Abstract)
Este proyecto constituye una simulación estocástica computacional diseñada para predecir y analizar la evolución clínica de pacientes sujetos a incertidumbre diagnóstica. Al tratar las condiciones de salud orgánicas reales como variables latentes inobservables, el sistema implementa un **Modelo Oculto de Markov (HMM)** de tiempo discreto en Python. 

La herramienta permite inferir la probabilidad del deterioro clínico del paciente a partir de la emisión de síntomas ruidosos, y simula tres posibles escenarios epidemiológicos a través del Método de Monte Carlo, permitiendo evaluar el impacto probabilístico de fármacos y patógenos agresivos en un entorno *in-silico*.

## 🧬 Arquitectura Matemática
El modelo se define a través de la tupla paramétrica $\lambda = (S, V, A, B, \pi)$:
* **S (Estados Ocultos):** Saludable, Enfermo Leve, Crítico.
* **V (Observaciones):** Asintomático, Fatiga/Malestar, Síntomas Severos.
* **A (Matriz de Transición):** Variable según el escenario (Control, Tratamiento, Agresivo).
* **B (Matriz de Emisión):** Probabilidad predefinida de error diagnóstico.
* **π (Estado Inicial):** Vector probabilístico de distribución en t=0.

## 📂 Estructura del Repositorio
* `Morales_Martinez_s25.ipynb`: Script interactivo en Google Colab con el algoritmo de simulación y gráficos.
* `resultados_estadisticos.csv`: Tabla de *output* con análisis descriptivo e intervalos de confianza poblacionales (IC 95%).
* `figura1_comparacion_escenarios.png`: Gráfico comparativo de las medias poblacionales por escenario simulado.
* `figura2_evolucion_temporal.png`: Dinámica del riesgo probabilístico diario.

## 🚀 Instrucciones de Ejecución y Reproducibilidad
Para garantizar la reproducibilidad académica, el entorno fija semillas de randomización (`np.random.seed(42)`). Siga estos pasos para ejecutar el proyecto localmente:

1. **Prerrequisitos:** Asegúrese de tener Python 3.8+ instalado.
2. **Instalación de Dependencias:**
   Abra su terminal y ejecute el siguiente comando:
   ```bash
   pip install numpy pandas matplotlib scipy hmmlearn
