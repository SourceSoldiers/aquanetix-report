## 5.2. Landing Page, Services & Applications Implementation.
El desarrollo de la pagina principal, acoplamiento de servicios e implementación de las aplicaciones se consideran como pasos de alta importancia en lo que refiere a la elaboración del proyecto. Con el apoyo de estas etapas, permite al equipo tranformar conceptos simples en productos preparados para su uso. Esta fase nos ayuda a traducir los requisitos y especificaciones obtenidas a código con la finalidad de cumplir con las necesidades de nuestros segmentos objetivos.

### 5.2.1. Sprint 1
El primer sprint de nuestro proyecto posee una gran importancia en lo que refiere al proceso de desarrollo ágil. A lo largo de este periodo, se ha dado un enfoque con mayor énfasis en la implementación de las caracetericas fundamentales así como en las funcionalidades de mayor prioridad en nuestra planificación de inicio.

#### 5.2.1.1. Sprint Planning 1.

Para este sprint, la reunión de Sprint Planning nos permite evaluar nuestra velocidad previa y definir las nuevas metas técnicas del proyecto. En esta fase, el equipo selecciona las historias de usuario prioritarias del backlog, estima el esfuerzo necesario y asigna las tareas. El objetivo principal es mantener la alineación del equipo y garantizar que las nuevas funcionalidades operativas se integren de manera fluida, estableciendo un plan de trabajo claro.

| Campo / Sección | Detalle |
| :--- | :--- |
| Sprint # | Sprint 1 |
| Date | 2026-04-22 |
| Time | 9:00 PM |
| Location | Google meet |
| Prepared By | Castro Solorza, Nicolas Eduardo |
| Attendees (to planning meeting) | Pinedo Sánchez, Sebastián Martín / Castro Solorza, Nicolás Eduardo / Cochachi Chagua, Sebastián Josué / Cabrera Novoa, Leonardo Moisés |
| Sprint 1  Review Summary | Al ser el primer sprint del proyecto (Fase de Inicio), no hay un Review de entregables previos. Se revisaron los requisitos del Primer Entregable (TB1), estableciendo como prioridad el diseño de la arquitectura base, diseño de base de datos, además de los flujos de registro de empresas. |
| Sprint 1  Retrospective Summary | De igual manera al ser el inicio del proyecto, se establecieron las normas de trabajo del equipo: reuniones de seguimiento (Daily Stand-ups) mediante Meet, uso de herramientas ágiles para el control de tareas, sumado a la necesidad de mantener una comunicación constante para evitar bloqueos técnicos en el desarrollo del backend. |
| Sprint 1 Goal | Para este sprint se requiere el cumplimiento de los siguientes objetivos: Establecer la arquitectura base del backend, desplegar el esquema de la base de datos relacional, configurar el registro de clientes (Enterprise) junto con la seguridad (Login). La métrica de cumplimiento se basará en el proceso de cómo nuestro "Board de Jira" luzca con el paso del tiempo, nuestro resultado final debe de mostrar todas las tareas en el lado derecho de la herramienta, ubicándolos en la columna "Terminado". |
| Sprint 1 Velocity | Para este sprint se han elegido 5 User Stories con estimaciones basadas en la serie de Fibonacci. |
| Sum of Story Points | 26 |

#### 5.2.1.2 Aspect Leaders and Collaborators

En esta sección se presenta la matriz de liderazgo y colaboración (LACX), donde se definen los roles de cada integrante del equipo en los distintos aspectos considerados dentro del Sprint.

Los aspectos seleccionados corresponden a las principales áreas del proyecto Aquanetix, incluyendo diseño UX/UI, desarrollo de la landing page, documentación y modelado del sistema.

| Team Member (Last Name, First Name) | GitHub Username | UX/UI Design | Landing Page | Documentation | Modeling |
|------------------------------------|----------------|-------------|-------------|--------------|----------|
| Bojórquez Bustinza, Renzo Alejandro | DeterminedSoul7 | C | C | C | L |
| Cabrera Novoa, Leonardo Moisés | u202415820 | C | C | C | C |
| Castro Solorza, Nicolás Eduardo | NicoCSE | C | L | L | C |
| Cochachi Chagua, Sebastian Josue | sebastiancochachi02-cmd | L | C | C | C |
| Pinedo Sanchez, Sebastián Martín | smp1107 | L | C | C | C |

#### 5.2.1.3 Sprint Backlog 1

El objetivo del presente Sprint fue el diseño y desarrollo de la landing page del sistema Aquanetix, enfocándose en la comunicación efectiva de la propuesta de valor, la presentación de funcionalidades clave y la facilitación del contacto con potenciales usuarios.

Durante este Sprint, el equipo trabajó de manera colaborativa en la construcción de las diferentes secciones de la landing page, asegurando una experiencia de usuario clara, intuitiva y alineada con los objetivos del sistema.

A continuación, se detallan las User Stories priorizadas y las tareas asociadas:

| US Id | Title | Task Id | Task Title | Description | Estimation (Hours) | Assigned To | Status |
|------|------|--------|------------|------------|-------------------|-------------|--------|
| US-35 | Product value visualization | T-01 | Landing page structure | Diseño e implementación de la estructura general y sección principal (hero) de la landing page | 6 | Sebastián Pinedo | Done |
| US-36 | System features visualization | T-02 | Features section development | Diseño y desarrollo de la sección de funcionalidades destacando las capacidades del sistema | 5 | Sebastián Cochachi | Done |
| US-37 | Contact information access | T-03 | Contact and CTA section | Implementación de sección de contacto y botones de llamada a la acción | 4 | Nicolás Castro | Done |
| US-35 | Product value visualization | T-04 | Content definition and UX writing | Definición del contenido textual y estructura comunicativa de la landing | 4 | Leonardo Cabrera | Done |
| US-36 | System features visualization | T-05 | Visual design elements | Diseño de elementos visuales y apoyo gráfico para mejorar la experiencia de usuario | 4 | Renzo Bojórquez | In-Process |

#### 5.2.1.4 Development Evidence for Sprint Review

| Repository | Branch | Commit Ids | Commit Message | Commit Message Body | Committed on (Date) |
|------------|--------|-----------|----------------|---------------------|---------------------|
| aquanetix-repo | develop | 4f01889ae5953aba422050a86048518fc2e68577 | docs: add epics for requirements |  | 18/04/2026 |
| aquanetix-repo | develop | 80782311c16b14e26ad36489823096a0602afeb2 | docs: add landing page UI design |  | 20/04/2026 |
| aquanetix-repo | develop | 056333d1b065eda419cb3e109ebf525a4c3749cc | docs: add C4 model diagrams |  | 21/04/2026 |
| aquanetix-repo | develop | 73157436b4d739e7e78aa21fb0a791de3101dc81 | fix: update repository links |  | 21/04/2026 |
| aquanetix-repo | develop | 68a41d56032b2c50eb7a681cc9581219c6923cd7 | docs: add web app mockups |  | 22/04/2026 |

#### 5.2.1.5 Execution Evidence for Sprint Review

En esta sección se presentan evidencias de la ejecución de la landing page desarrollada durante el Sprint.

Las siguientes capturas muestran la interacción del usuario con las diferentes secciones de la landing page, permitiendo validar la estructura de información, la propuesta de valor y la navegación definida para el sistema Aquanetix.

**Figura 1. Sección principal de la landing page**

<div align="center">
  <img src="/report/assets/LandingPage/Landing1.png">
</div>
La figura muestra la sección principal de la landing page, donde se presenta la propuesta de valor del sistema Aquanetix junto con un llamado a la acción dirigido al usuario.


**Figura 2. Sección informativa de la landing page**

<div align="center">
  <img src="/report/assets/LandingPage/Landing2.png">
</div>

En esta sección se describe el problema abordado y la solución propuesta por el sistema, permitiendo al usuario comprender el propósito y beneficios del servicio.

**Figura 3. Sección de funcionalidades**

<div align="center">
  <img src="/report/assets/LandingPage/Landing3.png">
</div>

La figura muestra las principales funcionalidades del sistema, destacando las capacidades de monitoreo, gestión de alertas y análisis de datos.

**Figura 4. Sección final y llamado a la acción**

<div align="center">
  <img src="/report/assets/LandingPage/Landing4.png">
</div>

En esta sección final se incluye un llamado a la acción que invita al usuario a interactuar con el sistema, junto con información adicional relevante.

#### 5.2.1.6 Services Documentation Evidence for Sprint Review

En el alcance del presente Sprint, no se han implementado servicios web ni endpoints documentados con OpenAPI, debido a que el desarrollo del proyecto se ha centrado principalmente en la construcción de la landing page estática y en el diseño del prototipo de la aplicación.
Por lo tanto, en esta fase no se cuenta con documentación de Web Services, ya que estos serán considerados en Sprints posteriores, donde se abordará la implementación técnica del sistema y la integración de servicios backend.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review.

Esta seccion se ha decidido omitir debido que, para este avance, solamente se ha enfocado en el diseño de Landing Page. En futuros entregables se procedera a brindar una informacion mas detallada de la aplicacion.

#### 5.2.1.8. Team Collaboration Insights during Sprint

Para el desarrollo de este primer sprint, todos los miembros del equipo desarrollaron y colaboraron de manera activa ycontinua. De tal modo, se muestra como evidencia los insights de cada miembro del equipo.
<p align = "left">
   <img src="/report/assets/insights/Team Collaboration Insights.jpg">
</p>
