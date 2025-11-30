Carga, Exploración, Limpieza y Visualización Básica de un Dataset


Este proyecto realiza un análisis exploratorio de datos (EDA) del catálogo de Netflix, utilizando un dataset público con más de 8.000 títulos entre películas y series. El objetivo es comprender la estructura del dataset, corregir inconsistencias y extraer conclusiones relevantes mediante visualizaciones claras y bien justificadas.


DATASET UTILIZADO:

Netflix Movies and TV Shows Dataset (Kaggle)
Incluye información como:

Tipo de contenido (Movie / TV Show)

Título

Director

Reparto

País de origen

Fecha de incorporación a Netflix

Año de lanzamiento

Rating (clasificación por edades)

Duración

Géneros

Descripción



ESTRUCTURA DEL REPO :

Proyecto-EDA/
├── data/
│   ├── netflix_titles.csv      # Dataset original
│   └── netflix_clean.csv       # Dataset limpio
├── notebooks/
|---├── 01 Exploración de datos.ipynb  # Exploración de datos
│   ├── 02_limpieza.ipynb       # limpieza de datos
│   └── 03_visualizacion.ipynb  # Visualizaciones y análisis final
└── README.md




RESUMEN DEL PROCESO 

✔ Exploración inicial

Revisión de columnas, tipos de datos y valores únicos.

Identificación de problemas comunes:

Fechas en formato texto

Valores nulos en director, cast, country

Ratings incorrectos

Duraciones mezcladas (“min” vs “Seasons”)

✔ Limpieza de datos

Corrección de registros desalineados (p. ej. duraciones en la columna rating).

Conversión de date_added a formato datetime y validación de fechas.

Tratamiento de valores nulos mediante imputación razonada (“Desconocido”, mediana).

Revisión de coherencia entre type y duration.

✔ Visualización

Histograma de años de lanzamiento.

Barras comparativas entre películas y series.

Análisis de ratings.

Visualización de países con más contenido




CONCLUSIÓN :

El catálogo de Netflix está fuertemente dominado por películas, aunque las series han crecido en los últimos años.

La mayor parte del contenido corresponde a producciones recientes (2010–2021).

Las clasificaciones por edad más frecuentes son TV-MA y TV-14, orientadas a un público adulto.

Estados Unidos es el país más presente en el catálogo, seguido de India y Reino Unido.

