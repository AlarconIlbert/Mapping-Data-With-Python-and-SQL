# Web Scraping y conexiones a PostgresSQL

## Descripción

Este proyecto tiene como objetivo realizar un análisis de datos de vinos a partir de un conjunto de datos proporcionado en formato CSV y JSON. Utilizamos herramientas de análisis de datos como pandas en Python para realizar diversas operaciones de filtrado y transformación en los datos.

Los objetivos de este proyecto de web scraping fueron los siguientes:

1. **Aprender las Bases**: Familiarizarse con las bibliotecas `requests` y `BeautifulSoup` y aprender cómo realizar solicitudes HTTP y analizar documentos HTML.

2. **Extracción de Datos Relevantes**: Identificar y extraer datos específicos de un sitio web, como encabezados, fechas y contenido de noticias.

3. **Manejo de Errores**: Implementar manejo de errores para abordar situaciones donde la página web no cumple con la estructura esperada o no contiene ciertos elementos.

4. **Organización de Datos**: Crear un DataFrame de Pandas para organizar y estructurar los datos extraídos de manera eficiente.

5. **Practicar la Automatización**: Practicar la automatización de tareas repetitivas de recopilación de datos, lo que puede ahorrar tiempo y esfuerzo en la obtención de información actualizada.

Estos objetivos fueron alcanzados con éxito y proporcionan una base sólida para futuros proyectos de web scraping y análisis de datos en Python.


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

## Elección de PostgreSQL como Base de Datos

En este proyecto, hemos elegido PostgreSQL como nuestro sistema de gestión de bases de datos. La elección de PostgreSQL se basa en varias consideraciones clave:

### 1. **Escalabilidad**

PostgreSQL es conocido por su capacidad de escalabilidad tanto vertical como horizontal. Esto significa que puedes comenzar con una configuración más pequeña y, a medida que tu aplicación o proyecto crezca, puedes escalar la base de datos para manejar cargas de trabajo más grandes sin problemas. PostgreSQL también admite clústeres y replicación, lo que permite una alta disponibilidad y una mejor distribución de la carga.

### 2. **Rendimiento**

PostgreSQL ofrece un rendimiento sólido y es altamente optimizable. Su motor de consulta es altamente eficiente, lo que lo hace adecuado para aplicaciones que requieren consultas complejas y análisis de datos intensivos.

### 3. **Características Avanzadas**

PostgreSQL es conocido por su amplia gama de características avanzadas, que incluyen soporte para tipos de datos personalizados, funciones y procedimientos almacenados, control de concurrencia avanzado y capacidades de georreferenciación. Estas características hacen que PostgreSQL sea una elección sólida para proyectos que requieren funcionalidades específicas y avanzadas.

### 4. **Licencia Open Source**

PostgreSQL es una base de datos de código abierto con una licencia que permite su uso gratuito y la posibilidad de modificar su código fuente según sea necesario. Esto lo convierte en una opción económica y flexible para proyectos de cualquier tamaño.

### 5. **Comunidad Activa**

PostgreSQL cuenta con una comunidad activa de desarrolladores y usuarios en todo el mundo. Esto significa que hay una amplia gama de recursos disponibles, incluyendo documentación, bibliotecas de código y soporte de la comunidad.

En resumen, PostgreSQL es una base de datos sólida y versátil que ofrece escalabilidad, rendimiento y una amplia gama de características avanzadas. Su naturaleza de código abierto y su comunidad activa lo convierten en una elección ideal para proyectos de cualquier tamaño y complejidad.
------
# Web Scraping con Python: Extracción de Datos de Páginas Web

El web scraping es una técnica utilizada para extraer datos de sitios web de manera automatizada. En Python, dos bibliotecas ampliamente utilizadas para realizar web scraping son `requests` y `BeautifulSoup`.

## Beneficios de la Biblioteca `requests`

La biblioteca `requests` es una herramienta poderosa para realizar solicitudes HTTP en Python. Algunos de sus beneficios clave incluyen:

- **Facilidad de Uso**: `requests` permite realizar solicitudes HTTP de una manera sencilla y legible en Python, lo que facilita la interacción con sitios web.

- **Flexibilidad**: Puede ser utilizada para realizar una variedad de solicitudes HTTP, como obtener páginas web, enviar datos de formularios, manejar autenticación y más.

- **Manejo de Errores**: `requests` incluye un manejo eficiente de errores HTTP, lo que permite detectar problemas al acceder a un sitio web.

- **Compatibilidad**: Es ampliamente compatible con diferentes versiones de Python y se integra bien con otras bibliotecas de Python.

## Beneficios de la Biblioteca `BeautifulSoup`

La biblioteca `BeautifulSoup` es una biblioteca de análisis HTML que se utiliza comúnmente junto con `requests` para extraer datos de páginas web. Sus beneficios incluyen:

- **Análisis Estructural**: `BeautifulSoup` permite analizar la estructura de un documento HTML o XML y extraer fácilmente información específica.

- **Navegación Simple**: Proporciona una forma sencilla de navegar por el DOM (Modelo de Objeto de Documento) de un documento web, lo que facilita la extracción de datos.

- **Soporte para Diferentes Parsers**: `BeautifulSoup` es compatible con varios analizadores HTML, lo que permite trabajar con diferentes tipos de documentos HTML.

- **Gran Comunidad y Documentación**: Es ampliamente utilizado y tiene una gran comunidad de usuarios, por lo que puedes encontrar abundante documentación y ejemplos en línea.

## Ejemplo de Uso

A continuación, se muestra un ejemplo de cómo se pueden utilizar `requests` y `BeautifulSoup` para realizar web scraping en Python:

```python
import requests
from bs4 import BeautifulSoup

# Realizar una solicitud HTTP
url = 'https://www.ejemplo.com'
response = requests.get(url)

# Analizar el contenido HTML de la página
soup = BeautifulSoup(response.text, 'html.parser')

# Extraer datos específicos
titulo = soup.find('h1').text
parrafos = soup.find_all('p')

# Imprimir los resultados
print('Título:', titulo)
for parrafo in parrafos:
    print('Párrafo:', parrafo.text)
```

-----

## Resultados

Durante el análisis, generamos varios DataFrames filtrados que se guardaron en archivos JSON en la carpeta `sample_data/`. Puedes utilizar estos archivos para consultas o análisis adicionales.

Durante este proyecto de web scraping, hemos logrado con éxito extraer datos de sitios web utilizando las bibliotecas `requests` y `BeautifulSoup`. Algunos de los resultados clave incluyen:

- Extracción de encabezados y contenido de noticias de un sitio web de noticias.

- Extracción de fechas de publicación y enlaces de noticias.

- Manejo de casos donde las noticias no contenían imágenes.

- Creación de un DataFrame de Pandas para almacenar y organizar los datos extraídos.

Estos resultados demuestran la capacidad de Python para automatizar la recopilación de información valiosa a partir de recursos en línea.


## Contribuciones

Las contribuciones a este proyecto son bienvenidas. Si deseas mejorar el análisis, agregar nuevas funcionalidades o realizar correcciones, no dudes en hacer una bifurcación del repositorio y enviar una solicitud de extracción.

## Licencia

Este proyecto se encuentra bajo la licencia [MIT](LICENSE), lo que significa que puedes utilizar, copiar y modificar el código como desees. Te animamos a dar crédito si utilizas este proyecto como base para tus propios análisis de datos.