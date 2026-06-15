
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

### Sprint 3

**Objetivo:**
El objetivo principal de este proyecto es aplicar los conocimientos adquiridos en programación orientada a objetos y uso de base de datos. 
A partir de este tp se deben aplicar los conocimientos adquiridos del versionado de datos según su tipo.

**Introducción y Contexto del problema:**
El sistema ha crecido en volumen de datos y complejidad, por lo que ya no es viable trabajar únicamente con archivos CSV.

En este Sprint se profesionaliza la solución incorporando:
* Persistencia en base de datos relacional.
* Uso de ORM mediante SQLAlchemy.
* Control de versiones de datos.
* Preparación para búsquedas avanzadas.

Para ello es necesario migrar la información procesada a una base de datos estructurada.
### Sprint 3

**Objetivo:**
Profesionalizar y escalar la solución de gestión de infracciones urbanas mediante la implementación
de persistencia en bases de datos relacionales, el uso de bases de datos vectoriales para búsquedas
por similitud y la integración de herramientas de control de versiones para archivos binarios
masivos.

**Introducción y Contexto:**
A medida que el sistema creció en volumen de datos y complejidad, el almacenamiento basado puramente
en archivos planos (CSV) dejó de ser viable, presentando riesgos de integridad, redundancia y
lentitud en las consultas. En este sprint, el proyecto dio un salto arquitectónico necesario:
migramos la información a una base de datos estructurada utilizando un ORM (SQLAlchemy) para
modelar lógicamente las entidades subyacentes (Vehículos, Radares, Multas y Evidencias).
Simultáneamente, se integró Data Version Control (DVC) para gestionar el almacenamiento de
imágenes pesadas sin saturar el sistema de control de versiones Git.

**Conclusión del Trabajo Desarrollado:**

La transición hacia un ecosistema dual de bases de datos ha sido un éxito rotundo.
por un lado, la base relacional gestionada por el ORM nos permitió garantizar la integridad
referencial y limpiar inconsistencias históricas, estructurando el esquema para reportes rápidos
y precisos. Por otro lado, la integración de redes neuronales (OpenClip) junto con la base de datos vectorial ChromaDB transformó nuestra capacidad analítica: el sistema extrae las características matemáticas (*embeddings*) de las fotografías, habilitando un motor de búsqueda que vincula instantáneamente la evidencia visual cruda con el historial del infractor. La arquitectura resultante es sólida, modular y escalable.
