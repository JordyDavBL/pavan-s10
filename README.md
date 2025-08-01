# **Trabajo Bimestral de Programación**
## Integrantes:
* BETANCOURTH LEON JORDY DAVID
* CUENCA GUAMAN STEVEEN ALEXANDER
* MARIA ÁNGEL ROJAS ROJAS 

## Objetivo 
El proposito del presente proyecto es realizar un análisis exploratorio y descriptivo de un conjunto de datos de nacimientos registrados en Ecuador, con el fin de identificar patrones **sociodemograficos** y de salud **materno-infantil**, mediante el uso de _**Apache Spark**_ en _**Zeppelin**_.

## Desarrollo

### 1.  ***Comprensión del reto y Revisión de Dataset***
Se revisó el contenido del archivo **CSV(_**ENV_2023.csv**_)** con los registros del nacimiento.

Se identificaron varias vartiables clave como: *edad_mad, tipo_part, peso, etnia, lugar_ocur, nivel_instruccion, prov_res, sabe_leer, apgar1, apgar5, etc.* 

Se defininió la estrategia de limpieza y tratamiento de datos nulos y erróneos,

### 2.  ***Limpieza y preprocesamiento***
Se usó ***Apache Spark*** para: 
* Convertir columnas numéricas con punto decimal.
* Tratar valores nulos o inválidos como ***"Sin información"*** y los valores que se encontraban como: "0", "" reemplazamos con ***null***.
* Normalizar tipos de datos (fechas, numéricos, categóricos).


### 3.  ***Análisis Descriptivo Inicial***
Se aplicó .groupBy()  para obtener:

Distribuciones por provincia, tipo de parto, sexo y semanas de gestación.

Comparaciones de peso, edad materna y número de hijos.

Se generaron las primeras visualizaciones con z.show() en Zeppelin.



### 4.  ***Consultas Específicas y Preguntas Analíticas***
Se formularon más de 10 preguntas analíticas como:

¿Qué provincias tienen más madres adolescentes?

¿Cómo varía el peso del recién nacido según sexo y semana?

¿Qué porcentaje de madres es analfabeta según provincia?

¿Cuál es la distribución de partos por área de residencia?



### 5.  ***Visualización y Análisis de Resultados***
Se graficaron los resultados con etiquetas, colores y escalas para mejor interpretación.

Se identificaron patrones notables, por ejemplo:

Mayor frecuencia de partos por cesárea en madres con educación superior.

Provincias con mayor número de nacimientos fuera de hospitales.

Mayor analfabetismo en ciertas zonas rurales.


### 6.  ***Generación de Dashboard HTML (manual)***
Se incrustaron los gráficos exportados como imágenes PNG dentro de un HTML tipo informe.

Se creó un menú lateral de navegación por cada pregunta analítica.

Cada sección del HTML incluye:

Título de la pregunta

Gráfico

Análisis o interpretación textual


### 7.  ***Revisión de Insights y Redacción de Análisis Final***
Se redactaron los análisis correspondientes a cada pregunta.

Se evaluaron variables con más impacto sobre nacimientos: tipo de establecimiento, estado civil, instrucción, edad.

Se organizaron los resultados para presentar hallazgos relevantes de forma clara.


## Utilidad del Análisis
Este proyecto permite:
* Evaluar condiciones de salud y sociales de madres y recién nacidos.
* Detectar zonas de riesgo (alta cesárea, baja instrucción, partos domiciliarios).
* Apoyar con datos el diseño de políticas públicas de salud materna.
