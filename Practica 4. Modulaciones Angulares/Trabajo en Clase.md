# Práctica de Modulación FM y Análisis Espectral

## Descripción
La **Práctica de Modulación FM y Análisis Espectral** tiene como objetivo estudiar la modulación de frecuencia (FM), su análisis espectral y el comportamiento de las emisoras de radio FM. En la **Parte A**, se realiza un análisis del espectro de emisoras FM entre 88 y 108 MHz utilizando GNU Radio para medir el ancho de banda y las características de las señales. En la **Parte B**, se estudian las características de las señales moduladas por fase (PM), incluyendo su análisis en bandas estrechas y anchas, y la medición de su espectro.

## Parte A: Análisis de Emisoras de Radio FM

### Objetivo:
- **Monitoreo del espectro de FM**: Se realiza un análisis del espectro de las emisoras FM en el rango de 88 a 108 MHz.
- **Estudio de Ancho de Banda**: Se mide el ancho de banda de las emisoras, comparándolo con las normativas del **Plan Técnico Nacional de Radiodifusión Sonora (PTNRS)**.
- **Demodulación y Características de la Señal**: Se analiza la señal de banda base, observando sus características, como la calidad de la señal y la variabilidad en el ancho de banda.

### Procedimiento:
1. **Configuración en GNU Radio**: Se utilizó GNU Radio para construir un diagrama de bloques que permitiera monitorear el espectro de las emisoras FM, con la posibilidad de demodular las señales para observar las características de la señal de banda base.
2. **Análisis Espectral**: Se observó el espectro de las emisoras en el rango de 88-108 MHz, midiendo su ancho de banda y verificando el cumplimiento de las normativas de modulación.
3. **Demodulación**: Se utilizó el bloque de demodulación de FM para obtener la señal de banda base, y se analizó su calidad y contenido.

### Resultados:
- Se identificaron varias emisoras de radio FM, y se observó que la mayoría cumplían con el límite de ancho de banda de 75 kHz establecido por el PTNRS para transmisiones monofónicas.
- La señal demodulada presentó una calidad adecuada, con pocas interferencias o distorsiones.

---

## Parte B: Análisis de Modulación de Fase (PM)

### Objetivo:
- **Estudio de Modulación de Fase (PM)**: En esta parte, se construyó un modulador de fase (PM) para analizar su comportamiento tanto en configuraciones de **banda estrecha** como de **banda ancha**.
- **Medición de Ancho de Banda**: Se estudió el ancho de banda de las señales moduladas y se compararon con las predicciones teóricas usando los coeficientes de Bessel.

### Procedimiento:
1. **Construcción del Modulador PM**: Se utilizó un diagrama de bloques en GNU Radio para simular un modulador de fase y analizar la señal modulada.
2. **Análisis de Banda Estrecha y Ancha**:
   - Para **banda estrecha** (\(k_p A_m < 0.1\)): Se observó el comportamiento de la señal en el dominio de tiempo y se midió el ancho de banda en el analizador de espectro.
   - Para **banda ancha** (\(k_p A_m > 4\)): Se observaron las distorsiones y el aumento del ancho de banda en el espectro.
3. **Cálculo de Coeficientes de Bessel**: Se calcularon los coeficientes de Bessel para las señales PM y se compararon con los valores experimentales obtenidos.

### Resultados:
- **Banda Estrecha (kpAm < 0.1)**:
  - Se observó una señal de modulación débil, con un ancho de banda aproximado de 20 kHz.
- **Banda Ancha (kpAm > 4)**:
  - La señal mostró una mayor distorsión y un ancho de banda más amplio, entre 40 kHz y 60 kHz.

---

## Conclusiones:
- **Emisoras de FM**: El análisis de las emisoras FM permitió confirmar que la mayoría de las emisoras cumplen con el límite de modulación de 75 kHz para transmisiones monofónicas.
- **Modulación de Fase (PM)**: El estudio de la modulación de fase reveló cómo el parámetro \(k_p A_m\) afecta tanto el ancho de banda como la forma de onda de la señal. Las señales con \(k_p A_m > 4\) mostraron un amplio espectro, mientras que las señales con \(k_p A_m < 0.1\) presentaron una modulación menos pronunciada.
- **Instrumentación**: El uso de GNU Radio, el analizador de espectro y el osciloscopio fue fundamental para realizar las mediciones precisas y comprender cómo las modulaciones afectan las señales en el dominio del tiempo y frecuencia.


