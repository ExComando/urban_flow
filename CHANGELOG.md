# Changelog - Grupo 52

## [Sprint 2 - Día 6] - 2026-05-24
### Agregado

- Finalizacion y resumen del proyecto.

### Autores
- [Dardo]

## [Sprint 2 - Día 5] - 2026-05-22
### Agregado

- Cálculo de multas a partir de la columna `exceso_velocidad`.
- Integración de imágenes asociadas a cada multa según `exceso_velocidad`.
- Identificación de imágenes sin correspondencia en el dataset principal.
- Análisis de multas pendientes de pago.
- Relación entre multas impagas y la existencia de imágenes asociadas.

### Autores
- [Saul]

## [Sprint 2 - Día 4] - 2026-05-21
### Agregado

- Extracción de patentes de imágenes con OCR.
- Matching de patentes reales del CSV con las extraídas de las imágenes.
- Modificación y grabado del CSV con nuevas columnas para las imágenes de patentes relacionadas.

### Autores
- [Martin]


## [Sprint 2 - Día 3] - 2026-05-19
### Agregado

- Conversión a escala de grises de las imágenes originales y almacenarlas.
- Realizar un suavizado de las imágenes en escala de grises y almacenarlas.
- Realizar una detección de bordes sobre las imágenes suavizadas para intentar detectar las patentes y almacenarlas.

### Autores
- [Rosendo]


## [Sprint 2 - Día 2] - 2026-05-18
### Agregado

- Verificación de datos de imágenes y cálculo de tamaños en KB.
- Clasificación de imágenes en 'plates' y 'completes' según su ancho.
- Exportación del diccionario estructurado a group_images.json.
- Implementación de la función de visualización aleatoria de imágenes.

### Autores
- [Dardo]






## [Sprint 2 - Día 1] - 2026-05-18
### Agregado

- Inicialización y configuración de Git.
- Clonado de repositorio.
- Descarga, extracción y ordenamiento del dataset de imágenes.

### Autores
- [Dardo]
# Changelog - Grupo 52

## [Sprint 3 - Día 1] - 2026-06-13
### Agregado

- Inicialización y configuración de Git.
- Clonado de repositorio.
- Migración de imágenes binarias a DVC.
- Diseño del Modelo Lógico y configuración de ORM SQLAlchemy.
- Poblado de base de datos relacional y vectorización en ChromaDB.

### Autores
- [Dardo]

## [Sprint 3 - Día 2] - 2026-06-13
### Agregado

- Creación de la función procesar_fila_csv.
- Uso de la multa para procesar una fila del archivo CSV.

### Autores
- [Rosendo]

## [Sprint 3 - Día 3] - 2026-06-13
### Agregado

- Creación de Modelo Relacional.

### Autores
- [Rosendo]
