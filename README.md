# Reto de Visión: Clasificación Automatizada con CNN

Proyecto académico de clasificación de prendas de vestir con una Red Neuronal Convolucional (CNN). El modelo utiliza el conjunto de datos **Fashion MNIST** y clasifica cada imagen en una de 10 categorías.

## Integrantes

- **Guillermo Andres Minero Alfaro:** preparación de datos, diseño y entrenamiento de la CNN.
- **Ruben Armando Vigil Mejia:** evaluación del modelo y análisis de negocio.

## Contenido del proyecto

El notebook incluye tres fases:

1. **Preparación de datos:** carga, normalización y ajuste de los tensores a `(28, 28, 1)`.
2. **Modelo y entrenamiento:** dos capas `Conv2D`, dos capas `MaxPooling2D`, capas densas y entrenamiento durante 10 épocas.
3. **Evaluación:** gráficas de accuracy y loss, evaluación sobre test, matriz de confusión y análisis de los errores más frecuentes.

## Tecnologías

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn

## Ejecución en Google Colab

1. Abrir [`main.ipynb`](main.ipynb) en Google Colab.
2. Seleccionar **Entorno de ejecución > Ejecutar todas**.
3. Esperar a que finalicen las 10 épocas de entrenamiento.
4. Revisar las gráficas, las métricas finales y la matriz de confusión.

Fashion MNIST se descarga automáticamente desde Keras. No es necesario cargar archivos de datos manualmente.

## Análisis de negocio

El modelo permite detectar qué categorías de prendas se confunden con mayor frecuencia. Estos errores pueden provocar etiquetado incorrecto, devoluciones, costos de envío, problemas de inventario y pérdida de confianza del cliente. Entre las posibles mejoras están agregar más ejemplos de las categorías problemáticas, revisar sus etiquetas y enviar predicciones de baja confianza a revisión humana.
