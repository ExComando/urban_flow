# Urban Flow - Proyecto Integrador
** (Inicialización y configuración de la herramienta de versionado carga del dataset 
y desarrollo de los distintos puntos.)**

## Objetivo
El objetivo principal de este proyecto es aplicar los conocimientos adquiridos 
en para el versionado de código, la organización, limpieza del código y la 
utilización de pandas.

## Introducción y Contexto
En el marco del crecimiento urbano acelerado, el análisis de datos de tráfico es vital para 
reducir la congestión. Este Sprint se sitúa en la fase de 'Analisis de Datos' inicial.

## Conclusión

A partir del análisis del dataset de multas por exceso de velocidad, se observa que los datos originales presentaban varios problemas de calidad, como fechas inválidas, horarios mal cargados, ubicaciones con formatos inconsistentes, patentes con caracteres especiales y valores faltantes en columnas relevantes para el cálculo de las multas.

Luego del proceso de limpieza y normalización, fue posible obtener un dataset más consistente para el análisis. Se detectó que una parte importante de los registros tenía datos inválidos o incompletos, especialmente en las velocidades registradas, velocidades máximas y radares, por lo que debieron eliminarse para evitar conclusiones incorrectas.

También se observó que algunas infracciones fueron registradas con fechas corregidas a `1932-01-01` y horarios corregidos a `00:00`, lo cual indica que el sistema original tenía errores de carga o registros defectuosos. Estos valores permiten identificar datos recuperados o incompletos, pero deben interpretarse con cuidado.

En conclusión, el dataset contiene información valiosa para el análisis de infracciones de tránsito, pero requiere una etapa previa de limpieza y normalización para que los resultados sean confiables.

