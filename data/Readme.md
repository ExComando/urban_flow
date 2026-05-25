
Resumen de Urban Flow (Gestión y Procesamiento de Datos):
El proyecto implementa una arquitectura estructurada de datos para el flujo urbano,
dividiendo la información en tres etapas clave dentro del directorio data/:

Data Raw (Cruda): Almacena las imágenes originales (data/raw/imgs/) capturadas
por los sensores o cámaras de tráfico sin ninguna modificación.

Data Interim (Intermedia): Se realiza un procesamiento previo donde las imágenes se agrupan
y estructuran mediante metadatos en un archivo JSON (data/interim/group_images.json)
para indexar el contenido de data/interim/imgs/.

Data Processed (Procesada): Es el resultado final listo para análisis o modelos de Machine Learning. Convierte la información visual en datos estructurados tabulares, consolidando las infracciones detectadas en un archivo final (data/processed/speeding_fines_image.csv) que cruza las imágenes de los vehículos con las multas por exceso de velocidad.

Conclusión: Existe una relación directa de transformación: el pipeline del proyecto
toma datos no estructurados (imágenes de cámaras de seguridad/tráfico) y, mediante
procesamiento intermedio, los convierte en datos estructurados (un archivo CSV analítico)
útiles para la toma de decisiones o fiscalización automatizada.
