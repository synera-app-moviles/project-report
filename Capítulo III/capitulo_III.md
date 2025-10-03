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

#### 3.1.2.3. SEO Tags and Meta Tags

#### 3.1.2.4. Searching Systems

#### 3.1.2.5. Navigation Systems

### 3.1.3. Landing Page UI Design

#### 3.1.3.1. Landing Page Wireframe

#### 3.1.3.2. Landing Page Mock-up

### 3.1.4. Mobile Applications UX/UI Design

#### 3.1.4.1. Mobile Applications Wireframes

#### 3.1.4.2. Mobile Applications Wireflow Diagrams

#### 3.1.4.3. Mobile Applications Mock-ups

#### 3.1.4.4. Mobile Applications User Flow Diagrams

#### 3.1.4.5. Mobile Applications Prototyping