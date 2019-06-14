# 1 - Taller número tres

###  1.1 - Cuál es el problema a tratar?

Se quiere mostrar las condiciones de vida actuales de la ciudad de Bogotá, desde el ámbito de ordenamiento territorial y movilidad.

### 1.2 - Por qué una experiencia interactiva ayuda a resolverlo?

Los temas de ordenamiento territorial y movilidad son dos grandes capítulos dentro del desarrollo de cualquier ciudad, por esto mismo, estos capítulos manejan volúmenes de información bastante considerables, una experiencia gráfica permite digerir con mayor facilidad este tipo de información; una experiencia gráfica interactiva permite además realizar análisis mucho más complejos por la capacidad que brinda las herramientas para poder interactuar con varias capas de información al tiempo y poder aplicar operaciones entre ellas.

### 1.3 - Descripcion del mapa tematico.

***Estrato Socioeconómico. Bogotá D.C:*** Esta capa es un archivo CSV, el cual no tiene un atributo geográfico, pero cuenta con la identificación del lote y su respectivo estrato. [URL descarga](https://datosabiertos.bogota.gov.co/dataset/estrato-socioeconomico-bogota-d-c)

***-Localidad. Bogotá D.C***:Se descargó el archivo shapefile que es de tipo polígono, el cual contaba entre otros atributos con el nombre de la localidad, código y acuerdo por el cual se adoptó. Su sistema de referencia es GCS_MAGNA. [URL descarga](https://datosabiertos.bogota.gov.co/dataset/localidad-bogota-d-c)

***-Lote. Bogotá D.C***: Se descargó el archivo shapefile que es de tipo polígono, el cual contaba entre otros atributos con el código del lote, dispersión, predial, código de la manzana. Su sistema de referencia es GCS_MAGNA.[URL descarga](https://datosabiertos.bogota.gov.co/dataset/lote)

***-Paradero SITP. Bogotá D.C:***: Se descargó el archivo shapefile que es de tipo punto, el cual contaba entre otros atributos con el código del paradero, nombre, tipo, dirección, servicio, rutas. Su sistema de referencia es GCS_MAGNA.[URL descarga](https://datosabiertos.bogota.gov.co/dataset/paradero-sitp-bogota-d-c)

***-Nodo de Transporte. Bogotá D.C***: Se descargo el archivo shapefile que es de tipo polígono, el cual contaba entre otros atributos con el código, nombre, tipo, modo, modo de transporte, dirección. Su sistema de referencia es GCS_MAGNA.[URL descarga](https://datosabiertos.bogota.gov.co/dataset/nodo-de-transporte-bogota-d-c)

***-Malla Vial Integral. Bogotá D.C.***: Se descargo el archivo shapefile que es de tipo línea, el cual contaba entre otros atributos con la clase, tipo, nombre, vía principal, vía generadora, nombre antiguo, etiqueta. Su sistema de referencia es GCS_MAGNA.[URL descarga]( https://datosabiertos.bogota.gov.co/dataset/malla-vial-integral-bogota-d-c)

***-Unidad de planeamiento zonal***: Edificación con cubierta de carácter permanente asociada a un lote destinada a proteger contra la intemperie a personas, animales o bienes. Su extensión geográfica es el Distrito Capital.[URL descarga](http://datosabiertos.bogota.gov.co/dataset/construccion-bogota-d-c)

### 1.4 Descripción de los métodos de clasificación seleccionados.

Para obtener el mapa de estratos primero se tuvo que realizar un join entre la tabla de estratos y el shapefile de lotes. A continuación, se realizó un intercept con el shapefile de localidades para obtener a qué localidad pertenecía cada lote. Luego, se intentó subir cargar el archivo a Carto, pero el procedimiento falló por el gran tamaño del archivo, por ello se tuvo que disolver los polígonos de los lotes por los atributos de estrato y localidad.
Para el mapa de transporte de Bogotá, se le borraron algunos elementos que no se consideraron relevantes para la información que se quería mostrar.
Al mapa de malla vial integral, no se le realizó ninguna modificación a su información.

### 1.5 - •	Descripción de las diferentes técnicas y métodos utilizados para la visualización de datos.

Los mapas que fueron publicados en carto, como se dijo anteriormente estaban conformados por capas, por lo cual estas debían ser editadas individualmente; por ejemplo, se les cambio el estilo a los elementos (color, grosor de línea), se configuraron algunos widgets como el conteo interactivo de elementos, se le adicionaron pop-ups para la visualización de algunos de sus atributos cuando se seleccionara un elemento en específico. Pro último se le agrego una leyenda a los mapas para la identificación de clases.

### 1.6 •	Descripción breve de las diferentes herramientas y procedimientos utilizadas para publicar el contenido en la web.

Para la visualización de datos primero se cargaron los archivos descargados de la página de datos abiertos a carto, luego se crearon los mapas a través de la adición de los archivos en forma de capas, luego con los mapas publicados, se recurrió a la herramienta de Story maps de ESRI para conformar la historia:
La herramienta de Story maps permite mezclar varios tipos de gráficos y texto, además que la presentación de cascada permite configurar la historia como si fuese una presentación; por ello, primero se configuraron los títulos como capítulos de la historia, luego se escribieron los textos donde se contaban los hechos, para enriquecer la experiencia se embebieron lo mapas que fueron publicados en carto. 
La experiencia estuvo acompañada de imágenes tomadas de fuentes como Flickr que son de dominio público.

### 1.7 •	Ventajas / desventajas / dificultades de la publicación de mapas utilizando herramientas en la nube respecto al software desktop.

## ***Ventajas***

* Permite visualizar mapas en equipos donde no se tenga instalado el software de escritorio, basta con que el equipo donde se quiera visualizar cuente con acceso a internet.
* Se pueden visualizar mapas desde equipos móviles.
* Permite un ambiente interactivo, donde se puede jugar con los atributos y visualización de los mapas.

## ***Desventajas***

* Es necesario pagar para usar la herramienta.
* En el modo gratuito para estudiantes limita algunas herramientas.
* Los mapas publicados en el modo gratuito siempre son públicos, por lo cual se pierde el control en cuanto a la privacidad de los mapas e información.

## ***Dificultades***

* La capacidad de procesamiento y almacenamiento en la nube son limitados, cuando se intenta cargar un archivo demasiado pesado, se requiere que este sea partido en porciones más pequeñas y luego sea indexado, para que así se pueda trabajar con él.
* Cuando se requiere realizar una tarea personalizada, es necesario recurrir a la programación, para ello es necesario contar con una capacitación adecuada para poder ejecutar estas tareas.

•	[URL de la experiencia interactiva](https://fr-ingenieria.maps.arcgis.com/apps/Cascade/index.html?appid=11912b51a46441cc81ae56beb1df818a)











