# 1 - Taller número dos

###  1.1 - Cuál es el problema a tratar?

La información de Geomorfología de las ciudades y asentamientos humanos es vital para la formulación de estudios de gestión del riesgo, por ello esta información debe ser recolectada, procesada, analizada y utilizada por instituciones como el IDIGER.

### 1.2 - Por qué un mapa ayuda a resolverlo?

Un mapa es bastante útil para ubicar espacialmente los lugares donde existen ciertos tipos de geomorfologías, además un mapa es una herramienta gráfica que muestra explícitamente las extensiones y limites de cada una de las áreas.
Por otro lado, esta capa es un insumo básico para fabricar otros mapas, ya que permite identificar los lugares que por su geomorfología permiten clasificar las zonas de amenaza alta, media y baja.

### 1.3 - Descripcion del mapa tematico.

El mapa temático fue hecho y publicado con la herramienta Carto.

El mapa ubica espacialmente los polígonos de geomorfología de la ciudad de Bogotá, los polígonos están clasificados dentro de las 41 categorías propuestas para este mapa:

***-Área de Recreación Activa y Pasiva***
***-Área Urbanizada***
***-Barras Puntuales***
***-Cantera Activa***
***-Cerros Remanentes o Relictos***
***-Colinas con Control Estructural***
***-Colinas Monoclinales y Escarpes Estructurales***
***-Colinas Residuales***
***-Conos de Planicie***
***-Crestas Redondeadas***
***-Escarpe de Erosión Menor***
***-Escarpe de Falla***
***-Escarpe de Terraza***
***-Escarpe Estructural***
***-EScarpe Estructural de Falla***
***-Escarpe Estructural Menor***
***-Escarpe y Contrapendiente Estructural***
***-Escarpe y Frente Estructural***
***-Excavaciones***
***-Flujos Torrenciales***
***-Frente Estructural***
***-Ladera de Acumulación***
***-Ladera en Contrapendiente Estructural***
***-Ladera en Pendiente Estructural***
***-Ladera Estructural de Moderada Pendiente***
***-Ladera Plana Ondulada***
***-Laderas de Piedemonte Degradadas***
***-Pendiente Estructural***
***-Pendientes y Escarpes Estructurales***
***-Plano de Abanico***
***-Plano de Inundación***
***-Plano de terraza***
***-Relleno Antrópico de Escombros***
***-Rellenos de basura o rellenos sanitarios***
***-Superficie de Aplanamiento***
***-Superficie de Erosión o aplanamiento***
***-Terrenos Ondulados***
***-Valle en U***
***-Vallecito en Forma de V***
***-Vega***

### 1.4 Descripción de los métodos de clasificación seleccionados.

El método de clasificación se realizó a partir de la variable componente, que se encontró dentro del shapefile descargado del visor web del IDIGER.

## 1.5 - Fuentes utilizadas en la elaboración del producto cartográfico.

Para la realización de este mapa se uso información obtenida en la página del IDIGER, descargada desde el [mapa temático](http://idiger.maps.arcgis.com/apps/webappviewer/index.html?id=fa4b277533584c3a95a9208b4d542e19).

El shapefile de Geomorfología fue obtenido desde la [URL](http://www.sire.gov.co/documents/82884/85260/Geomorfolog%C3%ADa_Urbana_Esc5000.zip/b7b6e61c-e4ae-4831-a7ae-8317ba8acfb3)

## 1.6 - Procedieminto realizado.

* Primero se descargó la información del visor web del IDIGER.

* Luego se cargo los datos como un archivo ZIP.

* Luego se creó un mapa agregando como capa la información de Geomorfología.

* Se configuró la visualización a partir de la variable componente.

* A este mapa se le configuró un widget para el conteo de las áreas por tipo de componente en la extensión de la vista actual, por lo cual este conteo es dinámico.

* Se cargo una leyenda a partir de las clases definidas por componentes.
* Se configuró un pop up con el atributo componente, con lo cual cuando se pica sobre cualquier polígono, se abre una ventana donde se especifica a que tipo de Geomorfología corresponde el elemento, esto ayuda en cuanto a la identificación dado que algunos polígonos son demasiado pequeños para que puedan ser identificados con una vista general del mapa.

[Se publicó como servicio público.](https://axel946.carto.com/builder/462d48f6-d5e2-438b-a640-8d9db33e0f7c/embed)

### 1.7 - Ventajas - Desventajas - Dificultades

## ***Ventajas:***

* Interfaz gráfica amigable.
* No es necesario programar para poder crear un mapa web.
* Un mapa web tiene la gran ventaja de ser interactivo y dinámico, a diferencia de un mapa estático producido como una salida gráfica de software como ArcGIS o QGIS

## ***Desventajas:***

* Es necesario pagar para usar la herramienta.
* En el modo gratuito para estudiantes limita algunas herramientas.
* Los mapas publicados en el modo gratuito siempre son públicos, por lo cual se pierde el control en cuanto a la privacidad de los mapas e información.

## ***Dificultades***

* Aunque la herramienta es bastante intuitiva, se deben conocer mejor las herramientas de análisis con las cuales cuenta el servicio.

### URL Mapa

* [Mapa](https://github.com/dersteppenwolf/cartografia_web)


