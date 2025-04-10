# CAPITULO 05: ARQUITECTURA TECNOLOGICA

__Objetivos__

- Desarrollar la Arquitectura Tecnológica de Destino de tal manera que permita que los componentes lógicos y fisicos de datos y aplicaciones, asi como aquellos de la Visión de la Arquitectura, correspondan a la Petición de Trabajo de Arquitectura y respondan a las preocupaciones de los interesados.
- Identificar los componentes candidatos del Plan de Itinerario de Arquitectura basándose en las brechas identificadas entre la Arquitectura Tecnológica de la Línea de Base y la Arquitectura Tecnológica de Destino. 

__Pasos__

- Seleccionar modelos de referencia, puntos de vista y herramientas.
- Desarrollar la descripción de la arquitectura tecnológica de la linea de base.
- Desarrollar la descripción de la arquitectura tecnológica de Destino.
- Realizar el Análisis de Brechas
- Definir los componentes candidatos del Plan de Itinerario
- Resolver los impactos en el panorama de Arquitectura

## LABORATORIO 05 : FASE D Arquitectura Tecnológica

En la oficina principal de ArchiSurance, ubicada en la sede de Home & Away, hay un servidor de propósito general y uno dedicado al
alojamiento web. El SSC, ubicado en la sede de PROFIT, cuenta con su propio servidor para el sistema de gestión documental.
Cada una de las tres oficinas administrativas cuenta con un servidor para sus aplicaciones.

Una red de área local (LAN) conecta servidores y computadoras personales en cada una de las tres ubicaciones de ArchiSurance,
que a su vez están conectadas por una red de área amplia (WAN) corporativa.

Para representar el punto de vista tecnológico de ArchiSurance, se puede utilizar el punto de vista tecnológico de ArchiMate

### 29 Vista de la tecnología - linea base

El punto de vista tecnológico contiene los elementos de infraestructura de software y hardware que respaldan la capa de
aplicación, como dispositivos físicos, redes o software de sistema, como sistemas operativos, bases de datos y middleware.

![imagen29](/img_vistas/D_Arquitectura%20de%20Tecnologia/29%20Vista%20de%20Infraestructura%20-%20LineaBase.png)

### 30 Vista de Infraestructura - Objetivo

![imagen30](/img_vistas/D_Arquitectura%20de%20Tecnologia/30%20Vista%20de%20Infraestructura%20-%20Objetivo.png)

### 31 Adquisición de Datos de Servicios IoT

En un conjunto de vistas independiente, ArchiSurance ha visualizado la adquisición de datos basada en IoT en la Figura 31,
como se describe en su nueva estrategia de Intimidad Digital con el Cliente. Para ello, ArchiSurance establece una pasarela de
adquisición de datos que puede conectarse a todo tipo de dispositivos inteligentes que generan datos relevantes. Estos dispositivos se
modelan como equipos. A su vez, los equipos pueden ubicarse en una instalación; en la Figura 31, vemos un sistema de alarma para el
hogar y un termostato inteligente dentro de una casa inteligente. Finalmente, el termostato inteligente está conectado a la red
energética, modelada como una red de distribución en el lenguaje ArchiMate.

![imagen31](/img_vistas/D_Arquitectura%20de%20Tecnologia/31%20Adquisicion%20Datos%20Servicios%20IoT.png)

### 32 Servicios de Dispositivos IoT

La implementación de la adquisición de datos de ArchiSurance se basa en una arquitectura de microservicios. Los dispositivos
IoT pueden registrarse en la puerta de enlace mediante una API REST3. También utiliza servicios de la API para notificar a
la puerta de enlace sobre los datos que adquiere. Por cada dispositivo registrado, se ejecutará una instancia de la funcionalidad
de adquisición de datos en un contenedor. La puerta de enlace se basa en una plataforma como servicio (PaaS), que proporciona
servicios de implementación, integración, gestión del ciclo de vida del servicio, contabilidad, seguridad, balanceo de carga,
almacenamiento, virtualización y más. Esto se muestra en la Figura 32.

![imagen32](/img_vistas/D_Arquitectura%20de%20Tecnologia/32%20Servicios%20de%20Dispositivos%20IoT.png)

### 33 Analisis GAP - Arquitectura Tecnologica
La Figura 33 visualiza los resultados de un análisis global de deficiencias para la Arquitectura Tecnológica. Se
prevé la eliminación de los servidores administrativos de propósito general. El clúster original de servidores de Home
& Away se convertirá en el clúster central de servicios administrativos de ArchiSurance, y se instalará un clúster
adicional de servidores de respaldo en el SSC de la sede de PROFIT.
También se instalará un servidor de respaldo para la gestión documental en el backoffice de Home & Away. La nueva suite de backoffice y el sistema de gestión documental se replicarán en sus respectivos servidores principales y de respaldo.

![imagen33](/img_vistas/D_Arquitectura%20de%20Tecnologia/33%20Analisis%20GAP%20Arquitectura%20Tecnologica.png)




