El objetivo de este ejercicio es familiarizarse con la relación entre usos del suelo y transporte a través de un indicador de accesibilidad agregado. Para ello, se plantea calcular el potencial que tienen tres localizaciones para acceder a mano de obra. Por ejemplo, una gran industria puede tener como factor de localización una elevada masa de población residente lo más cerca posible. Desde el punto de vista técnico, el objetivo es dotar al estudiante de la habilidad de realizar un flujo de trabajo completo, desde la adquisición de datos, tratamiento, almacenamiento en una base de datos espacial, análisis y evaluación de resultados.

El desarrollo de este caso práctico consta de las siguientes tareas:

Instalar PostgreSQL, con las extensiones PostGIS y pgRouting, y osm2po.
Conectar a la base de datos desde R.
Obtener la red de carreteras de la provincia elegida y zonas limítrofes (fuente recomendada OSM).
Obtener los polígonos de los municipios de la provincia elegida (fuente recomendada IGN).
Descargar los datos de población por municipio más recientes (fuente recomendada INE).
Calcular los centroides de los municipios utilizando funciones PostGIS desde R
Crear la topología de la red de carreteras utilizando funciones pgRouting desde
Vincular cada centroide con la red de carreteras
Utilizar las funciones de cálculo de rutas de pgRouting para obtener una matriz origen‐destino.
Calcular el potencial económico (también llamado potencial de mercado) de cada uno de los tres municipios seleccionados.
Presentar los resultados del cálculo del potencial económico de los tres municipios seleccionados en forma de tabla, gráfico o mapa, según se considere más oportuno.
Analizar el resultado (¿qué localización elegirías para una actividad con alta demanda de mano de obra?) y plantear mejoras al modelo y fuente de los datos. Por ejemplo, ¿qué sucedería si se incrementa o disminuye el parámetro de α de decaimiento con la distancia? ¿Qué datos aportarían mayor nivel de detalle espacial/temporal? Etc.
OPCIONAL: Calcular el potencial de mercado teniendo en cuenta los desplazamientos que se realizan entre los municipios del área de estudio por motivo de trabajo: a la masa de un municipio se le restan las personas que se desplazan fuera y se le suman las personas que acuden por motivo de trabajo. Fuente de datos: matrices de viajes de los estudios básicos por municipios del MITMA1. Immprescindible leer la descripción de los datos disponibles: https://movilidad‐opendata.mitma.es/README%20‐ %20formato%20ficheros%20movilidad%20MITMA%2020201228.pdf.