# Entrega: Reto, selección, configuración y entrenamiento del Modelo

En esta entrega, se exploran diferentes modelos compatibles con el problema a resolver, se realizan pruebas con diferentes modelos y distintos hiperparámetros. Finalmente, se selecciona el modelo a utilizar en base a la métrica de desempeño seleccionada.

Esta carpeta contiene los archivos solicitados para completar la actividad, está compuesta por:
* **Notebook_Modelo.ipynb**: Notebook donde se encuentra el código realizado y la implementación del modelo, además de las explicaciones pertinentes.
* **Reporte_Modelo.pdf**: Archivo donde se encuentran los datos del set de datos utilizado en la actividad en formato csv.

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

El set de datos se puede encontrar en: https://github.com/adrian-faz/Portafolio_Implementacion/blob/main/final/M2_ML/Entrega_Framework/iris.csv

## Problema

El problema presentado en este caso es de **clasificación**, pues se busca generar un modelo que sea capaz de clasificar en una de las 3 especies existentes en los datos, basandose en los otros datos, como lo son las longitudes y anchuras del sépalo y del pétalo. 

El modelo a utilizar fue el **Decision Tree Classifier**, el cual es un algoritmo de aprendizaje supervisado que descompone un problema complejo en subproblemas más simples, tomando decisiones basadas en las características de los datos. Este árbol se compone de nodos que representan condiciones, y ramas, que serían las posibles respuestas. Lo que se busca  es llegar a una "hoja" que contiene la clase a la que pertenece.

## Subcompetencias y archivos a revisar

Las competencias e indicadores a evaluar en esta entrega son las siguientes:

1. **SMA0401A**
   * Indicadores:
      * Usa un marco de trabajo o framework para implementar una técnica o algoritmo de aprendizaje máquina como: regresiones, árboles, clusters, etc...
       
   * Archivo donde se evalúa:
      * Actividad_Framework.ipynb



## Cambios implementados

A continuación se enlistan los puntos que no recibieron marcas en la rúbrica de retroalimentación y lo que se hizo para resolverlo:

1. "**El readme indica cuáles son los archivos que deberán revisarse para evaluar los indicadores de las subcompetencias**":
    * Se agregó una sección nueva en el readme con las subcompetencias a evaluar en esta actividad y los archivos en donde se pueden revisar.


