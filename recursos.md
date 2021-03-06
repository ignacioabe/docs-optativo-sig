# Recursos

## Software de escritorio

### QGIS

Sitio oficial: <https://qgis.org>

Las descargas oficiales se pueden encontrar en el [sitio de qgis](https://www.qgis.org/es/site/forusers/download.html). La versión actual es la `3.24`.

El programa es autocontenido y no tiene ningún requerimiento externo aparte de un sistema operativo medianamente actualizado.

- windows (instalador MSI): <https://qgis.org/downloads/QGIS-OSGeo4W-3.24.0-2.msi>
- macos: <https://qgis.org/downloads/macos/qgis-macos-pr.dmg>
- linux: usar instalador de paquetes según el sistema operativo.

### Open Refine

Sitio oficial: <https://openrefine.org/>

La versión actual es la `3.5.2`

- windows: <https://github.com/OpenRefine/OpenRefine/releases/download/3.5.2/openrefine-win-with-java-3.5.2.zip>
- macos: <https://github.com/OpenRefine/OpenRefine/releases/download/3.5.2/openrefine-mac-3.5.2.dmg>
- linux: <https://github.com/OpenRefine/OpenRefine/releases/download/3.5.2/openrefine-linux-3.5.2.tar.gz> (esta versión requiere la instalación separada de JAVA)

## Software en la nube (SaaS)

### Kepler.gl

Es simplemente una página web, así que no requiere ninguna instalación previa. Se puede revisar en <https://kepler.gl/>

### Google colaboratory

Instrucciones para activarlo

- Entrar (log in) en google drive con la cuenta UC.
<!-- - Abrir el [sitio web](https://colab.research.google.com/) -->
- Ir a la carpeta compartida del curso
- Ir la carpeta `optativo MPUR/archivos de trabajo/jupyterlab/
- Hacer clic secundario en el archivo `c5.1 python básico` y luego en `abrir con` -> `google colaboratory`.
- Es posible que los haga pasar por unos diálogos para incorporar *colab* a *drive*.

Instrucciones para que *colaboratory* lea datos directo desde google drive.

- Abrir el cuaderno `c5.2 pandas.ipynb`.
- Ejecutar la segunda celda de código, que dice lo siguiente:

```python
# permite acceso a archivos de drive
from google.colab import drive
drive.mount('/content/drive')
```

- Permitir que el *notebook* acceda a los archivos de *google drive*.
- Ejecutar la tercera celda. Si se completa sin errores, está todo ok.

## Software móvil GPS

- [osmand](https://osmand.net/) iOS - android
- [osmtracker](https://play.google.com/store/apps/details?id=net.osmtracker) sólo android
- [opentracks](https://play.google.com/store/apps/details?id=de.dennisguse.opentracks.playstore) sólo android - vale $3.000

## Datos geoespaciales

### Repositorio curso

- Carpeta compartida en [google drive](https://drive.google.com/drive/folders/1W9zvuSBB04ljfNTh9Ze0MmAwL0KR2CDu?usp=sharing)

Contiene:

- archivos de trabajo
  - jupyterlab
  - QGIS
- conjuntos de datos
  - geodatos
    - raster
    - vectorial
- entregas (por clase)
- grabaciones clases
- imágenes
- presentaciones
- referencia
- lista de curso (planilla)

### Chile

- [geoportal.cl](http://www.geoportal.cl)
- [INE](https://ine.cl) -> portal de mapas -> geodatos abiertos

### Openstreetmap

- [sitio principal](https://openstreetmap.org)
- [wiki](https://wiki.openstreetmap.org/wiki/Main_Page)
- [API overpass turbo](https://overpass-turbo.eu/)

### Satelitales/cobertura mundial

- [earth explorer](https://earthexplorer.usgs.gov)
  - requiere una cuenta de usuario
  - ver fotos landsat y sentinel, permite capas derivadas (NDVI u otras)

- [EOS landviewer](https://eos.com/landviewer/)
  - requiere una cuenta de usuario
  - fotos landsat
  - modelos de elevación digital (DEM)
    - ASTER (30 m/px)
    - GMTED2010 (hay distintas resoluciones disponibles)

## Teselas (imágenes cuadradas de fondo)

Referencia: [Artículo sobre cómo añadirlas](https://mappinggis.com/2018/03/como-anadir-mapas-base-en-qgis-3-0-openstreetmap-google-carto-stamen/)

Google Satellite: `http://www.google.cn/maps/vt?lyrs=s@189&gl=cn&x={x}&y={y}&z={z}`

Google Terrain: `https://mt1.google.com/vt/lyrs=t&x={x}&y={y}&z={z}`

ESRI Imagery/Satellite: `https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}`
