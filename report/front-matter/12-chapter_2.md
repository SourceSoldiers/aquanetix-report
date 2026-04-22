# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores
El ecosistema de soluciones tecnológicas aplicadas a la gestión de recursos hídricos a nivel global presenta un grado de maduración significativo. Sin embargo, una revisión crítica del mercado evidencia que la oferta de software e Internet de las Cosas (IoT) orientada a la economía circular hídrica en América Latina, particularmente en el Perú, se encuentra desatendida. Según el Banco Mundial (2025), el país requiere de una transformación infraestructural en sus métodos de saneamiento, destinando un programa de inversión de $200 millones para fomentar la transición hacia una economía circular que las soluciones actuales no son capaces  de consolidar.

 Las plataformas internacionales dominantes tienden a enfocarse en infraestructuras de países desarrollados, omitiendo las realidades logísticas, además de los marcos regulatorios locales estipulados por entidades como la Autoridad Nacional del Agua (ANA) junto con el Organismo de Evaluación y Fiscalización Ambiental (OEFA). Dicha desconexión tecnológica se traduce como una brecha de eficiencia crítica: según plantea la SUNASS (2025), el Perú necesita invertir una cantidad de 138,000 millones de soles en los próximos 30 años para cerrar la brecha de saneamiento, una cifra difícil de alcanzar empleando métodos tradicionales sin la adquisición y adopción de tecnologías de monitoreo de bajo costo y alta precisión.
 
Para una Empresa Prestadora de Servicios (EPS) o una operadora de residuos sólidos en el país, esta brecha significa que no existe un competidor directo, accesible, que cubra sus necesidades de extremo a extremo: desde la detección de anomalías químicas en tiempo real hasta la logística de redistribución para el reúso del agua. Por consiguiente, se han seleccionado para este análisis a tres competidores representativos (dos directos a nivel global sumados a uno indirecto corporativo), con el objetivo de demostrar cómo la arquitectura, combinada con el modelo de negocio de WebWarriors, ataca sus debilidades en el mercado peruano:

 #### 1.	Kando (Competencia Directa en Capa Transaccional Analítica):
 - **Perfil:** Empresa tecnológica global enfocada en la gestión de la calidad de aguas residuales mediante IoT, apoyada en el análisis de datos en la nube bajo el modelo Software as a Service (SaaS).

 - **Debilidad frente a nuestro nicho:** Es una solución de alto costo diseñada principalmente para "utility companies" norteamericanas al igual que europeas. Carece de un módulo logístico para la redistribución del agua recuperada, limitándose a la detección, sin lograr el cierre del ciclo de economía circular requerido en zonas de estrés hídrico.
 #### 2.	SmartCover Systems (Competencia Directa en Capa de Infraestructura Física):
 - **Perfil:** Proveedor especializado en el monitoreo remoto de sistemas de recolección de aguas residuales, enfocado en la prevención de desbordes (SSO) mediante sensores acústicos, así como satelitales.

 - **Debilidad frente a nuestro nicho:** Su enfoque es estrictamente volumétrico, orientado a la prevención de derrames. No realiza analítica química profunda (como variaciones críticas de pH) ni detección de gases tóxicos, variables fundamentales para habilitar el reúso del agua residual (ANA, 2026).
#### 3.	Veolia - Hubgrade (Competencia Indirecta en Capa Corporativa Integral):
 - **Perfil:** Gigante corporativo de servicios medioambientales que cuenta con "Hubgrade", una plataforma digital para el monitoreo, auditoría, además de optimización de recursos hídricos mediante gemelos digitales (digital twins).

 - **Debilidad frente a nuestro nicho:** Opera mediante proyectos multimillonarios "llave en mano". La barrera financiera, sumada a la rigidez burocrática de su implementación, resulta restrictiva e incluso prohibitiva para el grueso de municipalidades, al igual que operadoras medianas en el mercado peruano.


### 2.1.1. Análisis competitivo

El análisis competitivo estructurado a continuación emplea una matriz de variables del mercado (Landscape) junto con un análisis FODA cruzado (SWOT) para evaluar el posicionamiento estratégico de la solución propuesta frente a plataformas consolidadas.

| ¿Por qué llevar a cabo este análisis? | Competidor 1 | Competidor 2 | Competidor 3 | StartUp |
| :--- | :---| :--- | :--- | :--- |
| Comprender las fortalezas tecnológicas de los líderes del mercado IoT hídrico para diseñar una propuesta de valor localizada, accesible, enfocada en la redistribución logística (economía circular) que el mercado peruano necesita frente a las normativas de ANA u OEFA. | <img src="/report/assets/logos/kando-logo.png" width ="300" height="300"> | <img src="/report/assets/logos/smartcover_logo.png" width ="300" height="300"> | <img src="/report/assets/logos/veolia_logo.png" width ="300" height="300"> | <img src="/report/assets/logos/Aquanetix_Logo.png" width ="300" height="300"> |
| Overview / Perfil | Empresa global de SaaS/IoT especializada en inteligencia de aguas residuales para empresas de servicios públicos. | Empresa tecnológica norteamericana enfocada en monitoreo remoto de sistemas de recolección de aguas residuales. | Plataforma de monitoreo digital de una de las corporaciones ambientales más grandes del mundo. | Startup peruana de IoT enfocada en el monitoreo logístico de recuperación de agua residual para economía circular. |
| Ventaja competitiva | Algoritmos avanzados de IA para detectar orígenes específicos de contaminación en redes complejas. | Hardware de alta resistencia que no requiere ingreso a espacios confinados para su instalación. | Respaldo financiero junto a una infraestructura física masiva con capacidad de ejecución internacional. | Solución localizada a la normativa peruana, de bajo costo, con módulo exclusivo de redistribución. |
| ¿Qué valor ofrece a los clientes? | Visibilidad predictiva de la red para prevenir eventos de contaminación, protegiendo plantas de tratamiento. | Prevención de desbordamientos acompañada de una reducción de costos de mantenimiento preventivo. | Gestión integral combinando operaciones físicas con gemelos digitales en tiempo real. | Prevención de multas millonarias, protección laboral, además de habilitación comercial del agua recuperada. |
| Mercado objetivo | Grandes empresas de servicios de agua a nivel global (Estados Unidos, Europa). | Municipalidades o agencias de agua en Norteamérica. | Megacorporaciones industriales, mineras junto con gobiernos nacionales. | EPS (ej. SEDAPAL) sumadas a empresas operadoras de residuos sólidos en Perú. |
| Estrategias de marketing | Posicionamiento en conferencias B2B de WaterTech, así como publicaciones científicas. | Casos de estudio municipal, licitaciones públicas, apoyados en demostraciones directas de ROI. | Lobbying corporativo, contratos a largo plazo, reforzados por un posicionamiento de sostenibilidad. | Ventas B2B directas mediante programas piloto, buscando el alineamiento con metas de entidades gubernamentales. |
| Productos & Servicios | Hardware IoT acoplado a una Plataforma SaaS de analítica predictiva de calidad de agua. | Sensores de nivel acústicos, al igual que satelitales, vinculados a una plataforma de alertas. | Centro de hipervisión enfocado en la optimización de plantas en tiempo real. | Sensores IoT (Flujo, Gases, pH) integrados a un Dashboard SaaS con su respectivo módulo logístico de redistribución. |
| Precios & Costos | Alto. Licenciamiento Enterprise, implicando dependencia de consultoría especializada. | Alto. Costos elevados por importación de hardware patentado. | Muy Alto. Inversiones de capital intensivo (CAPEX) a largo plazo. | Accesible. Suscripción SaaS escalonada (OPEX) con hardware de ensamblaje local. |
| Canales de distribución | Venta directa B2B, estableciendo alianzas con consultoras ambientales. | Representantes regionales de ventas B2B. | Licitaciones gubernamentales junto a venta directa corporativa. | Plataforma web respaldada por despliegue in situ para pilotos iniciales. |
| Análisis SWOT: Fortalezas | Gran precisión analítica respaldada por una experiencia comprobada en múltiples ecosistemas internacionales. | Hardware duradero, destacando su fácil instalación (Out-of-the-box). | Capacidad inigualable de ejecutar proyectos integrales que combinan infraestructura con software. | Especialización normativa local, sumada a un enfoque inédito en el cierre de la brecha logística (economía circular). |
| Análisis SWOT: Debilidades | Solución agnóstica a la redistribución; no aborda la logística de reúso en países en desarrollo. | Enfoque volumétrico limitado; carencia de analítica química profunda (pH, gases). | Implementación altamente burocrática, lenta, resultando financieramente restrictiva para pymes. | Marca naciente sin base instalada inicial ni validación histórica de hardware a largo plazo. |
| Análisis SWOT: Oportunidades | Expansión hacia mercados emergentes forzados a digitalizar sus redes hídricas. | Crecimiento de ecosistemas de Smart Cities a nivel global. | Mandatos de eficiencia junto a auditorías impulsadas por organismos internacionales. | Regulaciones estrictas locales frente a la necesidad urgente de optimización dado el déficit hídrico nacional. |
| Análisis SWOT: Amenazas | Ingreso de startups locales que operen con estructuras de costos más eficientes. | Recortes de presupuestos municipales que paralicen adquisiciones tecnológicas. | Leyes antimonopolio junto a una potencial pérdida de flexibilidad operativa frente a competidores ágiles. | Resistencia estructural al cambio tecnológico en operadoras tradicionales, agravada por la informalidad del sector, dificultando la trazabilidad del agua recuperada. |



### 2.1.2. Estrategias y tacticas frente a competidores
Al momento de ingresar a un mercado caracterizado por infraestructuras heredadas junto a monopolios tecnológicos internacionales, la startup debe adoptarse a un pragmatismo estratégico. La viabilidad  del negocio no solo reside en competir en fuerza bruta de capital con corporaciones como Veolia, sino que se busca capturar un nicho crítico para resolver fricciones regulatorias, además de logísticas, que varios competidores globales ignoran.



A continuación, se detallan las estrategias operativas junto a las tácticas arquitectónicas que guiarán la construcción al igual que el despliegue del producto:

**1. Estrategia de Localización con Mitigación de Riesgos Normativos (Posicionamiento frente a Kando o Veolia)**
- 	**Objetivo Estratégico:** Diferenciarse radicalmente de las plataformas genéricas extranjeras, consolidando el software como una herramienta nativa de cumplimiento regulatorio, sirviendo como protección financiera para las empresas locales.

- **Táctica Ejecutable:** La arquitectura de la base de datos, operando en conjunto con el motor de alertas, se parametrizará rígidamente bajo los estándares exigidos por las autoridades nacionales. El sistema evaluará en tiempo real el pH junto a la emisión de gases tóxicos. Si los parámetros se acercan a los límites permisibles sancionables (los cuales pueden           desencadenar multas superiores a los S/ 128 millones, según el OEFA), el sistema generará bloqueos preventivos, emitiendo     reportes automatizados en el formato exacto requerido por los fiscalizadores (OEFA, 2024).

**2. Estrategia de Océano Azul: Cierre de la Cadena de Valor (Posicionamiento frente a SmartCover)**

- **Objetivo Estratégico:** Trascender la simple capa de telemetría e infraestructura de monitoreo, integrando la gestión comercial junto a la logística, habilitando la economía circular en el sector hídrico.

- **Táctica Ejecutable:** Mientras la competencia detecta un flujo de agua para luego emitir una alerta, la plataforma integrará un "Módulo de Logística de Redistribución". Al detectar que un volumen de agua residual cumple con los parámetros químicos para su reúso (conforme a los lineamientos de la ANA, 2026), el sistema no solo alertará a la planta, sino que orquestará la disponibilidad de este recurso en la plataforma, permitiendo su asignación junto a su transporte hacia sectores de alto déficit hídrico, transformando un desecho en un activo logístico.

**3. Estrategia Land and Expand mediante Reducción de Barreras CAPEX**

- **Objetivo Estratégico:** Vencer la resistencia financiera de las empresas estatales al igual que operadoras medianas que no pueden asumir los costos de implementación de licencias de competidores como Veolia.

- **Táctica Ejecutable:** El modelo de comercialización se ejecutará bajo un esquema de Software as a Service (SaaS), sustituyendo fuertes inversiones de capital (CAPEX) por gastos operativos manejables (OPEX). El ingreso inicial a la organización cliente se realizará a través de un piloto controlado en nodos críticos de la red de alcantarillado, demostrando empíricamente la reducción de los costos operativos (despliegue de cuadrillas de emergencia) como mecanismo de conversión hacia la adopción total del ecosistema de sensores.

**4. Estrategia de Cero Fricción en la Interfaz Operativa (UI/UX)**
  
- **Objetivo Estratégico:** Garantizar la adopción de la herramienta por parte del personal de campo al igual que operarios, mitigando el rechazo que generan los complejos tableros de control diseñados por la competencia exclusivamente para ingenieros de datos.

- **Táctica Ejecutable:** La interfaz de usuario (Front-end) se dividirá metodológicamente. El Back-Office web proveerá la densidad analítica requerida por la gerencia, mientras que el módulo para operadores de campo se construirá bajo principios de Mobile-First. Esta interfaz emitirá notificaciones Push asíncronas, directas, además de accionables, requiriendo un esfuerzo cognitivo mínimo para confirmar la atención de una obstrucción o riesgo biológico en tiempo real.

## 2.2. Entrevistas
Para que Aquanetix logre tener éxito como la aplicación que permitirá reutilizar el agua en estado deficiente, hemos planteado algunas preguntas para las entrevistas que nos pueden ayudar a conocer mejor a nuestros segmentos objetivo.

### 2.2.1. Diseño de entrevistas:
**Bloque de preguntas personales, dirigidas a ambos segmentos:**
1.	¿Cuál es su nombre completo?
2.	¿Cuál es su edad?
3.	¿En qué distrito reside?
4.	¿Cuál es su estado civil? / ¿Cómo está compuesta su familia?
5.	¿A qué se dedica? ¿Estudia o trabaja?
6.	¿Qué dispositivos tecnológicos prefiere utilizar?
7.	¿Cuáles son sus cualidades y debilidades?<br>

**Bloque de preguntas enfocadas en el segmento 1: Empresas prestadoras de servicios de agua y alcantarillados.**
1.	¿Cómo monitorean actualmente la calidad del agua en tiempo real antes de su tratamiento?
2.	¿Qué tan difícil es para la empresa identificar el punto exacto de una anomalía en la red?
3.	¿Cuántas veces al mes atienden emergencias por obstrucciones de flujo no detectadas a tiempo?
4.	¿Cuál es el costo estimado de una reparación de emergencia comparado con una programada?
5.	¿Cómo deciden qué zonas de la red necesitan mantenimiento preventivo?
6.	¿Cuentan con sensores IOT instalados actualmente? Si no, ¿cuál ha sido la principal barrera?
7.	¿Qué herramientas de software utilizan hoy para la gestión de cuadrillas de mantenimiento?<br>

**Bloque de preguntas enfocadas en el segmento 2: Empresas de gestión de residuos sólidos.**
1.	¿De qué manera obtienen actualmente el agua necesaria para sus procesos (lavado de contenedores, limpieza de compactadoras o riego de rellenos)?
2.	¿Qué porcentaje de sus costos operativos mensuales se destina exclusivamente al consumo de agua para actividades de mantenimiento y limpieza?
3.	¿Cómo están gestionando actualmente los lixiviados (líquido de basura)? ¿Cuentan con algún sistema dentro de sus plantas de acopio para tratar con ellos?
4.	¿Han considerado o implementado tecnologías de monitoreo inteligente para medir el nivel de llenado de sus depósitos de agua o residuos en tiempo real?
5.	¿Cuál es el mayor desafío logístico que enfrentan al coordinar la limpieza de grandes flotas de camiones recolectores?
6.	¿Qué herramientas o indicadores utilizan para medir la huella hídrica de sus servicios de gestión de residuos?
7.	Si implementaran un sistema para reutilizar agua en el lavado de su flota, ¿cuánto dinero tendrían que ahorrarse al mes para que consideren que la inversión valió la pena?

### 2.2.2. Registro de entrevistas

**Entrevista 1**

Nombres y Apellidos: Jorge Orellana

Evidencia:

<p align = "left"> <img src="/report/assets/interviews/Entrevista_Jorge_Orellana.png" width ="300" height="300"> </p>

Enlace:
Duración de la entrevista:

Resumen:
La entrevista inicia con la presentación de Jorge Orellana, un trabajador de SEDAPAL de 40 años, quien se encarga de la gestión y mantenimiento de redes de agua potable. En su labor utiliza herramientas como sistemas GIS y ERP básicos para organizar órdenes de trabajo, aunque la comunicación con las cuadrillas aún depende de radios y mensajería.

En cuanto al monitoreo del agua, señala que se realiza mediante muestreos manuales y sensores básicos en plantas, principalmente de pH y turbidez. Sin embargo, el monitoreo en tiempo real dentro de la red es limitado, lo que dificulta detectar anomalías a tiempo.

Uno de los principales desafíos es ubicar el punto exacto de fallas, ya que dependen de indicadores indirectos como cambios de presión o reportes de usuarios. Esto genera retrasos en la atención de problemas.

Finalmente, menciona que atienden entre 15 y 20 emergencias al mes, las cuales pueden costar hasta cuatro veces más que un mantenimiento programado. Destaca que el uso de IoT es aún limitado por costos y falta de infraestructura, pero sería clave para mejorar la eficiencia y anticiparse a fallas.


**Entrevista 2**

Nombres y Apellidos: Jorge Luis Castro Rojas

Evidencia:
<p align = "left">
  <img src="/report/assets/interviews/Entrevista_Jorge_Castro.png" width ="300" height="300">
</p>

Enlace:
Duración de la entrevista:

Resumen:
La entrevista inicia con la presentación de Jorge Luis Castro Rojas, un ingeniero sanitario de 48 años residente en Santiago de Surco. En su labor profesional, Jorge combina herramientas tradicionales con soluciones digitales modernas; utiliza Google Earth para la geolocalización de coordenadas, la plataforma Yorgos para el seguimiento de normativas y aplicaciones móviles como Timestamp Camera, que permite registrar evidencias fotográficas con datos precisos de tiempo y ubicación para sus reportes técnicos. 

En lo referente a la gestión operativa, Jorge destaca el uso del sistema SAP y la inteligencia artificial a través de Copilot para optimizar sus tareas diarias. El control de la calidad del agua es un proceso riguroso que incluye auditorías mensuales de laboratorios acreditados por INACAL y monitoreos diarios de parámetros críticos como el pH, la turbidez y el cloro residual. Sin embargo, el ingeniero señala que la falta de sensores de flujo e IoT en toda la red limita la capacidad de obtener datos en tiempo real.

Uno de los mayores desafíos técnicos mencionados por Jorge es la dificultad para localizar anomalías exactas en la red, como fugas o roturas de tuberías, debido a la carencia de planos digitalizados y mediciones de presión constantes. Actualmente, el mantenimiento preventivo se basa principalmente en la antigüedad de la infraestructura, una estrategia cuyo objetivo es anticiparse al deterioro natural de los materiales antes de que ocurran fallas críticas que comprometan el servicio.

Finalmente, Jorge nos revela que la empresa atiende entre 3 a 5 emergencias mensuales, las cuales representan un reto economico superior al mantenimiento programado especialmente cuando ocurren en días festivos o madrugadas. Él resalta que la integración de nuevas aplicaciones y tecnologías de monitoreo en línea sería fundamental para transformar la respuesta reactiva en una gestión proactiva, mejorando significativamente la eficiencia del servicio de agua y alcantarillado.

**Entrevista 3**

Nombres y Apellidos: Liliana del Pilar Sanchez Fajardo

Evidencia:
<p align = "left">
   <img src="/report/assets/interviews/Entrevista_Liliana_Sanchez.png" width ="300" height="600">
</p>
Enlace:
Duración de la entrevista:

Resumen:
Nos reunimos con Liliana de Pilar Sánchez Bajardo, residente del distrito de Comas, de 57 años, quien se desempeña como ingeniera ambiental y consultora en temas vinculados a la gestión del recurso hídrico. En su labor diaria utiliza principalmente la laptop y el teléfono celular para la coordinación de actividades. Entre sus principales cualidades destacó la responsabilidad, la puntualidad y el trabajo en equipo, mientras que señaló como debilidades su tendencia al perfeccionismo y su baja tolerancia frente a la impuntualidad y la falta de compromiso del personal.

En relación con el monitoreo de la calidad del agua, indicó que este se realiza mayormente mediante muestreos en puntos específicos de la red, complementados con sensores básicos en planta para medir parámetros como pH y turbidez. No obstante, señaló que el monitoreo en tiempo real a lo largo de toda la red de tuberías es limitado, lo que dificulta una supervisión continua. Asimismo, explicó que identificar el origen exacto de una anomalía resulta complejo, ya que muchas veces los problemas se detectan cuando disminuye la presión del agua o a partir de reportes de los usuarios.

Respecto a la operación del sistema, mencionó que se atienden aproximadamente entre 15 y 20 emergencias mensuales por obstrucciones de flujo no detectadas a tiempo, muchas de las cuales podrían prevenirse con una mayor incorporación de tecnología. También señaló que las reparaciones de emergencia implican costos considerablemente más altos que las programadas, debido a la urgencia, el uso de recursos adicionales y los posibles daños colaterales.

Finalmente, indicó que el mantenimiento preventivo se planifica principalmente en función de la antigüedad de las tuberías y el historial de fallas reportadas. Señaló que el uso de sensores inteligentes es aún limitado debido al alto costo de implementación y a los problemas de conectividad en redes subterráneas. Si bien se emplean sistemas como GIS y herramientas básicas de gestión, la comunicación con las cuadrillas se realiza mayormente por radio o aplicaciones de mensajería, lo que evidencia la necesidad de soluciones tecnológicas más integradas para mejorar la eficiencia operativa y reducir el impacto en la comunidad.


#### Segmento 2: Empresas gestoras de residuos sólidos
**Entrevista 1**

Edward Fernando Bojórquez Gonzales

Evidencia:
<p align = "left">
 <img src="/report/assets/interviews/Entrevista_Fernando_Foto.png" width ="300" height="300">
</p>

Enlace:

Duración de la entrevista:

Resumen:

Nos encontramos con Edward Fernando Bojórquez Gonzales, ciudadano del distrito de Lince, y administrador de una empresa de residuos sólidos. Tiene 56 años, es casado, y vive con su esposa e hijo. Prefiere el uso de laptops y computadoras personales, y es alguien organizado, metódico y orientado al trabajo en equipo, aunque también reconoce que no tiene mucha paciencia.

Primero, a Fernando se le preguntó de dónde obtenía el agua para sus procesos de lavado, y nos comentó que en su trabajo se apoya de la red pública de SEDAPAL para el lavado de unidades de transporte y contenedores. Además, si bien no cuentan con una planta de tratamiento de agua propia, reciben apoyo de otra empresa proveedora que maneja la recolección y tratamiento de lixiviados. Dentro de todo, el consumo de agua representa entre el 15% y 20% de los costos mensuales de la empresa.

Respecto al tema del monitoreo y sostenibilidad, él comentó que no utilizan sistemas inteligentes en tiempo real, sino que realizan mediciones volumétricas del caudal mediante equipos convencionales. Asimismo, utilizan la metodología del Water Footprint Network para medir su huella hidríca, predominando la huella azul, y para su caso predomina la huella azul, que representa el consumo de recursos hídricos superficiales y subterráneos.

Por último, Fernando nos mencionó que su mayor desafío logístico en su trabajo es optimizar el tiempo de lavado y mantenimiento de las unidades para cumplir con los cronogramas de los clientes. Asimismo, demostró interés en la implementación de sistemas de reutilización de agua que Aquanetix ofrece, siempre que generen un ahorro de entre el 30% y 40% de los costos actuales, lo cual justificaría la inversión y ayudaría a mejorar la eficiencia operativa.

**Entrevista 2**

Nombres y apellidos: José Ignacio Calle Chumacero

Evidencia:
<p align = "left">
  <img src="/report/assets/interviews/Entrevista_Jose_Ignacio_Foto.png" width ="300" height="300">
</p>

Enlace:

Duración de la entrevista:

Resumen:

Nos encontramos con José Ignacio Calle Chumacero, residente del distrito de Jesús María, y jefe de operaciones en RESITER Perú SAC. Tiene 33 años, y convive con su pareja y con sus dos hijos. Entre sus tecnologías preferidas están la laptop y el teléfono, así como IAs como ChatGPT, y es una persona puntual, responsable y dispuesta a mantener un compromiso, aunque también reconoce que presenta dificultades para cumplir con su agenda programada.

Para empezar, a José Ignacio se le preguntó sobre cómo conseguían el agua para los procesos de lavado, y él respondió que tercerizaban dicho proceso con la ayuda de una empresa aliada estratégica ubicada cerca de las rutas de sus clientes. Asimismo, respecto al tratado de lixiviados explicó que diseñan contenedores especiales con válvulas para separar el líquido sucio del sólido, enviando el líquido directamente a las rejillas de la planta del cliente para evitar el transporte de residuos húmedos. Dentro de todo, los gastos en agua y limpieza representan alrededor del 20% y 25% de sus costos operativos.

En cuanto a recursos tecnológicos, comentó que realizaron un plan piloto de monitoreo de llenado de contenedores en 2025, pero falló debido a lecturas incorrectas de los sensores, y por ello el proyecto está en pausa. Además, poseen un área de “Economía Circular” que ofrece asesoría “Cero Residuos” a sus clientes para monitorear su huella de carbono e hídrica.

Por último, José Ignacio destacó que el mayor desafío que enfrentan en su trabajo es el factor tiempo, pues la logística de lavado puede retrasar los servicios, por lo que buscan eficiencia en este proceso. Por ello, considerarían exitoso un sistema de reutilización de agua si este lograra un ahorro mínimo de 20,000 soles mensuales, lo cual justificaría la inversión tecnológica.

**Entrevista 3**

Cristian Qquecano De la Sota

Evidencia:
<p align = "left">
   <img src="/report/assets/interviews/Entrevista_Cristian_foto.jfif" width ="300" height="600">
</p>

Enlace:

Duración de la entrevista:

Resumen: 

Nos reunimos con Cristian Qquecano de la Sota. Él es un ingeniero ambiental de 38 años, reside en Jesús María, actualmente está soltero. Trabaja como supervisor de operaciones. Para sus labores diarias prefiere usar su celular Android, además de una laptop. Se considera una persona bastante organizada; sin embargo, confiesa estresarse mucho ante cambios repentinos de planes.

Durante nuestra conversación, explicó lo complicado de conseguir agua para el lavado de flota. La red pública resulta ineficiente. Por tal motivo, dependen de comprar camiones cisterna constantemente. Este gasto, sumado al canon por vertimientos, representa entre el 8% hasta el 12% del presupuesto operativo mensual.

Sobre el manejo de lixiviados, indicó que los almacenan en pozas de sedimentación. Tratar esos líquidos cuesta demasiado; por ello, prefieren pagar a plantas externas especializadas. Al consultarle sobre tecnologías de monitoreo inteligente, nos contó sobre algunas evaluaciones previas con sensores de ultrasonido. Lamentablemente, dichas iniciativas fueron incipientes, quedando relegadas a simples proyectos piloto. Su mayor dolor de cabeza diario es el tiempo de inactividad vehicular. Lavar 50 camiones pesados sin afectar las rutas nocturnas de recolección resulta un verdadero caos logístico. Respecto a la huella hídrica, admitió una falta total de estandarización. Apenas utilizan indicadores muy básicos basados en dividir los litros consumidos entre las toneladas de basura.

Finalmente, Cristian concluyó que cualquier sistema tecnológico de reutilización hídrica debe demostrar resultados contundentes. Para convencer a la gerencia, dicha inversión necesitaría garantizar un ahorro del 25% al 30% mensual, reduciendo facturas de consumo junto con los costos logísticos de cisternas.

### Análisis de entrevistas

#### Segmento 1: Empresas prestadoras de servicios de agua y alcantarillado.

#### Segmento 2: Empresas gestoras de residuos sólidos

Este análisis consolida los hallazgos de los entrevistados pertenecientes a este segmento, representados mediante porcentajes, empezando por las características objetivas:

> * El 100% de los participantes utiliza de forma mandatoria laptops y smartphones para la supervisión de operaciones. Un 67% muestra una adopción activa de herramientas de software avanzado o IA para optimizar su flujo de trabajo.
> * Los tres entrevistados ha reconocido el impacto financiero que posee el agua en sus trabajos. Combinando red pública, cisternas y vertimientos, el gasto en agua y limpieza es una carga crítica, representando en promedio entre el 14% y el 19% de los costos operativos mensuales.
> * El 100% de los entrevistados ha operado bajo sistemas convencionales o ha tenido experiencias fallidas con proyectos piloto (sensores de llenado o ultrasonido), lo cual genera una brecha tecnológica latente.
> * El 67% de los casos depende de proveedores externos para el tratamiento de lixiviados o el suministro de agua (cisternas), evidenciando una falta de autonomía hídrica.
> * Existe una brecha significativa en la medición de la huella hídrica, pues el 67% utiliza indicadores técnicos (estándares internacionales o ratios litros/tonelada), mientras que el 33% reconoce una falta total de estandarización en sus reportes de la misma.
> * Por último, para que la gerencia apruebe la implementación de Aquanetix, los expertos coinciden en que se debe garantizar un ahorro mínimo de entre el 25% y 40%.

Pasando a las características subjetivas, analizaremos los Pain Points de nuestros usuarios.
> * El 100% de los entrevistados manifiesta una preocupación crítica por el factor tiempo. El miedo a los retrasos operativos o al "caos logístico" por el lavado de flota es el principal movilizador emocional.
> * El 67% de los sujetos presenta un sesgo de escepticismo hacia nuevas implementaciones IoT. Este sentimiento nace de frustraciones pasadas con sensores que brindaron lecturas incorrectas o proyectos que quedaron en "pilotos incipientes".
> * El 33% expresa una frustración directa por la ineficiencia de los servicios públicos, lo que les genera una sensación de falta de control sobre sus propios procesos.

Respecto a los Gains de nuestros usuarios:
> * El 100% condiciona su satisfacción con el sistema a un ahorro económico tangible. La motivación subjetiva aquí es la "validación ante la gerencia"; necesitan que la tecnología sea una victoria financiera demostrable.
> * El 67% de los entrevistados muestra un compromiso intrínseco con la economía circular y la reducción de la huella hídrica, viendo en la tecnología una forma de alinear sus valores personales con los objetivos de la empresa.
> * El 66% valora la organización y la puntualidad por encima de otras cualidades. Su expectativa subjetiva frente a una aplicación que los ayude es que los ayude a reducir los cambios repentinos de planes causados por falta de agua o fallos logísticos.

## 2.3. Needfinding
### 2.3.1. User Personas

#### Segmento 1: Empresas prestadoras de servicios de agua y alcantarillado

#### Segmento 2: Empresas gestoras de residuos sólidos
<p align = "left">
  <img src="/report/assets/ux_pressia/Ricardo Sánchez's User Persona.png">
</p>

### 2.3.2. Task Matrix

#### User Persona 2: Ricardo Sánchez

| Tasks | Nombre: | Ricardo Sánchez |
| :--- | :--- | :--- |
|| Frecuencia: | Importancia: |
| Monitoreo de niveles de agua en tiempo real | Muy alta | Muy alta |
| Revisión de alertas de calidad de agua | Muy alta | Muy alta |
| Generación de reportes de ahorro (Return Of Investment) | Media | Alta |
| Consulta de indicadores de Huella Hídrica | Baja | Media |
| Verificación de estado de sensores | Alta | Muy alta |
| Ajuste de parámetros de reutilización | Baja | Media |

Las tareas más críticas para Ricardo son aquellas relacionadas con el monitoreo operativo y la fiabilidad del sistema, como la supervisión de niveles de agua en tiempo real y la verificación de alertas de calidad para evitar daños en la flota. Estas actividades son de frecuencia muy alta.

Su motivación central es la validación profesional y la paz mental, buscando garantizar un ahorro económico contundente que justifique la inversión ante la gerencia y le permita cumplir con sus cronogramas sin imprevistos.

En general, sus tareas reflejan un compromiso con la eficiencia y la sostenibilidad rentable, buscando transformar la gestión hídrica de la empresa a través de la automatización y el ejemplo de resultados medibles.

### 2.3.3. Journey Mapping

#### User Persona 1: 

#### User Persona 2: Ricardo Sánchez
<p align = "left">
  <img src="/report/assets/ux_pressia/Ricardo Sanchez's Journey Map.png">
</p>

### 2.3.4. Empathy Mapping

#### User Persona 1:

#### User Persona 2: Ricardo Sánchez
<p align = "left">
  <img src="/report/assets/ux_pressia/Ricardo Sánchez's Empathy Map.png">
</p>

### 2.4. Big Picture EventStorming

### 2.5. Ubiquitous Language

Usuario (User):
Profesional de empresas prestadoras de servicios de agua o gestión de residuos que utiliza Aquanetix para monitorear y gestionar la red hidráulica.
Términos relacionados: Operador, Supervisor, Perfil de usuario.

Operador (Operator):
Usuario encargado de supervisar los datos en tiempo real y gestionar alertas dentro del sistema.
Términos relacionados: Monitoreo, Alerta, Sensor.

Supervisor (Supervisor):
Usuario responsable de analizar la información del sistema y tomar decisiones operativas y estratégicas.
Términos relacionados: Reporte, Dashboard, Mantenimiento.

Sensor IoT (IoT Sensor):
Dispositivo instalado en la red hidráulica que mide variables como pH, flujo y gases.
Términos relacionados: Datos del sensor, Monitoreo, Parámetros del agua.

Monitoreo (Monitoring):
Proceso de seguimiento continuo de los parámetros del agua en tiempo real.
Términos relacionados: Datos del sensor, Dashboard, Red hidráulica.

Alerta (Alert):
Notificación generada cuando se detecta una anomalía en los parámetros del sistema.
Términos relacionados: Anomalía, Umbral, Incidencia.

Anomalía (Anomaly):
Variación fuera de los valores normales en los parámetros del agua.
Términos relacionados: Alerta, Monitoreo, Zona crítica.

Mantenimiento (Maintenance):
Acciones realizadas para prevenir o corregir fallas en la red hidráulica.
Términos relacionados: Zona crítica, Incidencia, Planificación.

Agua Reutilizable (Reusable Water):
Agua residual que cumple con los parámetros necesarios para su reutilización.
Términos relacionados: Validación de reutilización, Parámetros del agua.

Validación de Reutilización (Reuse Validation):
Proceso de verificación de que el agua cumple con las condiciones para ser reutilizada.
Términos relacionados: Agua reutilizable, Monitoreo, Parámetros.

Asignación de Agua (Water Allocation):
Distribución del agua reutilizada hacia procesos o sectores que la requieren.
Términos relacionados: Agua reutilizable, Logística, Reutilización.

Plataforma Aquanetix (Platform):
Sistema web que integra sensores IoT para monitorear, analizar y gestionar la red hidráulica y la reutilización del agua.
Términos relacionados: Dashboard, Monitoreo, Alertas.

## Referencias bibliográficas
- Autoridad Nacional del Agua (ANA). (2025). Plan estratégico 2025–2030. https://www.ana.gob.pe/sites/default/files/file_content/PLAN%20ESTRATEGICO%202025-2030.pdf 

- Autoridad Nacional del Agua (ANA). (2026). ANA promueve el reúso de aguas residuales para fortalecer la gestión sostenible del recurso hídrico. [Nota de prensa]. https://www.gob.pe/institucion/ana/noticias/1368267-ana-promueve-el-reuso-de-aguas-residuales-para-fortalecer-la-gestion-sostenible-del-recurso-hidrico

- Banco Mundial (2025, 30 de setiembre). Perú avanzará en estrategias de gestión de aguas residuales y economía circular con un programa del Banco Mundial de $200 millones. Grupo Banco Mundial. Recuperado el 30 de setiembre de 2025, de https://www.bancomundial.org/es/news/press-release/2025/10/01/peru-to-advance-wastewater-management-and-circular-economy-strategies-with-200-million-world-bank-program 

- European Commission. (2023). Solid waste management in Peru. Access to Markets. https://trade.ec.europa.eu/access-to-markets/en/country-assets/pe_solid_waste.pdf 

- Instituto Nacional de Estadística e Informática (INEI). (2023). Perú: Formas de acceso al agua y saneamiento básico – N° 10. https://www.gob.pe/institucion/inei/informes-publicaciones/4985657-peru-formas-de-acceso-al-agua-y-saneamiento-basico-nro-10 

- Organismo de Evaluación y Fiscalización Ambiental (OEFA). (2024). OEFA puede sancionar hasta con más de S/ 128 millones de soles a administrados que contaminen el aire. [Nota de prensa]. https://www.gob.pe/institucion/oefa/noticias/1001222-oefa-puede-sancionar-hasta-con-128-millones-de-soles-a-administrados-que-contaminen-el-aire 

- Superintendencia Nacional de Servicios de Saneamiento [SUNASS]. (2025, 16 de abril). Perú necesita S/138 mil millones para cerrar brechas en agua potable y saneamiento en el ámbito de las empresas prestadoras. https://www.gob.pe/institucion/sunass/noticias/1147343-peru-necesita-s-138-mil-millones-para-cerrar-brechas-en-agua-potable-y-saneamiento-en-el-ambito-de-las-empresas-prestadoras
