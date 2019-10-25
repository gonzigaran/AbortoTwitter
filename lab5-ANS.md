###### tags: `DiploDatos` `Mentoría` `FaMAF`

# Laboratorio 5: Aprendizaje No Supervisado

> **Análisis de las Posiciones del Aborto en Twitter** <br/>
> *Diplomatura en Ciencias de Datos, Aprendizaje Automático y sus aplicaciones.*

## Objetivo y alcance

Este último práctico tiene por objetivo profundizar en técnicas de análisis exploratorio de los datos, para representar mejor features que son díficiles de tomar en cuenta, como el texto de los tweets. 
Además, a partir de esta exploración, experimentar con técnicas de clustering, para evaluar el comportamiento de las asociaciones.

## Método

A partir del texto que haya en el dataset (podemos tomar tanto el texto de los *tweets* como el de la descripción de los *users*) podemos usar algún método de transformación para llevarlo a algún espacio de *features*, por ejemplo utilizando *word-embeddings* (ver en las [referencias](#Referencias)).

Luego de esta transformación se va a agregar un vector de fetures por instancia, con la que se va a poder realizar cualquier técnica de aprendizaje.

Utilizando este conjunto de vectores explorar las técnicas de clustering vistas en clase variando parámetros como:
- Cantidad de clusters 
- Utilizar o no más variables propias del dataset además de las generadas por word-embedding
- Variar las métricas de distancia

Para evaluar los posibles clusterings realizados se pueden utilizar los siguientes métodos analíticos:
- Medir lo desbalanceados que quedan los clusters (un cluster muy grande y muchos muy pequeños, es una mala agrupación)
- Observar las instancias más cercanas a los centroides de cada clusters (uno esperaria que fueran las instancias más características de ese cluster). Ver si tienen sentido semántico de que estén agrupadas juntas esas instancias y así poder caracterizar el cluster
- Utilizar e interpretar el cálculo de pureza (ver en las [referencias](#Referencias))
- Evaluar a partir de la clase que tiene cada tweet o user, cómo están distribuidos en los clusters (los clusters, ¿separan las clases?)

En el caso que se observe una separación por clase en los clusters, puede ser conveniente equilibrar las clases antes de realizar todo el proceso de clustering. 

## Estructura del informe

Para la entrega de este laboratorio, hay que mostrar principalmente 2 etapas (pueden estar en un mismo notebook o en 2 distintos):
1. En una parte, mostrar el preproceso del *word-embeddings*, generando un arreglo de features para cada instancia. Luego generar el dataset que se va a utilizar para el próximo paso.
2. En otra parte, realizar el clustering, a partir de los datos preprocesados. En esta última instancia, acompañar los clustering realizados por la evaluación y el análisis de los/las analistas.


### Referencias

- Word-Embeddings:
    - Gensim ([Link](https://pypi.org/project/gensim/))
    - Fastext ([Link](https://pypi.org/project/fasttext/))
    - Tutoriales de Gensim ([Link1](https://machinelearningmastery.com/develop-word-embeddings-python-gensim/), [Link2](http://nadbordrozd.github.io/blog/2016/05/20/text-classification-with-word2vec/))
- Cálculo de pureza ([Link](https://nlp.stanford.edu/IR-book/html/htmledition/evaluation-of-clustering-1.html)) 


**Fecha de entrega primera versión:** 15 días después de entregado el laboratorio.

**Fecha de entrega versión final:** Una semana luego de la respuesta del mentor.

