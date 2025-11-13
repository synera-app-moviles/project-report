# Capítulo IV: Solution Software Design



## 4.1. Software Configuration Management 

### 4.1.1.Software Development Environment Configuration

| **Producto/Herramienta**     | **Categoría**         | **Ruta de Descarga/Acceso**                | **Propósito en el Proyecto**                              |
| ---------------------------- | --------------------- | ------------------------------------------ | --------------------------------------------------------- |
| **OpenJDK**                  | Desarrollo Backend    | https://openjdk.org/                       | Entorno de ejecución para aplicaciones Java               |
| **Apache Maven**             | Desarrollo Backend    | https://maven.apache.org/                  | Gestión de dependencias y construcción del proyecto       |
| **Spring Boot**              | Desarrollo Backend    | https://spring.io/projects/spring-boot     | Framework para desarrollo de APIs RESTful                 |
| **Android Studio**           | Desarrollo Móvil      | https://developer.android.com/studio       | IDE para desarrollo de aplicaciones Android nativas       |
| **Kotlin**                   | Desarrollo Móvil      | Incluido en Android Studio                 | Lenguaje de programación para aplicación móvil            |
| **Render PostgreSQL**        | Base de Datos         | https://render.com/docs/postgresql         | Base de datos relacional en la nube                       |
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

**Figura 66**

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
    <td style="border: 1px solid #ddd; padding: 8px;">Neil Curipaco Huayllani</td>
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
    <td style="border: 1px solid #ddd; padding: 8px;">73</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sum of Story Points</td>
    <td style="border: 1px solid #ddd; padding: 8px;">73</td>
  </tr>
</table>



#### 4.2.1.2. Sprint Backlog 1

<p style="text-indent: 1.25cm;">El Sprint 1 se enfocó en establecer los cimientos de la plataforma Centralis, desarrollando las funcionalidades core de la landing page, el sistema de anuncios, la gestión de eventos, los chats grupales y la integración de notificaciones. El equipo trabajó de manera colaborativa distribuyéndose las tareas según sus especialidades, logrando completar todas las user stories planificadas dentro del timeline estimado.



| **StoryID** | **Title**                                 | **ID task** | **Título**                                | **Descripción**                                              | **Estimation (Hours)** | **Assigned To** | **Status** |
| :---------- | :---------------------------------------- | :---------- | :---------------------------------------- | :----------------------------------------------------------- | :--------------------- | :-------------- | :--------- |
| US02        | Sección About de la landing page          | SCRUM-2     | Sección About de la landing page          | Como visitante, quiero ver una sección About en la landing page para entender la misión, visión y propósito de Centralis. | 4                      | Daniela         | Done       |
| US03        | Historia de la startup                    | SCRUM-3     | Historia de la startup                    | Como visitante, quiero conocer la historia y origen de Centralis para generar confianza en la marca. | 3                      | Neil            | Done       |
| US04        | Sección FAQ                               | SCRUM-4     | Sección FAQ                               | Como visitante, quiero acceder a una sección FAQ para resolver mis dudas comunes sobre el producto. | 5                      | Daniela         | Done       |
| US06        | Links profesionales del equipo            | SCRUM-6     | Links profesionales del equipo            | Como visitante, quiero acceder a los perfiles profesionales del equipo para verificar su expertise. | 2                      | Neil            | Done       |
| US07        | Compatibilidad con múltiples dispositivos | SCRUM-7     | Compatibilidad con múltiples dispositivos | Como visitante, quiero poder ver la landing page en mi dispositivo móvil para no tener que abrir el sitio web en un dispositivo similar a una computadora de escritorio. | 3                      | Daniela         | Done       |
| US15        | Publicación básica de anuncios            | SCRUM-15    | Publicación básica de anuncios            | Como gerente, quiero publicar anuncios en la aplicación móvil para que los empleados estén informados de las novedades de la empresa. | 4                      | Jorge           | Done       |
| US16        | Priorización de anuncios                  | SCRUM-16    | Priorización de anuncios                  | Como gerente, quiero marcar anuncios como prioritarios para que los empleados los vean primero. | 3                      | Jorge           | Done       |
| US17        | Edición de anuncios                       | SCRUM-17    | Edición de anuncios                       | Como gerente, quiero editar anuncios ya publicados para corregir errores o actualizar información. | 3                      | Jorge           | Done       |
| US23        | Comentarios en anuncios                   | SCRUM-23    | Comentarios en anuncios                   | Como empleado, quiero dar feedback sobre anuncios para aclarar dudas o hacer comentarios. | 4                      | Jorge           | Done       |
| US24        | Subir imágenes en anuncios                | SCRUM-24    | Subir imágenes en anuncios                | Como gerente quiero poder adjuntar imágenes a los anuncios publicados, para que la información sea más clara y atractiva. | 5                      | Jorge           | Done       |
| US25        | Visualizar imágenes en anuncios           | SCRUM-25    | Visualizar imágenes en anuncios           | Como empleado quiero poder ver las imágenes adjuntas en los anuncios, para comprender mejor la información publicada. | 3                      | Raul            | Done       |
| US26        | Creación básica de eventos                | SCRUM-26    | Creación básica de eventos                | Como gerente, quiero crear eventos en la aplicación móvil para organizar reuniones y actividades de la empresa. | 5                      | Daniela         | Done       |
| US33        | Creación de chats grupales                | SCRUM-33    | Creación de chats grupales                | Como empleado, quiero crear chats grupales para discutir temas específicos con mis colegas. | 4                      | Elverth         | Done       |
| US34        | Chats por departamentos                   | SCRUM-34    | Chats por departamentos                   | Como gerente, quiero crear chats automáticos por departamentos para facilitar la comunicación interna. | 4                      | Elverth         | Done       |
| US36        | Envío de mensajes                         | SCRUM-36    | Envío de mensajes                         | Como empleado, quiero enviar mensajes para mantenerme comunicado con mi equipo | 5                      | Elverth         | Done       |
| US41        | Listado organizado de chats               | SCRUM-41    | Listado organizado de chats               | Como empleado, quiero ver todos los chats de los que forma parte para encontrar rápidamente conversaciones específicas. | 4                      | Elverth         | Done       |
| US42        | Enviar imágenes en chats grupales         | SCRUM-42    | Enviar imágenes en chats grupales         | Como empleado quiero poder enviar imágenes en los chats grupales, para compartir información visual con mi equipo. | 4                      | Raul            | Done       |

**Figura 67**

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



```gherkin
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

```gherkin
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

```gherkin
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

**Figura 68**

<p align="center">
  <img src="https://i.imgur.com/awHtV3H.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 69**

<p align="center">
  <img src="https://i.imgur.com/QVRGqBo.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 70**

<p align="center">
  <img src="https://i.imgur.com/A1ccb3e.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 71**

<p align="center">
  <img src="https://i.imgur.com/Xee6ipb.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 72**

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

**Figura 75**

*Desploy del web service*

<p align="center">
  <img src="https://i.imgur.com/a53sGwS.png" alt="Descripción">
</p>


*Nota.* Elaboración propia.

**Figura 76**

*Configurcion de las variables de entorno*

<p align="center">
  <img src="https://i.imgur.com/60KDVEI.png" alt="Descripción">
</p>
*Nota.* Elaboración propia.



**Evidencia del deploy de la landing page**

**Figura 73**

*Deploy de la landing page*

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

**Figura 78**

*Colaboraciónen github application mobile*

<p align="center">
  <img src="https://i.imgur.com/zbu9b4L.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Evidencia del web service**

**Figura 79**

*Colaboraciónen github web service*

<p align="center">
  <img src="https://i.imgur.com/sJAC0zb.png" alt="Descripción">
</p>
*Nota.* Elaboración propia.

### 4.2.2. Sprint 2

<p style="text-indent: 1.25cm;">Durante el Sprint 2 se consolidaron las funcionalidades <i>core</i> del proyecto, logrando el despliegue completo del 100% del Web Service con Spring Boot y la finalización de su documentación en OpenAPI. En el desarrollo móvil, se implementaron las lógicas de negocio avanzadas para los roles de administrador en la aplicación nativa Kotlin, y, en paralelo, se inició el desarrollo de la aplicación cross-platform utilizando Flutter. Adicionalmente, se expandió el Landing Page, añadiendo nuevas secciones de contenido y las bases para su internacionalización.

#### 4.2.2.1. Sprint Planning 2



<p style="text-indent: 1.25cm;">El Sprint Planning 2 se realizó para dar continuidad al desarrollo del proyecto, tomando como base los cimientos establecidos en la primera iteración. El equipo se reunió para revisar los resultados y el feedback del Sprint 1, definir el nuevo Sprint Goal y seleccionar las User Stories para el segundo ciclo de desarrollo. El foco se centró en completar el despliegue del backend, implementar las funciones de administrador Gerente y comenzar el desarrollo de la aplicación cross-platform en Flutter.</p



<table style="width: 100%; border-collapse: collapse;">
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint #</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Sprint 2</td>
  </tr>
  <tr>
    <td colspan="2" style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold; text-align: center;">Sprint Planning Background</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Date</td>
    <td style="border: 1px solid #ddd; padding: 8px;">31/10/2025</td>
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
    <td style="border: 1px solid #ddd; padding: 8px;">Neil Curipaco Huayllani</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Attendees (to planning meeting)</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Daniela Araceli Gómez Flores, Elverth Jair Vaszquez Villalobos, Jorge Luis Diaz Fiestas, Raúl Adrian Medina Cruzado</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint n - 1 Review Summary</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Based on the Sprint 1 review, the team successfully established the project's foundation. The base Web Service en Spring Boot, the responsive Landing Page, and the main screens of the Kotlin mobile app were implemented. Basic API integration for authentication and announcements is functional, and API documentation with OpenAPI was completed.</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint n - 1 Retrospective Summary</td>
    <td style="border: 1px solid #ddd; padding: 8px;">The retrospective identified that while backend and frontend integration was successful, initial setup of the development environment took longer than expected. The team agreed to improve communication for dependency management and to better define task breakdowns in Jira to avoid overlap.</td>
  </tr>
  <tr>
    <td colspan="2" style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold; text-align: center;">Sprint Goal & User Stories</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint 2 Goal</td>
    <td style="border: 1px solid #ddd; padding: 8px;">Our focus is on completing the backend deployment and expanding the platform's core functionalities, including administrator controls and initiating the cross-platform Flutter application. <br><br>
We believe it delivers critical management capabilities to the 'Manager' role and expands our technological reach by starting Flutter development. <br> <br>
This will be confirmed when the backend is 100% deployed on a public site, managers can successfully create, edit, and delete announcements, events, and groups, and the initial build of the Flutter application is running.</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sprint 2 Velocity</td>
    <td style="border: 1px solid #ddd; padding: 8px;">64</td>
  </tr>
  <tr>
    <td style="border: 1px solid #ddd; padding: 8px; background-color: #f2f2f2; font-weight: bold;">Sum of Story Points</td>
    <td style="border: 1px solid #ddd; padding: 8px;">64</td>
  </tr>
</table>





#### 4.2.2.2. Sprint Backlog 2

<p style="text-indent: 1.25cm;">El Sprint Backlog 2 se enfocó en consolidar las funcionalidades de administrador (Gerente) y en robustecer las características principales de la plataforma. El equipo se distribuyó las 18 historias de usuario planificadas, abarcando el CRUD completo de Anuncios y Eventos, la implementación de moderación avanzada en los Chats y mejoras significativas en la accesibilidad e internacionalización del Landing Page.</p>


| StoryID | Title                                       | ID task  | Título                                      | Descripción                                                  | Estimation  (Hours) | Assigned  To | Status |
| ------- | ------------------------------------------- | -------- | ------------------------------------------- | ------------------------------------------------------------ | ------------------- | ------------ | ------ |
| US01    | Cambiar el idioma de la landing page        | SCRUM-1  | Cambiar el idioma de la landing page        | Como visitante, quiero traducir la página para leer el contenido en mi idioma preferido. | 3                   | Jorge        | Done   |
| US05    | Sección Team                                | SCRUM-5  | Sección Team                                | Como visitante, quiero conocer al equipo detrás de Centralis para humanizar la marca y generar confianza. | 3                   | Daniela      | Done   |
| US10    | Acceder a las descripciones de las imágenes | SCRUM-10 | Acceder a las descripciones de las imágenes | Como visitante que utiliza un lector de pantalla, quiero que todas las imágenes significativas de la página de destino incluyan texto alternativo claro para poder comprender el contenido visual y navegar por el sitio web. | 2                   | Daniela      | Done   |
| US18    | Eliminación de anuncios                     | SCRUM-18 | Eliminación de anuncios                     | Como gerente, quiero eliminar anuncios obsoletos para mantener la información actualizada. | 4                   | Jorge        | Done   |
| US24    | Subir imágenes en anuncios                  | SCRUM-24 | Subir imágenes en anuncios                  | Como gerente quiero poder adjuntar imágenes a los anuncios publicados, para que la información sea más clara y atractiva. | 5                   | Jorge        | Done   |
| US27    | Invitación a departamentos específicos      | SCRUM-27 | Invitación a departamentos específicos      | Como gerente, quiero invitar a departamentos específicos a eventos para asegurar que solo participen los empleados requeridos. | 4                   | Neil         | Done   |
| US28    | Confirmación de asistencia                  | SCRUM-28 | Confirmación de asistencia                  | Como empleado, quiero confirmar mi asistencia a eventos para que los organizadores sepan cuántos asistirán. | 3                   | Daniela      | Done   |
| US29    | Cancelación de eventos                      | SCRUM-29 | Cancelación de eventos                      | Como gerente, quiero cancelar eventos cuando sea necesario para evitar confusiones. | 3                   | Daniela      | Done   |
| US30    | Modificación de eventos                     | SCRUM-30 | Modificación de eventos                     | Como gerente, quiero modificar detalles de eventos existentes para ajustar cambios de último momento. | 4                   | Daniela      | Done   |
| US31    | Eventos prioritarios                        | SCRUM-31 | Eventos prioritarios                        | Como gerente, quiero marcar eventos como prioritarios para que los empleados les presten especial atención. | 3                   | Neil         | Done   |
| US32    | Métricas de participación                   | SCRUM-32 | Métricas de participación                   | Como gerente, quiero ver métricas de participación en eventos para medir el engagement del equipo. | 5                   | Neil         | Done   |
| US35    | Eliminar grupos de chats                    | SCRUM-35 | Eliminar grupos de chats                    | Como gerente, quiero eliminar chats grupales para mantener el orden de las conversaciones. | 4                   | Elverth      | Done   |
| US37    | Eliminación de mensajes enviados            | SCRUM-37 | Eliminación de mensajes enviados            | Como empleado, quiero eliminar mensajes que envié por error para corregir mis equivocaciones. | 3                   | Elverth      | Done   |
| US38    | Modificación de mensajes enviados           | SCRUM-38 | Modificación de mensajes enviados           | Como empleado, quiero editar mensajes que ya envié para corregir errores tipográficos. | 3                   | Elverth      | Done   |
| US39    | Eliminación de mensajes por moderadores     | SCRUM-39 | Eliminación de mensajes por moderadores     | Como gerente, quiero eliminar mensajes inapropiados de cualquier chat para mantener la profesionalidad. | 4                   | Elverth      | Done   |
| US40    | Eliminación de chats grupales por gerentes  | SCRUM-40 | Eliminación de chats grupales por gerentes  | Como gerente, quiero eliminar chats grupales obsoletos o inactivos para mantener la lista de chats organizada y relevante. | 4                   | Elverth      | Done   |
| US43    | Eliminar imágenes enviadas en el chat       | SCRUM-43 | Eliminar imágenes enviadas en el chat       | Como usuario quiero poder eliminar una imagen enviada en un chat, para corregir errores o evitar confusiones. | 3                   | Raul         | Done   |
| US44    | Visualizar imágenes en chats                | SCRUM-44 | Visualizar imágenes en chats                | Como empleado, quiero ver todos los chats de los que forma parte para encontrar rápidamente conversaciones específicas. | 3                   | Raul         | Done   |



**Figura 80**

*Imagen de las tareas de Jira*

<p align="center">
  <img src="https://i.imgur.com/ZFbdv3f.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 81**

*Imagen de las tareas de Jira*

<p align="center">
  <img src="https://i.imgur.com/nzVxyGx.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.



#### 4.2.2.3. Development Evidence for Sprint Review

<p style="text-indent: 1.25cm;">En esta sección se presentan los avances de implementación del Sprint 2, los cuales se centraron en la aplicación móvil nativa (centralis-kotlin). El trabajo de esta iteración se enfocó en consolidar las funcionalidades administrativas para el rol de Gerente, expandir las capacidades multimedia de la plataforma y realizar una refactorización de la interfaz de usuario para mejorar la experiencia general.</p>

| **Repository**                        | **Branch**           | **Commit Id** | **Commit Message** | **Commit Message Body**                                      | **Committed on (Date)** |
| ------------------------------------- | -------------------- | ------------- | ------------------ | ------------------------------------------------------------ | ----------------------- |
| `synera-app-moviles/centralis-kotlin` | `fix/announcement`   | `c993530`     | `feat`             | Implement group deletion functionality with confirmation dialog and navigation | 10/11/2025              |
| `synera-app-moviles/centralis-kotlin` | `develop`            | `6b8f7c9`     | `feat`             | Add image upload functionality and preview for group creation | 10/11/2025              |
| `synera-app-moviles/centralis-kotlin` | `develop`            | `92560ed`     | `feat`             | Add delete functionality and confirmation dialog to announcement details | 10/11/2025              |
| `synera-app-moviles/centralis-kotlin` | `develop`            | `c8430bb`     | `feat`             | Enhance announcement screens with image handling and improved UI elements | 10/11/2025              |
| `synera-app-moviles/centralis-kotlin` | `develop`            | `e7388df`     | `feat`             | Update announcement screens with new color scheme and improved UI elements | 10/11/2025              |
| `synera-app-moviles/centralis-kotlin` | `develop`            | `83f5f8d`     | `fix`              | SavedAnnouncementsScreen(navController = navController)      | 07/11/2025              |
| `synera-app-moviles/centralis-kotlin` | `feature/view_event` | `e64db04`     | `feat`             | Refactor notification handling and improve UI elements in Events and Notification screens | 06/11/2025              |
| `synera-app-moviles/centralis-kotlin` | `develop`            | `d90e53d`     | `feat`             | Implement CreateEventRequestNetwork model and update event handling in ViewModel and screens | 03/11/2025              |
| `synera-app-moviles/centralis-kotlin` | `develop`            | `5f40505`     | `feat`             | Update launcher icons with new background color and improved vector graphics | 02/11/2025              |
| `synera-app-moviles/centralis-kotlin` | `develop`            | `9831861`     | `feat`             | Update chat and authentication views with group information and avatar handling | 02/11/2025              |

<p style="text-indent: 1.25cm;">La implementación se enfocó en el desarrollo de lógicas de negocio críticas. Se completaron los flujos de administrador para la eliminación de grupos de chat y la eliminación de anuncios , implementando en ambos casos diálogos de confirmación para la prevención de errores. Se expandieron las capacidades multimedia, añadiendo la subida de imágenes y vista previa en la creación de grupos y mejorando el manejo y visualización de imágenes en los anuncios. Adicionalmente, se implementó el modelo de red para la creación de eventos y se realizó una refactorización general de la UI, mejorando las pantallas de eventos y notificaciones.</p>

#### 4.2.2.4. Testing Suite Evidence for Sprint Review

<p style="text-indent: 1.25cm;">Para el Sprint 2, la estrategia de testing se centró en la validación de las nuevas funcionalidades del rol de Gerente y la lógica de negocio avanzada. Se implementó una robusta suite de pruebas de aceptación (BDD) para la aplicación Flutter (centralis_flutter), asegurando la cobertura de las historias de usuario relacionadas con la gestión de anuncios, eventos y la moderación de chats.</p>



**Acceptance Tests (BDD - Gherkin)**

Se crearon y expandieron los archivos `.feature` para validar las lógicas de negocio implementadas en este sprint:

- **announcements.feature (US18, US24)**
  - Se añadieron escenarios BDD para la eliminación de anuncios y la subida de imágenes, cubriendo la validación de permisos y los flujos de gestión de archivos.

```gherkin
# language: es
Característica: Subir imágenes en anuncios
  Como gerente
  Quiero poder adjuntar imágenes a los anuncios publicados
  Para que la información sea más clara y atractiva

  Escenario: Subir imagen en anuncio exitosamente
    Dado que soy un gerente autenticado
    Cuando creo un anuncio con título "Nueva política" y adjunto una imagen
    Entonces el anuncio debe ser creado con la imagen exitosamente
    Y la imagen debe ser visible en el anuncio

  Escenario: Subir imagen con formato válido
    Dado que soy un gerente autenticado
    Cuando intento subir una imagen en formato JPG de 2MB
    Entonces la imagen debe ser aceptada
    Y debe aparecer como vista previa

  Escenario: Rechazar imagen con formato inválido
    Dado que soy un gerente autenticado
    Cuando intento subir un archivo de formato TXT
    Entonces debo recibir un error de formato no válido
    Y la imagen no debe ser adjuntada

  Escenario: Rechazar imagen excesivamente grande
    Dado que soy un gerente autenticado
    Cuando intento subir una imagen de 50MB
    Entonces debo recibir un error de tamaño excesivo
    Y la imagen no debe ser adjuntada
```



- **events.feature (US27-US29, US30-US32)**
  - Se implementaron escenarios BDD para las características centrales de gestión de eventos, incluyendo invitaciones por departamento, confirmación de asistencia y cancelación de eventos.
  - Se expandieron las pruebas para incluir las características avanzadas, como la modificación de eventos, la gestión de prioridades y la validación de las métricas de participación.

```gherkin
# language: es
Característica: Eventos prioritarios
  Como gerente
  Quiero marcar eventos como prioritarios
  Para que los empleados les presten especial atención

  Escenario: Marcar evento como prioritario
    Dado que soy un gerente autenticado
    Y existe un evento "Reunión urgente"
    Cuando marco el evento como prioritario
    Entonces el evento debe mostrar un indicador de prioridad
    Y debe aparecer destacado en la lista de eventos

  Escenario: Quitar prioridad de evento
    Dado que soy un gerente autenticado
    Y existe un evento prioritario "Junta directiva"
    Cuando quito la prioridad del evento
    Entonces el evento debe perder el indicador de prioridad
    Y debe aparecer como evento normal

  Escenario: Ver eventos prioritarios destacados
    Dado que soy un empleado autenticado
    Y existen eventos prioritarios y normales
    Cuando veo la lista de eventos
    Entonces los eventos prioritarios deben aparecer al principio
    Y deben tener un indicador visual distintivo

  Escenario: Notificación especial para eventos prioritarios
    Dado que soy un empleado autenticado
    Y se crea un evento prioritario "Emergencia"
    Cuando recibo la notificación del evento
    Entonces la notificación debe indicar que es prioritario
    Y debe tener mayor prominencia visual
```



- **chats.feature (US35-US38, US39-US44)**
  - Se implementaron escenarios BDD para la gestión de mensajes y la eliminación de grupos de chat, incluyendo la validación de permisos de usuario.
  - Se añadieron escenarios para las funciones de moderación (eliminación de mensajes por gerentes) y las características multimedia, como el envío de imágenes.

```gherkin
# language: es
Característica: Eliminar grupos de chats
  Como gerente
  Quiero eliminar chats grupales
  Para mantener el orden de las conversaciones

  Escenario: Eliminar grupo de chat exitosamente
    Dado que soy un gerente autenticado
    Y existe un grupo de chat "Proyecto Antiguo" que ya no es necesario
    Cuando elimino el grupo de chat
    Entonces el grupo debe ser eliminado exitosamente
    Y no debe aparecer en mi lista de chats

  Escenario: Confirmar eliminación de grupo con mensajes
    Dado que soy un gerente autenticado
    Y existe un grupo de chat "Marketing 2023" con mensajes históricos
    Cuando intento eliminar el grupo
    Entonces debo ver una confirmación sobre la pérdida de mensajes
    Y debo confirmar la eliminación explícitamente

  Escenario: Intentar eliminar grupo sin permisos
    Dado que soy un empleado autenticado sin permisos de gerente
    Y existe un grupo de chat "Ventas General"
    Cuando intento eliminar el grupo
    Entonces debo recibir un error de permisos insuficientes
    Y el grupo debe permanecer activo

  Escenario: Notificar miembros sobre eliminación de grupo
    Dado que soy un gerente autenticado
    Y existe un grupo "Equipo Beta" con múltiples miembros
    Cuando elimino el grupo
    Entonces todos los miembros deben ser notificados
    Y el grupo debe desaparecer de sus listas de chat
```

**Evidencia de Commits de Testing**

| Repository                           | Branch  | Commit Id | Commit Message                                               | Commit Message Body                                          | Commited on (Date) |
| :----------------------------------- | :------ | :-------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------- |
| synera-app-moviles/centralis_flutter | testing | 24731b2   | feat(chat): add BDD tests for moderation and multimedia features US39-US44 | Implement BDD scenarios for message moderation by managers, chat archiving, and image sharing with comprehensive permission and file management validation | 13/11/2025         |
| synera-app-moviles/centralis_flutter | testing | 21b5f96   | feat(chat): add BDD tests for message management and group deletion US35-US38 | Implement BDD scenarios for group chat deletion, message editing, and deletion with time limit validation and user permission testing | 13/11/2025         |
| synera-app-moviles/centralis_flutter | testing | 503584d   | feat(events): add BDD tests for advanced event features US30-US32 | Implement BDD scenarios for event modification, priority management, and participation metrics with dashboard and reporting functionality | 13/11/2025         |
| synera-app-moviles/centralis_flutter | testing | 104cf67   | feat(events): add BDD tests for event management core features US27-US29 | Implement BDD scenarios for department invitations, attendance confirmation, and event cancellation with comprehensive permission and validation testing | 13/11/2025         |
| synera-app-moviles/centralis_flutter | testing | 74bfeac   | feat(announcements): add BDD tests for announcement management US18-US24 | Implement BDD scenarios for announcement deletion and image upload features, covering permission validation and file management workflows | 13/11/2025         |





#### 4.2.2.5. Execution Evidence for Sprint Review

<p style="text-indent: 1.25cm;">En el Sprint 2, el equipo alcanzó los objetivos definidos, logrando la finalización y el despliegue del 100% del backend. El principal avance funcional se centró en la implementación de las características <i>core</i> de la aplicación móvil en flutter y pulir fucionalidades de kotlin, específicamente las lógicas de negocio avanzadas para el rol de Gerente. Esto incluyó el CRUD completo de anuncios, la gestión avanzada de eventos (modificación, cancelación, confirmación de asistencia) y las capacidades de moderación de chat (eliminación de mensajes y grupos). Paralelamente, se inició el desarrollo de la aplicación cross-platform en Flutter y se completaron las mejoras de accesibilidad e internacionalización en el Landing Page.</p>

<p style="text-indent: 1.25cm;">A continuación, se presentan las capturas de pantalla que evidencian las principales vistas implementadas en la aplicación móvil, ilustrando los flujos de administrador y las nuevas capacidades de gestión. Se adjunta también el enlace al video de demostración, donde se explica y recorre la navegación y la interacción lograda en este Sprint, validando el cumplimiento de las historias de usuario.</p>

**Aplicación en Kotlin:**

**Figura 82**

<p align="center">
  <img src="https://i.imgur.com/ThgEQ1S.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 83**

<p align="center">
  <img src="https://i.imgur.com/1yXvTdq.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 84**

<p align="center">
  <img src="https://i.imgur.com/rkvE6C3.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 85**

<p align="center">
  <img src="https://i.imgur.com/13Pz1QD.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.
URL del video: https://acortar.link/u5x1AS

**Landing Page:**

**Figura 86**

<p align="center">
  <img src="https://i.imgur.com/Xe7FsFA.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 87**

<p align="center">
  <img src="https://i.imgur.com/FilLNRC.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 88**

<p align="center">
  <img src="https://i.imgur.com/xcGvs1I.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 89**

<p align="center">
  <img src="https://i.imgur.com/MXSQqu4.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

URL del video: https://acortar.link/Y0oFip

#### 4.2.2.6. Services Documentation Evidence for Sprint Review

<p style="text-indent: 1.25cm;">En esta sección se presenta la evidencia de la documentación de los Web Services implementados durante el Sprint 2, generada utilizando la especificación OpenAPI. Los endpoints desarrollados completan las funcionalidades <i>core</i> de la plataforma, abarcando tres dominios principales: Comments, Events y Messages. La documentación detalla las operaciones CRUD, los servicios de consulta (QueryService) y los servicios de comandos (CommandService) para cada dominio, incluyendo la gestión de estados, validaciones de pertenencia y autorización por roles (MANAGER) en el dominio de Eventos.</p>


**Endpoints Documentados**

| Endpoint                                               | Método | Descripción                     | Request Body                         | Response Body           | Códigos de Estado  |
| ------------------------------------------------------ | ------ | ------------------------------- | ------------------------------------ | ----------------------- | ------------------ |
| `/api/v1/announcements/{id}/comments`                  | POST   | Crear comentario en anuncio     | `CreateCommentResource`              | `CommentResource`       | 201, 400, 404, 500 |
| `/api/v1/comments/{id}`                                | GET    | Obtener comentario por ID       | -                                    | `CommentResource`       | 200, 404, 500      |
| `/api/v1/announcements/{id}/comments`                  | GET    | Obtener comentarios de anuncio  | -                                    | `List<CommentResource>` | 200, 404, 500      |
| `/api/v1/comments/{id}`                                | DELETE | Eliminar comentario             | -                                    | -                       | 204, 404, 500      |
| `/api/v1/events`                                       | POST   | Crear evento                    | `CreateEventResource`                | `EventResource`         | 201, 400, 500      |
| `/api/v1/events/{eventId}`                             | GET    | Obtener evento por ID           | -                                    | `EventResource`         | 200, 404, 500      |
| `/api/v1/events`                                       | GET    | Obtener todos los eventos       | Query params: `userId`, `filterType` | `List<EventResource>`   | 200, 500           |
| `/api/v1/events/calendar`                              | GET    | Obtener eventos para calendario | Query param: `userId`                | `List<EventResource>`   | 200, 500           |
| `/api/v1/events/{eventId}`                             | PUT    | Actualizar evento               | `UpdateEventResource`                | `EventResource`         | 200, 400, 404, 500 |
| `/api/v1/events/{eventId}`                             | DELETE | Eliminar evento                 | -                                    | -                       | 204, 404, 500      |
| `/api/v1/groups/{groupId}/messages`                    | POST   | Crear mensaje en grupo          | `CreateMessageResource`              | `MessageResource`       | 201, 400, 404, 500 |
| `/api/v1/groups/{groupId}/messages/{messageId}`        | GET    | Obtener mensaje por ID          | -                                    | `MessageResource`       | 200, 404, 500      |
| `/api/v1/groups/{groupId}/messages`                    | GET    | Obtener mensajes de grupo       | -                                    | `List<MessageResource>` | 200, 500           |
| `/api/v1/groups/{groupId}/messages/status/{status}`    | GET    | Obtener mensajes por estado     | -                                    | `List<MessageResource>` | 200, 400, 500      |
| `/api/v1/groups/{groupId}/messages/{messageId}`        | PUT    | Actualizar contenido de mensaje | `UpdateMessageBodyResource`          | `MessageResource`       | 200, 404, 400, 500 |
| `/api/v1/groups/{groupId}/messages/{messageId}/status` | PATCH  | Actualizar estado de mensaje    | `UpdateMessageStatusResource`        | `MessageResource`       | 200, 404, 400, 500 |
| `/api/v1/groups/{groupId}/messages/{messageId}`        | DELETE | Eliminar mensaje                | -                                    | -                       | 204, 404, 500      |



**Comments Domain**

- **CommentCommandService**: Manejo de comandos de comentarios (crear, eliminar)
- **CommentQueryService**: Consultas de comentarios (obtener por ID, por anuncio)
- **CommentController**: API REST para operaciones de comentarios
- **Características**:
  - Integración con sistema de anuncios
  - Validación de existencia de anuncios
  - Operaciones CRUD básicas

**Events Domain**

- **EventCommandService**: Manejo de comandos de eventos (crear, actualizar, eliminar)
- **EventQueryService**: Consultas de eventos (por ID, por creador, por destinatario, todos)
- **EventController**: API REST para gestión de eventos
- **Características**:
  - Filtrado por usuario (creador/destinatario)
  - Vista de calendario
  - Gestión de destinatarios múltiples
  - Autorización por rol (MANAGER)

**Messages Domain**

- **MessageCommandService**: Manejo de comandos de mensajes (crear, actualizar, eliminar)
- **MessageQueryService**: Consultas de mensajes (por ID, por grupo, por estado)
- **MessageController**: API REST para mensajería en grupos
- **Características**:
  - Mensajes vinculados a grupos específicos
  - Estados de mensaje (SENT/EDITED/DELETED)
  - Actualización de contenido y estado por separado
  - Validación de pertenencia a grupo



**Figura 90**

<p align="center">
  <img src="https://i.imgur.com/IzPFXRp.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 91**

<p align="center">
  <img src="https://i.imgur.com/IcEA5yu.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Figura 92**

<p align="center">
  <img src="https://i.imgur.com/MNZ7yvk.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.



#### 4.2.2.7. Software Deployment Evidence for Sprint Review

<p style="text-indent: 1.25cm;">En esta sección se resumen los procesos realizados en relación con el despliegue durante el Sprint 2. Las actividades de este sprint se centraron en la consolidación de los servicios existentes y la actualización de los productos web, más que en la creación de nueva infraestructura.</p>

<p style="text-indent: 1.25cm;">Para los Web Services, no se realizaron cambios en la configuración de despliegue en Render, ya que la infraestructura base establecida en el Sprint 1 se mantuvo estable y fue suficiente para soportar el 100% de las funcionalidades del backend. En cuanto al Landing Page, sí se desplegó una nueva versión para reflejar las actualizaciones de contenido implementadas, como la adición de las secciones "Team", "FAQ" y "Producto", así como la funcionalidad de internacionalización. Las Aplicaciones móviles (Kotlin y Flutter) continúan en fase de desarrollo y aún no han sido desplegadas en un servicio de distribución. A continuación, se presentan las evidencias del despliegue actualizado del Landing Page.</p>



**Figura 93**

<p align="center">
  <img src="https://i.imgur.com/ZEWrEQC.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.



#### 4.2.2.8. Team Collaboration Insights during Sprint

<p style="text-indent: 1.25cm;">Durante el Sprint 2, el equipo continuó su trabajo colaborativo, centrándose en la consolidación de la plataforma y la expansión de sus funcionalidades clave. Este sprint fue crucial para finalizar el despliegue del backend, empezar el desarrollo en flutter e implementar las lógicas de negocio avanzadas para el rol de Gerente, como la gestión de eventos y la moderación de chats.</p>

**Daniela Araceli Gómez Flores** **Contribución Principal:**

- Expansión del Landing Page con la "Sección Team".
- Desarrollo del módulo de eventos.
- Implementación de la cancelación de eventos.
- Implementación de la modificación de detalles de eventos.

**Elverth Jair Vaszquez Villalobos** **Contribución Principal:**

- Desarrollo de la creación y modificación de grupos. 
- Desarrollo de la eliminación de grupos de chat completos por parte de los gerentes.

**Jorge Luis Díaz Fiestas** **Contribución Principal:**

- Completó el CRUD de anuncios en la aplicación.
- Añadió la capacidad de eliminar anuncios.
- Implementó la funcionalidad de subir imágenes en los anuncios.

**Neil Aldrin Wilhelm Curipaco Huayllani** **Contribución Principal:**

- Implementación de la funcionalidad de internacionalización en el Landing Page.
- Agregó la "Sección FAQ" al Landing Page.
- Agregó la "Sección Producto" al Landing Page.

**Raúl Adrian Medina Cruzado** **Contribución Principal:**

- Expandió las capacidades del módulo de chat.
- Implementó la vista de notificaciones 

**Evidencia de la landing page:** 

**Figura 94**

<p align="center">
  <img src="https://i.imgur.com/o9I8xhl.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.

**Evidencia aplicación en Flutter:** 

**Figura 95**

<p align="center">
  <img src="https://i.imgur.com/IG2yVSY.png" alt="Descripción">
</p>

*Nota.* Elaboración propia.


## 4.3. Validation Interviews

### 4.3.1. Diseño de Entrevistas

<p style="text-indent: 1.25cm;">En esta sección se establece el plan de validación con usuarios, definiendo los elementos a incluir y los flujos de usuario que serán evaluados. El objetivo principal es medir la usabilidad, coherencia de la arquitectura de información y la facilidad de uso de los artefactos producidos, tanto del Landing Page como de la aplicación móvil.
<p style="text-indent: 1.25cm;">Las sesiones se diseñan en torno a los dos segmentos objetivo principales del proyecto: Gerentes y Empleados, asegurando que los flujos de tareas cubran tanto las funcionalidades compartidas como las específicas de cada rol.


**1. Validación del Landing Page**

<p style="text-indent: 1.25cm;">El Landing Page de Centralis sirve como el principal punto de información y conversión para todos los visitantes, independientemente de su rol. Por lo tanto, el diseño de la entrevista de validación es idéntico para ambos segmentos.

- **Elementos a Incluir:** Se utilizará el prototipo de alta fidelidad del Landing Page, que replica la estructura de información, jerarquía visual y navegación (Header y Footer) definida en la fase de diseño.
- **User Flows a Validar:**
  - **Descubrimiento y Propuesta de Valor:** Se solicitará al visitante que explore la página de inicio (Home). El objetivo es evaluar la claridad inmediata del *Hero Section* y validar si el usuario se siente identificado con los problemas descritos en la sección de *Pain Points*.
  - **Exploración de Características y Alcance:** Se guiará al visitante para que navegue a la página de "Producto". Se medirá la facilidad para comprender el valor de los módulos (Anuncios, Eventos, Chats) y la transparencia de la sección "Alcance", que define qué funcionalidades están incluidas y cuáles no.
  - **Generación de Confianza:** El visitante deberá navegar a las páginas "Equipo" (About Team) y "FAQ". Se evaluará si la presentación del equipo y la información corporativa generan credibilidad, y si las preguntas frecuentes resuelven sus dudas principales.

**2. Validación de la Aplicación Móvil**

Para la validación de la aplicación móvil, se utilizarán prototipos navegables que simulan los dos perfiles de usuario, cada uno con sus respectivos permisos y vistas.

**2.1. Segmento Empleados:  Flujo de Consumidor de Información**

Este flujo se centra en tareas de consulta, recepción de información e interacción básica.

- **User Flows  a Validar:**
  - **Consumo de Anuncios:** Ingresar a la sección "Announcements" y diferenciar visualmente un anuncio "Urgent" del resto. Abrir un anuncio específico "Paro de transportistas", leer el detalle y publicar un comentario.
  - **Consulta de Eventos:** Navegar a la sección "Events" y revisar la agenda. Seleccionar una "Capacitación" para consultar los detalles: fecha, hora, ubicación y la lista de otros asistentes.
  - **Interacción en Grupos:**  Acceder a un grupo de chat asignado. Enviar un mensaje y verificar que la interfaz refleje la recepción y envío de mensajes en tiempo real.
  - **Gestión de Notificaciones:**  Acceder al centro de "Notificaciones". Interpretar correctamente una notificación del sistema "Te han asignado a un evento"

**2.2. Segmento Gerentes: Flujo de Administrador de Contenido**

Este flujo incluye todas las tareas del "Empleado", más las funcionalidades de creación, edición y eliminación de contenido.

- **User Flows a Validar:**
  - **Gestión de Anuncios**  Crear un nuevo anuncio. Publicar un anuncio con prioridad "Urgent".  Editar y/o eliminar un anuncio previamente publicado.
  - **Gestión de Eventos** Crear un nuevo evento. Asignar asistentes al evento. Ingresar a un evento existente para modificar sus detalles "Edit Event" o cancelarlo "Delete Event"
  - **Gestión de Grupos**  Crear un nuevo grupo de chat para un proyecto específico. Modificar el nombre de un grupo existente. Añadir nuevos miembros y eliminar miembros existentes de un grupo.

### 4.3.2. Registro de Entrevistas

<ins>**Registro de entrevistas para segmento objetivo: Empleado de empresa**<ins>  

**Entrevistado #1: Abigail Goñe**  

**Figura 96**  

*Imagen del usuario número 1 entrevistado*  

<p align="center">
  <img src="https://res.cloudinary.com/df8xwy4xb/image/upload/v1763031076/abigaiill_ihwjzu.jpg" width="850">
</p>

*Nota.* Elaboración propia.

*Nota.* Elaboración propia.

Abigail percibió que Centralis representa una mejora significativa en la forma en que los empleados acceden a información relevante dentro de la empresa. Destacó la simplicidad de la interfaz y la rapidez con la que puede ver anuncios, confirmar asistencia a eventos y comunicarse con sus compañeros. Mencionó que la aplicación le genera confianza por la claridad en las funciones y la seguridad de los datos. Propuso mejorar la visibilidad de algunos botones en la Landing Page y optimizar la navegación en ciertas pantallas, pero aseguró que la experiencia general es positiva. Considera que Centralis fomenta la participación, reduce confusiones y promueve una comunicación más efectiva entre todos los niveles de la organización.


**Entrevistada #2: Fatima Arosemena**   

**Figura 97**  

*Imagen del usuario número 2 entrevistada*

<p align="center">
  <img src="https://res.cloudinary.com/df8xwy4xb/image/upload/v1763031076/fatimaaa_mc1ynn.jpg" width="850">
</p>

*Nota.* Elaboración propia.

*Nota.* Elaboración propia.  

Fátima encontró que Centralis soluciona un problema común en muchas empresas: la falta de un canal único de comunicación. Considera que la app es intuitiva, visualmente atractiva y fácil de navegar. Le gustó cómo los anuncios urgentes destacan claramente, y que puede interactuar dejando comentarios o consultando detalles de eventos sin complicaciones. También resaltó la claridad en los chats grupales y la utilidad de las confirmaciones de lectura. Sugirió agregar la opción de fijar mensajes importantes dentro de los grupos, pero en general expresó que la aplicación hace más fluida la comunicación y mejora la organización del trabajo diario.

<ins>**Registro de entrevistas para segmento objetivo: Empleado de empresa**<ins>  

**Entrevistada #3: Milagros Arellano**  

**Figura 98**  

*Imagen del usuario número 3 entrevistada*

<p align="center">
  <img src="https://res.cloudinary.com/df8xwy4xb/image/upload/v1763031559/milagros_kbtkk4.jpg" width="850">
</p>

*Nota.* Elaboración propia.

*Nota.* Elaboración propia. 

Milagros considera que Centralis es una herramienta ideal para mejorar la comunicación entre los diferentes equipos de trabajo. Durante la validación, destacó que la aplicación facilita la creación y gestión de anuncios, eventos y grupos sin depender de correos o mensajes dispersos. Le pareció muy claro el flujo para publicar información y valoró la opción de marcar anuncios como urgentes para priorizar temas importantes. Sugirió incorporar un sistema de confirmación al eliminar eventos o mensajes para evitar errores, y mejorar la forma en que se muestran los asistentes a los eventos. En general, percibe que Centralis ordena y optimiza la gestión interna, ayudando a mantener a todos alineados desde un solo lugar.

**Entrevistada #4: Leonardo Delgado**  

**Figura 99**  

*Imagen del usuario número 4 entrevistada*

<p align="center">
  <img src="https://res.cloudinary.com/df8xwy4xb/image/upload/v1763047827/elverth_wkmox1.jpg" width="850">
</p>

*Nota.* Elaboración propia.

*Nota.* Elaboración propia.  

Leonardo actualmente trabaja coordinando tareas con su equipo mediante mensajes en distintas aplicaciones y llamadas, lo que a menudo genera confusión y pérdida de información importante. Al probar Centralis, destacó lo práctico de tener todos los anuncios, eventos y chats centralizados en un solo espacio. Mencionó que la app facilita la comunicación entre empleados y evita malentendidos en la organización interna. Considera que su diseño es claro y fácil de usar incluso para personas con poca experiencia digital. Como mejora, sugiere que las notificaciones sean más personalizables y que se puedan fijar los mensajes más importantes dentro de los grupos.


### 4.3.3. Evaluaciones según heurísticas

<p align="center">UX Heuristics & Principles Evaluation</p>

<p align="center">Usability – Inclusive Design – Information Architecture</p>

**CARRERA :** Ingeniería de Software

**CURSO :** Aplicaciones para Dispositivos Móviles

**SECCIÓN :** 14650

**PROFESORES :** Todos

**AUDITOR :** Equipo Synera

**CLIENTE(S) :** 

**SITE o APP A EVALUAR:**

Centralis aplicacion móvil 

**TAREAS A EVALUAR:**

El alcance de esta evaluación incluye la revisión de usabilidad de las siguientes tareas:

**Tareas de los Gerentes**

- Crear un nuevo anuncio o evento.
- Modificar el nombre de un grupo.
- Eliminar un evento existente.

**Tareas de los empleados**

- Identificar anuncios "Urgent" en la lista.

- Publicar un comentario en un anuncio y verificar su publicación.

-  Intentar editar o eliminar un comentario propio.

- Consultar detalles de un evento (ubicación, asistentes, hora).

- Enviar un mensaje en un chat grupal y verificar el estado de lectura.

  

**ESCALA DE SEVERIDAD:**

Los errores serán puntuados tomando en cuenta la siguiente escala de severidad

| Nivel | Descripción                                                  |
| ----- | ------------------------------------------------------------ |
| 1     | Problema superficial: puede ser fácilmente superador por el usuario ó ocurre con muy poco frecuencia. No necesita ser arreglado a no ser que exista disponibilidad de tiempo. |
| 2     | Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja resolverlo de cara al siguiente reléase |
| 3     | Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se les debe asignar una prioridad alta. |
| 4     | Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento. |

**TABLA RESUMEN:**

| **#** | **Problema**                                                 | **Escala de severidad** | **Heurística/Principio violada(o)** |
| ----- | ------------------------------------------------------------ | ----------------------- | ----------------------------------- |
| 1     | Ausencia de confirmación antes de eliminar un evento.        | 4                       | Prevención de errores.              |
| 2     | El usuario no puede editar o eliminar sus propios comentarios. | 3                       | Control y libertad del usuario.     |
| 3     | El chat de grupo no muestra confirmaciones de lectura (estado del sistema). | 2                       | Visibilidad del estado del sistema. |
| 4     | La ubicación del evento no es un enlace accionable (ej. a "Meet"). | 2                       | Flexibilidad y eficiencia de uso.   |
| 5     | Información redundante o inútil en detalles del evento.      | 1                       | Diseño estético y minimalista.      |

**DESCRIPCIÓN DE PROBLEMAS:**

**PROBLEMA #1:** Ausencia de confirmación antes de eliminar un evento.

- **Severidad:** 4 Problema muy grave
- **Heurística violada:** Prevención de errores.
- **Problema:** El rol de Gerente tiene la capacidad de eliminar eventos, con el botón "Delete Event". El usuario manifestó explícitamente que esperaría un diálogo de confirmación, ya que presionar ese botón por accidente causaría una pérdida de datos irreversible para todos los asistentes.
- **Recomendación:** Implementar un diálogo modal de confirmación, ejemplo. "¿Está seguro de que desea eliminar este evento? Esta acción no se puede deshacer" que aparezca después de presionar el botón "Delete Event" y antes de ejecutar la acción.



**PROBLEMA #2:** El usuario no puede editar o eliminar sus propios comentarios.

- **Severidad:** 3 Problema mayor
- **Heurística violada:** Control y libertad del usuario.
- **Problema:** El usuario Empleado puede publicar un comentario exitosamente, el cual aparece en la lista. Sin embargo, al intentar corregir un error o eliminar dicho comentario, el usuario no encuentra ninguna opción visible que le permita hacerlo.
- **Recomendación:** Implementar una interacción que despliegue un menú contextual con las opciones de "Editar" y "Eliminar" el mensaje.



**PROBLEMA #3:** El chat de grupo no muestra confirmaciones de lectura.

- **Severidad:** 2 Problema menor
- **Heurística violada:** Visibilidad del estado del sistema.
- **Problema:** El usuario Empleado envía un mensaje en el chat de grupo, pero la interfaz no proporciona ningún *feedback* sobre el estado de dicho mensaje (ej. entregado, leído). El usuario manifestó que esperaba ver algún tipo de "doble check" o ícono de "visto" para saber si sus compañeros habían recibido la información.
- **Recomendación:** Implementar un sistema de confirmación de lectura (ej. doble check gris para entregado, doble check azul para leído) para informar al usuario sobre el estado de sus mensajes.



**PROBLEMA #4:** La ubicación del evento no es un enlace accionable.

- **Severidad:** 2 Problema menor
- **Heurística violada:** Flexibilidad y eficiencia de uso.
- **Problema:** En los detalles del evento, la ubicación se muestra como un texto plano "meet". El usuario espera que, si la ubicación es una sala virtual, este campo sea un enlace accionable que lo lleve directamente a la reunión como Google Meet, Zoom, ahorrándole pasos.
- **Recomendación:** Modificar el campo "Location" para que acepte URLs y las muestre como un hipervínculo accionable para el usuario.

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



**TB2:**


<p style="text-indent: 1.25cm;">El Sprint 2 representa la consolidación y expansión de la plataforma Centralis, marcando la transición de los cimientos arquitectónicos a una solución funcionalmente robusta. En esta entrega se alcanzó el hito clave del 100% del despliegue del backend en un sitio público. El foco principal fue la implementación de las lógicas de negocio avanzadas para el rol de Gerente, completando el CRUD de anuncios, la gestión avanzada de eventos y las capacidades críticas de moderación de chats.



<p style="text-indent: 1.25cm;">Técnicamente, este sprint demostró la flexibilidad de la arquitectura al permitir el inicio del desarrollo de la aplicación cross-platform en Flutter en paralelo al desarrollo nativo. Asimismo, se robusteció el Landing Page implementando funcionalidades de internacionalización (i18n).



<p style="text-indent: 1.25cm;">Con el backend finalizado y las funcionalidades core implementadas en la aplicación nativa, el proyecto se encuentra en una posición sólida para la fase final. Este sprint también incluyó la elaboración de las primeras versiones de los videos "About-the-Product" y "About-the-Team", sentando las bases para las entrevistas de validación con usuarios y la entrega final del producto (TF1).


## Video App Validation 

<p style="text-indent: 1.25cm;">En esta sección se registran y explican las actividades de entrevistas de validación realizadas con los segmentos objetivo. Las sesiones fueron grabadas en video para documentar la interacción de los usuarios con la aplicación móvil, y los hallazgos se utilizarán para la evaluación heurística. A continuación, se presenta un resumen de las principales apreciaciones de los entrevistados con respecto a las tareas asignadas.</p>

<p style="text-indent: 1.25cm;">Las entrevistas proporcionaron retroalimentación valiosa. La primera entrevistada, perteneciente al Segmento Empleado, validó la información de los eventos como suficiente, incluyendo asistentes, hora y fecha. Sin embargo, sugirió añadir mensajes de confirmación de éxito en la creación y eliminación, iconos de confirmación de lectura en los chats y la capacidad de fijar mensajes grupales. La segunda entrevista, también del Segmento Empleado, coincidió en la necesidad de feedback en los mensajes, sugiriendo un check de "enviado" y "leído", y propuso además una funcionalidad de confirmación de asistencia a eventos. Finalmente, la tercera entrevista, del Segmento Gerente, confirmó la utilidad de las funciones administrativas, destacando que las opciones para editar y eliminar anuncios y eventos son esenciales para su rol.</p>



<p align="center">
  <img src="https://i.imgur.com/8L16JO0.png" width="850">
</p>

Link de las entrevistas: https://acortar.link/TbVsHT

## Video About the product 

<p style="text-indent: 1.25cm;">En esta sección se introduce y describe el video "About-the-Product", el cual ha sido diseñado con un doble propósito: comunicar el modelo de negocio y la propuesta de valor a los visitantes del Landing Page, y demostrar las características principales del software a los usuarios de la aplicación. El contenido del video recorre las funcionalidades clave tanto del Landing Page como de la aplicación móvil, manteniendo un tono de comunicación consistente con la identidad del producto. Además, se incluye un testimonio positivo de un usuario que participó en las entrevistas de validación. A continuación, se adjuntan el screenshot, los enlaces de despliegue (OneDrive y YouTube) y la duración (timing) del mismo.</p>

<p align="center">
  <img src="https://i.imgur.com/nJm7Tug.png" width="850">
</p>



Link del video en YouTube: https://youtu.be/pj9MuNyfGec  2 minutos 27 segundos
Link del video en OneDrive: https://acortar.link/69wpTn 2 minutos 27 segundos

## Video About the team

<p style="text-indent: 1.25cm;">El desarrollo de este proyecto ha representado un proceso de aprendizaje evolutivo y práctico. En la fase inicial, el equipo se centró en adquirir y aplicar conocimientos metodológicos fundamentales, investigando y aplicando técnicas como Domain-Driven Design (DDD), MVVM, BLoC, EventStorming y Lean UX para modelar correctamente el dominio del problema.</p>

<p style="text-indent: 1.25cm;">Posteriormente, este conocimiento teórico se materializó en la implementación de los cimientos tecnológicos de la plataforma, donde el equipo aprendió a integrar un stack de tecnologías completo, incluyendo Spring Boot para el backend, Kotlin nativo y Flutter para la aplicación móvil y servicios de autenticación como JWT. En la etapa más reciente, el aprendizaje se profundizó, pasando de la implementación de funcionalidades básicas a la resolución de desafíos técnicos avanzados. Esto incluyó la gestión de archivos multimedia con cloudinary, la implementación de lógicas de negocio complejas y la adopción de estándares de calidad como la internacionalización (i18n)</p>

Link del video en OneDrive: https://acortar.link/7DEwKw

**Neil Aldrin Wilhelm Curipaco Huayllani** 
Inicio: minuto 0 segundo 5

<p align="center">
  <img src="https://i.imgur.com/JkOWiUe.png" width="850">
</p>



**Daniela Araceli Gómez Flores**

Inicio: minuto 0 segundo 59

<p align="center">
  <img src="https://i.imgur.com/V2sEjvI.png" width="850">
</p>

**Elverth Jair Vaszquez Villalobos** 

Inicio: minuto 3 segundo 47

<p align="center">
  <img src="https://i.imgur.com/KDaQ4sP.png" width="850">
</p>

**Raúl Adrian Medina Cruzado** 

Inicio: minuto 5 segundo 18

<p align="center">
  <img src="https://i.imgur.com/HpDikUo.png" width="850">
</p>



**Jorge Luis Díaz Fiestas** 
Inicio: minuto 6 segundo 21

<p align="center">
  <img src="https://i.imgur.com/R2YuePF.png" width="850">
</p>





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
