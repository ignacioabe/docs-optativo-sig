# Índice optativo MPUR

---

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

---

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

- cómo el SIG utiliza los datos geoespaciales
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
    - wiki
    - API overpass turbo (web y qgis)
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

Tarea para la casa.
<!-- 10 minutos -->

- armar los grupos
- elegir la ciudad
- buscar datos públicos para chile o la ciudad elegida
- revisarlos y crear una visualización interesante

### Clase 3: SIG: creación de datos
<!-- pendiente -->
### Clase 4: Cambios en el tiempo
<!-- pendiente -->
### Clase 5: Geopython
<!-- pendiente -->
### Clase 6: Análisis de ciudades (revisión avances)
<!-- pendiente -->
### Clase 7: Exámen
<!-- pendiente -->
