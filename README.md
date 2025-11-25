1. Visión General del Proyecto: Objetivos y Contexto
Este proyecto tiene como objetivo transformar datos crudos de incidentes criminales en una herramienta de inteligencia interactiva.
Se abordó el ciclo completo de análisis, desde la limpieza rigurosa en Python hasta la presentación de hallazgos en Power BI.

El foco principal fue la limpieza y estandarización de los campos de fecha y hora para asegurar la fiabilidad de todos los análisis temporales y geoespaciales.
Para determinar que todos los datos estuvieran es su formato correcto y que no hubieran datos nulos.

2. Resultados Clave (Dashboard)
El dashboard permite la exploración dinámica de los datos.

🚨 Cuatro Perspectivas de Análisis:
Localización de Crímenes: Análisis geoespacial de las 5 áreas principales.
Lo que demuestro en esta hoja es saber que areas fueron las que tuvieron mas crimenes y saber en que fechas hubo mas crimenes en estas áreas,
y asi demostrar donde se puede mejorar la actividad policiaca

Perfil Demográfico: Distribución de crímenes por Sexo y Etnia.
Este hoja demuestra asi a que tipo de personas y sexos se dirige mas los crimenes y poder asi tomar medidas sobre aquellas personas que sufre mas este tipo de crimenes

Uso de Armas: Composición de crímenes por Tipo de Arma utilizada.
Es esencial esta porque nos dice que armas son las mas utilizadas durante los diferentes crimenes 

Estado/Resolución: Tasa y estado final de detención de los incidentes.
Para determinar como se esta siguiendo los detenedios si ya estan en proceso, investigacion o que tipo de personas realizo el crimen ya sea aldulto o menor de edad

3. Metodología y Stack Tecnológico
El proceso de ETL (Extract, Transform, Load) fue el siguiente:

Fase I: Limpieza y Transformación (crimenes.ipynb)
Se utilizó el poder de Pandas para garantizar la calidad de los datos antes de la visualización.

Formato de Fechas y Tiempo: Conversión estricta a tipos datetime para permitir el slicing temporal en Power BI.

Preparación para ETL: Se preparó la tabla final para el modelo de datos dimensional en Power BI, optimizando la carga.

Fase II: Modelado y Visualización (Crimenes 2023_2025.pbix)
Modelado: Implementación de un modelo estrella simple con tablas de hechos y dimensiones.

DAX: Creación de medidas para los KPIs principales (e.g., Total de Crímenes, Total de armas).

Visualización: Diseño de las cuatro páginas de análisis detalladas a continuación.

