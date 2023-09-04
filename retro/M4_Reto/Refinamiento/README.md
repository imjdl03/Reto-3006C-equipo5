# **Momento de Retroalimentación: Reto Evaluación y Refinamiento de modelo**
En esta carpeta se incluye el jupyter notebook donde se refina un algoritmo de aprendizaje máquina utilizando un framework para determinar si los pasajeros del titanic sobreviven o no.

### Introducción
El problema que se está tratando de solucionar es determinar si un pasajero del Titanic sobrevive o no basado en diferentes caraterísticas, como el puerto en el que embarcó, su edad, sexo, entre otros. Esto nos genera un problema de **clasificación binaria**.

### Set de datos
El set de datos utilizado es el del titanic, obtenido de la plataforma de Kaggle. Para consultarlo a más detalle se puede consultar en siguiente [link](https://www.kaggle.com/competitions/titanic/data?select=train.csv). El set tiene 891 registros y cuenta con las siguientes variables: Passenger ID, Survival, Ticket class (PClass), Sex, Age, Number of siblings / spouses aboard the Titanic (sibsp), Number of parents / children aboard the Titanic (parch), Ticket number, Passenger fare, Cabin number, Port of Embarkation.
Debido a que el set de datos no viene listo para usar, realizamos una [limpieza de datos](https://github.com/imjdl03/Reto-3006C-equipo5/tree/main/retro/M4_Reto/Limpieza). En esta limpieza se realizó un one hot encoding para las variables que eran categóricas. Además, habian algunos registros que les faltaban datos como la edad. Basados en su titulo y su clase determinamos un aproximado de la edad que podrían haber tenido. Para ver con más detalle la limpieza de datos se sugiere visitar esa entrega.

### Métricas
Para seleccionar el mejor modelo, se utilizará el **accuracy score**. La elección de este parámetro se debe a que queremos tratar de predecir la mayor cantidad de resgistros correctamente. 

### Modelo utilizado
Se realizaron pruebas con diferentes modelos, hasta llegar a la decisión de utilizar una **regresión logistica**. Esta elección se debe a que este es un modelo que nos permite resolver problemas de clasificación, sin tener un overfitting muy grande, como nos pasaa con un random forest. Además, de todos los modelos probados fue el que mejor rendimiento mostró. Para ver con más detalle la selección del modelo se recomienda visitar el siguiente [link](https://github.com/imjdl03/Reto-3006C-equipo5/tree/main/retro/M4_Reto/Modelacion)

## Estructura del repositorio
* refinamiento.ipynb: En este archivo se encuentra el refinamiento del Random Forest.

## Archivos para revisión
A continuación se presentan los archivos que están listos para ser retroalimentados: 

* **Momento de Retroalimentación: Reto Evaluación y Refinamiento de modelo** Archivo para revisión **retro/M4_Reto/Refinamiento/refinamiento.ipynb** o en: https://github.com/imjdl03/Reto-3006C-equipo5/tree/main/retro/M4_Reto/Refinamiento/refinamiento.ipynb

* **Momento de Retroalimentación: Reto Evaluación y Refinamiento de modelo** Archivo para revisión **retro/M4_Reto/Refinamiento/Refinamiento%20del%20modelo.pdf** o en: https://github.com/imjdl03/Reto-3006C-equipo5/blob/main/retro/M4_Reto/Refinamiento/Refinamiento%20del%20modelo.pdf
