# Capítulo V: Product Implementation, Validation & Deployment.
## 5.1. Software Configuration Management.

Durante el desarrollo de la aplicación web, se gestionaron múltiples elementos como prototipos, documentación UX, código fuente y versiones del sistema. Para ello, se utilizaron herramientas colaborativas que facilitaron el trabajo en equipo y permitieron llevar un control adecuado de los cambios realizados.

### 5.1.1. Software Development Environment Configuration.

El entorno de desarrollo del proyecto fue configurado utilizando herramientas digitales basadas en la nube, las cuales permitieron el trabajo colaborativo y la integración de las distintas fases del desarrollo de la aplicación web.

### Github

Utilizado como repositorio principal para la gestión del código fuente, control de versiones y trabajo colaborativo entre los integrantes del equipo.

[GitHub](https://github.com/)

<p align="center">
<img src="../assets/development_environment/Github.png"/>
</p>

### Uxpressia

Herramienta utilizada para la elaboración de entregables UX como user personas, mapas de empatía y customer journey.

[UXPressia](https://uxpressia.com/)

<p align="center">
  <img src="../assets/development_environment/Uxpressia.png" width="500"/>
</p>

### Miro

Plataforma empleada para la organización de ideas, diagramas, brainstorming y planificación del proyecto. Facilitó la estructuración inicial de la solución.

[Miro](https://miro.com/)

<p align="center">
  <img src="../assets/development_environment/Miro.png" width="500"/>
</p>

### Figma

La herramienta empleada para la organización de ideas, diagramas, brainstorming y planificación del proyecto. Facilitó la estructuración inicial de la solución.

[Figma](https://www.figma.com/)

<p align="center">
  <img src="../assets/development_environment/Figma.png" width="500"/>
</p>

### VSCode

Permitió trabajar de manera eficiente con archivos HTML, CSS y JavaScript, facilitando la organización del código, la edición en tiempo real y la integración con el repositorio del proyecto.

[VSCode](https://code.visualstudio.com/)

<p align="center">
  <img src="../assets/development_environment/VSCode.png" width="500"/>
</p>

### Meet

Herramienta de comunicación utilizada para la coordinación del equipo durante el desarrollo del proyecto. A través de reuniones virtuales, se realizaron seguimientos de avances, toma de decisiones y organización de tareas.

[Meet](https://meet.google.com/)

<p align="center">
  <img src="../assets/development_environment/Meet.png" width="500"/>
</p>


## 5.1.2 Source Code Management

La gestión del código fuente del proyecto se realizó mediante la plataforma GitHub, la cual fue utilizada como sistema de control de versiones para organizar y dar seguimiento a todos los cambios realizados durante el desarrollo.

El proyecto cuenta con dos repositorios principales:

- Repositorio del informe (documentación): https://github.com/NicoCSE/Aquanetix-report  
- Repositorio de la Landing Page: https://github.com/NicoCSE/Landing-Page-Aquanetix

En el repositorio del informe se gestionaron todos los avances relacionados a la documentación del proyecto, mientras que en el repositorio de la Landing Page se desarrolló la parte visual y funcional del producto.

### GitFlow Workflow

Para la organización del desarrollo se implementó el modelo GitFlow como estrategia de control de versiones. Este modelo permitió estructurar el trabajo del equipo y mantener un flujo ordenado de integración.

Las ramas utilizadas en el proyecto fueron:

- **main**: contiene la versión estable del proyecto.
- **develop**: rama principal de trabajo donde se integran los avances del equipo.

La rama develop fue utilizada como base para el desarrollo continuo del proyecto, permitiendo consolidar los cambios antes de integrarlos a la versión final.

Adicionalmente, para el desarrollo de nuevas funcionalidades se considera el uso de ramas tipo feature, siguiendo buenas prácticas de control de versiones.

### Convenciones de Ramas

Se estableció la siguiente convención para la creación de ramas:

- Feature branches:
  feature/nombre-funcionalidad

Ejemplo:
feature/landing-page  
feature/chapter-5  

Estas ramas permiten desarrollar funcionalidades de manera independiente sin afectar la estabilidad del proyecto.

### Semantic Versioning

Para el control de versiones del proyecto se adoptó el uso de Semantic Versioning (SemVer), siguiendo la estructura:

vMAJOR.MINOR.PATCH

Donde:
- MAJOR: cambios importantes o incompatibles  
- MINOR: nuevas funcionalidades  
- PATCH: corrección de errores  

Ejemplo:
v1.0.0  

Esto permite mantener un control claro sobre la evolución del proyecto.

### Conventional Commits

Para estandarizar los mensajes de commits, se aplicó la convención de Conventional Commits, lo que permitió mejorar la organización y trazabilidad del repositorio.

Los tipos de commits utilizados fueron:

- feat: nuevas funcionalidades  
- docs: cambios en documentación  
- fix: corrección de errores  
- chore: tareas menores o mantenimiento  

Ejemplos reales del proyecto:

feat: add section 5.1 software configuration management with images  
docs: add development environment images  
fix: correct image path in markdown  
chore: update repository structure  

El uso de estas convenciones permitió identificar fácilmente el tipo de cambio realizado en cada commit y mejorar la colaboración entre los integrantes del equipo.

<p align="center">
  <img src="" width="700"/>
</p>

<p align="center">
Historial de commits en la rama develop del repositorio, evidenciando el uso de Conventional Commits y el trabajo colaborativo del equipo.
</p>

La evidencia mostrada refleja el uso adecuado de Conventional Commits, así como la participación activa de los integrantes del equipo en el desarrollo del proyecto.

## 5.1.3 Source Code Style Guide & Conventions

Con el objetivo de garantizar la consistencia, legibilidad y mantenibilidad del proyecto, el equipo definió una guía de estilo basada en las tecnologías actualmente utilizadas en el desarrollo de la Landing Page.

Esta guía establece estándares que permiten mantener un código limpio, organizado y comprensible para todos los integrantes del equipo.

### HTML

Para la estructura del documento HTML se establecieron las siguientes convenciones:

- Uso de etiquetas en minúsculas (lowercase)
- Correcto cierre de todos los elementos HTML
- Uso de etiquetas semánticas como `header`, `nav`, `main`, `section` y `footer`
- Inclusión de atributos `alt` en imágenes para mejorar la accesibilidad
- Estructuración jerárquica del contenido

Ejemplo:

```html
<section>
  <h1>Inteligencia Hídrica</h1>
  <p>Monitoreo en tiempo real</p>
</section>
```

### CSS

Para los estilos del sistema se definieron las siguientes convenciones:

- Uso de kebab-case para nombres de clases
- Nombres descriptivos según la funcionalidad del elemento
- Reutilización de clases para evitar duplicidad
- Separación de estilos en archivos independientes
- Organización de estilos personalizados en archivos CSS dedicados
Ejemplo:

```css
.water-shadow {
  box-shadow: 0 12px 32px rgba(0, 50, 125, 0.06);
}
```

### Uso de Tailwind CSS

Se empleó Tailwind CSS como framework de estilos utilitarios, permitiendo:

- Construcción rápida de interfaces  
- Diseño responsive  
- Consistencia visual en los componentes  

El uso de clases utilitarias permite reducir la cantidad de código CSS personalizado y mejorar la mantenibilidad del proyecto.

### 5.1.4. Software Deployment Configuration.

En esta sección se especifica la configuración y los pasos necesarios para el despliegue de los productos digitales de la solución Aquanetix. El despliegue se ha automatizado para garantizar que los cambios realizados en los repositorios de código fuente se reflejen de manera satisfactoria en los entornos de producción.

## Despliegue de la Landing Page

1. Se creo el repositorio en Github en la organizacion del equipo WebWarriors, coloco que sea de manera publica

<p align="center">
  <img src="" width="700"/>
</p>

2. Publicación Directa: El código fuente desarrollado en VS Code fue sincronizado directamente con la rama main mediante comandos de Git.

<p align="center">
  <img src="" width="700"/>
</p>

3. Hosting: La visualización del producto se gestiona a través de la infraestructura de GitHub, asegurando que el HTML y los estilos de Tailwind CSS sean accesibles de forma pública una vez realizado el push de los archivos.

<p align="center">
  <img src="" width="700"/>
</p>
