# Entrega: Evaluación y Refinamiento del modelo

En esta entrega, se aplicaron técnicas de regularización y refinamiento para mejorar el modelo seleccionado. Además, se realizó una evaluación del modelo y se interpretaron los resultados obtenidos.

Esta carpeta contiene los archivos solicitados para completar la actividad, está compuesta por:
* **Notebook_Refinamiento.ipynb**: Notebook donde se encuentra el código realizado, en donde se trabaja con el modelo seleccionado previamente para refinar sus hiperparámetros y aplicar técnicas de regularización, permitiendo tener el mejor modelo posible.  
* **Reporte_Refinamiento.pdf**: Reporte donde se describe de manera detallada el proceso seguido en la parte de Refinamiento, se definen los hiperparámetros modificados y se realiza la evaluación e interpretación final del modelo. 

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

1. **El reporte incluye una sección donde se expliquen las métricas utilizadas para comprobar el desempeño de los modelos desarrollados**:
   * En esta nueva versión, se incluye una explicación detallada de la métrica utilizada (accuracy), además de que se describe cómo se obtiene y su fórmula matemática.
2. **El reporte incluye una sección donde se hagan pruebas relacionadas con el efecto de la regularización**:
   * La regularización de nuestro modelo se realizó por medio de la optimización de parámetros con la herramienta Optuna. En esta nueva versión de la entrega, se incluyó una sección  dedicada a la regularización del modelo, y se explican los hiperparámetros relacionados a la regularización que Optuna toma en cuenta, y se realiza una comparación de los resultados antes y después de la regularización. 
3. **La interpretación de los resultados es correcta y está soportada por gráficas, tablas, o argumentos sólidos**:
   * Para evaluar el desempeño de manera visual, se agregaron gráficas de curvas ROC, las cuales permiten comparar la capacidad de los modelos de clasificación binaria. Se incluyó una gráfica antes y una después del refinamiento y regularización para así identificar cómo mejoró el modelo. 



