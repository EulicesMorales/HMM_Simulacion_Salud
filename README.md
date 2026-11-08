# Modelado Probabilístico de la Evolución Clínica (HMM)

## Descripción
Este repositorio contiene la implementación en Python de un Modelo Oculto de Markov (HMM) para simular la evolución clínica de pacientes en 3 escenarios diferentes (Evolución Natural, Tratamiento Efectivo y Variante Agresiva).

## Archivos del Repositorio
* `Morales_Martinez_s25.ipynb`: Código fuente de la simulación con semillas fijas.
* `resultados_estadisticos.csv`: Tabla con las métricas extraídas (Media, Desviación Estándar, Mínimo, Máximo e Intervalos de Confianza).
* `figura1_comparacion_escenarios.png` y `figura2_evolucion_temporal.png`: Gráficos de resultados.

## Instrucciones de Ejecución (Reproducibilidad)
Para ejecutar este proyecto de manera local o en la nube:
1. Asegúrese de tener instalado Python 3.
2. Instale las librerías necesarias ejecutando: `pip install numpy pandas matplotlib scipy hmmlearn`
3. Abra el archivo principal y ejecute todas las celdas. La semilla aleatoria está fijada (`seed=42`) para garantizar que los resultados sean reproducibles.
