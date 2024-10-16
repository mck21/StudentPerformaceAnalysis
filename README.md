# Análisis de Factores que Influyen en el Rendimiento Académico de los Estudiantes

Este repositorio contiene un análisis del [dataset de Kaggle](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors/data) que examina varios factores que podrían influir en el rendimiento académico de los estudiantes.<br><br>
> [!IMPORTANT]
Aquí puedes acceder al [análisis en Google Sheets](https://docs.google.com/spreadsheets/d/1xaC4Uw8iyd0s6YDOQmCVE0gIYyCW9urNs5iH_Bp2bMw/edit?usp=sharing) (enlace con acceso para cualquier persona)

## 1. Exploratory Data Analysis (EDA)

### 1.1. Comprensión General de los Datos

El conjunto de datos muestra varios factores que podrían influir en el rendimiento académico de los estudiantes, como horas de estudio, asistencia, implicación parental, acceso a recursos, y más. La variable objetivo es **Exam_Score** (puntuación del examen). Las filas representan estudiantes con diferentes niveles de motivación, ingresos familiares, calidad de los profesores y otros factores. El análisis se centra en cómo estos aspectos, especialmente las horas de estudio, motivación y la calidad de la enseñanza, afectan las notas de los exámenes.

### 1.2. Transformación y Limpieza

- **Eliminar duplicados**
  <p align="center">
    <img src="https://github.com/mck21/StudentPerformaceAnalysis/blob/main/img/duplicados.png" />
  </p>
  
- **Tratar los valores nulos**
  <p align="center">
   <img src="https://github.com/mck21/StudentPerformaceAnalysis/blob/main/img/null_values.png" />
  </p>
  Cambiamos las celdas vacías por “Unknown” en las columnas **Teacher_Quality**, **Parental_Education_Level** y **Distance_from_Home**.

- **Corregir/borrar datos erróneos o formatos incorrectos** (no se encontraron errores significativos).

### 1.3. Patrones y Outliers

- **Tablas dinámicas**: Se utilizaron para observar la relación entre las puntuaciones del examen y el resto de factores.
- **Gráficos**: BarCharts, LineCharts, AreaChart, DonutChart.
- **Formato condicional**: Se aplicó formato condicional para resaltar los valores en la nota de los exámenes.
  <p align="center">
   <img src="https://github.com/mck21/StudentPerformaceAnalysis/blob/main/img/formaro_condicional.png" />
  </p>

## 2. Dashboard

Se ha creado un dashboard interactivo que permite filtrar los datos según género, tipo de escuela, influencia de los compañeros y distancia a la escuela.

<p align="center">
  <img src="https://github.com/mck21/StudentPerformaceAnalysis/blob/main/img/dashboard.png" />
</p>

## 3. Conclusiones e Interpretación de Resultados
Con los resultados puestos en gráficos en el dashboard podemos ver mejor los patrones y tendencias de este conjunto de 6607 estudiantes.
 - Vemos que todas las gráficas referidas a la variable objetivo (nota del examen) tienen cierta correlación.
 - Hasta valores de la nota cerca de 77, las gráficas siguen una tendencia ascendente, mientras que por encima de este valor empiezan a verse irregularidades en la tendencia.
 - En cuanto a la media de horas estudiadas, podemos apreciar que los estudiantes con notas más altas no precisan dedicar tantas horas como los estudiantes de notas más bajas. Esto se puede deber a la calidad del estudio; no por invertir más tiempo significa que el alumno aprenda más.
 - La media de horas de sueño es ligeramente más baja de cara a los alumnos con mejor nota. Esto se puede atribuir a factores como el estrés o, en casos independientes, a las horas invertidas en el estudio.
 - Los valores bajos de asistencia acarrean peores notas entre los estudiantes; sin embargo, según los resultados, con una asistencia de entre el 70% y el 80% de las clases sería suficiente para algunos alumnos que han obtenido una nota de entre 80 y 93.
 - En cuanto a las clases particulares, apreciamos que a más clases tomadas por el alumno, mejor nota obtiene, siendo lo normal tomar entre 1 y 3 clases. El alumno que ha obtenido mejor nota ha tomado 5 clases particulares.
 - Apreciamos hasta dos puntos de diferencia en la nota media global entre los alumnos cuyos padres presentan alto nivel de implicación (68.09) y bajo nivel de implicación (66.36).
 - Analizando la nota previa respecto a la de este examen, apreciamos una tendencia ascendente, lo que significa que la mayoría de estudiantes han mejorado su rendimiento.
 - También vemos una tendencia ascendente en la nota media a medida que más horas de ejercicio físico realizan los estudiantes. Una mejor salud implica un mejor rendimiento.
 - Por último, podemos ver hasta 1.1 puntos de diferencia en la media global entre los alumnos que presentan discapacidades para aprender y los que no.
