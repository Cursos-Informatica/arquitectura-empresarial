# CAPITULO 06: OPORTUNIDADES Y SOLUCIONES

Esta es la primera fase que directamente se refiere a la implementación. Describe el proceso de identificación de los medios de entrega (proyecto, programas o carteras) que proporcionan la Arquitectura de Destino identificada en las fases anteriores.

__Objetivos__
- Generar la version inicial y completa del Plan de Itinerario de Arquitecturam basándose en el Análisis de Brechas y en los componentes candidatos del Plan de Itinerario de Arquitectura resultates de las Fases B, C y D.
- Determinar si un enfoque incremental es requerido, y si fuera asim identificar las Arquitecturas de Transición que proporcionarán valor continuo de negocio.

__Pasos__

- Determinar o confirmar atributos claves para el cambio empresarial
- Determinar limitaciones del negocio para la implementación
- Examinar y consolidar resultados de los Análisis de Brechas realizdos en las Fases B a D
- Examinar los requerimientos consolidados entre funciones de negocio relacionadas
- Consolidar y reconciliar los requerimientos de interoperabilidad
- Refinar y validar dependencias
- Confirmar el Grado de Preparación y riesgos para la transformación del negocio
- Formular la estrategia de Implementación y Migración
- Identificar y agrupar los paquetes de trabajo principales
- Identificar las Arquitecturas de Transición
- Crear el Plan Itinerario de Arquitectura y el Plan de Implementación y Migración


## LABORATORIO 05 : FASE E Oportunidades y Soluciones

En el lenguaje ArchiMate, las arquitecturas de línea base, de destino y de transición, así como sus relaciones, se muestran utilizando
el punto de vista de migración:

### 34 Vista de Migración

El punto de vista de la migración implica modelos y conceptos que pueden utilizarse para especificar la transición de una arquitectura
existente a una arquitectura deseada.

La Figura 34 muestra un ejemplo del punto de vista de migración de ArchiMate para ilustrar cómo el grupo ArchiSurance planea
migrar de su arquitectura base a la arquitectura objetivo deseada. El departamento de TI de ArchiSurance no dispone de recursos
suficientes para estandarizar los sistemas de backoffice y, simultáneamente, integrar los sistemas CRM. Por lo tanto, se proponen
las siguientes posibles vías de migración: una propone reemplazar primero los dos sistemas CRM por un sistema central para
toda la empresa, manteniendo los sistemas de backoffice separados por división (Transición A), y luego unificar los sistemas de
backoffice en una única suite de backoffice (Transición C); otra propone implementar primero una única suite de backoffice
con dos CRM (Transición B), y luego reemplazar los dos sistemas CRM por un sistema central para toda la empresa (Transición C).
Posteriormente, se implementará la solución de almacenamiento de datos e IoT.

![imagen34](/img_vistas/E_Oportunidades%20y%20Soluciones/34%20Vista%20de%20Migración.png)