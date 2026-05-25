# Urban Flow - Proyecto Integrador
Inicialización y configuración de la herramienta de versionado carga del dataset 
y desarrollo de los distintos puntos.

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

# Urban Flow - Grupo 52

## Sprint en curso: Sprint 2

### Objetivo
El objetivo actual es desarrollar un sistema automatizado que determine qué
multas de tránsito poseen evidencia visual válida mediante el tratamiento de
imágenes y la extracción de información visual.

### Introducción y Contexto del Trabajo
Los radares urbanos generan registros administrativos de multas de forma
automática y las cámaras asociadas registran la evidencia visual que acompaña
y valida la infracción.

En este sprint de trabajo nos enfocamos en resolver las siguientes problemáticas
del sistema:
- No todas las multas administrativas tienen una imagen asociada.
- No todas las imágenes guardadas corresponden realmente a una infracción.
- Pueden existir errores de detección en el sistema heredado.
