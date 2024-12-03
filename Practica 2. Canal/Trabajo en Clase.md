
# Práctica 2: Análisis de Señales con Variación de Ruido y Frecuencia de Corte

## Descripción
La **Práctica 2** se centra en el análisis de señales bajo diferentes condiciones de ruido y variación de parámetros como la frecuencia de entrada y la frecuencia de corte. En la **Parte A**, se estudió cómo elegir correctamente la frecuencia de corte de una señal y cómo el ruido afecta su comportamiento. En la **Parte B**, se complementó este análisis utilizando herramientas como el analizador de espectro y el osciloscopio para observar cómo varía la potencia de la señal dependiendo de los parámetros ajustados.

## Parte A: Análisis de Frecuencia de Corte y Ruido
### Objetivo:
- Estudiar el efecto de la **frecuencia de corte** en la transmisión de una señal con ruido.
- Analizar cómo varían las características de la señal al cambiar parámetros como:
  - **Frecuencia de entrada**.
  - **Amplitud del ruido**.
  - **Frecuencia de corte**.

### Procedimiento:
1. Se generó una señal de entrada con ruido superpuesto, variando tanto la **frecuencia de la señal** como la **amplitud del ruido**.
2. Se utilizó un filtro con frecuencia de corte ajustable para observar cómo afectaba la selección de la frecuencia de corte a la salida de la señal.
3. Se analizaron los efectos del ruido en función de los parámetros ajustados y se determinó cómo seleccionar la frecuencia de corte óptima para minimizar su impacto.

### Resultados:
- Se observó que una frecuencia de corte mal seleccionada puede atenuar señales deseadas o permitir que el ruido domine la señal.
- La amplitud del ruido afecta significativamente la claridad de la señal, pero puede ser mitigada al ajustar correctamente la frecuencia de corte.

## Parte B: Análisis en el Dominio del Espectro y Tiempo
### Objetivo:
- Complementar el análisis realizado en la Parte A utilizando un **analizador de espectro** y un **osciloscopio**.
- Observar cómo varía la potencia de la señal en función de:
  - **Presencia o ausencia de ruido**.
  - **Frecuencia de la señal**.
  - **Frecuencia de corte**.
  - **Frecuencia de la portadora**.
  - **Amplitud del ruido y señal**.
  - **Ganancia del transmisor**.

### Procedimiento:
1. Se inyectó la señal generada en la Parte A en el analizador de espectro y osciloscopio.
2. Se ajustaron parámetros como:
   - **Frecuencia de la señal de entrada**.
   - **Amplitud del ruido y señal**.
   - **Frecuencia de corte del filtro**.
   - **Frecuencia de la portadora**.
   - **Ganancia del transmisor**.
3. Se compararon las mediciones de potencia y el comportamiento de la señal en presencia y ausencia de ruido.

### Resultados:
- En el **analizador de espectro**, se observó cómo la potencia de la señal variaba al introducir ruido, mostrando un incremento significativo en el ruido de fondo.
- En el **osciloscopio**, se visualizó cómo el ruido afecta la forma de onda de la señal en el dominio del tiempo.
- Se concluyó que ajustar correctamente la frecuencia de corte y la ganancia del transmisor es clave para mantener la integridad de la señal.

## Archivos del Proyecto:
- **`Practica_2_ParteA.grc`**: Archivo de GNU Radio con la configuración utilizada en la Parte A para generar y analizar señales con ruido.
- **`Practica_2_ParteB.grc`**: Archivo de GNU Radio configurado para el análisis complementario con el analizador de espectro y osciloscopio.
- **`Practica_2_ParteA.py`**: Script en Python generado para la ejecución de la Parte A.
- **`Practica_2_ParteB.py`**: Script en Python generado para la ejecución de la Parte B.

## Conclusiones:
- La selección adecuada de la frecuencia de corte es esencial para minimizar el impacto del ruido en las señales.
- Herramientas como el analizador de espectro y el osciloscopio permiten observar de forma clara cómo varían las características de una señal, como su potencia y forma de onda, en función de parámetros ajustables.
- Ajustar
