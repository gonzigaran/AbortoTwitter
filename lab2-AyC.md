

# Laboratorio 2: Análisis Exploratorio y Curación de Datos

> **Análisis de las Posiciones del Aborto en Twitter** <br/>
> *Diplomatura en Ciencias de Datos, Aprendizaje Automático y sus aplicaciones.*

## Objetivo y alcance

En este laboratorio el objetivo va a ser empezar a transformar el dataset para los primeros experimentos de aprendedores en las siguientes materias. 
Como gran objetivo es lograr un único dataset, que condence toda la información importante para lograr aprender si un user o tweet tiene una inclinación por estar a favor o en contra de la ley de interrupción voluntaria del embarazo.

Hay 2 formas de encarar la curación del dataset:
- Generar un único dataset de users, combinando los users de Junio y Agosto
- Generar un único dataset de tweets, combinando los users de Junio y Agosto

En el primer caso, hay que lograr condensar la información de los tweets que realizó cada usuarie en su fila del dataset de users. Por ejemplo: contar la cantidad de tweets que tiene cada une, los X hashtags mas usados, utilizar para los users de junio la columna `posicion` que tienen los tweets, cantidad de favs/retweets obtenidos en esos tweets, etc. Además en este caso se puede anonimizar el nombre de los usuarios cómo se vio en la materia. 

En el segundo caso, primeramente hay que explorar la tabla de datos y detectar variables erroneas, o información repetida. Luego hay que analizar de que manera aprovechar la variable más representativa del dataset que es `text`, por ejemplo extrayendo los hashtags, y para los X hashtags más usados analizar si aparece o no el hashtag en el tweet. Por último se puede implementar un `wordcloud` a partir de los textos, diferenciandolo por la `posición`. 

Luego de haber obtenido el dataset deseado, hay que asegurarse de tener la tabla limpia y guardada en un archivo nuevo. 

## Método

Para este laboratorio pueden usar tanto Python como R, y además de generar las variables nuevas que puedan ser necesarias más adelante, hay que limpiar los datos realizando un tratamiento similar de los datos al [laboratorio 1](https://github.com/DiploDatos/AnalisisYCuracion/blob/master/notebooks/Limpieza.ipynb)


## Estructura del informe

El informe debe estar en un formato de notebook, puede ser una notebook de jupyter notebook, como una generada por RStudio.

Si bien se espera una notebook para poder ver el código/tratamiento que se va haciendo a los datos, es una muy buena práctica acompañar las celdas de código con celdas de texto explicando lo que se está haciendo y para qué o que se busca. En particular en la elección de las variables generadas. 

Por último, comprobar que el dataset pase el [checklist del Banco Mundial](https://dimewiki.worldbank.org/wiki/Checklist:_Data_Cleaning) (se puede realizar al comienzo también)

### Hints:

- Para poder obtener todos los hashtags de los tweets con python:
```python
import re
hashtags = df['text'].apply(lambda x: re.findall(r"#(\w+)", x)).sum()
# Para eliminar repiticiones
hashtags = list(set(hashtags))
```
- Para ir probando el código de generar nuevas variables, trabajar con una muestra pequeña para no tener que procesar mucho en cada prueba. 
- Recordar guardar el dataset limpio en un nuevo archivo y no modificar los datos crudos!

**Fecha de entrega primera versión:** 15 días después de entregado el laboratorio.

**Fecha de entrega versión final:** Una semana luego de la respuesta del mentor.
