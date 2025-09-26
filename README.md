🗺️ Mapa Interactivo de Cancún con Capas GIS

Este proyecto consiste en una página web (maptest.html) que utiliza Mapbox GL JS para mostrar un mapa base centrado en Cancún, al cual se superponen dos tipos de capas de información geográfica (GIS): una capa WMS (Raster) y una capa vectorial GeoJSON (Polígonos), con una simbología temática y una leyenda dinámica.

Características Principales ✨

Visualizador de Mapas: Implementación de un mapa interactivo usando la librería Mapbox GL JS (v3.4.0).

Capas Múltiples: Configuración para consumir y visualizar diferentes tipos de servicios GIS.

Capa Vectorial (GeoJSON): Carga de polígonos (crecimientoG.geojson) que representan la expansión urbana de Cancún por periodos.

Simbología Temática: Aplicación de una escala de color cuantitativa/categórica utilizando la expresión ['match'] de Mapbox, basada en la propiedad "LUSTRO" (valores de 1975 a 2025).

Leyenda Dinámica: Inclusión de un componente HTML/CSS/JS para mostrar la leyenda correspondiente a la escala de color aplicada a la capa GeoJSON.

Capa WMS (Opcional): Estructura de código para añadir un servicio WMS (Web Map Service) como capa raster sobre el mapa base.

🚀 Requisitos Previos

Para que este código funcione correctamente, necesitas:

Token de Acceso de Mapbox: Una clave pública de Mapbox (reemplazar la clave de ejemplo en el código con tu propio token).

Servidor Web Local: El navegador requiere que los archivos GeoJSON externos se carguen a través de un servidor web (ej. http://localhost:8000/) para evitar errores de CORS (Cross-Origin Resource Sharing). No funcionará si se abre directamente el archivo HTML desde el disco duro (file:///).

Archivo GeoJSON: El archivo de datos vectoriales crecimientoG.geojson debe estar ubicado en la ruta ./datos/crecimientoG.geojson (relativo al maptest.html).
