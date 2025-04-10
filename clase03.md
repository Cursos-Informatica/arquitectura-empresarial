# CAPITULO 03: ARQUITECTURA DE NEGOCIOS 

## Fase B: Arquitectura de Negocio

__Objetivos__
- Desarrollar la Arquitectura de Negocio de Destino describiendo cómo la empresa tiene que operar para alcanzar los objetivos de negocio, responder a las motivaciones estratégicas definidas en la Visión de la Arquitectura y responder a la Petición de Trabajo de Arquitectura y las preocupaciones de los interesados.
- Identificar componentes candidatos para el Plan de itinerario de Arquirctura basándose en las brechas identificadas entre la Arquitectura de Negocio de la Linea Base y la Arquitectura de Negocio de Destino.

__Pasos__
- Seleccionar modelos de referencia, Puntos de vista y herramientas
- Desarrollar la descripción de la arquitectura de Negocio de la Linea Base.
- Desarrollar la descripción de la Arquitectura de Negocio Destino
- Realizar un Análisis de Brechas.
- Definir los componentes candidatos del PLan de itinerario.
- Resolver los impactos al Panorama de Arquitectura
- Conducir una revisión formal con los interesados
- Finalizar la Arquitectua de Negocios
- Crear el Documento de Definición de arquitectura.

## LABORATORIO 03 : FASE B Arquitectura de Negocios

### 09 Vista Organizacional
El punto de vista de la organización se centra en la organización de una empresa, un departamento, una red de
empresas o cualquier otra entidad organizativa. Desde este punto de vista, los modelos se pueden presentar como
diagramas de bloques anidados, pero también de forma más tradicional, como organigramas. El punto de vista de la organización
es muy útil para identificar competencias, autoridad y responsabilidades en una organización.

![imagen09](/img_vistas/B_Arquitectura_Negocio/09%20Vista%20Organizacional.png)

### 10 Descomposición Organizacional - Anidado
![imagen10](/img_vistas/B_Arquitectura_Negocio/10%20Descomposición%20Organizacional%20-%20Anidado.png)

### 11 Flujo de Valor
El punto de vista del flujo de valor permite al arquitecto empresarial crear una descripción general estructurada de un flujo de
valor, las capacidades que respaldan las etapas de ese flujo de valor, el valor creado y las partes interesadas involucradas.

![imagen11](/img_vistas/B_Arquitectura_Negocio/11%20Flujo%20de%20Valor.png)

### 12 Vista de modelo de Capacidad
El Mapa de Capacidades permite al Arquitecto de Negocio crear una visión general estructurada de las capacidades de la empresa. Un
mapa de capacidades suele mostrar dos o tres niveles de capacidades en toda la empresa. Por ejemplo, se puede sombrear para crear un mapa
de calor que identifique las áreas que requieren inversión.

![imagen12](/img_vistas/B_Arquitectura_Negocio/12%20Vista%20de%20modelo%20de%20capacidad.png)

### 13 Mapeo de Flujo de Valor cruzado con capacidades
![imagen13](/img_vistas/B_Arquitectura_Negocio/13%20Mapeo%20de%20Flujo%20de%20valor%20cruzado%20con%20capacidades.png)

### 14 Vista de Funciones de Negocio - Linea Base
El punto de vista de la función empresarial muestra las principales funciones empresariales de una organización
y sus relaciones en términos de flujos de información, valor o bienes entre ellas.

![imagen14](/img_vistas/B_Arquitectura_Negocio/14%20Vista%20de%20Funciones%20del%20Negocio%20-%20Linea%20Base.png)

### 15 Capacidad - Realización
Tenga en cuenta que las funciones de negocio se diferencian de las capacidades. Las capacidades representan las
habilidades actuales o deseadas de una organización, materializadas por su personal, procesos, información y tecnología. Se
centran en resultados de negocio específicos y se utilizan para fines de planificación estratégica, como se describe
en la Fase A: Visión de la Arquitectura (página 10). Por el contrario, las funciones de negocio describen lo que realmente
hace la organización; se gestionan explícitamente y están más estrechamente alineadas con la estructura organizativa.
Múltiples funciones de negocio pueden (junto con otros elementos) contribuir a la materialización de una capacidad

Un ejemplo es la nueva capacidad de Gestión Digital de Clientes que ArchiSurance pretende implementar como parte de su
estrategia de Interacción Digital con el Cliente (véase la Figura 13). Esta capacidad se materializará en parte mediante la
función de relaciones con el cliente, pero también mediante una función de inteligencia empresarial (aún por
desarrollar) y diversos recursos como analistas de datos, gestores de riesgos, aplicaciones de adquisición y análisis de
datos, y datos de comportamiento del cliente.

Por supuesto, al trazar un mapa de las capacidades actuales de la organización, sus funciones de negocio actuales suelen
ocupar un lugar destacado, ya que lo que una organización hace debe ser algo que pueda hacer. Al describir la
Arquitectura Empresarial Base, el valor de un mapa de capacidades reside principalmente en el análisis de los niveles
de capacidad actuales y deseados, por un lado, y en descubrir las capacidades que la organización ya posee, pero que no
reconoce ni gestiona como funciones de negocio, por otro.

![imagen15](/img_vistas/B_Arquitectura_Negocio/15%20Capacidad%20-%20Realizacion.png)

### 16 Proceso de Negocios

Un proceso de negocio de ArchiMate agrupa el comportamiento según un orden de actividades. Produce un conjunto definido
de productos o servicios. Una arquitectura de procesos muestra los procesos de negocio más importantes y sus
relaciones, y posiblemente los pasos principales dentro de cada uno de ellos. Normalmente no muestra todos los detalles de un
flujo de proceso, que es el propósito de los lenguajes de diseño de procesos de negocio. Podemos definir un punto de
vista de Proceso de Negocio y especificar su contenido utilizando el mecanismo de puntos de vista definido en el
lenguaje ArchiMate:
El punto de vista del proceso de negocio se utiliza para mostrar la estructura y composición de alto nivel de uno o más
procesos de negocio.

![imagen16](/img_vistas/B_Arquitectura_Negocio/16%20Proceso%20de%20Negocios.png)

### 17 Mapeo Flujo de Valor y Proceso de Negocio
![imagen17](/img_vistas/B_Arquitectura_Negocio/17%20Mapeo%20Flujo%20de%20Valor%20y%20Proceso%20de%20Negocio.png)

### 18 Vista de Realización de Requerimiento

El punto de vista de realización de requisitos permite al diseñador modelar la realización de requisitos por parte de los elementos
centrales, como actores comerciales, servicios comerciales, procesos comerciales, servicios de aplicación, componentes de
aplicación, etc. Normalmente, estos requisitos resultan del punto de vista de realización de objetivos.

![imagen18](/img_vistas/B_Arquitectura_Negocio/18%20Vista%20de%20Realización%20de%20Requerimientos.png)

### 19 Analisis de Brechas de Capacidades

La estrategia de Intimidad Digital con el Cliente de ArchiSurance también requiere cambios en la Arquitectura Empresarial.

![imagen19](/img_vistas/B_Arquitectura_Negocio/19%20Analisis%20de%20Brechas%20de%20Capacidades.png)

### 20 Vista de Mapa de Recursos

Estas capacidades requieren personal con los conocimientos y las habilidades adecuadas para la era digital, dispositivos inteligentes
para la adquisición de datos y los propios datos del cliente.
El Mapa de Recursos permite al Arquitecto de Negocio crear una visión general estructurada de los recursos de la empresa. Un mapa
de recursos también puede mostrar las relaciones entre los recursos y las capacidades que respaldan.

![imagen20](/img_vistas/B_Arquitectura_Negocio/20%20Vista%20de%20Mapa%20de%20Recursos.png)

### 21 Vista de Realización de Recursos 

Estos recursos son implementados por el resto de las arquitecturas de negocio, sistemas de información y tecnología,
que constituyen el objeto de las fases B, C y D del TOGAF ADM. La Figura 21 muestra una pequeña parte de lo que esto
puede resultar. Cabe destacar que esta no representa todos los elementos necesarios para implementar estos recursos,
sino solo una muestra representativa, que muestra nuevamente la implementación de la estrategia de racionalización a la
izquierda y la estrategia de intimidad digital con el cliente a la derecha. En la práctica, se suelen crear vistas separadas
para mostrar cómo se implementan las capacidades y los recursos individuales.

![imagen21](/img_vistas/B_Arquitectura_Negocio/21%20Vista%20de%20Realizacion%20de%20Recursos.png)
