# Actividad-Integradora-1
Proyecto de procesamiento del lenguaje natural.
Hacer un modelo que prediga el sentiminto de diferentes bases de datos, audios a texto,  Tweets, posts de Reddit, comentarios de youtube.
Para esto se utilizaron diferentes modelos de clasificación de texto. 


## Requerimientos ⚙️
El código está hecho en un Jupyter Notebook con Python 3.
Para poder correr el codigo es necesario modelos y carpetas que podran ser encontrados en:           
Bert: https://drive.google.com/drive/folders/1yW85oTu1QoWCcHDDWXHuZPz_1FzHkC-Y?usp=sharing                  
Datasets:https://drive.google.com/drive/folders/1jUdgEgJg_9HBD5qOjoOU7588qtrEnbBV?usp=sharing           
Pickles de nltk:https://drive.google.com/drive/folders/1htOuDJZcQcUsbtHvK9gjNSN4FYYg5KZi?usp=sharing            
Modelo de lstm bidirectional:https://drive.google.com/drive/folders/1-M6b4gPP8XYFhteOORckacs4fGXk7kbb?usp=sharing       
Modelo de Gru:https://drive.google.com/drive/folders/1s04QDkmWtcL6eAnrNfFtolFPVEFRMaRg?usp=sharing       
Modelo de lstm:https://drive.google.com/drive/folders/1s04QDkmWtcL6eAnrNfFtolFPVEFRMaRg?usp=sharing         
Twitter data:https://drive.google.com/file/d/1ofTAKF5Hg50m-1GUuWYb2EeOpWvmNjlu/view?usp=sharing          



## Avtividad integradora contenidos

### Modelo Ensamble
Para los modelos de nltk se utiliza una base de datos de criticas de películas para evaluar si son positivas o negativas utilizando clasificadores establecidos.

### Speach to text
En esta sección se encuentra una función llamada Sound2text que recibe un audio en formato wav y con ayuda de la librería speachbrain lo convierte a texto (solo funciona
en inglés)


### Filtrar por usuario
En esta parte puedes buscar tweets de un usuario y después aplicar un análisis de sentimientos sobre sus últimos 10 tweets. Solo es necesario insertar el 
nombre de usuario en "user"


### Reddit PRAW
En esta sección se conecta a una instancia de PRAW y se puede hacer una búsqueda por usuario de las publicaciones que ha hecho. Estas publicaciones han sido procesadas para eliminar links,
subreddits y usuarios.

### Youtube API
En esta sección se conecta al API de youtube mediante una API Key y se implementó la funcionalidad de buscar por video de youtube los comentarios del video.

### RNN ARCHITECTURES
Para complemetar el módelo previamente realizado en la clase de procesamiento del lenguaje natural, se crearon redes neuronales recurrentes en tres arquitecturas diferentes. 
A lo largo de toda esta sección se crearon tres arquitecturas principales, RNN simple, LSTM y Bidirectional RNN. Se crearon diferentes redes, con diferentes capas e hiperparametros para obtener una mejor precisión a la hora de predecir. 
### DATA CLEANSING
En esta estapa del codigo se limpio y preparo una base de datos que contenia tweets etiquetados. Con ayuda de la libreria ntlk se removieron las stopwords, puntuaciones y links en cada tweet. Para al final obtener, una base de datos que se pueda utilizar en el entrenamiento de las redes neuronales. 
### Simple RNN
En esta etapa se prueban diferentes modelos de redes neuronales recurrentes simples, utilizando la libreria keras.


### Modelo 2 RNN Y Modelo 3 RNN

Estas secciones fueron utilizadas para probar modelos de simple rnn que no pasaron del 50% de accuracy

### LSTM (Long Short-Term Memory) networks
 En esta etapa se prueban diferentes modelos de redes neuronales recurrentes LSTM, utilizando la libreria keras. Con diferentes hiperparamteros en busqueda de un mejor resultado.


### Bidirectional LSTM (BRNN)
En esta etapa se prueban diferentes modelos de redes neuronales recurrentes Bidireccionales, utilizando la libreria keras. Con diferentes hiperparamteros en busqueda de un mejor resultado.

### Bert
Esta seccion es utilizada para correr un inferencias del modelo bert, este modelo fue entrenado en otro notebook: https://colab.research.google.com/drive/1LZ3-FGEd6JBsVlKkmamONMNcNpojsRYc?authuse
Solo necesita las carpetas y scripts  necesarias de bert, un texto y el modelo entrenado en el link anterior.

### GRU
En esta sección se entreno una rnn gru, se guardo y luego con una celda se corre el modelo con cualquier texto para realizar una predicción

### Rnns validation
Esta sección corre una RNM de lstm y una red de lstm bidireccional. Lamentablemente los entrenamientos de estas redes se perdieron ya que el colab fallo en guardar el kernel de ese momento, el accuracy de estos modelos se encontraba alrededor del 80%. Pero los modelos están guardados y pueden ser corridos con las celdas  disponibles.




### STREAMLIT
Para poder correr streamlit desde colab es necesario crear una cuenta gratuita en  Ngrok lo cual nos permite crear un tunel seguro entre nuestro sistema local hacia el publico y elegir el puerto para el deployment. Despues es necesario instalar streamlit ngrok con pip install. Despues del pip install se creo un framework en donde se puede crear una oracion tanto positiva como negativa y se puede elegir el modelo realizado con keras para poder hacer la prediccion. Mientras que cuando se escoge la opcion de social media esta prediccion se realiza mediaante el modulo de sentiment_mod.py que se realizo en actividades pasadas. Para eso es necesario que el .py se encuentre en el directorio/






## Autores 📝

_Equipo 3_

* **Adrian Mancilla Uribe**
* **Jorge Mariles**
* **Daniel Jauregui Gómez**
* **Fernando Isunza Fonseca**
* **Paola Gabriela Almada** 
