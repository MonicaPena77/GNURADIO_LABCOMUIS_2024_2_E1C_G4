# Práctica 3: Modulaciones Lineales y Análisis de Señales Moduladas

## Descripción
La **Práctica 3** está centrada en la **modulación de amplitud (AM)**, con el objetivo de entender y analizar las envolventes complejas de las señales moduladas. En la **Parte A**, se construyeron diferentes modelos para la envolvente compleja de modulaciones lineales, utilizando herramientas de análisis en el dominio del tiempo y frecuencia. En la **Parte B**, se amplió el análisis mediante señales aleatorias, tanto de audio como binarias, para explorar el comportamiento de la modulación en diferentes configuraciones.

## Parte A: Construcción de la Envolvente Compleja y Análisis de Modulador AM
### Objetivo:
- **Construcción del modelo de la envolvente compleja**: Se desarrolló un modelo que representa la envolvente compleja de una señal modulada en amplitud.
- **Análisis de la señal modulada**: Se examinaron tres configuraciones de modulación (ka*Am = 1, ka*Am > 1, ka*Am < 1) y se analizaron las señales generadas en el dominio del tiempo (con el osciloscopio) y frecuencia (con el analizador de espectro).
- **Cálculo de la potencia de la señal envolvente compleja**: Se calcularon y compararon las potencias de la señal envolvente y de la señal modulada.

### Procedimiento:
1. Se construyó el bloque jerárquico en GNU Radio para la modulación AM con entrada \(m(t)\) y salida \(g(t)\), usando los bloques generados previamente en prácticas anteriores.
2. Se conectó la salida del **USRP** al bloque **Modulador de Amplitud** y se observó la señal modulada \(s(t)\).
3. Se realizaron mediciones de la señal \(s(t)\) en el dominio del tiempo (osciloscopio) y en el dominio de la frecuencia (analizador de espectro).
4. Se consideraron tres casos con distintos valores de \(ka * Am\) para analizar cómo el índice de modulación afecta la señal.

### Resultados:
- **Medición de potencia**: Se midió la potencia de la señal envolvente compleja \(g(t)\) y de la señal modulada \(s(t)\), comparando los resultados con el bloque de potencia medido en la práctica anterior.
- Se observaron las bandas laterales de la señal modulada, y se usaron los marcadores en el analizador de espectro para obtener los niveles de potencia.

## Parte B: Modulación de Amplitud con Señales Aleatorias
### Objetivo:
- **Modulación con señales aleatorias**: En esta fase se utilizaron señales aleatorias como parte del mensaje para la modulación en amplitud.
- **Evaluación de señales de audio y binarias**: Se realizaron pruebas con una señal de audio y una señal binaria en diferentes configuraciones de modulación (modulación al 75%, 100% y 150%).

### Procedimiento:
1. **Generación de señales aleatorias**:
   - **Caso 1**: Una señal de audio.
   - **Caso 2**: Una señal binaria.
   
2. **Modulación AM**: Se utilizó el bloque de modulación AM de la Parte A para modular estas señales aleatorias.
3. **Análisis en osciloscopio y analizador de espectro**:
   - Se midió el **índice de modulación absoluto** en el osciloscopio para varios valores de modulación.
   - Se estimó el **ancho de banda** de la señal modulada en el analizador de espectro.

### Resultados:
- **Índice de Modulación**:
  - Para cada caso, se observó el índice de modulación absoluto \(ka \times Am\) y se verificó cómo varía la modulación con diferentes configuraciones.
  
  **Casos de Modulación**:
  1. **Caso 1** (75% modulación): Frecuencia de portadora 300 MHz, Ganancia TX = 10 dB, 10 muestras por símbolo.
  2. **Caso 2** (100% modulación): Frecuencia de portadora 250 MHz, Ganancia TX = 15 dB, 5 muestras por símbolo.
  3. **Caso 3** (150% modulación): Frecuencia de portadora 350 MHz, Ganancia TX = 20 dB, 2 muestras por símbolo.

- **Análisis del tiempo de bit y banda ancha**:
  - **Tiempo de Bit**: A medida que aumentaba la modulación, el tiempo por bit disminuía, lo que reflejaba una transmisión de datos más rápida.
  - **Ancho de Banda**: Se estimó el ancho de banda de cada señal y se observaron los resultados en el analizador de espectro.

### Resultados del Análisis:
1. **Caso 1**: Ancho de banda = 1.8477 MHz.
2. **Caso 2**: Ancho de banda = 250.9033 MHz.
3. **Caso 3**: Ancho de banda = 1.9467 MHz.

## Archivos del Proyecto:
- **`Practica3A.grc`**: Diagrama de bloques en GNU Radio para la construcción del modulador AM y análisis de la envolvente compleja.
- **`lab3_parteb2.grc`**: Diagrama de bloques para la modulación con señales aleatorias (audio y binarias).
- **`Practica3A.py`**: Script en Python para la Parte A de la práctica.
- **`Practica3_ParteB_Punto2.py`**: Script en Python para la Parte B de la práctica.

## Conclusiones:
- **Modulación en AM**: La modulación de amplitud es un proceso eficiente para la transmisión de señales en sistemas de comunicación, y la selección del índice de modulación adecuado es crucial para evitar distorsiones.
- **Análisis de ancho de banda y tiempo de bit**: A medida que el índice de modulación aumenta, el tiempo de bit disminuye, lo que permite una transmisión de datos más rápida, pero también implica un mayor ancho de banda.
- **Instrumentación**: El uso del osciloscopio y el analizador de espectro es fundamental para observar las características de la señal modulada y realizar mediciones precisas de la potencia, frecuencia y ancho de banda.


