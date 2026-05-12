# Capítulo IV: Product Design

## 4.1. Style Guidelines:
Se considera un **Style Guideline** al conjunto de reglas y estándares que definen el cómo se debe redactar, diseñar y/o presentar diversas interfaces web, documentos, software u otros productos creativos, con el fin de asegurar una coherencia visual de un proyecto. A continuación se procederá a describir de forma más detallada los parámetros implementados en nuestra propuesta. 
### 4.1.1. General Style Guidelines
#### Branding
La identidad de Aquanetix se basa en el principio de "Ingeniería Hídrica Circular". Buscamos proyectar una imagen de tecnología de vanguardia aplicada directamente a la regeneración de un recurso natural. El logo es la materialización de este concepto: la fusión de la gota (naturaleza) y el nodo (tecnología/IoT).

Principios de Diseño:

> * Tecno-Naturaleza: Los componentes visuales deben equilibrar lo orgánico (formas fluidas del agua) con lo geométrico (precisión de los datos).
> * Claridad Operativa: La interfaz debe priorizar la legibilidad de métricas críticas sobre la ornamentación.
> * Transparencia: Reflejar la honestidad académica de la UPC en la presentación de datos.

#### Tipografía
La tipografía debe reflejar la solidez de una solución corporativa/municipal.
> * Encabezados (Manrope): Se utilizará en pesos Bold (700) y SemiBold (600). Su estructura geométrica y moderna da una imagen de startup sólida.
> * Cuerpo de Texto y Labels (Inter): Se utilizará para toda la lectura de datos, tablas y etiquetas. Es la fuente estándar en interfaces de alta densidad por su claridad en tamaños pequeños.
 <div align="center"><img src="../assets/LandingPage/tipografía.jpg" width ="400" height="700"></div>

#### Colores
La paleta utilizada para el sitio web le da un mayor protagonismo a los azules vibrantes:
> * Azul cobalto (#007BFF): El color que representa la identidad de la app, usado para botones principales, navegación y estados de "Agua Limpia".
> * Verde esmeralda (#10B981): Acentos de éxito, sostenibilidad, recuperación y estados "Activo/Óptimo".
> * Verde bosque (#064E3B): Fondos de secciones oscuras, iconos de naturaleza y estados de "Eco-impacto".
> * Blanco pizarrón (#F1F5F9): Fondos de la aplicación (UI), tarjetas de datos y separación de secciones.
<div align="center"><img src="../assets/LandingPage/paleta de colores.jpg" width ="400" height="700"></div>

#### Principios de espaciado
Utilizaremos un sistema de espaciado basado en una rejilla de 8px (base 8). Esto garantiza que todos los componentes (gráficos de sensores, menús, tarjetas) tengan una relación matemática limpia. El espacio negativo debe ser amplio para reducir la "carga cognitiva" en dashboards complejos.

#### Tono de comunicación
Los tonos de comunicación serán mayormente serios, con un toque de entusiasmo. Queremos priorizar la precisión técnica y la confianza municipal, a la vez que queremos transmitir que el cambio es posible mediante la tecnología.


### 4.1.2. Web Style Guidelines:

Para la interfaz web de Aquanetix, el diseño se fundamenta en una estructura modular basada en contenedores limpios, priorizando la rápida lectura de grandes volúmenes de datos operativos. Los paneles de control principales utilizarán una disposición en cuadrícula para permitir a los supervisores visualizar métricas complejas de manera estructurada. Además, se aplicarán bordes sutilmente redondeados junto con sombras difuminadas para generar jerarquía visual. De este modo, aseguramos mantener la atención del usuario enfocada estrictamente en los indicadores críticos, como el porcentaje de llenado de lixiviados o las alertas de sobreconsumo, previniendo la fatiga visual durante jornadas extensas de monitoreo.
Por otro lado, respecto a la interactividad de la plataforma, los componentes están diseñados para ofrecer retroalimentación inmediata, cambiando de estado visualmente al recibir clics o desplazamientos del cursor. Resulta indispensable que toda la interfaz responda fluidamente a distintos tamaños de pantalla mediante principios de diseño adaptable (responsive design). Así, garantizamos una experiencia de uso coherente tanto para un gerente que exporta reportes de huella hídrica desde una computadora de escritorio en la oficina, como para un operario que ingresa registros en tiempo real desde su teléfono móvil en medio del patio de maniobras.
