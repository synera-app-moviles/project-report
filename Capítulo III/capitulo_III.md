# Capítulo III: Requirements specification 
## 3.1. Product design

### 3.1.1. Style Guidelines

#### 3.1.1.1. General Style Guidelines

### 3.1.2. Information Architecture

#### 3.1.2.1. Organization Systems

<p style="text-indent: 1.25cm;">Para la aplicación móvil Centralis, se han implementado sistemas de organización que optimizan la experiencia del usuario según el tipo de contenido y las tareas a realizar. La organización se ha diseñado considerando los diferentes segmentos de usuarios (gerentes y empleados) y sus objetivos específicos dentro de la plataforma.

**Organización Jerárquica (Visual Hierarchy)**

<p style="text-indent: 1.25cm;">Se aplica organización jerárquica en las pantallas donde es necesario establecer claramente la relación de importancia entre los elementos de contenido y guiar la atención del usuario hacia la información más relevante.

**Casos de aplicación:**

- **Pantallas de listado (Anuncios, Eventos, Chats):** Los elementos más importantes como títulos de anuncios, nombres de eventos o grupos de chat se presentan con mayor prominencia mediante tamaño de fuente más grande y peso tipográfico en negrita. La información secundaria (descripciones, fechas, metadatos) mantiene una jerarquía visual menor pero permanece legible y accesible.
- **Pantallas de detalle:** El título del contenido ocupa la posición visual más destacada, seguido por la descripción principal y finalmente los atributos complementarios. Los botones de acción primaria utilizan contraste de color y tamaño para destacar su importancia funcional.
- **Perfiles de usuario:** La información personal y profesional se organiza con el nombre del usuario como elemento principal, seguido por los detalles secundarios como cargo, departamento y datos de contacto.

**Organización Secuencial (Step-by-step)**

Se emplea organización secuencial en los flujos que requieren que el usuario complete una serie de pasos definidos para alcanzar un objetivo específico.

**Casos de aplicación:**

- **Formularios de creación y edición:** Todos los procesos de creación (anuncios, eventos, grupos de chat) y edición de perfil siguen una secuencia lógica donde los campos se presentan en orden vertical, guiando al usuario a través del flujo de manera intuitiva.
- **Procesos de autenticación:** Las pantallas de registro e inicio de sesión representan el ejemplo más puro de organización secuencial, donde cada campo constituye un paso necesario en el proceso de acceso a la plataforma.

**Organización Matricial**

<p style="text-indent: 1.25cm;">Si bien no ha sido el enfoque principal en el diseño actual, la organización matricial se considera para futuras implementaciones que requieran visualización de datos complejos o comparativos, como dashboards de métricas avanzadas para gerentes.

**Esquemas de Categorización de Contenido**

1. **Categorización por Tópicos**

Es el esquema principal utilizado para organizar el contenido central de la aplicación:

- **Anuncios:** Agrupados por tipo (general, prioritario, departamental)
- **Eventos:** Organizados por categoría (reuniones, capacitaciones, eventos sociales)
- **Chats:** Segmentados por propósito (departamentales, proyectos específicos, grupos temporales)

2. **Categorización Cronológica**

Se aplica en contextos donde la temporalidad es un factor crítico:

- **Linea de tiempo de anuncios:** Los anuncios se ordenan por fecha de publicación, mostrando los más recientes primero
- **Calendario de eventos:** Los eventos se organizan por fecha y hora de realización
- **Historial de chats:** Los mensajes se muestran en orden cronológico inverso (más recientes al final)

3. **Categorización según Audiencia**

Este esquema responde directamente a la segmentación de usuarios identificada:

- **Contenido para gerentes:** Incluye funcionalidades de creación, edición, paneles de control y métricas de engagement
- **Contenido para empleados:** Se centra en consumo de información, confirmaciones y comunicación colaborativa
- **Contenido segmentado por departamentos:** Anuncios y eventos específicos para áreas organizacionales particulares

4. **Categorización Alfabétic**a

Se utiliza de forma complementaria en situaciones que requieren búsqueda y localización rápida:

- **Lista de empleados** en selección de destinatarios
- **Directorio de grupos de chat** para facilitar la navegación
- **Búsqueda de eventos y anuncios** históricos

<p style="text-indent: 1.25cm;">Esta combinación de sistemas de organización asegura que los usuarios puedan encontrar y interactuar con el contenido de manera eficiente, mientras se mantiene la coherencia con los objetivos de negocio y las necesidades específicas de cada segmento de usuario.

#### 3.1.2.2. Labelling Systems

<p style="text-indent: 1.25cm;">El sistema de etiquetado de Centralis se fundamenta en principios de simplicidad y claridad, diseñado para facilitar la comprensión inmediata y evitar ambigüedades en la interacción del usuario. Las etiquetas se conciben como elementos mínimos pero altamente informativos que guían al usuario a través de la aplicación de manera intuitiva.

**Principios Fundamentales**

- **Simplicidad:** Cada etiqueta utiliza el menor número de palabras posible sin sacrificar el significado. Se prioriza la brevedad y la precisión léxica.

- **Claridad:** Las etiquetas son directas y autoexplicativas, eliminando cualquier posibilidad de interpretación múltiple o confusión semántica.

- **Consistencia:** Se mantiene uniformidad terminológica a lo largo de toda la aplicación, asegurando que un mismo concepto o acción se represente siempre con la misma etiqueta.

- **Orientación a la Tarea:** Las etiquetas de acciones describen explícitamente el resultado de la interacción, permitiendo al usuario predecir las consecuencias de sus acciones.

**Categorías de Etiquetas y su Aplicación**

1. **Navegación Principal**

<p style="text-indent: 1.25cm;">Las etiquetas de navegación representan los conjuntos de información principal accesibles desde la barra de navegación inferior:

- **Announcements:** Agrupa todas las funcionalidades relacionadas con comunicados formales y noticias corporativas
- **Events:** Representa el conjunto de actividades programadas, reuniones y eventos de la organización
- **Chats:** Engloba las conversaciones grupales organizadas por departamentos y proyectos
- **Profile:** Contiene la información personal, preferencias y configuración del usuario

<p style="text-indent: 1.25cm;">Cada etiqueta se complementa con iconografía representativa que refuerza la asociación visual-concepto, creando un sistema de navegación redundante que asegura la comprensión.

**2. Títulos de Sección y Pantalla**

<p style="text-indent: 1.25cm;">Estas etiquetas definen el contexto y propósito específico de cada pantalla:

- **New Announcement:** Indica el proceso de creación de un nuevo comunicado formal
- **Event Details:** Señala la visualización de información detallada de un evento específico
- **Edit Profile:** Define la modificación de información personal del usuario
- **Group Chat:** Identifica conversaciones organizadas por temas o equipos

**3. Campos de Formulario**

<p style="text-indent: 1.25cm;">Las etiquetas de formulario guían la entrada de datos mediante descriptores concisos:

- **Title/Description:** Para contenido textual breve y extendido respectivamente
- **Date/Location:** Para información temporal y espacial
- **First Name/Last Name:** Para datos personales estructurados
- **Department/Position:** Para información organizacional

<p style="text-indent: 1.25cm;">Estas etiquetas se complementan con texto de placeholder que proporciona ejemplos contextuales ("Type a message...", "Enter event title..."), creando un sistema de ayuda integrado.

**4. Botones de Acción**

<p style="text-indent: 1.25cm;">Las etiquetas de acción utilizan verbos activos que describen resultados específicos:

- **Publish/Save:** Para confirmación y persistencia de datos
- **Edit/Delete:** Para modificación y eliminación de contenido
- **Confirm Read:** Para acknowledgment de recepción de información
- **Send/View:** Para envío de mensajes y visualización de detalles

**5. Indicadores de Estado**

<p style="text-indent: 1.25cm;">Etiquetas que comunican atributos y condiciones del sistema:

- **Priority:** Indica urgencia o importancia de contenido
- **Seen by:** Muestra el estado de lectura o recepción
- **Attendees:** Representa participantes confirmados en eventos

<p style="text-indent: 1.25cm;">Este sistema de etiquetado minimiza la carga cognitiva del usuario mientras maximiza la eficiencia en la navegación y comprensión de la aplicación, creando una experiencia cohesiva y predecible a través de todos los módulos de Centralis.

#### 3.1.2.3. SEO Tags and Meta Tags

#### 3.1.2.4. Searching Systems

<p style="text-indent: 1.25cm;">El sistema de búsqueda de Centralis está diseñado específicamente para contextos donde los usuarios necesitan localizar y seleccionar empleados de manera eficiente.

El sistema de búsqueda se implementa en dos escenarios fundamentales:

- **Selección de asistentes** durante la creación de eventos
- **Incorporación de miembros** en la formación de grupos de chat

<p style="text-indent: 1.25cm;">Estos contextos fueron identificados como los de mayor frecuencia e impacto en la productividad de los gerentes, quienes requieren un mecanismo ágil para localizar colaboradores específicos dentro de la organización.

**Barra de Búsqueda Integrada**

- **Ubicación:** Incorporada directamente en las secciones de selección de empleados dentro de los formularios de creación
- **Placeholder descriptivo:** "Search for employees..." para indicar claramente el propósito
- **Funcionamiento en tiempo real:** Los resultados se actualizan dinámicamente mientras el usuario escribe.

**Lista Dinámica de Empleados**

- **Presentación clara:** Lista scrollable debajo de la barra de búsqueda mostrando empleados que coinciden con el término buscado
- **Resaltado de coincidencias:** El texto que coincide con la búsqueda se destaca visualmente para facilitar el escaneo

**Gestión de Selecciones**

- **Sección de confirmación:** Área dedicada que muestra los "Empleados Seleccionados" como recordatorio visual de las elecciones realizadas
- **Mecanismo de selección:** Checkboxes o toque directo para añadir/remover empleados de la selección
- **Retroalimentación inmediata:** Los cambios en la selección se reflejan instantáneamente en la interfaz



**Figura 49**


<p align="center">
  <img src="https://i.imgur.com/j243TuJ.png" alt="Descripción">
</p>
*Nota.* Elaboración propia.



**Figura 50**

<p align="center">
  <img src="https://i.imgur.com/4rbxUe5.png" alt="Descripción">
</p>
*Nota.* Elaboración propia.

<p style="text-indent: 1.25cm;">La Landing Page de Centralis está diseñada como una página de presentación estática cuyo propósito principal es proporcionar información esencial sobre la aplicación y dirigir a los usuarios hacia las plataformas de descarga. Dada su naturaleza informativa y la limitada cantidad de contenido, no se implementa un sistema de búsqueda por las siguientes razones:

- **Volumen de contenido reducido:** La Landing Page contiene únicamente secciones clave (valor proposition, características, testimonios, llamados a la acción) que pueden recorrerse completamente mediante scroll tradicional.
- **Propósito orientado a la conversión:** El objetivo principal es guiar al usuario hacia la descarga de la aplicación, no proporcionar acceso a bases de datos extensas o contenido complejo que requiera mecanismos de búsqueda.
- **Experiencia lineal planificada:** El contenido está estructurado para ser consumido de manera secuencial, presentando la información en un orden lógico que maximiza la comprensión y el engagement.

<p style="text-indent: 1.25cm;">Este sistema de búsqueda está optimizado para los casos de uso más frecuentes en Centralis, permitiendo a los gerentes completar sus tareas de selección de personal de manera rápida y sin distracciones, mientras mantiene una interfaz limpia y comprensible. 

#### 3.1.2.5. Navigation Systems

<p style="text-indent: 1.25cm;">El sistema de navegación de Centralis está diseñado bajo principios de usabilidad y eficiencia, proporcionando múltiples capas de interacción que guían a los usuarios a través de la aplicación de manera intuitiva y satisfactoria. La navegación se adapta a los diferentes contextos de uso y perfiles de usuario, optimizando el cumplimiento de metas tanto para empleados como para gerentes.


**1. Navegación Principal**

**Descripción:** Constituye el eje central de navegación para las secciones fundamentales de la aplicación. Una barra de navegación persistente ubicada en la parte inferior de la pantalla proporciona acceso constante a las áreas principales.

- **Cuatro secciones clave:** Announcements (Anuncios), Events (Eventos), Chats (Chats), Profile (Perfil)
- **Diseño icónico-textual:** Cada sección combina un icono representativo con una etiqueta textual concisa
- **Persistencia contextual:** Visible en la mayoría de las vistas principales, manteniendo la orientación del usuario
- **Navegación instantánea:** Un solo toque transporta al usuario a la pantalla principal de cada sección

**Ventajas:** Proporciona acceso rápido y constante a las áreas centrales, facilita el cambio de contexto y mantiene la orientación espacial dentro de la aplicación.



**2. Navegación Jerárquica**

**Descripción:** Permite a los usuarios explorar contenido desde vistas generales hacia detalles específicos, con mecanismos claros de retorno.

- **Drill-down por selección:** Toque en elementos de lista (anuncios, eventos, chats) para acceder a pantallas de detalle
- **Botón de retroceso dedicado:** Icono de flecha en la AppBar superior izquierda para regresar a la vista anterior
- **Compatibilidad con navegación nativa:** Uso del botón de retroceso del sistema operativo Android
- **Preservación de estado:** Mantiene el contexto y posición al retornar a listas anteriores



**3. Navegación Contextual**

**Descripción:** Proporciona acceso directo a acciones primarias relacionadas con el contexto actual de la pantalla.

- **Botones de AppBar:** Acciones específicas como notificaciones, filtros o búsqueda según el contexto
- **Floating Action Buttons (FAB):** Botones flotantes para acciones principales de creación (nuevos anuncios, eventos, grupos)



**4. Navegación Secuencial**

**Descripción:** Orienta al usuario a través de secuencias estructuradas para completar tareas complejas.

- **Procesos de autenticación:** Registro e inicio de sesión con pasos definidos
- **Creación de contenido:** Formularios para anuncios, eventos y grupos con progresión lógica
- **Edición de perfiles:** Flujos organizados para modificación de información personal



**Sistema de Navegación para Landing Page**

- **Navegación vertical continua:** Contenido organizado en secciones secuenciales accesibles mediante scroll
- **Menú hamburguesa:** Acceso secundario para navegación directa a secciones específicas
- **Llamados a acción estratégicos:** Botones prominentes que dirigen hacia descargas y registro
- **Jerarquía visual clara:** Uso de tamaño, color y espaciado para guiar la atención



<p style="text-indent: 1.25cm;">La Landing Page emplea un sistema de navegación simplificado que responde a su naturaleza informativa y de conversión. El scroll unidireccional optimiza la presentación del valor proposition, mientras el menú hamburguesa proporciona acceso rápido para usuarios con objetivos específicos.



### 3.1.3. Landing Page UI Design

#### 3.1.3.1. Landing Page Wireframe

#### 3.1.3.2. Landing Page Mock-up

### 3.1.4. Mobile Applications UX/UI Design

#### 3.1.4.1. Mobile Applications Wireframes

#### 3.1.4.2. Mobile Applications Wireflow Diagrams

#### 3.1.4.3. Mobile Applications Mock-ups

#### 3.1.4.4. Mobile Applications User Flow Diagrams

#### 3.1.4.5. Mobile Applications Prototyping

<p style="text-indent: 1.25cm;">El presente apartado expone los prototipos de interfaz de usuario (UI) desarrollados para la aplicación móvil Centralis, los cuales simulan la interacción y navegación entre las principales vistas del sistema. Estos prototipos fueron elaborados en Figma, siguiendo los paths definidos en los User Flow Diagrams, con el objetivo de validar tempranamente la experiencia de usuario y las decisiones de arquitectura de información adoptadas.

En cuanto a los flujos de interacción, el prototipo contempla las siguientes secuencias:

- **Autenticación:** registro de nuevos usuarios, inicio de sesión y completado de perfil.

- **Gestión de anuncios:** creación, edición y visualización de comunicados corporativos con distintos niveles de prioridad.

- **Gestión de eventos:** programación, edición y confirmación de asistencia a reuniones o capacitaciones internas.

- **Mensajería interna:** creación de grupos de chat, envío de mensajes y administración de miembros.

- **Perfil del usuario:** edición de datos personales y cierre de sesión.



**Figura 51**

<p align="center">
  <img src="https://i.imgur.com/84sVlcs.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

Link del video : https://acortar.link/Rkmy5z



