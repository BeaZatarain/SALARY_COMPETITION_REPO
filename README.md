# SALARY_COMPETITION

![cabecera](https://github.com/BeaZatarain/SALARY_COMPETITION_REPO/blob/main/img/descarga.jpg)

## Descripción general del proyecto

Estamos ante un proyecto que consiste en la creación de un modelo predictivo para tratar de predecir los salarios de un cierto número de empleados a partir de una base de datos de una competición de [Kaggle](https://www.kaggle.com/competitions/predict-salary-for-data-science-jobs)

## Exploración y limpieza de los datos

La información que se ha utilizado en este proyecto proviene de los siguientes CSVs:

 - **salaries_data.csv**: muestra de datos proporcionados para la competición, en el que se encuentran tanto la variable dependiente como el       resto de variables independientes.
 - **testeo.csv**: muestra que no incluye la variable dependiente, es decir, los salarios a predecir. Donde se terminará de entrenar el modelo    predictivo. 
 - **testeo_1.csv**: archivo que parte de 'salaries_data' donde se ha realizado la correspondiente exploración y limpieza de datos, además de    la creación del modelo predictivo.
 - **muestra.csv**: resultado de la predicción que se ha subido a la competición de Kaggle.
 
Con ello, tal y como se explica arriba, dentro **testeo_1.csv** se ha procedico a explorar los datos proporcionados y su correspondiente limpieza con el fin de optimizar lo máximo posible el proceso de creación de un modelo predictivo. 
 
En este sentido, las pricipales tareas de limpieza y exploración que se han llevado a cabo han sido:

  1. Comprobación de existencia de nulos. 
  2. Distribución de columnas categóricas vs. numéricas. 
  3. Eliminación de columnas redundantes. 
  4. Transformación de columnas categóricas en columnas numéricas, analizando y aplicando el mejor método posible para cada caso. 
  5. Análisis de posible colinealidad alta entre columnas. 
  
## Definición del modelo predictivo

Una vez los datos están listos para la creación del modelo predictivo, hemos empleado una función en Python diseñada para identificar el modelo predictivo que mejor se ajuste a los datos dados. 

Con ello, en este caso, el modelo proporcionado por la función utilizada ha sido **'Modelo elastic'** con los siguientes hiperparámetros alpha=0.5 y l1_ratio=0.5.

De este modo, en la fase de entrenamiento, la predicción presentaba un error de 57238.80854422544 (RMSE) y finalmente aplicado a todos los datos, el error disminuyó a 52978.03633.

  
  
 