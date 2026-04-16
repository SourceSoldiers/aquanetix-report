
# CAPÍTULO 1: INTRODUCCIÓN

## 1.1. Startup Profile
### 1.1.1. Descripción de la startup

Source Soldiers es una startup tecnológica conformada por estudiantes de la Universidad Peruana de Ciencias Aplicadas (UPC), dedicada al diseño de soluciones avanzadas para la preservación y recuperación del recurso hídrico. Tenemos como objetivo mitigar la crisis del agua en el Perú mediante el uso de tecnología IoT aplicada a la infraestructura hidráulica, controlada mediante una aplicación web llamada Aquanetix.

Nuestra misión es desarrollar un ecosistema digital conectado a sensores de última generación que permita estudiar y recuperar agua en estado deficiente, brindando a las empresas y municipalidades las herramientas necesarias para una gestión sostenible.

Nuestra visión es convertirnos en el referente nacional de economía circular hídrica, logrando que el agua recuperada sea un motor de desarrollo para las zonas más necesitadas del país y reduciendo significativamente el impacto ambiental de las aguas residuales.

### 1.1.2. Perfiles de los integrantes del equipo:
| Foto | Nombre | Descripción |
| :--- | :--- | :--- |
| <img src="/report/assets/team_members/Foto_Renzo.png" width ="300" height="300"> | Renzo Alejandro Bojórquez Bustinza | Buen día, mi nombre es Renzo Bojórquez, soy estudiante de la carrera de Ingeniería de Software, cursando el quinto ciclo de mi carrera. Considero ser alguien perseverante y responsable con los trabajos, tanto individuales como en equipo. Para este proyecto aportaré de la mejor manera posible con ideas y con mi conocimiento adquirido a lo largo de la carrera para conseguir un resultado satisfactorio.|
| <img src="/report/assets/team_members/fotosebastian.png" width ="300" height="300"> | Sebastián Martín Pinedo Sanchez | Hola, soy Sebastián y estudio Ingeniería de Software, actualmente voy en el quinto ciclo. Me considero una persona tranquila y me gusta trabajar en equipo, manteniendo siempre un buen ambiente con mis compañeros. Estoy dispuesto a dar lo mejor de mí en el proyecto y aportar con ideas, además de aprender de los demás y compartir lo que sé para que podamos lograr un buen resultado juntos.|
| <img src="/report/assets/team_members/Foto_NicoPrincipal.jpeg" width ="300" height="300"> | Nicolas Eduardo Castro Solorza | Hola queridos lectores, mi nombre es Nicolas Castro y actualmente soy un estudiante de la carrera de Ingenieria de Software que cursa su quinto ciclo. Me considero como una persona perseverante, bondadoso y dispuesto a cumplir cualquier objetivo que se me proponga. Como líder de grupo, procuraré en motivar de forma positiva a mis demas compañeros para cumplir con las expectativas del curso y progresar como futuros ingenieros de Software. |
|  | |  |
| <img src="/report/assets/team_members/foto_SebastianC.png" width ="300" height="300"> | Sebastian Josué Cochachi Chagua | Hola soy Sebastián, estudiante de 5to ciclo de Ingeniería de Software. Disfruto trabajar en equipo porque creo firmemente que el buen ambiente es clave para el éxito de cualquier proyecto. Estoy comprometido a aportar con mis conocimientos técnicos y manteniendo siempre una actitud abierta para aprender de los demás. Busco sumar valor a través del intercambio de ideas y el apoyo mutuo con mis compañeros.|
| <img src="/report/assets/team_members/foto_Andrea.png" width ="300" height="300"> | Andrea Khristina Correa Rodriguez | Hola, soy Andrea, estudiante de Ingeniería de Software en la UPC y actualmente curso el quinto ciclo. Me considero una persona amable, paciente y dispuesta a ayudar y contribuir en todo momento. Me gusta trabajar en equipo y cumplir con responsabilidad los objetivos propuestos. En este proyecto, aportaré con mis conocimientos y una actitud colaborativa para lograr un buen resultado junto a mi equipo. |

## 1.2. Solution Profile
### 1.2.1. Antecedentes y problemática

En el Perú, uno de los principales problemas relacionados al agua no es solo el acceso, sino su reusabilidad. En Lima, se generan grandes cantidades de aguas residuales todos los días, pero solo una parte recibe un tratamiento adecuado. Esto hace que mucha agua que podría reutilizarse simplemente se pierda, en lugar de aprovecharse como un recurso útil (ANA, 2025).
Frente a esto, la Autoridad Nacional del Agua ha señalado que el reúso de aguas residuales es una alternativa importante para enfrentar la escasez de agua en el país. Sin embargo, en la práctica, su implementación sigue siendo limitada, principalmente por la falta de monitoreo y tecnología que permita gestionar mejor la calidad del agua (ANA, 2026).
Además, este problema se ve empeorado por la mala gestión de residuos sólidos. Según la European Commission (2023), en el Perú existen deficiencias en todo el proceso de manejo de residuos, incluyendo su tratamiento y reutilización. Incluso, solo el 2.3% de los residuos que podrían recuperarse son realmente aprovechados, lo que refleja un bajo desarrollo de la economía circular.
En resumen, esto demuestra que existe una gran perdida en recuperar y reutilizar recursos. En el caso del agua, esto refuerza la necesidad de implementar soluciones tecnológicas que permitan manejar, tratar y transformar el agua residual en un recurso reutilizable.

Con el fin de profundizar y ordenar la problemática previamente descrita, se utilizó la técnica de las 5 'W's y 2 'H's, la cual permite analizar el problema desde las distintas dimensiones y comprender con mayor claridad en qué contexto ocurre y cuál es su impacto.
#### What (¿Qué?)
El problema central está relacionado con la falta de monintoreo continuo y en tiempo real de la calidad y el flujo del agua residual, así como con la limitada detección temprana de condiciones peligrosas en las redes de alcantarillado. De acuerdo con la Autoridad Nacional del Agua (ANA, 2025), en Lima Metropolitana se generan aproximadamente 1,2 millones de metros cúbicos de aguas residuales al día, de los cuales solo alredeor del 20% recibe un tratamiento adecuado. Esta situación evidencia una pérdida considerable de agua que podría ser tratada y reutilizada, especialmente en un contexto de creciente escasez.
#### Who (¿Quiénes?)
La problemática afecta principalmente a las empresas prestadoras de servicios de agua y alcantarillado, y a las empresas operadoras de residuos sólidos, así como a sus operadores de campo, quienes desarrollan sus labores en entornos con riesgos sanitarios y ambientales. De manera indirecta, también se ven impactadas las municipalidades, los organismos reguladores ambientales y la población urbana, considerando que entre el 85 % y 90 % de la población urbana peruana accede al agua a través de redes públicas de abastecimiento (Instituto Nacional de Estadística e Informática, 2023).
#### Where (¿Dónde?)
El problema se presenta principalmente en zonas urbanas e industriales del país, con mayor incidencia en Lima Metropolitana, región que concentra tanto la mayor generación de aguas residuales como de residuos sólidos. Según datos del INEI (2023), la provincia de Lima genera aproximadamente 3,6 millones de toneladas de residuos sólidos domiciliarios al año, una parte de los cuales es dispuesta de forma inadecuada, contribuyendo a la contaminación de ríos y otros cuerpos de agua cercanos.
#### When (¿Cuándo?)
La problemática es permanente y recurrente, ya que se manifiesta durante la operación diaria de los sistemas de alcantarillado y gestión de residuos. Sus efectos se intensifican cuando no se detectan a tiempo obstrucciones, fallas operativas o variaciones en la calidad del agua, lo que obliga a las empresas a realizar intervenciones de emergencia, incrementando los costos operativos (ANA, 2025).
#### Why (¿Por qué?)
Este problema persiste principalmente debido a la limitada adopción de tecnologías de monitoreo inteligente, la dependencia de inspecciones manuales y la escasa integración de información para la toma de decisiones. A ello se suma el bajo nivel de desarrollo de la economía circular en el país. El Ministerio del Ambiente (MINAM, 2023) señala que los niveles de reaprovechamiento de residuos en el Perú siguen siendo reducidos, lo que dificulta la valorización de recursos y la protección de las fuentes hídricas.
#### How (¿Cómo?)
La ausencia de sensores que permitan medir variables como pH, flujo y condiciones peligrosas en puntos críticos de la infraestructura impide detectar de manera temprana desviaciones en la calidad del agua o situaciones de riesgo. Como consecuencia, las empresas suelen actuar de forma reactiva, cuando el problema ya se ha producido, lo que incrementa los costos de mantenimiento, expone al personal operativo y desaprovecha oportunidades para recuperar y reutilizar el agua residual.
#### How Much (¿Cuánto impacta?)
El impacto de esta problemática es económico, ambiental y social. Desde el punto de vista financiero, las empresas enfrentan elevados costos operativos y el riesgo de sanciones por incumplimiento de la normativa ambiental. El Organismo de Evaluación y Fiscalización Ambiental (OEFA, 2024) indica que las multas por infracciones ambientales pueden superar los S/ 128 millones. Asimismo, la pérdida diaria de grandes volúmenes de agua reutilizable limita los esfuerzos por reducir el déficit hídrico y frena el avance hacia una gestión sostenible del recurso (ANA, 2026).
### 1.2.2. Lean UX Process
#### 1.2.2.1. Lean UX Problem Statement
"Actualmente, las empresas prestadoras de servicios hídricos y operadoras de residuos en Lima enfrentan una falta crítica de visibilidad en tiempo real sobre la calidad y el flujo del agua en sus redes, lo que genera altos costos operativos por mantenimiento reactivo ante obstrucciones y graves riesgos de seguridad por gases tóxicos no detectados. Existe una brecha significativa entre la recolección de agua en estado deficiente y su potencial reaprovechamiento, perdiendo la oportunidad de cerrar el ciclo de economía circular en zonas industriales con alto estrés hídrico. Ante esta situación, ¿cómo podríamos utilizar tecnología IoT (PH, gases y flujo) para monitorear y transformar el agua residual en un recurso recuperable, optimizando la gestión operativa de las empresas y facilitando su redistribución logística hacia los sectores que más la necesitan?"
#### 1.2.2.2. Lean UX Assumptions
User Assumptions:<br>
•	Creemos que nuestros clientes necesitan reducir sus multas por vertimientos fuera de norma (PH).<br>
•	Creemos que los operadores de campo prefieren recibir alertas en dispositivos móviles que realizar inspecciones manuales programadas.<br>
Business Assumptions:<br>
•	Creemos que las empresas están dispuestas a pagar una suscripción si el ahorro en mantenimiento preventivo supera el costo del servicio.<br>
•	Creemos que el mayor valor agregado es el módulo de logística para la redistribución (economía circular).<br>
#### 1.2.2.3. Lean UX Hypothesis Statements:
Creemos que al proporcionar sensores de PH y flujo a las empresas de alcantarillado, lograremos que se reduzcan los costos de mantenimiento. Sabremos que estaremos en lo correcto cuando veamos una disminución del 20% en el número de cuadrillas enviadas por emergencias de obstrucción.<br>
Creemos que integrar detectores de gases tóxicos en el plan base lograremos aumentar la seguridad percibida por los trabajadores. Sabremos que tenemos razón cuando el 80% de los usuarios califiquen la plataforma como "esencial para la seguridad".<br>
Creemos que automatizar la logística de redistribución de agua recuperada lograremos que las empresas operadoras generen una nueva línea de impacto social. Sabremos que tenemos razón cuando al menos 2 sectores necesitados reciban agua monitoreada por nuestra plataforma en los primeros 6 meses.<br>

#### 1.2.2.4. Lean UX Canvas
| **1. Business Problem** | **2. Business Outcomes** |
| :--- | :--- |
| Las EPS y operadoras de residuos en Lima carecen de visibilidad en tiempo real de sus redes, resultando en mantenimiento reactivo y multas de la OEFA (hasta S/ 128M), riesgos por gases tóxicos en ductos, y desperdicio de las aguas residuales en Lima. | • Reducción del 20% en salidas de cuadrillas de emergencia por obstrucciones.<br>• Cero infracciones por parámetros de PH fuera de norma.<br>• Al menos 2 sectores vulnerables reciban agua recuperada en el primer semestre.<br>• 80% de adopción de la plataforma como EPP digital. |
| **3. Users & Customers** | **4. User Benefits** |
| • **Empresas prestadoras de servicios de agua y alcantarillados (EPS):** Entidades responsables de la red matriz de agua y alcantarillado (ej. Sedapal).<br> •**Empresas operadoras de residuos sólidos:** <br>Empresas privadas que gestionan el transporte, tratamiento y disposición de residuos sólidos e industriales. | • Reducción de costos por multas: Evitar sanciones de la OEFA mediante el monitoreo preventivo de vertimientos.<br>• Seguridad Laboral: Prevención de accidentes fatales por inhalación de gases (H2S) en colectores.<br> • Optimización de Activos: Mayor vida útil de la infraestructura al detectar niveles críticos de acidez (pH).<br> • Logística Inteligente: Planificación eficiente de rutas para la recolección y redistribución de agua tratada.<br> |
| **5. Solutions** | **6. Hypotheses** |
| Implementar una plataforma web conectada a sensores que puedan medir el pH, flujo, gases del estado del agua en tiempo real. La solución incluirá alertas automáticas para detectar anomalías, un panel de control para visualizar datos y un módulo de logística que facilite la redistribución del agua recuperada hacia zonas que la necesiten. | Creemos que si las EPS y operadores de residuos cuentan con monitoreo en tiempo real, podrán anticiparse a problemas como obstrucciones, contaminación o presencia de gases peligrosos. Sabremos que esto es cierto cuando se reduzcan las salidas de emergencia en al menos 20% y cuando los usuarios consideren la plataforma útil para la toma de decisiones en el area operativa. |
| **7. What’s the most important thing we need to learn first?** | **8. What’s the least amount of work we need to do to learn that?** |
| ¿Están las empresas dispuestas a pagar la suscripción basándose en el ahorro proyectado? ¿La tecnología de los sensores resiste la corrosión y condiciones de los colectores de Lima? | Realizar entrevistas a gerentes de operaciones y jefes de cuadrilla y presentar un prototipo simple (mockup) de la plataforma para recoger feedback. También se puede simular el uso de alertas con datos básicos para validar si la solución resulta útil en la práctica. |

## 1.3. Segmentos objetivo
Nuestra aplicación se dirige a dos segmentos clave en el ecosistema de gestión de agua y residuos en Perú, enfocados en resolver la contaminación y subutilización del agua en estado deficiente. Ambos segmentos operan en un mercado con alta demanda por soluciones IoT debido a regulaciones ambientales estrictas (Ley General del Ambiente y DS 015 2015 MINAM) y la escasez hídrica crónica en zonas urbanas como Lima.<br>

**1. Empresas prestadoras de servicios de agua y alcantarillados (EPS).** <br>
Perfil demográfico y operativo:
Principalmente medianas y grandes empresas estatales o mixtas, con sede en capitales provinciales (80% en Lima Metropolitana). Emplean entre 500–5,000 trabajadores, enfocadas en recolección, tratamiento y distribución de agua. Ejemplos: SEDAPAL (Lima) y EPS regionales como SEDACUSCO o SEDAPAR.
Estadísticas de sustento:
- Cubren alrededor del 85–90% de la población urbana peruana, según datos de acceso al agua por red pública en el área urbana publicados por el Instituto Nacional de Estadística e Informática (INEI, 2023).
- En Lima Metropolitana se generan aproximadamente 1,2 millones de m³ de aguas residuales diariamente, de las cuales solo alrededor del 20% recibe tratamiento, según informes de la ANA y análisis académicos sobre saneamiento en Lima (ANA, 2025; PUCP, 2018).
- El sistema de sanciones ambientales (OEFA) permite multas de hasta más de S/ 128 millones por incumplimientos ambientales, lo que da base al contexto de riesgos financieros asociados a la contaminación de aguas (OEFA, 2024).
Oportunidad:
Estas empresas necesitan herramientas de monitoreo en tiempo real, reactivas y predictivas, para mejorar el tratamiento de aguas residuales y avanzar hacia metas de reutilización de agua, alineadas con el Plan Estratégico 2025–2030 de la ANA (ANA, 2025).

**2. Empresas operadoras de residuos sólidos** <br>
Perfil demográfico y operativo:
Empresas privadas o consorcios de tamaño mediano (100–1,000 empleados), con operaciones en municipios urbanos e industriales. Concentran el 70% de sus actividades en Lima y Callao, gestionando recolección, transporte y disposición final. Ejemplos: Urbaser, FCC Ambiente o empresas locales como Residuos Perú.
Estadísticas de sustento:
- En Perú se generan alrededor de 7,5 millones de toneladas de residuos sólidos urbanos anuales, según informes de gestión de residuos de la Comisión Europea–Acceso a Mercados (European Commission–Access to Markets, s. f.).
- La provincia de Lima genera cerca de 3,6 millones de toneladas de residuos sólidos domiciliarios al año, según la Encuesta Nacional de Residuos Sólidos Urbanos del INEI (INEI, 2023).
- Un quinto de la basura de Lima (20%) termina en vertederos no autorizados, cuya escorrentía contamina ríos como el Rímac, Chillón y Lurín (Woima Corporation, 2024).
- Solo una fracción muy baja del reciclaje formal se realiza en Perú, lo que refuerza la baja tasa de material reciclado declarada en estudios sectoriales (Molpack, 2025; Mastercard Center, 2018).
Oportunidad:
Estas empresas requieren detección temprana de sólidos/desechos, optimización de rutas y reducción de vertimientos que contaminan fuentes de agua, en línea con la necesidad de mejorar la gestión de residuos y la protección de cuencas (Woima Corporation, 2024; European Commission, s. f.).

## Fuentes:
-	Autoridad Nacional del Agua (ANA). (2025). Plan estratégico 2025–2030.
https://www.ana.gob.pe/sites/default/files/file_content/PLAN%20ESTRATEGICO%202025-2030.pdf
-	Autoridad Nacional del Agua (ANA). (2026, 19 de marzo). ANA promueve el reúso de aguas residuales para fortalecer la gestión sostenible del recurso hídrico [Nota de prensa].
https://www.gob.pe/institucion/ana/noticias/1368267-ana-promueve-el-reuso-de-aguas-residuales-para-fortalecer-la-gestion-sostenible-del-recurso-hidrico
-	European Commission – Access to Markets. (s. f.). Solid waste management in Peru.
https://trade.ec.europa.eu/access-to-markets/en/country-assets/pe_solid_waste.pdf
-	Instituto Nacional de Estadística e Informática (INEI). (2023). Componente 3: Residuos (Encuesta Nacional de Residuos Sólidos Urbanos).
https://www.inei.gob.pe/media/MenuRecursivo/publicaciones_digitales/Est/Lib1926/cap03.pdf
-	Instituto Nacional de Estadística e Informática (INEI). (2023). Perú: Formas de acceso al agua y saneamiento básico – N° 10.
https://www.gob.pe/institucion/inei/informes-publicaciones/4985657-peru-formas-de-acceso-al-agua-y-saneamiento-basico-nro-10
-	Instituto Nacional de Estadística e Informática (INEI). (2023). Perú: Formas de acceso al agua y saneamiento básico – N° 11.
https://www.gob.pe/institucion/inei/informes-publicaciones/6313803-peru-formas-de-acceso-al-agua-y-saneamiento-basico-nro-11
-	Mastercard Center for Inclusive Growth. (2018). Opportunity assessment: Inclusive waste management in Peru.
https://www.mastercardcenter.org/pdfs/Inclusive-Waste-Mgmt-in-Peru-March-2018.pdf
-	Molpack. (2025, 2 de noviembre). Recycling in Peru: A stretch to go with steps already taken.
https://molpack.net/en/recycling-in-peru-a-stretch-to-go-with-steps-already-taken/
-	Organismo de Evaluación y Fiscalización Ambiental (OEFA). (2024). OEFA puede sancionar hasta con más de S/ 128 millones de soles a administrados que contaminen el aire [Nota de prensa].
https://www.gob.pe/institucion/oefa/noticias/1001222-oefa-puede-sancionar-hasta-con-128-millones-de-soles-a-administrados-que-contaminen-el-aire
-	Pontificia Universidad Católica del Perú [PUCP]. (2018, 7 de mayo). La situación de las aguas residuales en Lima. PuntoEdu PUCP.
https://puntoedu.pucp.edu.pe/voces-pucp/la-situacion-de-las-aguas-residuales-en-lima/
-	Woima Corporation. (2024). Drowning in waste – Case Lima, Peru.
https://www.woimacorporation.com/drowning-in-waste-case-lima-peru/
-	European Commission. (2023). Solid waste management in Peru.
https://trade.ec.europa.eu/access-to-markets/en/country-assets/pe_solid_waste.pdf
-	Autoridad Nacional del Agua. (2026). ANA promueve el reúso de aguas residuales para fortalecer la gestión sostenible del recurso hídrico.
https://www.gob.pe/institucion/ana/noticias/1368267-ana-promueve-el-reuso-de-aguas-residuales-para-fortalecer-la-gestion-sostenible-del-recurso-hidrico
