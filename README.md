# Proyecto de Calidad y Trazabilidad de Datos

## 1. Fuente de los Datos
Los datos utilizados en este proyecto provienen de la plataforma **iNaturalist**. 
* **Especie:** Pez León (Pterois volitans).
* **Archivo original:** `observations-677791.csv`.

## 2. Fecha de descarga
* Los datos fueron descargados el día: **[Escribe aquí la fecha de hoy o cuando bajaste el archivo]**.

## 3. Transformaciones Realizadas
Para asegurar la calidad de la serie temporal/imágenes, se realizaron las siguientes acciones en RStudio:
* **Conversión de vacíos:** Se identificaron celdas sin información y se transformaron al formato estándar `NA`.
* **Validación de Carga:** Se implementó un código de seguridad para verificar la existencia del archivo antes de abrirlo.
* **Manejo de Errores:** Se utilizó una estructura `tryCatch` para evitar que el programa falle si el archivo está dañado.
* **Limpieza de Nombres:** Se normalizaron los encabezados de las columnas para asegurar la consistencia.

## 4. Versiones del Archivo
* **Versión Original (v1):** `observations-677791.csv` (Datos crudos).
* **Versión Procesada (v2):** `observations_limpias.csv` (Datos con NAs estandarizados y listos para análisis).

## 5. Flujo del Proyecto
1. Revisión de calidad (Detección de faltantes y duplicados).
2. Programación de script robusto (Validación y Excepciones).
3. Exportación de base de datos depurada.