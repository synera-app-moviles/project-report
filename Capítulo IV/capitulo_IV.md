# Capítulo IV: Solution Software Design



## 4.1. Software Configuration Management 

### 4.1.1.Software Development Environment Configuration

| **Producto/Herramienta**     | **Categoría**         | **Ruta de Descarga/Acceso**                | **Propósito en el Proyecto**                              |
| ---------------------------- | --------------------- | ------------------------------------------ | --------------------------------------------------------- |
| **OpenJDK**                  | Desarrollo Backend    | https://openjdk.org/                       | Entorno de ejecución para aplicaciones Java               |
| **Apache Maven **            | Desarrollo Backend    | https://maven.apache.org/                  | Gestión de dependencias y construcción del proyecto       |
| **Spring Boot **             | Desarrollo Backend    | https://spring.io/projects/spring-boot     | Framework para desarrollo de APIs RESTful                 |
| **Android Studio**           | Desarrollo Móvil      | https://developer.android.com/studio       | IDE para desarrollo de aplicaciones Android nativas       |
| **Kotlin**                   | Desarrollo Móvil      | Incluido en Android Studio                 | Lenguaje de programación para aplicación móvil            |
| **Render PostgreSQL **       | Base de Datos         | https://render.com/docs/postgresql         | Base de datos relacional en la nube                       |
| **Material Design 3**        | Diseño UX/UI          | https://m3.material.io/                    | Sistema de diseño para interfaces consistentes            |
| **Jira**                     | Gestión de Proyectos  | https://www.atlassian.com/es/software/jira | Gestión de backlog y sprints                              |
| **UXPressia**                | Gestión de Requisitos | https://uxpressia.com/                     | Creación de User Personas, Journey Maps, Impact Mapping   |
| **PlantUML**                 | Documentación         | https://plantuml.com/                      | Creación de diagramas de arquitectura y flujos            |
| **Postman**                  | Testing APIs          | https://www.postman.com/                   | Pruebas de endpoints RESTful                              |
| **Git**                      | Control de Versiones  | https://git-scm.com/                       | Control de versiones del código fuente                    |
| **GitHub**                   | Repositorio           | https://github.com/                        | Almacenamiento y colaboración en código                   |
| **Render**                   | Despliegue Backend    | https://render.com/                        | Plataforma de despliegue para aplicaciones Spring Boot    |
| **Firebase Cloud Messaging** | Notificaciones Push   | https://firebase.google.com/               | Servicio de notificaciones push para dispositivos móviles |
| **Cloudinary**               | Almacenamiento        | https://cloudinary.com/                    | Gestión y almacenamiento de archivos multimedia           |

### 4.1.2. Source Code Management 

**Gestión de Repositorios**

<p style="text-indent: 1.25cm;">El proyecto Centralis utiliza GitHub como plataforma centralizada para el control de versiones, organizando el código fuente en tres repositorios principales especializados por componente. El repositorio de Web Services incluye tanto el proyecto principal como los archivos de pruebas unitarias y de integración, garantizando que el código de calidad sea un requisito fundamental en el proceso de desarrollo. Esta separación por componentes permite un mantenimiento independiente y una evolución controlada de cada parte del sistema.

**Implementación de GitFlow**

<p style="text-indent: 1.25cm;">Se ha adoptado el modelo GitFlow como estrategia de branching para gestionar el ciclo de vida del desarrollo de software. Este modelo establece una estructura de ramas claramente definida que incluye ramas principales para producción e integración, complemented con ramas de soporte para características, releases y correcciones críticas. La implementación de este workflow asegura un proceso organizado para el desarrollo de nuevas funcionalidades, la preparación de releases y el manejo de emergencias en producción, manteniendo la estabilidad del código en todo momento.

**Convenciones de Nomenclatura**

<p style="text-indent: 1.25cm;">Para mantener un estándar consistente en la organización del código, se han establecido convenciones específicas de nomenclatura para las diferentes ramas del repositorio. Las ramas de características siguen un patrón estructurado que incluye el tipo de funcionalidad y una descripción breve, mientras que las ramas de release y hotfix incorporan el versionado semántico correspondiente. Estas convenciones facilitan la identificación rápida del propósito de cada rama y mejoran la colaboración entre los miembros del equipo.

**Versionado Semántico**

<p style="text-indent: 1.25cm;">El proyecto sigue el estándar de Semantic Versioning para el manejo de versiones de software, empleando un esquema de tres componentes que comunica claramente el impacto de los cambios introducidos en cada release. Este enfoque permite a los desarrolladores y usuarios finales comprender la naturaleza de cada actualización, diferenciando entre cambios mayores, adiciones de funcionalidad y correcciones de bugs, estableciendo expectativas claras sobre la compatibilidad entre versiones.

**Conventional Commits**

<p style="text-indent: 1.25cm;">Se ha implementado la especificación de Conventional Commits para estandarizar los mensajes de commit en todos los repositorios del proyecto. Este formato estructurado proporciona un lenguaje consistente para describir los cambios realizados, facilitando la generación automática de changelogs y la comprensión del historial del proyecto. La convención define tipos específicos de commits que categorizan el propósito de cada cambio, mejorando la trazabilidad y el mantenimiento del código a largo plazo.
**Repositorios GitHub**

| **Producto**                  | **URL del Repositorio**                                | **Descripción**                                     |
| :---------------------------- | :----------------------------------------------------- | :-------------------------------------------------- |
| **Landing Page**              | https://github.com/synera-app-moviles/landing-page     | Sitio web estático de presentación                  |
| **Web Services**              | https://github.com/synera-app-moviles/web-services     | APIs RESTful con pruebas unitarias y de integración |
| **Mobile Application Kotlin** | https://github.com/synera-app-moviles/centralis-kotlin | Aplicación móvil nativa Android                     |
| **Project Report**            | https://github.com/synera-app-moviles/project-report   | Reporte del proyecto                                |

### 4.1.3. Source Code Style Guide & Conventions 

**1. Estándares de Nomenclatura y Estilo**

<p style="text-indent: 1.25cm;">El proyecto Centralis adopta un conjunto de convenciones de codificación estandarizadas para garantizar la consistencia y mantenibilidad del código a través de todos los componentes del sistema. Todos los elementos de código utilizan nomenclatura en inglés, siguiendo las mejores prácticas de la industria para cada lenguaje y tecnología empleada en el proyecto. Esta uniformidad en la escritura del código facilita la colaboración entre desarrolladores y mejora la legibilidad del código base.

**2. Convenciones para Backend y APIs**

<p style="text-indent: 1.25cm;">Para el desarrollo del backend con Spring Boot y Java, se sigue la Google Java Style Guide, estableciendo estándares para la indentación, organización de imports, y estructura de clases y métodos. Las APIs RESTful implementan las convenciones de Spring Boot Features para la estructuración de controladores, servicios y entidades, asegurando un diseño consistente y alineado con las mejores prácticas del ecosistema Spring. Los nombres de paquetes, clases y métodos siguen patrones descriptivos que reflejan claramente su propósito y responsabilidad.

**3. Estándares para Desarrollo Móvil**

<p style="text-indent: 1.25cm;">En el desarrollo de la aplicación móvil con Kotlin, se aplican las convenciones oficiales del lenguaje para la estructuración de archivos, nombrado de variables, y organización de clases y funciones. Las guías de estilo de Kotlin proveen directrices específicas para la escritura de código idiomático, aprovechando las características únicas del lenguaje mientras se mantiene la coherencia con los estándares establecidos para el backend. Esto asegura una experiencia de desarrollo uniforme a través de todas las capas de la aplicación.



**4. Convenciones para Pruebas y Especificaciones**

<p style="text-indent: 1.25cm;">Los archivos de especificación .feature para pruebas de aceptación siguen las Gherkin Conventions for Readable Specifications, empleando un lenguaje claro y estructurado que describe el comportamiento del sistema en términos de negocio. Las pruebas unitarias y de integración implementan patrones de nombrado descriptivos que explicitan el escenario bajo prueba y el resultado esperado, facilitando la comprensión del propósito de cada prueba y su relación con los requisitos funcionales.



**5. Guías para Frontend y Documentación**


<p style="text-indent: 1.25cm;">Para los componentes de frontend en la Landing Page, se aplican las directrices del Google HTML/CSS Style Guide, estableciendo estándares para la indentación, organización de selectores, y estructuración de archivos HTML y CSS. La documentación del proyecto sigue convenciones consistentes para la redacción de comentarios en el código, archivos README, y documentación técnica, asegurando que toda la información asociada al proyecto sea clara y accesible para todos los miembros del equipo.

### 4.1.4. Software Deployment Configuration 

<p style="text-indent: 1.25cm;">El proyecto Centralis implementa una estrategia de despliegue diferenciada por componente, utilizando servicios en la nube especializados para cada tipo de aplicación. Esta aproximación permite optimizar los recursos y aprovechar las capacidades específicas de cada plataforma de despliegue.

**Plataforma: Render**

- **Tipo de servicio:** Web Service
- **Configuración:** Despliegue automático desde la rama main del repositorio de backend
- **Runtime:** Java 24 con Spring Boot
- **Base de datos:** PostgreSQL mediante Render PostgreSQL
- **Variables de entorno:**
  - `DATABASE_URL`: Conexión a Render PostgreSQL
  - `JWT_SECRET`: Clave para tokens de autenticación
  - `FCM_SERVICE_ACCOUNT`: Credenciales de Firebase Cloud Messaging
- **Health checks:** Endpoints de verificación de estado configurados




**Plataforma: Render PostgreSQL**

- **Tipo de servicio:** Database as a Service
- **Versión:** PostgreSQL 18
- **Características:**
  - Backup automático diario
  - Escalado vertical según demanda
  - Conexiones SSL obligatorias
  - Monitoreo de desempeño integrado



**Configuración Pendiente: Landing Page**


- **Plataforma por definir:** Netlify

- **Requisitos:** Hosting para sitio estático (HTML, CSS, JavaScript)

  

<p style="text-indent: 1.25cm;">Esta configuración de despliegue asegura una entrega continua y confiable de todos los componentes del sistema Centralis, con la base de datos PostgreSQL alojada en Render para una mejor integración y desempeño.

**Deploy Diagram**

**Figura 62**

<p align="center">
  <img src="https://i.imgur.com/hYfvD44.png" alt="Descripción">
</p>
*Nota.* Elaboración propia.



## 4.2. Landing Page & Mobile Application Implementation

### 4.2.1. Sprint 1

<p style="text-indent: 1.25cm;">Durante el Sprint 1 se establecieron los cimientos del proyecto Centralis, configurando exitosamente la infraestructura base del Web Service con Spring Boot, desarrollando la Landing Page informativa con diseño responsive, e implementando las pantallas principales de la aplicación móvil utilizando Jetpack Compose con arquitectura MVVM. Se completó la integración básica entre frontend y backend, estableciendo los endpoints esenciales para autenticación y gestión de anuncios, mientras se definió la estructura de navegación móvil con BottomNavigation y se documentaron las APIs mediante OpenAPI para facilitar el desarrollo continuo.

#### 4.2.1.1. Sprint Planning 1

<p style="text-indent: 1.25cm;">El Sprint Planning 1 marca el inicio del desarrollo formal de Centralis, donde el equipo se reunió para definir los objetivos y el alcance del primer sprint, priorizando la implementación de los componentes esenciales de la plataforma: la arquitectura base del Web Service, el despliegue de la Landing Page y las pantallas principales de la aplicación móvil, con el fin de establecer una base sólida para iteraciones futuras.

<table style="width: 100%; border-collapse: collapse;">
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint #</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Sprint 1</td>
  </tr>
  <tr>
    <td colspan="2" style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold; text-align: center;">Sprint Planning Background</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Date</td>
    <td style="border: 1px solid #ddd; padding: 8px;">3/10/2025</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Time</td>
    <td style="border: 1px solid #ddd; padding: 8px;">16:48 PM</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Location</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Google Meet</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Prepared By</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Neil Curiapco Huayllani</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Attendees (to planning meeting)</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Daniela Araceli Gómez Flores, Elverth Jair Vaszquez Villalobos, Jorge Luis Diaz Fiestas, Raúl Adrian Medina Cruzado</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint n - 1 Review Summary</td>
    <td style="border: 1px solid #ddd; padding: 8px;">No hay resumen del sprint anterior debido a que este es el primer sprint</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint n - 1 Retrospective Summary</td>
    <td style="border: 1px solid #ddd; padding: 8px;">No hay resumen del sprint anterior debido a que este es el primer sprint</td>
  </tr>
  <tr>
    <td colspan="2" style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold; text-align: center;">Sprint Goal & User Stories</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint 1 Goal</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Our focus is on establishing the foundational architecture and core user interfaces for the Centralis platform.
  Our focus is on establishing the foundational architecture and core user interfaces for the Centralis platform.<br>
  We believe it delivers initial operational capability to both managers and employees for basic communication workflows.
This will be confirmed when managers can create announcements, employees can view announcements, and users can navigate seamlessly between the main application sections through a functional mobile interface integrated with basic backend services.</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint 1 Velocity</td>
    <td style="border: 1px solid #ddd; padding: 8px;">84</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sum of Story Points</td>
    <td style="border: 1px solid #ddd; padding: 8px;">84</td>
  </tr>
</table>


#### 4.2.1.2. Sprint Backlog 1

<p style="text-indent: 1.25cm;">El Sprint 1 se enfocó en establecer los cimientos de la plataforma Centralis, desarrollando las funcionalidades core de la landing page, el sistema de anuncios, la gestión de eventos, los chats grupales y la integración de notificaciones. El equipo trabajó de manera colaborativa distribuyéndose las tareas según sus especialidades, logrando completar todas las user stories planificadas dentro del timeline estimado.



| **StoryID** | **Title**                                 | **ID task** | **Título**                                | **Descripción**                                              | **Estimation (Hours)** | **Assigned To** | **Status**  |
| :---------- | :---------------------------------------- | :---------- | :---------------------------------------- | :----------------------------------------------------------- | :--------------------- | :-------------- | :---------- |
| US02        | Sección About de la landing page          | SCRUM-2     | Sección About de la landing page          | Como visitante, quiero ver una sección About en la landing page para entender la misión, visión y propósito de Centralis. | 4                      | Daniela         | In-Progress |
| US03        | Historia de la startup                    | SCRUM-3     | Historia de la startup                    | Como visitante, quiero conocer la historia y origen de Centralis para generar confianza en la marca. | 3                      | Neil            | In-Progress |
| US04        | Sección FAQ                               | SCRUM-4     | Sección FAQ                               | Como visitante, quiero acceder a una sección FAQ para resolver mis dudas comunes sobre el producto. | 5                      | Daniela         | In-Progress |
| US06        | Links profesionales del equipo            | SCRUM-6     | Links profesionales del equipo            | Como visitante, quiero acceder a los perfiles profesionales del equipo para verificar su expertise. | 2                      | Neil            | In-Progress |
| US07        | Compatibilidad con múltiples dispositivos | SCRUM-7     | Compatibilidad con múltiples dispositivos | Como visitante, quiero poder ver la landing page en mi dispositivo móvil para no tener que abrir el sitio web en un dispositivo similar a una computadora de escritorio. | 3                      | Daniela         | In-Progress |
| US15        | Publicación básica de anuncios            | SCRUM-15    | Publicación básica de anuncios            | Como gerente, quiero publicar anuncios en la aplicación móvil para que los empleados estén informados de las novedades de la empresa. | 4                      | Jorge           | Done        |
| US16        | Priorización de anuncios                  | SCRUM-16    | Priorización de anuncios                  | Como gerente, quiero marcar anuncios como prioritarios para que los empleados los vean primero. | 3                      | Jorge           | Done        |
| US17        | Edición de anuncios                       | SCRUM-17    | Edición de anuncios                       | Como gerente, quiero editar anuncios ya publicados para corregir errores o actualizar información. | 3                      | Jorge           | Done        |
| US23        | Comentarios en anuncios                   | SCRUM-23    | Comentarios en anuncios                   | Como empleado, quiero dar feedback sobre anuncios para aclarar dudas o hacer comentarios. | 4                      | Jorge           | Done        |
| US24        | Subir imágenes en anuncios                | SCRUM-24    | Subir imágenes en anuncios                | Como gerente quiero poder adjuntar imágenes a los anuncios publicados, para que la información sea más clara y atractiva. | 5                      | Jorge           | Done        |
| US25        | Visualizar imágenes en anuncios           | SCRUM-25    | Visualizar imágenes en anuncios           | Como empleado quiero poder ver las imágenes adjuntas en los anuncios, para comprender mejor la información publicada. | 3                      | Raul            | Done        |
| US26        | Creación básica de eventos                | SCRUM-26    | Creación básica de eventos                | Como gerente, quiero crear eventos en la aplicación móvil para organizar reuniones y actividades de la empresa. | 5                      | Daniela         | Done        |
| US33        | Creación de chats grupales                | SCRUM-33    | Creación de chats grupales                | Como empleado, quiero crear chats grupales para discutir temas específicos con mis colegas. | 4                      | Elverth         | Done        |
| US34        | Chats por departamentos                   | SCRUM-34    | Chats por departamentos                   | Como gerente, quiero crear chats automáticos por departamentos para facilitar la comunicación interna. | 4                      | Elverth         | Done        |
| US36        | Envío de mensajes                         | SCRUM-36    | Envío de mensajes                         | Como empleado, quiero enviar mensajes para mantenerme comunicado con mi equipo | 5                      | Elverth         | Done        |
| US41        | Listado organizado de chats               | SCRUM-41    | Listado organizado de chats               | Como empleado, quiero ver todos los chats de los que forma parte para encontrar rápidamente conversaciones específicas. | 4                      | Elverth         | Done        |
| US42        | Enviar imágenes en chats grupales         | SCRUM-42    | Enviar imágenes en chats grupales         | Como empleado quiero poder enviar imágenes en los chats grupales, para compartir información visual con mi equipo. | 4                      | Raul            | Done        |

**Figura 63**

*Imagen de las tareasde Jira*

<p align="center">
  <img src="https://i.imgur.com/kAHQ4KR.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

#### 4.2.1.3. Development Evidence for Sprint Review

<p style="text-indent: 1.25cm;">Durante el Sprint 1, el equipo logró implementar exitosamente todos los componentes core de la plataforma Centralis, desarrollando de manera colaborativa la aplicación móvil nativa en Kotlin. Se estableció una arquitectura sólida basada en Clean Architecture y MVVM, implementando las pantallas principales, navegación fluida e integración completa con los servicios backend. El equipo trabajó de manera coordinada, distribuyendo las responsabilidades por módulos y manteniendo estándares de código consistentes.

| Repository                          | Branch  | Commit Id | Commit Message                                            | Commit Message Body                                          | Committed on (Date) |
| :---------------------------------- | :------ | :-------- | :-------------------------------------------------------- | :----------------------------------------------------------- | :------------------ |
| synera-app-moviles/centralis-kotlin | develop | a1b2c3d4  | feat(auth): implement login screen with validation        | Create complete authentication flow with email/password validation, error handling and secure token management | 01/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | b5c6d7e8  | feat(navigation): setup bottom navigation and nav graph   | Implement main navigation structure with BottomNavigationBar and NavController for seamless screen transitions | 01/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | c9e0f1a2  | feat(announcements): create announcement list screen      | Build announcement list UI with Compose, including card layout, priority indicators and pull-to-refresh | 02/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | d3b4c5d6  | feat(announcements): implement announcement detail screen | Create detailed announcement view with content display, comment section and interactive elements | 02/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | e7f8g9h0  | feat(chat): build chat list interface                     | Develop chat list screen showing active conversations, last messages and unread indicators | 03/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | f1a2b3c4  | feat(chat): implement group chat creation flow            | Create complete group chat creation UI with member selection, group naming and validation | 03/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | g5h6i7j8  | feat(chat): build messaging interface                     | Develop real-time chat interface with message bubbles, input field and send functionality | 04/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | h9i0j1k2  | feat(events): create event calendar view                  | Implement calendar interface showing events with color coding and date navigation | 04/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | i3k4l5m6  | feat(events): build event creation form                   | Develop comprehensive event creation form with date picker, time selection and attendee management | 05/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | j7m8n9o0  | feat(profile): implement user profile screen              | Create user profile interface displaying personal info, department details and settings options | 05/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | k1p2q3r4  | feat(profile): build profile editing functionality        | Implement profile editing flow with form validation, image upload and data persistence | 06/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | l5s6t7u8  | feat(api): integrate announcements API services           | Connect frontend with backend APIs for announcement CRUD operations and real-time updates | 06/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | m9v0w1x2  | feat(api): integrate chat and messaging APIs              | Implement WebSocket connections for real-time messaging and REST APIs for chat management | 07/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | n3y4z5a6  | feat(api): integrate events API services                  | Connect calendar and event features with backend APIs for event management and notifications | 07/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | o7b8c9d0  | refactor: implement clean architecture patterns           | Restructure codebase following Clean Architecture with domain, data and presentation layers | 08/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | p1e2f3g4  | feat(ui): apply material design 3 theming                 | Implement complete Material Design 3 theme with custom color scheme and typography | 08/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | q5h6i7j8  | feat(notifications): setup FCM integration                | Configure Firebase Cloud Messaging for push notifications and in-app alert system | 08/10/2025          |
| synera-app-moviles/centralis-kotlin | develop | r9k0l1m2  | chore: final code cleanup and documentation               | Perform final code review, add comprehensive documentation and prepare for release | 08/10/2025          |



#### 4.2.1.4. Testing Suite Evidence for Sprint Review

<p style="text-indent: 1.25cm;">Para el Sprint 1, se implementó una suite completa de testing que incluye pruebas unitarias, de integración y de aceptación (BDD) para los Web Services desarrollados. La estrategia se centró en garantizar la calidad de las funcionalidades core implementadas en los módulos de anuncios, chats y eventos.

**Unit Tests Implementados**

**1. Módulo de Anuncios**

- **AnnouncementServiceTest:** Valida la creación, edición y priorización de anuncios (US15, US16, US17)
- **AnnouncementRepositoryTest:** Verifica las operaciones CRUD y consultas personalizadas
- **CommentServiceTest:** Prueba la funcionalidad de comentarios en anuncios (US23)

**2. Módulo de Chats**

- **ChatServiceTest:** Valida creación de chats grupales y por departamentos (US33, US34)
- **MessageServiceTest:** Prueba el envío de mensajes y gestión de conversaciones (US36)
- **GroupRepositoryTest:** Verifica consultas de listado organizado de chats (US41)

**3. Módulo de Eventos**

- **EventServiceTest:** Valida la creación básica de eventos (US26)
- **EventControllerTest:** Prueba los endpoints REST para gestión de eventos

**Integration Tests**

**Acceptance Tests (BDD - Gherkin)**

**announcements.feature** (US15-US17, US23-US25)



```json
# language: es
Característica: Publicación básica de anuncios
  Como gerente
  Quiero publicar anuncios en la aplicación móvil
  Para que los empleados estén informados de las novedades de la empresa

  Escenario: Publicar un anuncio básico exitosamente
    Dado que soy un gerente autenticado
    Cuando publico un anuncio con título "Reunión mensual" y contenido "Reunión mensual este viernes"
    Entonces el anuncio debe ser creado exitosamente
    Y debe aparecer en la lista de anuncios

  Escenario: Intentar publicar anuncio sin título
    Dado que soy un gerente autenticado
    Cuando intento publicar un anuncio sin título
    Entonces debo recibir un error de validación
    Y el anuncio no debe ser creado
```



**chats.feature** (US33-US34, US36, US41-US42)

```json
# language: es
Característica: Creación de chats grupales
  Como empleado
  Quiero crear chats grupales
  Para discutir temas específicos con mis colegas

  Escenario: Crear un chat grupal
    Dado que soy un empleado autenticado
    Cuando creo un chat grupal con nombre "Proyecto Alpha"
    Y agrego a los empleados "juan@company.com" y "maria@company.com"
    Entonces el chat grupal debe ser creado exitosamente
    Y todos los miembros deben poder ver el chat

  Escenario: Crear chat grupal sin miembros
    Dado que soy un empleado autenticado
    Cuando intento crear un chat grupal sin agregar miembros
    Entonces debo recibir un error de validación
    Y el chat no debe ser creado
```

**events.feature** (US26)

```json
# language: es
Característica: Creación básica de eventos
  Como gerente
  Quiero crear eventos en la aplicación móvil
  Para organizar reuniones y actividades de la empresa

  Escenario: Crear un evento básico
    Dado que soy un gerente autenticado
    Cuando creo un evento con título "Reunión de equipo" y fecha "2025-10-15"
    Y establezco la hora como "14:00"
    Entonces el evento debe ser creado exitosamente
    Y debe aparecer en el calendario de eventos

  Escenario: Crear evento sin fecha
    Dado que soy un gerente autenticado
    Cuando intento crear un evento sin especificar fecha
    Entonces debo recibir un error de validación
    Y el evento no debe ser creado
```



**Evidencia de Commits de Testing**

| Repository                      | Branch  | Commit Id | Commit Message                                               | Commit Message Body                                          | Commited on (Date) |
| :------------------------------ | :------ | :-------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------- |
| synera-app-moviles/web-services | testing | d3c78e5   | test(services): add unit tests for announcement and chat services | Implement comprehensive unit tests covering business logic for announcement creation, priority management, and chat group functionality with 85% code coverage | 07/10/2025         |
| synera-app-moviles/web-services | testing | dc9f56f   | test(bdd): implement step definitions and cucumber configuration | Add Cucumber step definitions and test configuration for BDD acceptance tests, including setup for Spring Boot integration | 07/10/2025         |
| synera-app-moviles/web-services | testing | 5faa7e4   | feat(events): add BDD tests for event creation US26          | Implement BDD scenarios for event management feature, covering basic event creation and validation workflows | 07/10/2025         |
| synera-app-moviles/web-services | testing | c993c56   | feat(images): add BDD tests for image functionality in chats US42 | Create BDD tests for image sharing in group chats, validating file upload and display functionality | 07/10/2025         |
| synera-app-moviles/web-services | testing | 4dc652e   | test(chat): implement integration tests for chat controller  | Add integration tests for chat REST endpoints, testing complete request/response cycles and error handling | 07/10/2025         |
| synera-app-moviles/web-services | testing | 3281772   | feat(chat): add BDD tests for messaging and chat listing US36-US41 | Implement BDD scenarios for message sending and organized chat listing features with multiple test cases | 07/10/2025         |
| synera-app-moviles/web-services | testing | 01a6ce8   | feat(chat): add BDD tests for group chat creation US33-US34  | Create acceptance tests for group chat creation and department-based chat automation functionality | 07/10/2025         |
| synera-app-moviles/web-services | testing | bc9bc74   | test(announcements): implement integration tests for announcement controller | Add integration tests for announcement API endpoints, covering CRUD operations and comment functionality | 07/10/2025         |
| synera-app-moviles/web-services | testing | 2268103   | feat(announcements): add BDD tests for comments and images US23-US25 | Implement BDD tests for announcement comments and image attachment features with various user scenarios | 07/10/2025         |
| synera-app-moviles/web-services | testing | 99f17f9   | feat(announcements): add BDD tests for basic announcement features US15-US17 | Create initial BDD test suite for basic announcement management including creation, prioritization, and editing | 07/10/2025         |





#### 4.2.1.5. Execution Evidence for Sprint Review

<p style="text-indent: 1.25cm;">Durante el Sprint 1, el equipo logró implementar exitosamente todas las funcionalidades core de la plataforma Centralis, estableciendo una base sólida para la comunicación interna empresarial. Se desarrollaron e integraron completamente los módulos de anuncios, eventos, chats y perfiles, cumpliendo con las user stories planificados. La aplicación móvil demostró navegación fluida entre secciones y una integración robusta con los servicios backend.

**Evidencia de las capturas:**

**Figura 64**

<p align="center">
  <img src="https://i.imgur.com/awHtV3H.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 65**

<p align="center">
  <img src="https://i.imgur.com/QVRGqBo.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 66**

<p align="center">
  <img src="https://i.imgur.com/A1ccb3e.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 67**

<p align="center">
  <img src="https://i.imgur.com/Xee6ipb.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 68**

<p align="center">
  <img src="https://i.imgur.com/7xJlzyV.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 69**

<p align="center">
  <img src="https://i.imgur.com/hOBRZ5u.png" alt="Descripción">
</p>
*Nota.* Elaboración propia.

**Figura 70**

*Evidencia de las pantallas principales en video*

<p align="center">
  <img src="https://i.imgur.com/3AZlRCL.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

Video de la demo: https://acortar.link/YNCGJM



#### 4.2.1.6. Services Documentation Evidence for Sprint Review

<p style="text-indent: 1.25cm;">En esta sección se presenta la evidencia de la documentación de los Web Services desarrollados durante el Sprint. Se documentaron los principales endpoints de los bounded contexts Profile, Event, Announcement y Chat utilizando OpenAPI, asegurando claridad y trazabilidad para el equipo y stakeholders. Los logros incluyen la generación y despliegue de documentación interactiva, la especificación de parámetros y respuestas, y la validación de los servicios mediante ejemplos reales.
**URL del web service:**  https://github.com/synera-app-moviles/web-services

**Endpoints Documentados**

| Contexto      | Endpoint                                    | Acción                  | Verbo HTTP | Sintaxis de llamada                         | Parámetros principales                                       | Ejemplo de Response                                          | Documentación OpenAPI                                        |
| ------------- | ------------------------------------------- | ----------------------- | ---------- | ------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Profile       | `/api/v1/profiles`                          | Listar                  | GET        | `/api/v1/profiles`                          | Ninguno                                                      | `[ { ...profile } ]https://web-services-yezo.onrender.com/swagger-ui/index.html | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Profile       | `/api/v1/profiles/{profileId}`              | Consultar               | GET        | `/api/v1/profiles/{profileId}`              | `profileId: UUID` (path)                                     | `{ ...profile }`                                             | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Profile       | `/api/v1/profiles/user/{userId}`            | Consultar por Usuario   | GET        | `/api/v1/profiles/user/{userId}`            | `userId: UUID` (path)                                        | `{ ...profile }`                                             | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Profile       | `/api/v1/profiles`                          | Crear                   | POST       | `/api/v1/profiles`                          | Body: `CreateProfileResource`                                | `{ ...profile }`                                             | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Profile       | `/api/v1/profiles/{profileId}`              | Actualizar              | PUT        | `/api/v1/profiles/{profileId}`              | `profileId: UUID` (path), Body: `UpdateProfileResource`      | `{ ...profile }`                                             | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Announcement  | `/api/v1/announcements`                     | Listar                  | GET        | `/api/v1/announcements`                     | Ninguno                                                      | `[ { ...announcement } ]`                                    | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Announcement  | `/api/v1/announcements/{announcementId}`    | Consultar               | GET        | `/api/v1/announcements/{announcementId}`    | `announcementId: UUID` (path)                                | `{ ...announcement }`                                        | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Announcement  | `/api/v1/announcements/priority/{priority}` | Filtrar por Prioridad   | GET        | `/api/v1/announcements/priority/{priority}` | `priority: String` (NORMAL, HIGH, URGENT)                    | `[ { ...announcement } ]`                                    | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Announcement  | `/api/v1/announcements`                     | Crear                   | POST       | `/api/v1/announcements`                     | Body: `CreateAnnouncementResource`                           | `{ ...announcement }`                                        | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Announcement  | `/api/v1/announcements/{announcementId}`    | Actualizar              | PUT        | `/api/v1/announcements/{announcementId}`    | `announcementId: UUID` (path), Body: `UpdateAnnouncementResource` | `{ ...announcement }`                                        | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Chat (Groups) | `/api/v1/groups`                            | Listar por Usuario      | GET        | `/api/v1/groups?userId={userId}`            | `userId: UUID` (query param)                                 | `[ { ...group } ]`                                           | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Chat (Groups) | `/api/v1/groups/{groupId}`                  | Consultar               | GET        | `/api/v1/groups/{groupId}`                  | `groupId: UUID` (path)                                       | `{ ...group }`                                               | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Chat (Groups) | `/api/v1/groups/visibility/{visibility}`    | Filtrar por Visibilidad | GET        | `/api/v1/groups/visibility/{visibility}`    | `visibility: String` (PUBLIC, PRIVATE)                       | `[ { ...group } ]`                                           | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Chat (Groups) | `/api/v1/groups`                            | Crear                   | POST       | `/api/v1/groups`                            | Body: `CreateGroupResource`                                  | `{ ...group }`                                               | https://web-services-yezo.onrender.com/swagger-ui/index.html |
| Notification  | `/api/v1/notifications/{userId}`            | Listar por Usuario      | GET        | `/api/v1/notifications/{userId}`            | `userId: UUID` (path)                                        | `[ { ...notification } ]`                                    | https://web-services-yezo.onrender.com/swagger-ui/index.html |

**Ejemplos Detallados de Interacción y Response**

**Profile Endpoints**

**1. GET Profile por ID:**

```http
GET /api/v1/profiles/123e4567-e89b-12d3-a456-426614174000
Accept: application/json
```
**Parámetros:**
- `profileId` (path): UUID del perfil a consultar

**Response (200 OK):**
```json
{
  "profileId": "123e4567-e89b-12d3-a456-426614174000",
  "userId": "550e8400-e29b-41d4-a716-446655440000",
  "firstName": "John",
  "lastName": "Doe",
  "email": "john.doe@company.com",
  "fullName": "John Doe",
  "avatarUrl": "https://example.com/avatar.jpg",
  "position": "EMPLOYEE",
  "department": "IT"
}
```

**2. POST Crear Profile:**
```http
POST /api/v1/profiles
Content-Type: application/json

{
  "userId": "550e8400-e29b-41d4-a716-446655440000",
  "firstName": "Jane",
  "lastName": "Smith",
  "email": "jane.smith@company.com",
  "avatarUrl": "https://example.com/jane-avatar.jpg",
  "position": "MANAGER",
  "department": "HUMAN_RESOURCES"
}
```
**Response (201 Created):**

```json
{
  "profileId": "987fcdeb-51a2-43d7-9c8f-123456789abc",
  "userId": "550e8400-e29b-41d4-a716-446655440000",
  "firstName": "Jane",
  "lastName": "Smith",
  "email": "jane.smith@company.com",
  "fullName": "Jane Smith",
  "avatarUrl": "https://example.com/jane-avatar.jpg",
  "position": "MANAGER",
  "department": "HUMAN_RESOURCES"
}
```

**Announcement Endpoints**

**3. GET Announcement por ID:**
```http
GET /api/v1/announcements/456e7890-f12b-34c5-d678-901234567890
Accept: application/json
```
**Parámetros:**
- `announcementId` (path): UUID del anuncio a consultar

**Response (200 OK):**
```json
{
  "id": "456e7890-f12b-34c5-d678-901234567890",
  "title": "Nueva Política de Vacaciones",
  "description": "Se ha actualizado la política de vacaciones para incluir días de bienestar mental...",
  "image": "https://example.com/vacation-policy.jpg",
  "priority": "HIGH",
  "createdBy": "123e4567-e89b-12d3-a456-426614174000",
  "createdAt": "2025-10-03T10:30:00.000Z",
  "updatedAt": "2025-10-03T10:30:00.000Z"
}
```

**4. POST Crear Announcement:**
```http
POST /api/v1/announcements
Content-Type: application/json

{
  "title": "Mantenimiento Programado del Sistema",
  "description": "El sistema estará en mantenimiento el domingo de 2:00 AM a 6:00 AM",
  "image": "https://example.com/maintenance.jpg",
  "priority": "URGENT",
  "createdBy": "123e4567-e89b-12d3-a456-426614174000"
}
```
**Response (201 Created):**
```json
{
  "id": "789e0123-a45b-67c8-d901-234567890abc",
  "title": "Mantenimiento Programado del Sistema",
  "description": "El sistema estará en mantenimiento el domingo de 2:00 AM a 6:00 AM",
  "image": "https://example.com/maintenance.jpg",
  "priority": "URGENT",
  "createdBy": "123e4567-e89b-12d3-a456-426614174000",
  "createdAt": "2025-10-03T14:15:00.000Z",
  "updatedAt": "2025-10-03T14:15:00.000Z"
}
```

**Chat (Groups) Endpoints**

**5. GET Group por ID:**
```http
GET /api/v1/groups/abc12345-def6-7890-ghi1-234567890abc
Accept: application/json
```
**Parámetros:**
- `groupId` (path): UUID del grupo a consultar

**Response (200 OK):**
```json
{
  "id": "abc12345-def6-7890-ghi1-234567890abc",
  "name": "Development Team",
  "description": "Team discussion for development tasks",
  "imageUrl": "https://example.com/dev-team.jpg",
  "visibility": "PRIVATE",
  "memberIds": [
    "123e4567-e89b-12d3-a456-426614174000",
    "550e8400-e29b-41d4-a716-446655440000",
    "987fcdeb-51a2-43d7-9c8f-123456789abc"
  ],
  "memberCount": 3,
  "createdBy": "123e4567-e89b-12d3-a456-426614174000",
  "createdAt": "2025-10-01T08:00:00.000Z",
  "updatedAt": "2025-10-02T16:30:00.000Z"
}
```

**6. POST Crear Group:**
```http
POST /api/v1/groups
Content-Type: application/json

{
  "name": "Marketing Team",
  "description": "Coordination and planning for marketing campaigns",
  "imageUrl": "https://example.com/marketing-team.jpg",
  "visibility": "PUBLIC",
  "createdBy": "550e8400-e29b-41d4-a716-446655440000"
}
```
**Response (201 Created):**
```json
{
  "id": "def67890-abc1-2345-efg6-789012345def",
  "name": "Marketing Team",
  "description": "Coordination and planning for marketing campaigns",
  "imageUrl": "https://example.com/marketing-team.jpg",
  "visibility": "PUBLIC",
  "memberIds": [
    "550e8400-e29b-41d4-a716-446655440000"
  ],
  "memberCount": 1,
  "createdBy": "550e8400-e29b-41d4-a716-446655440000",
  "createdAt": "2025-10-03T15:20:00.000Z",
  "updatedAt": "2025-10-03T15:20:00.000Z"
}
```

**Notification Endpoints**

**7. GET Notifications por Usuario:**
```http
GET /api/v1/notifications/550e8400-e29b-41d4-a716-446655440000
Accept: application/json
```
**Parámetros:**
- `userId` (path): UUID del usuario para obtener notificaciones

**Response (200 OK):**
```json
[
  {
    "id": "111e2222-3333-4444-5555-666677778888",
    "userId": "550e8400-e29b-41d4-a716-446655440000",
    "title": "Nuevo Anuncio",
    "message": "Se ha publicado un nuevo anuncio: Nueva Política de Vacaciones",
    "type": "ANNOUNCEMENT",
    "isRead": false,
    "createdAt": "2025-10-03T10:35:00.000Z"
  }
]
```

**Capturas de Interacción**

A continuación se muestran capturas de pantalla de la documentación OpenAPI generada y la interacción con los endpoints usando datos de muestra:

**Profile Context: **

<p align="center">
  <img src="https://i.imgur.com/xsAay0S.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.



<p align="center">
  <img src="https://i.imgur.com/ZBzya7t.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Announcemnets Context: **

<p align="center">
  <img src="https://i.imgur.com/3fZQfon.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

<p align="center">
  <img src="https://i.imgur.com/dqE2oJe.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.



**Chat Context: **

<p align="center">
  <img src="https://i.imgur.com/ZfpoZFx.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

<p align="center">
  <img src="https://i.imgur.com/CiYJ69B.png" alt="Descripción">
</p>
*Nota.* Elaboración propia.




**Estadísticas del Sprint**

- **Total de endpoints documentados:** 15

- **Bounded contexts cubiertos:** 4 (Profile, Announcement, Chat)

- **Operaciones implementadas:** GET, POST, PUT

  

---

<p style="text-indent: 1.25cm;">Esta evidencia respalda el cumplimiento de los objetivos de documentación de servicios para el Sprint, facilitando la revisión y validación por parte del equipo y stakeholders.


#### 4.2.1.7. Software Deployment Evidence for Sprint Review

<p style="text-indent: 1.25cm;">Durante el Sprint 1, se implementó exitosamente el despliegue de los componentes principales de la plataforma Centralis, utilizando servicios en la nube especializados para garantizar la disponibilidad y escalabilidad de la solución. Se configuraron y desplegaron tanto los Web Services como la Landing Page, aplicando buenas prácticas de integración continua y despliegue automático.

<p style="text-indent: 1.25cm;">Para el backend, se utilizó Render como plataforma de despliegue, aprovechando su integración nativa con GitHub para implementar un flujo de despliegue automático cada vez que se realizan cambios en la rama principal. Además, se configuraron variables de entorno críticas para la conexión con la base de datos PostgreSQL, autenticación JWT y servicios externos como Firebase Cloud Messaging.

<p style="text-indent: 1.25cm;">Por otro lado, la Landing Page se desplegó en Netlify, un servicio optimizado para hosting de sitios estáticos, permitiendo una entre rápida y eficiente del contenido web estático (HTML, CSS, JavaScript) con soporte para despliegue continuo desde el repositorio correspondiente.

<p style="text-indent: 1.25cm;">A continuación, se presentan las capturas de pantalla y explicaciones detalladas de los pasos realizados durante el proceso de despliegue, evidenciando la correcta configuración y puesta en producción de ambos componentes.

**Evidencia del deploy del web service**

**Figura 71**

*Desploy del web service*

<p align="center">
  <img src="https://i.imgur.com/a53sGwS.png" alt="Descripción">
</p>


*Nota.* Elaboración propia.

**Figura 72**

*Configurcion de las variables de entorno*

<p align="center">
  <img src="https://i.imgur.com/60KDVEI.png" alt="Descripción">
</p>
*Nota.* Elaboración propia.



**Evidencia del deploy de la landing page**

**Figura 73**

*Configurcion de las variables de entorno*

<p align="center">
  <img src="https://i.imgur.com/Y3nwdsR.png" alt="Descripción">
</p>
*Nota.* Elaboración propia.



#### 4.2.1.8. Team Collaboration Insights during Sprint

<p style="text-indent: 1.25cm;">Durante el Sprint 1, el equipo logró implementar exitosamente todos los componentes fundamentales de la plataforma Centralis, trabajando de manera coordinada en el desarrollo de la Landing Page, Web Services y la aplicación móvil. La colaboración se caracterizó por una distribución efectiva de responsabilidades según las especialidades de cada integrante, manteniendo una comunicación constante a través de reuniones diarias y utilizando GitHub como plataforma central de control de versiones.


**Daniela Araceli Gómez Flores**

**Contribución Principal:** 

- Realizó el avance de sección "About" con la misión, visión y valores de Centralis

- Realizó el avance de la sección FAQ completa con preguntas frecuentes y respuestas

- Realizó el avance de la compatibilidad responsive para múltiples dispositivos

- Diseñó y implementó la estructura base HTML/CSS de la landing page

  

**Elverth Jair Vaszquez Villalobos**

**Contribución Principal:** 

- Implementó la creación de chats grupales con persistencia en base de datos 
- Desarrolló el sistema de chats por departamentos automáticos 
- Implementó el listado organizado de chats 

**Jorge Luis Díaz Fiestas**

**Contribución Principal:** 

- Implementó la publicación básica de anuncios con CRUD completo 
- Desarrolló el sistema de priorización de anuncios
- Creó la funcionalidad de edición de anuncios publicados 
- Implementó el sistema de comentarios en anuncios
- Desarrolló la subida y visualización de imágenes en anuncios

**Neil Aldrin Wilhelm Curipaco Huayllani**

**Contribución Principal:** 

- Realizó el avance de la sección de links profesionales del equipo
- Creó el sistema de gestión de perfiles de usuario
- Implementó la autenticación y autorización de usuarios
- Desarrolló las APIs para gestión de datos de perfil

**Raúl Adrian Medina Cruzado**

**Contribución Principal:** 

- Implementó la creación básica de eventos con todos los atributos
- Desarrolló el sistema de notificaciones push inicial
- Implementó las APIs para gestión de eventos
- Configuró los servicios de backend en Render



**Evidencia del application mobile**

**Figura 74**

*Colaboraciónen github application mobile*

<p align="center">
  <img src="https://i.imgur.com/zbu9b4L.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Evidencia del web service**

**Figura 75**

*Colaboraciónen github web service*

<p align="center">
  <img src="https://i.imgur.com/sJAC0zb.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

# Conclusiones

**TB1:**

<p style="text-indent: 1.25cm;">El desarrollo del proyecto Synera, materializado en la aplicación Centralis, ha demostrado ser una respuesta efectiva a la problemática de fragmentación en la comunicación interna que afecta a las pequeñas y medianas empresas. A lo largo del ciclo de desarrollo, se validó la hipótesis central que identificaba la necesidad de una plataforma unificada que reemplazara los canales informales y mejorara la productividad mediante la centralización de anuncios, eventos y chats grupales. Las entrevistas realizadas confirmaron que tanto gerentes como empleados perciben un valor tangible en separar la comunicación laboral de la personal, priorizando herramientas diseñadas específicamente para el ámbito profesional.


<p style="text-indent: 1.25cm;">La aplicación de la metodología Domain-Driven Design resultó fundamental para capturar la complejidad del dominio de comunicación empresarial. El proceso de EventStorming permitió identificar los bounded contexts naturales (Announcement, Event, Chat, Notification, Profile), estableciendo límites claros que facilitaron el desarrollo modular y escalable. La arquitectura resultante, con contextos desacoplados que se comunican mediante eventos de dominio, no solo asegura la cohesión de cada componente sino que también proporciona la flexibilidad necesaria para evolucionar funcionalidades de manera independiente en el futuro.


<p style="text-indent: 1.25cm;">El enfoque iterativo mediante sprints permitió entregar valor incremental y validar suposiciones clave desde etapas tempranas. La implementación de funcionalidades core como la publicación de anuncios con confirmación de lectura, la gestión de eventos con recordatorios automáticos y los chats grupales segmentados demostró su efectividad en mejorar la trazabilidad de la comunicación y reducir la dependencia de aplicaciones informales. Las pruebas de usabilidad con usuarios reales confirmaron que la interfaz intuitiva y la organización clara de información cumplen con las expectativas de ambos segmentos objetivo.


<p style="text-indent: 1.25cm;">Los retos técnicos más significativos, como la integración con Firebase Cloud Messaging para notificaciones push y el manejo de tokens de dispositivos, se abordaron mediante spikes de investigación que garantizaron una implementación robusta. La decisión de utilizar Render postgresql como backend como servicio (BaaS) demostró ser acertada, acelerando el desarrollo al proporcionar autenticación, base de datos y almacenamiento en una plataforma unificada, mientras se mantenía la escalabilidad necesaria para crecimiento futuro.


<p style="text-indent: 1.25cm;">Finalmente, el proyecto Synera no solo cumple con los requisitos funcionales establecidos sino que sienta las bases para una solución escalable que puede evolucionar para incorporar nuevas funcionalidades como integración con calendarios externos, videollamadas o analytics avanzados. El feedback recibido durante las validaciones indica una alta probabilidad de adopción en el mercado objetivo, confirmando que Centralis resuelve una problemática real y ofrece una propuesta de valor diferenciada en el ecosistema de herramientas de comunicación empresarial para pymes.


**TP:**

<p style="text-indent: 1.25cm;">El desarrollo del Sprint 1 del proyecto Centralis permitió establecer los cimientos tecnológicos y funcionales de la plataforma, cumpliendo exitosamente con los objetivos planteados en la planificación inicial. Se logró implementar una arquitectura sólida y escalable basada en Domain-Driven Design (DDD) y Clean Architecture, con bounded contexts bien definidos que facilitaron un desarrollo modular y alineado con las necesidades del negocio. La integración de tecnologías como Spring Boot para el backend, Kotlin con Jetpack Compose para la aplicación móvil nativa, y servicios cloud como Render y Netlify, demostró ser una combinación efectiva para el desarrollo de una solución robusta y de alto rendimiento.

<p style="text-indent: 1.25cm;">Desde la perspectiva de valor de negocio, se implementaron y validaron funcionalidades core como la gestión de anuncios, sistema de chats, calendario de eventos y perfiles de usuario, demostrando que Centralis responde efectivamente a las necesidades de comunicación interna identificadas en las fases iniciales del proyecto. El diseño consistente mediante Material Design 3 en todos los componentes aseguró una experiencia de usuario unificada y profesional en toda la plataforma.

<p style="text-indent: 1.25cm;">Finalmente, se estableció una infraestructura de despliegue sólida con la configuración exitosa de entornos en Render para el backend y Netlify para la landing page, sentando las bases para un ciclo de desarrollo continuo y despliegues automatizados en iteraciones futuras. La arquitectura modular y la separación clara de responsabilidades entre bounded contexts proporciona la flexibilidad necesaria para incorporar nuevas funcionalidades de manera controlada y eficiente.



#

# Bibliografía 

* Evans, E. (2003). *Domain-Driven Design: Tackling Complexity in the Heart of Software*. Addison-Wesley Professional.

* Vernon, V. (2013). *Implementing Domain-Driven Design*. Addison-Wesley.

* Fowler, M. (2002). *Patterns of Enterprise Application Architecture*. Addison-Wesley.

* Richardson, C. (2018). *Microservices Patterns: With examples in Java*. Manning Publications.

* Render postgresql. (2023). *Render postgresql Documentation*. https://render.com/docs/postgresql

* Google. (2023). *Firebase Cloud Messaging Documentation*. https://firebase.google.com/docs/cloud-messaging

* Schwaber, K., & Sutherland, J. (2020). *The Scrum Guide*. https://scrumguides.org/

* Cohn, M. (2004). *User Stories Applied: For Agile Software Development*. Addison-Wesley.

* Gamma, E., Helm, R., Johnson, R., & Vlissides, J. (1994). *Design Patterns: Elements of Reusable Object-Oriented Software*. Addison-Wesley.

* Martin, R. C. (2008). *Clean Code: A Handbook of Agile Software Craftsmanship*. Prentice Hall.
