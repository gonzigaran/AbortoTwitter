# Análisis de Posiciones del aborto en Twitter

Repositorio para presentar el proyecto integrador para la [Diplomatura en Ciencia de Datos, Aprendizaje Automático y sus aplicaciones](http://diplodatos.famaf.unc.edu.ar/) dictado en FaMAF - UNC. 

En este proyecto se trabaja con datos de twitter recolectados durante el tratamiento en Sendaores y Diputados sobre el proyecto de Interrupción Voluntaria del Embarazo (ILE).

## Motivación

Con este proyecto vamos a trabajar sobre un set de datos que trata un tema que estuvo (y sigue estando) en la agenda pública, generando posiciones muy marcadas y expresadas en las redes sociales. Por un lado vamos a conocer cómo vienen los datos en Twitter, que análisis podemos hacer sin tener en cuenta el contenido del tweet y por último analizar el aporte que da el texto.

### Descripción del problema

A partir del tratamiento en las cámaras de Diputados y Senadores sobre el proyecto de Interrupción Voluntaria del Embarazo, la discusión se trasladó a las redes sociales. En este caso se cuenta con publicaciones realizadas en Twitter, que permite un acceso a los datos mucho más simple que otras redes sociales. El dataset (obtenido y preprocesado por [Pablo Celayes](https://www.linkedin.com/in/pablogabrielcelayes/)) cuenta con información de tweets (y sus usuaries correspondientes) que se realizaron sobre la fecha del tratamiento en diputados (junio/2018) y en senadores (agosto/2018), a partir de hashtags relacionados al tema. Con estos datos se pueden analizar comportamientos de usuaries, y clasificación sobre la postura tomada de las diferentes cuentas. 
El dataset consiste en 4 archivos CSV, 2 para junio/2018 y 2 para la fecha de agosto/2018. Para cada fecha hay un archivo con les usuaries que publicaron, y uno de tweets.
Para les usuaries se cuenta con información de cantidad de seguidores, cantidad de seguidos, cantidad de tweets que escribió, descripción, nombre, si la cuenta está verificada o no, fecha de creación, etc.
Para el dataset de tweets se tiene fecha, cantidad de favoritos y retweets, el texto, el usuario, si es un retweet o no. 


## Datasets

Los datos están en dos tipos de archivos, con los siguientes notebooks los exploramos introductoriamente: [para archivos de usuaries](users.ipynb) y [para archivos de tweets](tweets.ipynb)

Los datos fueron recolectados con diferentes métodos para ambos períodos, y en los 2 casos no se cuenta con la totalidad de los tweets con esos hashtags, sino con una muestra.


#### [Dataset de Usuaries](users.ipynb)

|    Columnas   |  Descripción  |
| ------------- | ------------- |
| `screen_name` | Nombre de la cuenta | 
| `location`    | Ubicación de la cuenta | 
| `followers_count`    | Cantidad de seguidores | 
| `statuses_count`    | Cantidad de tweets que escribió/retuiteó la cuenta en toda su historia. | 
| `description`    | Descripción de la cuenta | 
| `friends_count`    | Cantidad de seguidos | 
| `favourites_count`    | Cantidad de favs que la cuenta dió en toda su historia. | 
| `created_at`    | Fecha de creación de la cuenta | 
| `id`    | ID de la cuenta | 
| `name`    | Nombre completo que se le pone a la cuenta | 
| `verified`    | Si la cuenta está verificada o no (por ejemplo para les famoses) | 


#### [Dataset de Tweets](tweets.ipynb)


|    Columnas   |  Descripción  |
| ------------- | ------------- |
| `id` | ID del tweets | 
| `created_at` | Fecha de creación del tweets | 
| `favorite_count` | Cantidad de favoritos que tiene el tweet | 
| `retweet_count` | Cantidad de retweet del tweet | 
| `full_text` | Texto completo del tweet | 
| `posicion` | Posición que se tiene con respecto al aborto de acuerdo a *hashtags* usados. | 
| `favorited` | Si el tweet recibió algún like | 
| `retweeted` | Si el tweet recibió algún retweet | 
| `user_name` | *username* de la cuenta que realiza el tweet | 
| `user_id` | ID de la cuenta que realiza el tweet | 
| `original_id` | En el caso de que el tweet sea un retweet, te da el id del tweet. Si no, coincide con el `id` | 
