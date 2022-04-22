# Índice optativo MPUR

## Estructura general sesiones

- primer módulo: teoría (80 minutos)
  - conversación introductoria
  - cátedra teórica
- descanso (20 minutos)
- segundo módulo: práctica
  - uso de herramientas
  - resolución de dudas
  - preguntas de exploración para la casa

En cada clase se revisará una herramienta que permitirá analizar uno o más temas (ej: NDVI -> vegetación). La idea es que vayan explorando la ciudad gradualmente con las herramientas vistas en clases para ir construyendo acumulativamente los trabajos.

## Clases

<!-- REMOTA -->

### Clase 1: introducción

<!-- teoría -->

Aspectos prácticos

- introducción personal
- presentación de los alumnos
- presentación del curso (PDF)
- metodología clases (ver arriba)

Contenidos curso

- Por qué crecen las ciudades?
  - Cómo crecen?
  - Cómo se cuantifica este crecimiento?
  - Cuáles son las consecuencias de este crecimiento?
- Qué son los sistemas de información geográfica (SIG)?
  - Cuál es su experiencia con SIG?
- En qué consiste la filosofía de código abierto?
- Qué son los datos abiertos?
  - Qué tipo de datos abiertos podemos encontrar? (casos extranjeros)
  - En qué consiste la visualización de datos?
- De qué modo la tecnología ha impactado en las materias del curso? (SIG - cartografía - datos - crecimiento urbano)

<!-- práctica -->

- principales herramientas de software a usar (mostrar brevemente)
  - SIG
    - QGIS
    - kepler.GL
  - análisis y limpieza
    - openRefine
    - Python
    - pandas / geopandas
    - otros
  - publicación web
    - leaflet
    - mapbox

<!-- PRESENCIALES -->

### Clase 2: SIG, lectura datos

<!-- Explicación problemas viaje. -->
<!-- Dudas sobre programación bimestre. -->

<!-- https://github.com/ignacioabe/docs-optativo-sig/blob/main/indice.md#clase-2-sig-lectura-datos -->

<!-- teoría -->

<!-- esto amerita tener unos esquemas ya diseñados -->

Aspectos básicos cartografía/mapeo
<!-- 25 minutos -->

- para qué sirve
- técnicas (ref. James Corner)
- sistemas de referencia de coordenadas - SRC
  - no hay solución perfecta
  - familias de proyecciones (planas, cilíndricas y cónicas)
  - distorsiones (forma, área, dirección, distancia)
  - sistemas comunes
    - wgs84 (EPSG:4326)
    - wgs84 / pseudo mercator (EPSG:3857)
    - utm19s (EPSG:32719)
- soportes gráficos
  - estáticos
    - impresos (láminas, diarios, libros, etc)
    - digitales
  - interactivos
    - web
    - aplicaciones móviles

Geodatos
<!-- 25 minutos -->

- cómo el SIG utiliza los datos geoespaciales (vínculos)
- formatos geoespaciales
  - vectoriales
    - CSV
    - shapefile
    - geojson
    - geopackage
    - teselas
  - raster
    - TIFF
    - DEM
    - txt
    - teselas
- fuentes
  - de terceros
    - openstreetmap
    - datos abiertos gubernamentales
    - ONGs
    - aplicaciones / empresas
  - propias
    - catastros en terreno (GPS, papel)
    - trazado de imágenes
    - encuestas
    - otros (sensores, IA, etc.)

<!-- pausa 10 minutos -->

Obtención de datos
<!-- 40 minutos -->
- obtención de datos
  - OSM
    - qué es
    - [wiki](https://wiki.openstreetmap.org/wiki/Main_Page)
    - API overpass turbo ([web](https://overpass-turbo.eu/) y qgis)
  - gubernamentales
    - [geoportal.cl](http://www.geoportal.cl)
    - [INE](https://ine.cl) -> portal de mapas -> geodatos abiertos
    - [earth explorer](https://earthexplorer.usgs.gov)
    - [EOS landviewer](https://eos.com/landviewer/)
- estructura carpetas
  - importancia del orden
  - ejemplo personal

<!-- pausa 10 minutos -->

Uso herramientas SIG
<!-- 50 minutos -->

- QGIS
  - interfaz
  - revisión de datos (ciclovías, condominios)
- openrefine
  - interfaz
  - depuración de datos (permisos edificación)
- Kepler.gl
  - interfaz
  - visualización de datos (permisos edificación)

Explicación tarea (ver archivo `tareas/tarea-clase-2.md`)

### Clase 3: SIG: creación de datos

Revisión de tarea anterior, búsqueda de datos
<!-- 30 minutos? -->

Teoría
<!-- 30 minutos -->

- introducción
- (navegación y cartografía) básica, medieval y moderna
- creación de información geoespacial
  - vectorial
    - levantamiento en terreno (con o sin GPS)
    - trazado fotos
    - encuestas
    - aplicaciones (uber, strava, etc)
    - geocodificación
    - derivada (procesos vectoriales)
  - raster
    - vuelos
    - satélites
    - drones
    - digitalización mapas
    - derivada (procesos raster)

<!-- pausa 10 minutos -->

Práctica: creación de datos
<!-- 50 minutos -->

- herramientas
  - en terreno
    - GPS o app equivalente [opentracks](https://f-droid.org/packages/de.dennisguse.opentracks/)
    - papel o [field papers](http://fieldpapers.org/?locale=es)
  - en el escritorio
    - QGIS
      - importación de datos GPS
      - interoperabilidad con AUTOCAD (ejemplo)
      - edición de capas
        - geometría
        - atributos
          - creación de columnas nuevas y derivadas
      - creación de capas
        - SRC y campos
        - imágenes de fondo (google + sectra)
        - dibujo de geometrías
        - ingreso datos
        - herramientas básicas de selección
        - herramienta vectoriales
          - de geoproceso
          - de geometría
          - de análisis

<!--  pausa 10 minutos -->

OPENSTREETMAP
<!-- 30 minutos -->

- creación de cuenta
- edición en ID
  - puntos clave antes de editar*
  - importación de datos GPS
  - trazado
  - claves / valores

Explicación de nueva tarea
<!-- 30 minutos? -->

Revisión grupos y ciudades asignadas
<!-- 30 minutos? -->

Explicación tarea (ver archivo `tareas/tarea-clase-3.md`)

### Clase 4: Cambios en el tiempo

Introducción teórica
<!-- 30 minutos o menos -->

- el tiempo en los datos
  - cómo se registra? pasado y presente
    - datos no geográficos (series de tiempo)
    - datos raster
    - datos vectoriales
  - características
    - formato
    - resolución temporal
    - señal, ruido y ciclos
  - métodos
- el tiempo en la cartografía
  - dos dimensiones ya ocupadas
  - [Charles Joseph Minard](https://www.nationalgeographic.com/culture/article/charles-minard-cartography-infographics-history)
  - [barcos en la bahía de San Francisco](https://labs.mapbox.com/bites/00318/?embed)

Herramientas prácticas
<!-- 90 min -->

- información vectorial
  - formateo fechas (openrefine) *permisos?*
  - controlador temporal en QGIS
  - filtro temporal en KEPLER.gl

- información raster
  - arreglo fechas en open refine
  - [google earth engine - timelapse](https://earthengine.google.com/timelapse/)
  - EOS Landviewer
  - georreferenciación de mapas antiguos (Biblioteca Nacional - Mapoteca)

Revisión avances grupos
<!-- 45 minutos -->

Nuevo encargo
<!-- 15 minutos -->

### Clase 5: Python para análisis estadístico y geográfico

#### Introducción
<!-- teoría, 30 min -->

- qué es la programación? (P+R)
- qué es un lenguaje de programación (P+R)
- python
  - características
    - alto nivel
    - interpretado
    - énfasis en legibilidad
  - usos más frecuentes
    - ciencia
      - estadística
      - aprendizaje automático
    - web

#### Elementos de lenguaje y sintaxis
<!-- teoría y práctica - ir pasando de pizarra a cuaderno, 30 minutos -->

Ver instrucciones [aquí](https://github.com/ignacioabe/docs-optativo-sig/blob/main/recursos.md#software-en-la-nube-saas) y cuaderno de código en la carpeta de drive `optativo MPUR/archivos de trabajo/jupyterlab/c5.1 python básico.ipynb`

- instalación de google collab en drive
- autorizar acceso a archivos
- comentario
- variable
- tipos de datos
  - str (cadena)
  - float (decimal)
  - int (entero)
  - bool (booleano)
  - conjuntos (lista, tupla, set)
  - operadores
    - aritmética
    - comparación
    - lógica
    - asignación
- bucles
  - for
  - while
- funciones
- módulos
  - pip
  - pandas
  - geopandas

#### Pandas
<!-- pizarra y jupyter, 60 min -->

Ver `optativo MPUR/archivos de trabajo/jupyterlab/c5.2 pandas.ipynb`

- funcionalidad
  - análisis datos
  - manipulación de datos
- uso básico
  - tipo de datos: dataframe
  - partes de un dataframe
  - lectura `pd.read_csv()`
  - revisión básica
    - tamaño `.shape`
    - columnas `.columns`
    - detalle columnas `info()`
    - primeras filas `head()`
    - fila individual `.iloc[n]`
  - revisión por columna
    - indexado `df.["a"]`
    - descripción `.describe()`
    - conteo de valores `value_counts()`
    - agrupado por otra columna `groupby()`
    - filtro por valor `df[df.a == 1]`
  - gráficos simples `plot()`

#### Geopandas
<!-- revisión rápida, cuaderno, 10 min -->

Ver `optativo MPUR/archivos de trabajo/jupyterlab/c5.3 geopandas.ipynb`

- funcionalidad
- tipo de datos: geodataframe
- src `df.src`
- geometría `df.geometry`
- operaciones geométricas

Revisión entregas anteriores
<!-- 45 minutos -->

Entrega nueva tarea
<!-- 15 minutos -->

### Clase 6: Visualización de datos y revisión pre exámen

#### Visualización de datos
<!-- 1 hora -->

- en qué consiste
- distribución de valores numéricos: medidas de tendencia central, histograma
- esquemas de color: secuencial, divergente, cualitativo
- mapeo cantidad a color: clases y modos
- otros elementos visuales: forma, tamaño, etc
- aplicación práctica en QGIS
- aplicación práctica en KEPLER.gl

#### Corrección de trabajos
<!-- 1,5 horas -->

Revisar lo que le falta a cada uno y ponerle nota preliminar como medida de la calidad y nivel de completitud.

#### Entrega tarea final
<!-- 0,5 horas -->

Ver `./tareas/tarea-clase-6-final.md`

### Clase 7: Examen
<!-- pendiente -->