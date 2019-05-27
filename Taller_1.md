# 1 - Taller número uno

###  1.1 - Cuál es el problema a tratar?

Hurto al comercio, en la Localidad de los Martires de la ciudad de Bogota Distrito Capital de Colombia, en el periodo comprendido entre el año  2017 y 2018.

### 1.2 - Por qué un mapa ayuda a resolverlo?

El simple hecho de tener una visión general del área de estudio y/o interés desde una perspectiva geográfica, aumenta la colaboración para las personas que tomaran la decisión frente a la problemática a tratar.
De igual forma la integración con otras disciplinas básicas e instrumentales, en especial la matemática, la Geoestadística, Fotointerpretación, Geomorfología aplicada y Sistemas de información Geográfica, generan un andamiaje perfecto para la elaboración de productos finales, con los cuales se asesora de manera adecuada y acertada a los decisores.

### 1.3 - Descripcion del mapa tematico.

Aunque la base de datos contaba con una tipología para clasificar el hurto a comercio, se optó por mostrar cuales eran los lugares donde se concentraba la mayor parte de los casos reportados de este delito en la localidad de los Martires de la ciudad de Bogotá.

El mapa temático señala a partir de un código de colores las zonas donde hay puntos calientes, es decir, los lugares donde hay una mayor concentración de reportes.

### 1.4 Descripción de los métodos de clasificación seleccionados.

1. ***Hot spot***: Muestra en cada agrupación de datos el grado de representatividad del cluster mediante un grado de confianza.

2. ***Mapa de interpolación mediante el método de Kriging***: Hace una interpolación de valores a partir del valor de z obtenido en el archivo generado con la herramienta "Hot spot", con lo cual ayuda a obtener valores de la variable "z" en lugares donde no se dispone información, o lugares que se encuentran entre dos puntos con datos de "z".

Se considera que el mejor método para presentar los resultados es mediante el mapa de interpolación, dado que los cluster ayudan a entender mejor la concentración de los eventos de hurtos espacialmente en la ciudad de Bogotá.

## 1.5 - Fuentes utilizadas en la elaboración del producto cartográfico.

Para la creación de este mapa, se utilizó datos abierto de la página de [estadística de la Policía Nacional de Colombia](https://www.policia.gov.co/grupo-informaci%C3%B3n-criminalidad/estadistica-delictiva), referente al hurto del comercio.

## 1.6 - Procedieminto realizado.

Ingresamos a la página de estadística de la Policía Nacional de Colombia, en la parte inferior, encontramos **Delitos de Alto Impacto** y **año** en donde escogemos el delito de nuestra preferencia y el año en el cual deseamos conocer la información.

Una vez se solicita la información de nuestro interés en cuanto al delito y el año deseado, es entregada por la página web, un archivo de Excel con extensión xls, el cual ya puede ser manipulado en cualquier software cartográfico. 

Seguidamente utilizando el software cartografico ArcGis version 10.6.1, se desarrolla el ejercicio, así:

* La base de datos se encontraba en un formato .xls, por lo cual se tuvo que migrar a un tipo .txt para que se pudiera mostrar como coordenadas sobre el gráfico.
* Se creó un shapefile con los puntos, asignando el sistema de coordenadas WGS 84.
* Se agruparon los datos que guardaban cercanía, a partir de su distancia (esto con ayuda de la herramienta "Collect events".
* Seguidamente se obtuvieron los puntos calientes, a partir de la herramienta "Hot spot analysis".
* Se elabora el mapa de interpolación mediante el método de Kriging.
* Finalmente se edita gráficamente los datos obtenidos para producir el producto cartografico [MAPA](Taller 1)

### 1.7 - Ventajas - Desventajas - Dificultades


 











