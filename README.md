# Práctica 1: Introducción a GNU Radio y Reconocimiento de Equipos

## Descripción
La **Práctica 1** está dividida en dos partes principales que nos introducen al uso de **GNU Radio**, un entorno de desarrollo para procesar señales de radiofrecuencia, y el reconocimiento de equipos mediante la comparación de señales medidas con señales generadas. En la **Parte A**, trabajamos con señales de diferentes formas (seno, triangular, etc.) y analizamos cómo la variación de parámetros como la frecuencia y la frecuencia de muestreo afecta a las señales. En la **Parte B**, realizamos un reconocimiento entre las amplitudes medidas y las generadas para diferentes frecuencias, utilizando herramientas como **MATLAB** para la comparación y el cálculo del porcentaje de error.

## Parte A: Introducción a GNU Radio
### Objetivo:
- **Inyección de señales**: Generamos señales de diferentes tipos (seno, triangular, etc.) en GNU Radio.
- **Análisis de la señal**: Examinamos la **amplitud** y **potencia en dB** de las señales generadas.
- **Impacto de la variación de parámetros**: Modificamos parámetros como la **frecuencia** y la **frecuencia de muestreo** para observar cómo estos afectan a las señales.

### Procedimiento:
1. **Generación de señales**: Usamos bloques de GNU Radio como "Signal Source" para generar señales de tipo seno y triangular.
2. **Análisis en tiempo y frecuencia**: Utilizamos bloques de análisis como "Scope Sink" para visualizar las señales en el dominio del tiempo y "FFT Sink" para observarlas en el dominio de la frecuencia.
3. **Variación de parámetros**: Experimentamos con valores como la frecuencia de la señal y la frecuencia de muestreo para estudiar su efecto en las características de la señal, como la amplitud y la potencia.

### Resultados:
- Se observó cómo la amplitud de las señales variaba al cambiar la frecuencia y la frecuencia de muestreo.
- Las señales generadas fueron analizadas en términos de su potencia en dB y se pudo ver cómo estas propiedades cambiaban conforme ajustábamos los parámetros de la señal.

## Parte B: Reconocimiento de Equipos
### Objetivo:
- **Reconocimiento de señales**: Comparamos las amplitudes de las señales generadas (desde la Parte A) con las amplitudes medidas.
- **Uso de MATLAB**: Usamos MATLAB para comparar las señales y calcular el porcentaje de error en las mediciones de amplitud para diferentes frecuencias.

### Procedimiento:
1. **Medición de amplitudes**: Con GNU Radio, medimos las amplitudes de las señales generadas para varias frecuencias.
2. **Análisis en MATLAB**: Exportamos los resultados de las mediciones a MATLAB, donde comparamos las amplitudes medidas contra las generadas para diferentes frecuencias.
3. **Cálculo del error**: En MATLAB, calculamos el porcentaje de error entre las amplitudes medidas y las amplitudes generadas.

### Resultados:
- Se calcularon los porcentajes de error entre las amplitudes medidas y las generadas para distintas frecuencias.
- Los resultados fueron analizados para determinar la precisión de las mediciones y la posible desviación en función de la frecuencia.

## Archivos del Proyecto:
- **`Lab_comu_1.py`**: Script en Python para la Parte A y B de la práctica, contiene el flujo de trabajo en GNU Radio.
- **`Lab_comu_I_parte1.grc`**: Archivo GRC con la configuración de la señal generada en la Parte A.
- **`Lab_comu_I_parte2.grc`**: Archivo GRC adicional para la Parte A, experimentando con diferentes parámetros de la señal.
- **`Lab_comu_I_parte3.grc`**: Otro archivo GRC de la Parte A, donde se modificaron otros parámetros de la señal.
- **`Lab_comu_I_parte4.grc`**: Continuación de los experimentos con señales en la Parte A.
- **`Lab_comu_I_parte5.grc`**: Archivo GRC con nuevas configuraciones de señales para la Parte A.
- **`Lab_comu_I_parte6.grc`**: Archivo adicional de experimentación con señales en GNU Radio.
- **`Monica_Peña_Kmila_Contreras_E1C_G4.py`**: Script de Python con la implementación del análisis de la Parte B, utilizado para la comparación de amplitudes generadas y medidas y cálculo del porcentaje de error.

