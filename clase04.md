# CAPITULO 04: ARQUITECTURA DE SISTEMA DE INFORMACIÓN  

## Fase C: Arquitectura de Sistemas de Información

__Objetivos__
- Desarrollar un arquitectura de aplicacion de destino que sea funcional a la arquitectura de negocios y a la visión de la arquitectura, y que responda a la vez a la petición de trabajo de arquitectura y a las preocupaciones de los interesados.
- Identificar componentes candidatos del plan de itinerario de arquitectura basándose en las brechas identificadas entre la arquitectura de aplicaciones de la linea de base y la arquitectura de aplicaciones de destino.

__Pasos__
- Seleccionar modelos de referencia, puntos de vista y herramientas.
- Desarrollar la descripción de la arquitectura de aplicaciones de la linea base
- Desarrollar la descripción de la arquitectura de aplicación de Destino
- Realizar analisis de brechas
- Definir los componentes candidatos que conforman el plan itinerario
- Resovler los impoactos al panorama de arquitectura
- Conducir una revisión formal con los interesados
- Finalizar la arquitectura de aplicación
- Crear el documento de definición de arquitectura


## LABORATORIO 04 : FASE C Arquitectura de SI - Aplicaciones

Desde la fusión, las tres divisiones han adoptado un portal web común, un paquete de software para centros de contacto y un
sistema de gestión documental. Además, la empresa ha seleccionado una solución CRM estratégica y la ha implementado
tanto para Home & Away como para PROFIT.
Sin embargo, debido al enfoque de la gerencia en minimizar los riesgos
posteriores a la fusión y a la mejora continua del rendimiento diario de cada división, la racionalización de las aplicaciones
empresariales principales no ha comenzado. Ahora que ArchiSurance ha cumplido las expectativas de rendimiento
posteriores a la fusión, los inversores esperan un ahorro sustancial en costos de TI mediante la adopción de un conjunto
común de aplicaciones centradas en el producto y el cliente. Por lo tanto, persisten varios desafíos. Home & Away aún
utiliza sus paquetes de administración de pólizas y aplicaciones financieras previos a la fusión, mientras que PROFIT
y Legally Yours aún utilizan sus propias aplicaciones monolíticas personalizadas.

### 22 Cooperacion Aplicaciones - Linea Base

El lenguaje ArchiMate define un punto de vista de cooperación de aplicaciones para mostrar una descripción general
del panorama de aplicaciones y las dependencias entre las aplicaciones:

El punto de vista de Cooperación de Aplicaciones describe las relaciones entre los componentes de la aplicación en términos
de los flujos de información entre ellos o de los servicios que ofrecen y utilizan. Este punto de vista se utiliza generalmente
para crear una visión general del panorama de aplicaciones de una organización. También se utiliza para expresar la
cooperación (interna) o la orquestación de servicios que, en conjunto, respaldan la ejecución de un proceso de negocio.

![imagen22](/img_vistas/C_Arquitectura_Sistemas/22%20Cooperacion%20Aplicaciones.png)

![imagen22a](/img_vistas/C_Arquitectura_Sistemas/22%20Visualizer.png)

### 23 Cooperacion Aplicaciones - Objetivo
![imagen23](/img_vistas/C_Arquitectura_Sistemas/23%20Cooperacion%20Aplicaciones%20-%20Objetivo.png)

### 24 Uso de Aplicacion - Linea Base

El punto de vista de Uso de Aplicaciones describe cómo se utilizan las aplicaciones para dar soporte a uno o más procesos de negocio y
cómo las utilizan otras aplicaciones. Este punto de vista puede ser útil al diseñar una aplicación, ya que permite identificar los servicios que
dicha aplicación debe proporcionar a los procesos de negocio que eventualmente soportará, o a otras aplicaciones. De igual manera, este
punto de vista también puede ser útil al analizar procesos de negocio y optimizarlos mediante un uso eficiente de dichos servicios de
aplicación. Además, dado que este punto de vista describe las dependencias de los procesos de negocio con respecto a las aplicaciones, puede
resultar una herramienta muy útil para los gerentes de operaciones responsables de la ejecución de dichos procesos. El concepto de
Servicio de Aplicación desempeña un papel fundamental en este punto de vista. La Figura 24 muestra un subconjunto de los servicios
ofrecidos por las aplicaciones utilizadas por la división Home & Away de ArchiSurance, y qué subprocesos del proceso de gestión de
siniestros utilizan cada uno de estos servicios.

![imagen24](/img_vistas/C_Arquitectura_Sistemas/24%20Uso%20de%20la%20Aplicacion%20-%20Linea%20Base.png)

### 25 Comportamiento de Aplicación - Objetivo

El comportamiento de la solución de almacenamiento de datos, en el contexto de la adquisición de datos, por un lado,
y de los procesos y funciones de negocio, por otro, se muestra en la Figura 25. La prima de seguro de cada cliente se
basa, en parte, en los datos que adquieren de diferentes dispositivos. Estos datos se procesan para crear perfiles
específicos de cada cliente que se utilizan para el cálculo de sus primas de seguro. A nivel agregado, estos datos
también se utilizan para desarrollar nuevos tipos de productos de seguros y para evaluar y ajustar la exposición general
al riesgo de la empresa.

![imagen25](/img_vistas/C_Arquitectura_Sistemas/25%20Comportamiento%20de%20Aplicacion%20-%20Objetivo.png)

### 26 Analisis GAP - Arquitectura Aplicacion

Los resultados de un análisis de brechas global para la arquitectura de aplicaciones se visualizan en la Figura 26.
Varios componentes de aplicaciones que existían en la arquitectura de línea base ya no están presentes en la
arquitectura de destino: las aplicaciones de backoffice separadas y el sistema CRM de seguros de gastos legales separado.

La funcionalidad de CRM para los clientes de seguros de gastos legales es asumida por el sistema CRM general; por lo
tanto, no requiere nuevos componentes (aunque podría ser necesario adaptar o reconfigurar el sistema CRM general
existente, lo cual no se refleja en el análisis de deficiencias). Además, se introduce una suite de aplicaciones de backoffice
completamente nueva y una nueva solución de almacenamiento de datos.

![imagen26](/img_vistas/C_Arquitectura_Sistemas/26%20Analisis%20GAP%20-%20Arquitectura.png)


## LABORATORIO 04 : FASE C Arquitectura de SI - Datos

La arquitectura de datos de ArchiSurance describe las principales relaciones entre sus objetos de negocio conceptuales y
sus objetos de datos lógicos. El lenguaje ArchiMate define la perspectiva de la estructura de la información para este propósito:

### 27 Estructura de Datos
El punto de vista de la Estructura de la Información es comparable a los modelos de información tradicionales creados
durante el desarrollo de casi cualquier sistema de información. Muestra la estructura de la información utilizada en la
empresa o en un proceso o aplicación de negocio específico, en términos de tipos de datos o clases (orientadas a objetos).

![imagen27](/img_vistas/C_Arquitectura_Sistemas/27%20Estructura%20de%20Datos.png)

### 28 Diseminación de Datos
El propósito del diagrama de Diseminación de Datos es mostrar la relación entre la entidad de datos, el servicio de negocio y
los componentes de la aplicación. El diagrama muestra cómo los componentes de la aplicación deben implementar físicamente las
entidades lógicas. Esto permite un dimensionamiento eficaz y refinar la infraestructura de TI.
Además, al asignar valor comercial a los datos, se puede obtener una indicación de la criticidad comercial de los
componentes de la aplicación.

![imagen28](/img_vistas/C_Arquitectura_Sistemas/28%20Difusion%20de%20Datos.png)

