# Proyecto de Análisis de Datos de Vinos

## Descripción

Este proyecto tiene como objetivo realizar un análisis de datos de vinos a partir de un conjunto de datos proporcionado en formato CSV y JSON. Utilizamos herramientas de análisis de datos como pandas en Python para realizar diversas operaciones de filtrado y transformación en los datos.

## Conjunto de Datos

El conjunto de datos se compone de información sobre vinos, incluyendo detalles como el nombre del vino, región, variedad, puntuación y notas.

## Archivos del Proyecto

El proyecto incluye los siguientes archivos y carpetas:

- **`wine-ratings.csv`**: El archivo CSV original que contiene los datos de vinos.

- **`wine-ratings.json`**: El archivo JSON generado a partir de los datos del CSV.

- **`sample_data/`**: Una carpeta que contiene el conjunto de datos original y otros archivos relacionados.

## Requisitos

Asegúrate de tener Python y las siguientes bibliotecas instaladas para ejecutar el código:

- Pandas
- Json
- Jupyter Notebook

Puedes instalar estas bibliotecas utilizando `pip`:

pip install pandas
pip install jupyter


## Ejecución

Para ejecutar el análisis de datos, sigue estos pasos:

1. Clona o descarga este repositorio en tu máquina local.

2. Abre el cuaderno Jupyter Notebook `wine_analysis.ipynb` utilizando Jupyter Notebook.

3. Ejecuta las celdas del cuaderno para realizar el análisis de datos.

4. Puedes ajustar las consultas y operaciones según tus necesidades.

**Filtrar por Tipo de Vino (Vino Blanco)**

En esta consulta, nos enfocamos en identificar todos los vinos blancos presentes en nuestro conjunto de datos. Los vinos blancos tienen sus propias características únicas, y queríamos explorarlos en detalle.

Para realizar esta consulta, utilizamos pandas para filtrar el conjunto de datos original y seleccionar solo aquellos vinos que se clasifican como "Vino Blanco". Los resultados de esta consulta se exportaron a un archivo JSON llamado `white_wines.json` que contiene todos los vinos blancos en el conjunto de datos.

Puede acceder a los detalles de estos vinos blancos en el archivo JSON `white_wines.json`.

---

**Filtrar por Puntuación Alta**

En esta consulta, nos propusimos identificar todos los vinos que han recibido una puntuación igual o superior a 90 puntos. Las puntuaciones son un indicador importante de la calidad de un vino, y queríamos resaltar aquellos que se destacan.

Utilizamos pandas para filtrar el conjunto de datos original y seleccionar solo aquellos vinos con una puntuación de 90 o más. Los resultados se exportaron a un archivo JSON llamado `high_rated_wines.json` que contiene los detalles de estos vinos de alta puntuación.

Puede explorar estos vinos de alta puntuación en el archivo JSON `high_rated_wines.json`.

---

**Filtrar por Región de Austria**

En esta consulta, nos centramos en los vinos que provienen de la región de Austria. Queríamos destacar los vinos austriacos y explorar sus características únicas.

Para llevar a cabo esta consulta, utilizamos pandas para identificar y seleccionar los vinos cuya región contiene "Austria". Los resultados se guardaron en un archivo JSON llamado `austria_wines.json`, que contiene detalles sobre los vinos de esta región.

Puede obtener más información sobre los vinos austriacos en el archivo JSON `austria_wines.json`.

---

**Filtrar por Notas con "fruit bouquet"**

Esta consulta se enfocó en encontrar vinos que tuvieran notas de cata que incluyeran la frase "fruit bouquet". Queríamos destacar los vinos que ofrecen esta característica particular en su perfil de sabor.

Utilizamos pandas para identificar y seleccionar los vinos cuyas notas de cata contienen la frase "fruit bouquet". Los resultados se exportaron a un archivo JSON llamado `fruit_bouquet_wines.json`, que contiene detalles sobre estos vinos con notas especiales.

Puede explorar más sobre estos vinos en el archivo JSON `fruit_bouquet_wines.json`.

---

**Filtrar por Tipo de Vino (Vino Tinto)**

En esta consulta, nos centramos en identificar todos los vinos tintos en nuestro conjunto de datos. Los vinos tintos tienen sus propias características distintivas, y queríamos resaltarlos específicamente.

Para realizar esta consulta, utilizamos pandas para filtrar el conjunto de datos original y seleccionar solo aquellos vinos que se clasifican como "Vino Tinto". Los resultados se exportaron a un archivo JSON llamado `red_wines.json`, que contiene detalles sobre los vinos tintos en el conjunto de datos.

Puede obtener más información sobre estos vinos tintos en el archivo JSON `red_wines.json`.

---

## Resultados

Durante el análisis, generamos varios DataFrames filtrados que se guardaron en archivos JSON en la carpeta `sample_data/`. Puedes utilizar estos archivos para consultas o análisis adicionales.

## Contribuciones

Las contribuciones a este proyecto son bienvenidas. Si deseas mejorar el análisis, agregar nuevas funcionalidades o realizar correcciones, no dudes en hacer una bifurcación del repositorio y enviar una solicitud de extracción.

## Licencia

Este proyecto se encuentra bajo la licencia [MIT](LICENSE), lo que significa que puedes utilizar, copiar y modificar el código como desees. Te animamos a dar crédito si utilizas este proyecto como base para tus propios análisis de datos.