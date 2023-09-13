# Entrega: Reto, selección, configuración y entrenamiento del Modelo

En esta entrega, se exploran diferentes modelos compatibles con el problema a resolver, se realizan pruebas con diferentes modelos y distintos hiperparámetros. Finalmente, se selecciona el modelo a utilizar en base a la métrica de desempeño seleccionada.

Esta carpeta contiene los archivos solicitados para completar la actividad, está compuesta por:
* **Notebook_Modelo.ipynb**: Notebook donde se encuentra el código realizado, en donde se prueban 3 diferentes modelos con hiperparámetros distintos, se evalúan los modelos con un conjunto de validación y se selecciona al mejor modelo.
* **Reporte_Modelo.pdf**: Reporte donde se incluye la descripción y explicación detallada de lo que se realizó para seleccionar el modelo, se describen los hiperparámetros utilizados y incluye el modelo seleccionado.

## Set de Datos 

El set de datos utilizado se llama "train_clean.csv", y este incluye 886 registros de personas que abordaron el Titanic. Cada registro cuenta con las siguientes características:

* Survived
* Pclass
* Sex
* Age
* SibSp
* Parch
* Fare
* Variables binarias de Embarked (Embarked_Q, Embarked_S, Embarked_C)
* Variables binarias de Title (Title_Master, Title_Officer, Title_Mr, Title_Mrs, Title_Miss, Title_Royal)

En donde, se busca predecir si la persona sobrevivió o no en base a las otras características que se tienen como "datos de entrada".

El set de datos se puede encontrar en: https://github.com/imjdl03/Reto-3006C-equipo5/blob/main/final/Data/train_clean.csv

## Modelo ML seleccionado

El problema presentado en este caso es de **clasificación**, pues se busca generar un modelo que sea capaz de clasificar en si una persona sobrevivió o no, basandose en los otros datos involucrados.

El modelo final seleccionado fue la **Regresión Logística**, el cual es un algoritmo de aprendizaje supervisado que estima la probabilidad de que una instancia pertenezca a una categoría particular. Se utiliza la función logística o sigmoide, la cual transforma su salida para caer entre 0 y 1, y esto permite representarla como una probabilidad. La regresión logística utiliza variables predictoras para calcular ponderaciones que maximizan la verosimilitud de clasificar correctamente las observaciones. Normalmente se usa 0.5 como el umbral, si la probabilidad modelada es superior a este valor, la instancia se clasifica en la categoría 1, y si es inferior, en la categoría 0. De los modelos probados compatibles con problemas de clasificación, la Regresión Logística fue el que nos arrojó un mejor resultado en cuestión de ajuste del modelo y su poco nivel de overfitting a comparación de los demás modelos.


## Cambios implementados

A continuación se enlistan los puntos que no recibieron marcas en la rúbrica de retroalimentación y lo que se hizo para resolverlo:

1. **El readme incluye una descripción del modelo de ML seleccionado**:
   * El readme ahora incluye la descripción detallada de el modelo seleccionado (Regresión Logística), la cual no estaba incluida en la entrega pasada.

2. **El reporte incluye el nombre del dataset utilizado**
   * El reporte y el readme ahora incluyen el nombre del dataset utilizado.

3. **El reporte incluye una descripción breve de los datos incluidos en el dataset (cantidad de registros/muestras, número de características, número de clases de salida o rango de valores de salida)**
   * El reporte ahora incluye una descripción más detallada de los datos que se incluyen, explicando las características que permanecieron, la cantidad de registros y las posibles salidas.

4. **El reporte incluye una descripción del tipo de problema a resolver (regresión o clasificación)**
   * El reporte ahora incluye una descripción más detallada del problema que se está resolviendo, incluyendo la explicación del por qué se trata de un problema de clasificación.

5. **El reporte incluye una descripción de los hiper-parámetros utilizados para entrenar el modelo**
    * El reporte ahora incluye una descripción de cada uno de los hiperparámetros que se modificaron para encontrar el mejor modelo. Se explica para qué sirven y se prueba con diferentes valores de cada uno para analizar su efecto. 

6. **El modelo seleccionado se escogió de forma correcta (es acorde al tipo de problema)**
    * Se definieron ciertos parámetros para cada modelo probado, con un rango de valores para cada uno, se probó con diferentes configuraciones y se obtuvo la mejor configuración para cada uno de los 3 modelos probados. Después de encontrar la mejor configuración de cada uno, se compararon todos los modelos y se seleccionó el más adecuado. El proceso se encuentra en el Notebook y la descripción detallada de cada hiperparámetro y cada modelo se encuentar en el reporte. 

7. **El reporte incluye una descripción de las métricas de desempeño para el subconjunto de entrenamiento**
   * En el reporte ahora se incluye la definición de la métrica seleccionada, cómo funciona y la fórmula matemática de la misma. 

8. **Los hiper-parámetros seleccionados para entrenar el modelo son adecuados**:
   * El reporte ahora cuenta con una explicación detallada de cada hiperparámetro utilizado en los diferentes modelos, y para seleccionar las mejores combinaciones, se utilizó el método de "grid-search", el cual ayuda a encontrar los valores óptimos para cada hiperparámetro.


