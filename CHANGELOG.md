# Changelog - Grupo [Número]

## [Día 1] - 2026-04-16
### Agregado
- Estructura de directorios.

Notebook principal del Sprint 1: 01_Urban_Flow-DARDO DARIO CALLADO.ipynb.
Variable de seguridad desactivar_git_push dentro del notebook.

- Rama Sprint_1.
- README y CHANGELOG iniciales.

### Autores
- [DARDO]

---

## [Día 2] - 2026-04-17
### Agregado
Desarrollo del Ejercicio 2:
- Creación de la estructura de carpeta si no existe
- Descarga y guardado del dataset
- Mostrar primeras 5 filas
- Mostrar tipos de datos
- Mostrar valores nulos


### Autores
- [ROSENDO]


---


## [Día 3] - 2026-04-18
### Agregado
Desarrollo del Ejercicio 3:
- Normalizar fechas
- Normalizar horas
- Normalizar ubicaciones
- Limpiar y normalizar patentes
- Limpieza de valores relevantes para multas
- Detección y limpieza de outliers
- Nuevo atributo `exceso_velocidad_real`
- Nuevo atributo `exceso_velocidad`
- Limpieza de no infractores
- Grabado del dataset limpio en `urban_flow/data/interim/speeding_fines.csv`

### Autores
- [MARTIN]

---


## [Día 4] - 2026-04-23
### Agregado
Desarrollo del Ejercicio 4:
- Definicion de la clase FineAnalyzer
- Encampsulamineto de los datos
- Implementacion de los metodos
- Creacion del objecto e invocacion de cada uno de los metodos en celdas separadas
- Actualizacion del README.md


### Autores
- [DARDO]


## [Día 5] - 2026-04-24
### Agregado
Desarrollo del Ejercicio 5:
- Creacion de grafico de barra, torta, linea

### Autores
- [SAUL]

---


## [Día 6] - 2026-04-24
### Agregado
Desarrollo del Ejercicio 6:
- Calcular y mostrar la proporción de infracciones registradas en la fecha 1932-01-01
- Calcular y mostrar la proporción de infracciones registradas en la hora 00:00

### Autores
- [MARTIN]

---

## [Día 7] - 2026-04-25
### Agregado
Desarrollo del Ejercicio 7:
- Redacción de la conclusión

### Autores
- [ROSENDO]

---


# Changelog - Grupo 52

## [Sprint 2 - Día 1] - 2026-05-18
### Agregado

- Inicialización y configuración de Git.
- Clonado de repositorio.
- Descarga, extracción y ordenamiento del dataset de imágenes.

### Autores
- [Dardo]

## [Sprint 2 - Día 2] - 2026-05-18
### Agregado

- Verificación de datos de imágenes y cálculo de tamaños en KB.
- Clasificación de imágenes en 'plates' y 'completes' según su ancho.
- Exportación del diccionario estructurado a group_images.json.
- Implementación de la función de visualización aleatoria de imágenes.

### Autores
- [Dardo]

## [Sprint 2 - Día 3] - 2026-05-19
### Agregado

- Conversión a escala de grises de las imágenes originales y almacenarlas.
- Realizar un suavizado de las imágenes en escala de grises y almacenarlas.
- Realizar una detección de bordes sobre las imágenes suavizadas para intentar detectar las patentes y almacenarlas.

### Autores
- [Rosendo]

## [Sprint 2 - Día 4] - 2026-05-21
### Agregado

- Extracción de patentes de imágenes con OCR.
- Matching de patentes reales del CSV con las extraídas de las imágenes.
- Modificación y grabado del CSV con nuevas columnas para las imágenes de patentes relacionadas.

### Autores
- [Martin]

## [Sprint 2 - Día 5] - 2026-05-22
### Agregado

- Cálculo de multas a partir de la columna `exceso_velocidad`.
- Integración de imágenes asociadas a cada multa según `exceso_velocidad`.
- Identificación de imágenes sin correspondencia en el dataset principal.
- Análisis de multas pendientes de pago.
- Relación entre multas impagas y la existencia de imágenes asociadas.

### Autores
- [Saul]
