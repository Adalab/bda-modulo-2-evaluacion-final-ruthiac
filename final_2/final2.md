# MÓDULO 2: FINAL

Este proyecto consiste en la **extracción, almacenamiento y análisis de datos de películas** utilizando Python, Mysql, Json y librerias de py como Pandas, Numpy.


## 1️⃣ Extracción de datos de películas

-ENPOINT: https://beta.adalab.es/resources/apis/pelis/pelis.json

- Se transforman en un **DataFrame de Pandas** para preprara para su analisis, filtar, ordenar, moldear datos y limpiarlos .
- Ademas, se convierte los datos datos nulos que pueden aparecer de diferentes formas como por ejemplo ;'Nan','nan;, etc. y listas dentro de las columnas para que sean compatibles con MySQL.

---

## 2️⃣ Conexión a MySQL y Creaccion de la Base de Datos (BD)--

## 3️⃣ Inserción de datos en la base de datos

- Los datos del DataFrame se limpian y transforman.
- Se insertan en la tabla `movies` mediante `executemany`.

---

## 4️⃣ Obtención de información a partir de los datos

Se realizan varias consultas a sql, por ejemplo:

- **Películas con duración superior a 120 minutos**
SELECT COUNT(*) FROM movies WHERE duracion_minutos > 120.

- **CONCLUSION**
- Se logro obterner datos de la API publica en formato json.
- Se logro crear BD "movies"y tabla "movies" insertando los datos ejecutando executemany
- Se logro insertar datos a la BD
- Se logro obtener informaciona partir de los datos.
Cabe destacar la importancia de transformar los datos para poder usar con los distintos programas, en el ejercicio se adapto los datos desde formato Json a Py luego por un datafrma a Panda y esto conectarlos con Mysql.