# Actividad-Integradora-1
Proyecto de procesamiento del lenguaje natural.
Hacer un modelo que prediga el sentiminto de diferentges 


## Requerimientos ⚙️
El código está hecho en un Jupyter Notebook con Python 3.



## ¿Cómo funciona la recolección de imágenes? 📄

### 1. Base de datos en línea 📦

La página [Shutterstock](https://www.shutterstock.com/es/) proporciona una gran base de datos de imágenes de diversas índoles. Dentro del HTML renderizado se despliegan varias páginas con imágenes asociadas al término de búsqueda ingresado, de las cuales se extraen los URLs de las distintas imágenes usando principalemente las bibliotecas **beautifulsoup4**, **selenium**, **cv2**, y **urllib**.

### 2. Funcionalidad del programa 💻

El programa cuenta con tres funcionalidades principales: búsqueda, descarga y limpieza de carpetas. En primera instancia, la búsqueda se refiere a que el programa realiza la búsqueda de las imágenes con base en el término ingresado previamente por el usuario.

Posteriormente, el programa descarga las imágenes en formato **.jpg** dentro de dos carpetas creadas a priori con el mismo nombre del término de búsqueda. Asimismo, cada una de estas carpetas se deben de encontrar dentro de las carpetas de entrenamiento y prueba respectivamente; estas también debieron ser creadas a priori por el usuario. En caso de no crear dichas carpetas, las imágenes no serán almacenadas. Cabe destacar que, cada quinta imagen es descargada en la carpeta de prueba. En consecuencia, el 80% de las imágenes encontradas son almacenadas en la carpeta de entrenamiento; mientras que, el 20% son descargadas en la prueba.

Finalmente, se cuenta con una función que se encarga de limpiar las carpetas de entrenamiento y prueba del término de búsqueda, si es que este ya ha sido buscado previamente, con el objetivo de no llenar o sobrescribir las imágenes guardadas en ambas carpetas.

### 3. Requerimientos previos a la ejecución del programa 📈📁

Antes que nada, el programa usa el navegador Firefox, por lo que se debe contar el driver correspondiente en el disco C:. En este caso, el driver corresponde al geckodriver.exe. Igualmente, debe de encontrarse en la siguiente ruta: C:\webdrivers. En otras palabras, el driver debe de situarse dentro de una carpeta llamada 'webdrivers' localizada en el disco C:.

Ahora bien, para la ejecución de este proyecto, el usuario debe de crear a priori las carpetas mencionadas en el mismo directorio en el que se ejecuta el programa. En otras palabras, el usuario debe de crear inicialmente dos carpetas: una de entrenamiento (train) y otra de prueba (test). En seguida, dentro de cada una de estas el usuario debe de crear una nueva carpeta con el nombre del término de búsqueda por cada nuevo término de búsqueda a realizar. De esta manera, las imágenes son guardadas así: **/train/<término_de_búsqueda> y /test/<término_de_búsqueda>**. Si un término de búsqueda se repite, la carpeta con el término de búsqueda repetido se limpiará y se almacenarán otras imágenes gracias a la función descrita anteriormente.

### 4. Ejecución del programa 🛠️ 🚀

Al ejecutar el programa, el usuario debe ingresar el término de búsqueda deseado. Después, el programa se encarga de limpiar las carpetas del término de búsqueda. En seguida, el programa prosigue a navegar en la página web para recolectar los URLs de las imágenes con base en el término de búsqueda ingresado. En este proyecto, se especificó que únicamente se recolectaran las imágenes encontradas en las primeras tres páginas de resultados de la página web. Una vez obtenidas los URLs de la página actual, el programa descarga las imágenes en las carpetas correspondientes y sigue así hasta concluir con la tercera página de resultados. De esta manera, el programa finaliza su ejecución.



## Autores 📝

_Equipo 3_

* **Adrian**
* **Jorge**
* **Daniel Jauregui Gómez**
* **Fernando Isunza Fonseca**
* **Paola **
