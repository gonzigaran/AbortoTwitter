

# Laboratorio 1: Análisis y Visualización de Datos

> **Análisis de las Posiciones del Aborto en Twitter** <br/>
> *Diplomatura en Ciencias de Datos, Aprendizaje Automático y sus aplicaciones.*

## Objetivo y alcance

En esta primera aproximación a los datos se pretende comenzar por analizar el conjunto de usuaries de los que se tiene datos. El objetivo general es poder ver cómo es la distribución de les usuaries de acuerdo a algunas variables con las que se cuenta. Por ejemplo: seguidores/seguidos, cantidad de tweets, fecha de creación de la cuenta, etc. y poder concluir y visualizar resultados y relaciones entre variables.

Cómo guía para trabajar en este práctico se pueden usar alguna de las siguientes preguntas disparadoras:
- ¿Les usuaries tienden a tener muchos seguidores? ¿Y seguidos?
- ¿Las cuentas se registraron hace mucho tiempo o cerca de la fecha de recolección de los datos? ¿El dataset tiene muchas cuentas que se crearon entre la votación en diputades y senadores?
- ¿Mientras más tiempo tiene la cuenta, más tweets tiene?
- ¿Si la cuenta está verificada, twitea más?
- ¿Son independientes las variables de que sea verificade y que tenga más de X seguidores? ¿Y con seguidos?
- ¿La cantidad de favs se relaciona con la cantidad de seguidos?

Y se pueden plantear muchas preguntas más como disparadores del informe. El objetivo es intentar responder preguntas de este estilo en el informe y utilizar lo aprendido en la materia como herramienta para ello.

## Método

Para poder realizar este análisis se puede utilizar todo lo visto en clase:
- Analizar los estadísticos clásicos como la media, la moda, mediana y desviación estándar para variables numéricas. 
- Ver si la variable a analizar responde a alguna distribución conocida. ¿Cambia cuando filtramos por la clase de si la cuenta está verificada o no? Se puede ver gráficamente con gráficos como [este](https://seaborn.pydata.org/generated/seaborn.violinplot.html).
- Calcular correlaciones entre variables, calcular probabilidades marginales y conjuntas. 
- Analizar outliers.

## Estructura del informe
El informe debe estar en un formato que no sea un Jupyter Notebook, por ejemplo .html, .pdf, .md. El objetivo es poder redactar y justificar las conclusiones obtenidas a partir de las preguntas disparadores, utilizando material gráfico y/o interactivo como soporte para complementar las ideas. 

### Ejemplos:
- [We are from our childhood](https://www.kaggle.com/jkokatjuhha/we-are-from-our-childhood) (Si bien es un notebook, tiene ejemplos de gráficos que son muy buenos para mostrar una idea)
- [Informe Correpi](http://www.correpi.org/2019/archivo-2018-cada-21-horas-el-estado-asesina-a-una-persona/) (ejemplo de uso de visualizaciones como complemento)
- [Irregularidades en los sorteos de causas de corrupción](https://www.lanacion.com.ar/politica/revelan-que-hay-irregularidades-en-los-sorteos-de-causas-de-corrupcion-nid2092357)

**Fecha de entrega primera versión:** 10 días después de finalizada la materia.

**Fecha de entrega versión final:** Una semana luego de la respuesta del mentor.
