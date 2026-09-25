# Laboratorio de Estadística · Distribución de frecuencias

**Herramienta web para construir tablas de distribución de frecuencias de datos no agrupados y descargarlas como imagen JPG.**

🔗 **Usar la herramienta:** https://temocbzc.github.io/tabla-frecuencias/

## Sobre el Laboratorio de Estadística

Este módulo es parte del **Laboratorio de Estadística**, un proyecto de herramientas digitales abiertas para los cursos de **Estadística y Probabilidad I y II** de nivel bachillerato, pensado especialmente para el **Colegio de Ciencias y Humanidades (CCH) de la UNAM**.

El laboratorio sigue la propuesta del Programa de Estudios 2024 del CCH, que pide incorporar la computadora y las herramientas tecnológicas para organizar datos, calcular medidas y construir gráficas. La intención es que el tiempo de clase se dedique a **analizar e interpretar** la información y no a hacer cálculos repetitivos a mano.

Cada módulo tiene dos formas de trabajo:

| Modalidad | Para qué sirve |
|---|---|
| **Herramienta web** | Se usa desde el navegador de la computadora o del celular, sin instalar nada. Ideal para obtener y comparar resultados rápidamente. |
| **Cuaderno de Python (Colab)** | El alumno ve, paso a paso, cómo se programa cada cálculo. Es una introducción a la programación aplicada a la estadística. |

---

## Este módulo: tabla de distribución de frecuencias

**Ubicación en el programa:** Estadística y Probabilidad I · Unidad 1, *Análisis de información estadística para una variable* · Representación tabular.

### Qué hace

1. Recibe los datos de una muestra, ya sea en un **archivo CSV** o escritos directamente en la página.
2. Construye la tabla de distribución de frecuencias para **datos no agrupados**.
3. Genera una imagen **JPG** en alta resolución, lista para una presentación, un reporte o una tarea.

Funciona con variables **cuantitativas discretas** (número de hermanos, calificaciones, número de mascotas) y **cualitativas** (medio de transporte, color favorito, turno).

### Columnas de la tabla

| Símbolo | Nombre | Cálculo |
|:---:|---|---|
| $i$ | Enumeración | Número de renglón |
| $x_i$ | Valor de la variable | Cada valor distinto observado en la muestra |
| $f_i$ | Frecuencia absoluta | Número de veces que aparece $x_i$ |
| $fr_i\ \%$ | Frecuencia relativa porcentual | $\dfrac{f_i}{n}\times 100$ |
| $F_i$ | Frecuencia absoluta acumulada | $f_1 + f_2 + \dots + f_i$ |
| $Fr_i\ \%$ | Frecuencia relativa acumulada porcentual | $fr_1 + fr_2 + \dots + fr_i$ |

donde $n$ es el tamaño de la muestra. Se cumple siempre que $\sum f_i = n$, que el último $F_i$ es igual a $n$ y que el último $Fr_i\ \%$ es igual a $100\ \%$.

### Formato del archivo CSV

- La **celda A1** lleva el **nombre de la variable**.
- Debajo, en la misma columna, van **todos los datos**, uno por celda.
- En Excel o Google Sheets: *Archivo → Guardar como / Descargar → CSV*.

```
Número de hermanos
2
1
3
0
2
```

En el repositorio hay un archivo de ejemplo: [`ejemplo_numero_de_hermanos.csv`](ejemplo_numero_de_hermanos.csv).

### Privacidad

Los datos se procesan **solo en el navegador** del usuario. No se envían ni se guardan en ningún servidor.

### Recomendaciones de uso

- La tabla de datos no agrupados es adecuada cuando la variable tiene **pocos valores distintos** (hasta unos 15 o 20). Si hay muchos valores distintos, por ejemplo estaturas o tiempos con decimales, conviene una tabla de **datos agrupados** en intervalos de clase.
- La herramienta maneja sin problema muestras de miles de datos.

---

## Actividades sugeridas para el aula

1. **Recolectar datos del grupo.** Hacer una encuesta breve (número de hermanos, tiempo de traslado redondeado, medio de transporte), capturarla en una hoja de cálculo y construir la tabla.
2. **Interpretar la tabla.**
   - ¿Cuál es la **moda**?
   - ¿Qué porcentaje del grupo tiene un valor **menor o igual** a cierto $x_i$? ¿En qué columna se lee directamente?
   - ¿Por qué el último $F_i$ siempre es igual a $n$?
3. **Comparar grupos.** Construir la tabla de dos grupos distintos y comparar las distribuciones con las frecuencias relativas; las absolutas no sirven para comparar si los grupos son de distinto tamaño.
4. **Datos con sentido social.** Siguiendo los ejes transversales del programa (perspectiva de género, sustentabilidad, educación cívica), usar datos abiertos de fuentes como el INEGI o datos.gob.mx sobre temas cercanos a los alumnos.
5. **Verificar a mano.** Calcular a mano las primeras filas y comprobar el resultado con la herramienta o con el cuaderno de Python.

---

## Mapa del laboratorio

Módulos organizados según el Programa de Estudios 2024 de Estadística y Probabilidad del CCH.

### Estadística y Probabilidad I

| Unidad | Tema | Módulo | Estado |
|---|---|---|:---:|
| 1. Análisis de información estadística para una variable | Representación tabular | Distribución de frecuencias, datos no agrupados | ✅ Disponible |
| | Representación tabular | Distribución de frecuencias, datos agrupados | 🔜 Planeado |
| | Representación gráfica | Barras, circular, puntos, histograma, polígono de frecuencias, ojiva | 🔜 Planeado |
| | Medidas de tendencia central | Media, mediana, moda | 🔜 Planeado |
| | Medidas de dispersión | Rango, varianza, desviación estándar, coeficiente de variación | 🔜 Planeado |
| | Medidas de posición | Cuartiles, deciles, percentiles, diagrama de caja | 🔜 Planeado |
| | Regla empírica | Distribuciones simétricas y unimodales | 🔜 Planeado |
| 2. Datos bivariados | Variables cualitativas | Tablas de contingencia | 🔜 Planeado |
| | Variables cuantitativas | Diagrama de dispersión, correlación de Pearson, regresión lineal | 🔜 Planeado |
| 3. Azar y probabilidad | Enfoque frecuencial | Simulación de experimentos aleatorios y estabilización de frecuencias | 🔜 Planeado |
| | Probabilidad condicional | Eventos independientes y dependientes | 🔜 Planeado |

### Estadística y Probabilidad II

| Unidad | Tema | Módulo | Estado |
|---|---|---|:---:|
| 1. Modelos de probabilidad | Variables aleatorias | Distribución binomial | 🔜 Planeado |
| | Variables aleatorias | Distribución normal | 🔜 Planeado |
| 2. Distribuciones muestrales | Medias y proporciones | Simulador del Teorema del Límite Central | 🔜 Planeado |
| 3. Inferencia estadística | Estimación | Intervalos de confianza | 🔜 Planeado |
| | Pruebas | Pruebas de hipótesis | 🔜 Planeado |

---

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `index.html` | Herramienta web (un solo archivo, sin dependencias que instalar) |
| `tabla_frecuencias_datos_no_agrupados.ipynb` | Cuaderno de Python para Google Colab, con explicación paso a paso |
| `ejemplo_numero_de_hermanos.csv` | Datos de ejemplo para probar la herramienta |

---

## Autor

**Dr. Ignacio Cuauhtemoc Benitez Zuniga** · Profesor de Estadística y Probabilidad, Colegio de Ciencias y Humanidades, UNAM.

Proyecto desarrollado dentro del trabajo sobre el uso de la inteligencia artificial generativa en la enseñanza de la estadística en el bachillerato.

## Referencia

Colegio de Ciencias y Humanidades, UNAM (2024). *Programas de Estudio. Área de Matemáticas. Estadística y Probabilidad I–II.* https://cch.unam.mx/sites/default/files/programas2024/ESTADISTICA_PROBABILIDAD_I_II.pdf
