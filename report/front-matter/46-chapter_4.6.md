
### 4.6. Domain-Driven Software Architecture
En esta seccion, se ha tomado el tiempo de 2 horas para identificar los diversos puntos de integración con servicios externos y definir la estructura necesaria por cada Bounded Context, con la seguridad de implementar una arquitectura SaaS escalable.
### 4.6.1. Design-Level EventStorming
<div align="center"><img src="/report/assets/miro/Design-Level Event Storming.jpg" width ="100%"></div>

### 4.6.2. Software Architecture Context Diagram

Este diagrama representa el nivel más alto de abstracción, mostrando el sistema como un solo elemento y detallando sus interacciones con el mundo exterior.

<div align="center"><img src="/report/assets/c4_diagrams/Diagrama_Contexto_Aquanetix.png" width ="100%"></div>

> * Centro del Sistema: Aquanetix se posiciona como el núcleo que recolecta y procesa datos para la reutilización de agua en estado deficiente.
> * Usuarios (Actors): Se identifican al Prestador de servicios de agua y al Gestor de residuos sólidos, quienes interactúan con la plataforma para sus respectivas labores operativas.
> * Sistemas Externos: El ecosistema se integra con Sensores IoT (PH, Gas y Flujo) para la captura de datos, Stripe para la gestión de pagos, Google Maps para la logística de rutas y Google Notifications para el envío de alertas móviles.

### 4.6.3. Software Architecture Container Diagrams

El diagrama de contenedores desglosa el sistema en sus unidades de ejecución principales, especificando las decisiones tecnológicas adoptadas.

<div align="center"><img src="/report/assets/c4_diagrams/Diagrama_Contenedores_Aquanetix.png" width ="100%"></div>

> * Web Application: Desarrollada en Vue.js, es la interfaz responsiva donde los usuarios visualizan el dashboard y alertas.
> * Landing Page: Un sitio estático construido con HTML, CSS y JS destinado al marketing y captación de clientes.
> * API Application: Es el contenedor central desarrollado en ASP.NET Core API con C#. Este monolito modular expone los servicios que consumen las aplicaciones web y procesa la información de los sensores.
> * Database: Un contenedor de MySQL que actúa como motor de base de datos relacional para la persistencia de toda la información del sistema.

### 4.6.4. Software Architecture Components Diagrams

Este diagrama profundiza en el contenedor API Application, revelando cómo se organiza internamente la lógica de negocio basada en los Bounded Contexts identificados en el proceso de diseño.

<div align="center"><img src="/report/assets/c4_diagrams/Diagrama_Componentes_Aquanetix.png" width ="100%"></div>

> * Sensores IoT: Componente encargado de procesar la telemetría técnica recibida del hardware.
> * Análisis de Calidad: Componente que determina la potabilidad o toxicidad del agua recolectada.
> * Suscripción: Componente que gestiona los planes comerciales, pagos y el ciclo de vida de los usuarios de la plataforma.
> * Mantenimiento y Distribución: Componentes que coordinan las operaciones de campo y la logística de entrega de agua recuperada a los sectores con necesidad hídrica.
> * Distribución del agua: Componente que coordina la logística de entrega del recurso hídrico certificado y el cálculo de indicadores de impacto.
