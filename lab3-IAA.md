

# Laboratorio 3: Introducción al Aprendizaje Automático

> **Análisis de las Posiciones del Aborto en Twitter** <br/>
> *Diplomatura en Ciencias de Datos, Aprendizaje Automático y sus aplicaciones.*

## Objetivo y alcance

Para esta materia el objetivo es poder hacer un primer acercamiento a un proceso de aprendizaje automático, haciendo especial énfasis en el proceso de elección de modelo, hiperparámetros, regulador, métricas, etc.

En este laboratorio no se espera que se encuentre el mejor modelo con sus mejores parámetros, sino que se logre la buena práctica de realizar los pasos necesarios en un proceso de aprendizaje automático, desde la división del dataset hasta la evaluación del modelo. 

Para realizar el práctico vamos a utilizar el dataset generado en la materia anterior, y tomar como variable a predecir la etiqueta sobre la posición que tiene el *tweet/user* sobre la discusión de la ley de interrupción voluntaria del embarazo.


## Método

El informe debe estar en un formato de notebook, puede ser una notebook de jupyter notebook, como una generada por RStudio.

Si bien se espera una notebook para poder ver el código/tratamiento que se va haciendo a los datos, es una muy buena práctica acompañar las celdas de código con celdas de texto explicando lo que se está haciendo y para qué o que se busca. En particular en este práctico, hay que acompañar con una justificación cada elección que se toma, desde la elección del modelo, la partición del dataset, la elección del método de evaluación, etc.


## Estructura del informe

El notebook deberá estar estructurado para poder contener los pasos necesario en un proceso de aprendizaje automático:

1. Carga de datos, separando el dataset la etiqueta a predecir.
1. Dividir el dataset en el conjunto de entrenamiento y conjunto de test
1. Elegir el modelo de clasificación a utilizar (cómo parte del modelo, está la elección de la función de regularización)
1. Elegir y justificar métrica de evaluación
1. Entrenamiento del modelo realizando *cross-validation*, seleccionando los hiperparámetros óptimos para la métrica seleccionada
1. Evaluar el modelo a partir del conjunto de *test* apartado *(se puede complementar con gráficos ilustrativos de los resultados como la matriz de confusión)*


### Ejemplo:

- Práctico resuelto de la materia del año pasado. El problema es otro, pero es un buen ejemplo de como son los pasos a seguir. ([Link](https://github.com/gonzigaran/DiploDatos2018/blob/master/IAA/lab2-esquema.ipynb))

**Fecha de entrega primera versión:** 15 días después de entregado el laboratorio.

**Fecha de entrega versión final:** Una semana luego de la respuesta del mentor.
