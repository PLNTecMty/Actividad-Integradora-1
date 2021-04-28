# Actividad-Integradora-1
Proyecto de procesamiento del lenguaje natural.
Hacer un modelo que prediga el sentiminto de diferentes bases de datos, audios a texto,  Tweets, posts de Reddit, comentarios de youtube.
Para esto se utilizaron diferentes modelos de clasificación de texto. 


## Requerimientos ⚙️
El código está hecho en un Jupyter Notebook con Python 3.

-Desde este punto se explicaran los contenidos del notebook

### Modelo Ensamble
Para los modelos de nltk se utiliza una base de datos de criticas de películas para evaluar si son positivas o negativas utilizando clasificadores establecidos.

### Speach to text
En esta sección se encuentra una función llamada Sound2text que recibe un audio en formato wav y con ayuda de la librería speachbrain lo convierte a texto (solo funciona
en inglés)


### Filtrar por usuario
En esta parte puedes buscar tweets de un usuario y después aplicar un análisis de sentimientos sobre sus últimos 10 tweets. Solo es necesario insertar el 
nombre de usuario en "user"


### Reddit PRAW


##RNN ARCHITECTURES

### DATA CLEANSING
Esta parte solo fue utilizada para limpiar la base de datos “Sentiment140 dataset with 1.6 million tweets” , disponible en kaggle, de stop words “@” , etc. para poder entrenar las rnns y bert.
##Simple RNN

##Modelo 2 RNN Y Modelo 3 RNN

Estas secciones fueron utilizadas para probar modelos de simple rnn que no pasaron del 50% de accuracy

##LSTM (Long Short-Term Memory) networks
 
## Modelo 2 

##Bidirectional LSTM (BRNN)


##Bert
Esta seccion es utilizada para correr un inferencias del modelo bert, este modelo fue entrenado en otro notebook: https://colab.research.google.com/drive/1LZ3-FGEd6JBsVlKkmamONMNcNpojsRYc?authuse
Solo necesita las carpetas y scripts  necesarias de bert, un texto y el modelo entrenado en el link anterior.

##GRU
En esta sección se entreno una rnn gru, se guardo y luego con una celda se corre el modelo con cualquier texto para realizar una predicción

##Rnns validation
Esta sección corre una RNM de lstm y una red de lstm bidireccional. Lamentablemente los entrenamientos de estas redes se perdieron ya que el colab fallo en guardar el kernel de ese momento, el accuracy de estos modelos se encontraba alrededor del 80%. Pero los modelos están guardados y pueden ser corridos con las celdas  disponibles.

##BIDIRECTIONAL

##LSTM

##STREAMLIT







## Autores 📝

_Equipo 3_

* **Adrian**
* **Jorge**
* **Daniel Jauregui Gómez**
* **Fernando Isunza Fonseca**
* **Paola** 
