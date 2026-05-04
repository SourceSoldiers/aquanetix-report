# Capítulo III: Requirements Specification

<h3>Epics</h3>

<table>
  <thead>
    <tr>
      <th>Epic ID</th>
      <th>Título</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>EP01</td>
      <td>Configuración del sistema de monitoreo</td>
      <td>Permite definir parámetros, condiciones y configuraciones necesarias para el funcionamiento del monitoreo y la detección de anomalías en la red.</td>
    </tr>
    <tr>
      <td>EP02</td>
      <td>Monitoreo en tiempo real</td>
      <td>Permite visualizar datos de sensores IoT (pH, flujo y gases) en tiempo real para la supervisión de la red.</td>
    </tr>
    <tr>
      <td>EP03</td>
      <td>Gestión de alertas</td>
      <td>Permite detectar anomalías en los parámetros del agua y generar alertas automáticas para prevenir riesgos.</td>
    </tr>
    <tr>
      <td>EP04</td>
      <td>Mantenimiento preventivo</td>
      <td>Permite identificar patrones de fallas y zonas críticas para optimizar la planificación del mantenimiento.</td>
    </tr>
    <tr>
      <td>EP05</td>
      <td>Dashboard y visualización</td>
      <td>Permite visualizar información consolidada mediante gráficos e indicadores para la toma de decisiones.</td>
    </tr>
    <tr>
      <td>EP06</td>
      <td>Gestión de reutilización de agua</td>
      <td>Permite identificar, validar y gestionar el uso de agua tratada para su reutilización en procesos operativos.</td>
    </tr>
    <tr>
      <td>EP07</td>
      <td>Reportes y análisis</td>
      <td>Permite generar reportes históricos y métricas que apoyen la evaluación del desempeño del sistema.</td>
    </tr>
    <tr>
      <td>EP08</td>
      <td>Landing Page informativa</td>
      <td>Permite presentar información del producto, beneficios y propuesta de valor a potenciales clientes.</td>
    </tr>
    <tr>
      <td>EP09</td>
      <td>Control de acceso por suscripción</td>
      <td>Permite manejar el acceso a los usuarios a la aplicación mediante una suscripción.</td>
    </tr>
  </tbody>
</table>


<h3>User Stories</h3>

<table>
  <thead>
    <tr>
      <th>Epic / Story ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>Relacionado con (Epic ID)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>US01</td>
      <td>Suscripción Automatizada y Control de Acceso</td>
      <td>Como operador técnico, quiero realizar el pago de mi suscripción mensual a través de una pasarela segura, para obtener acceso inmediato a los tableros de control y reportes de calidad del agua.</td>
      <td>Given que el operador registrado ha elegido una suscripción mensual. When el usuario ingresa una tarjeta válida y confirma la transacción a través de la pasarela de Stripe. Then el sistema debe recibir la confirmación de pago y actualizar el estado del usuario a activo en la base de datos.</td>
      <td>EP09</td>
    </tr>
    <tr>
      <td>US02</td>
      <td>Configuración de reglas de alerta</td>
      <td>Como operador técnico, quiero establecer condiciones de alerta para recibir notificaciones ante eventos críticos.</td>
      <td>Given existen umbrales definidos en el sistema. When el operador configura una regla de alerta. Then el sistema genera alertas cuando se cumplen las condiciones establecidas</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US03</td>
      <td>Ajuste de frecuencia de monitoreo</td>
      <td>Como operador técnico, quiero definir la frecuencia de captura de datos de los sensores para optimizar el monitoreo.</td>
      <td>Given el sistema cuenta con sensores activos. When el operador establece la frecuencia de monitoreo. Then el sistema aplica la periodicidad configurada para la recolección de datos</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US04</td>
      <td>Configuración de visualización del monitoreo</td>
      <td>Como usuario, quiero configurar la visualización de los datos para facilitar el análisis de la información.</td>
      <td>Given el usuario accede a la configuración de visualización. When selecciona los datos que desea visualizar. Then el sistema muestra la información según la configuración definida</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US05</td>
      <td>Visualización de datos en tiempo real</td>
      <td>Como operador técnico, quiero visualizar los datos de pH, flujo y gases en tiempo real para supervisar el estado de la red.</td>
      <td>Given el sistema recibe datos de sensores activos. When el operador accede al módulo de monitoreo. Then el sistema muestra los valores actualizados en tiempo real</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US06</td>
      <td>Monitoreo por zona crítica</td>
      <td>Como operador técnico, quiero consultar los datos de monitoreo por zona para identificar áreas con mayor riesgo operativo.</td>
      <td>Given existen sensores asociados a distintas zonas de la red. When el operador selecciona una zona específica. Then el sistema muestra los datos correspondientes a dicha zona</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US07</td>
      <td>Identificación de variaciones anómalas</td>
      <td>Como operador técnico, quiero detectar variaciones anómalas en los parámetros monitoreados para actuar antes de que ocurra una falla.</td>
      <td>Given el sistema monitorea continuamente los valores de los sensores. When se detecta una variación fuera de los rangos establecidos. Then el sistema marca el evento como anomalía</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US08</td>
      <td>Renovación automática de suscripción</td>
      <td>Como usuario, quiero que el sistema gestione la renovación automática de mi suscripción, para evitar interrupciones en el monitoreo de mis sensores y en la programación de mis pedidos de agua.</td>
      <td>Given que el cliente tiene una suscripción activa con la opción de renovación automática habilitada. When el sistema detecta que faltan 24 horas para el vencimiento del periodo contratado. Then el sistema debe realizar el cobro automático a través de Stripe y extender la vigencia del servicio.</td>
      <td>EP09</td>
    </tr>
    <tr>
      <td>US09</td>
      <td>Actualización automática de datos</td>
      <td>Como operador técnico, quiero que los datos del monitoreo se actualicen automáticamente para mantener información vigente durante la supervisión.</td>
      <td>Given el sistema recibe nuevos datos de sensores. When la información cambia. Then el sistema actualiza los valores mostrados sin intervención manual</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US10</td>
      <td>Consulta de historial reciente de monitoreo</td>
      <td>Como operador técnico, quiero revisar el historial reciente de los sensores para comparar cambios en el comportamiento de la red.</td>
      <td>Given el sistema almacena registros recientes de monitoreo. When el operador consulta el historial de un sensor o zona. Then el sistema muestra los datos registrados en el periodo reciente</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US11</td>
      <td>Generación automática de alertas</td>
      <td>Como operador técnico, quiero que el sistema genere alertas automáticas cuando detecte valores críticos para actuar oportunamente ante riesgos en la red.</td>
      <td>Given el sistema monitorea datos de pH, flujo y gases. When un valor supera los umbrales configurados. Then el sistema genera una alerta automáticamente</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US12</td>
      <td>Clasificación de alertas por nivel de riesgo</td>
      <td>Como operador técnico, quiero que las alertas se clasifiquen según su nivel de riesgo para priorizar la atención de incidencias.</td>
      <td>Given el sistema detecta una anomalía. When genera la alerta correspondiente. Then el sistema la clasifica según el nivel de riesgo definido</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US13</td>
      <td>Consulta de alertas activas</td>
      <td>Como supervisor, quiero consultar las alertas activas para identificar rápidamente los eventos que requieren atención inmediata.</td>
      <td>Given existen alertas generadas en el sistema. When el supervisor consulta las alertas activas. Then el sistema muestra únicamente las alertas que se encuentran vigentes</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US14</td>
      <td>Registro del historial de alertas</td>
      <td>Como supervisor, quiero acceder al historial de alertas para analizar incidentes previos y mejorar la toma de decisiones operativas.</td>
      <td>Given el sistema genera alertas durante la operación. When el supervisor consulta el historial. Then el sistema muestra el registro de alertas emitidas anteriormente</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US15</td>
      <td>Marcado de alertas atendidas</td>
      <td>Como operador técnico, quiero marcar alertas como atendidas para llevar control sobre las incidencias resueltas en la red.</td>
      <td>Given existe una alerta activa en el sistema. When el operador registra su atención. Then el sistema actualiza el estado de la alerta como atendida</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US16</td>
      <td>Identificación de zonas críticas</td>
      <td>Como operador técnico, quiero identificar zonas con mayor riesgo de fallas para priorizar acciones de mantenimiento.</td>
      <td>Given el sistema analiza datos históricos de monitoreo. When detecta patrones de riesgo en una zona. Then el sistema identifica dicha zona como crítica</td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US17</td>
      <td>Recomendación de mantenimiento preventivo</td>
      <td>Como operador técnico, quiero recibir recomendaciones de mantenimiento para prevenir fallas en la red.</td>
      <td>Given el sistema detecta condiciones de riesgo. When analiza tendencias en los datos. Then el sistema genera recomendaciones de mantenimiento</td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US18</td>
      <td>Programación de intervenciones</td>
      <td>Como supervisor, quiero programar intervenciones de mantenimiento para organizar las actividades operativas.</td>
      <td>Given existe una zona identificada como crítica. When el supervisor agenda una intervención. Then el sistema registra la programación del mantenimiento</td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US19</td>
      <td>Seguimiento de mantenimiento realizado</td>
      <td>Como supervisor, quiero registrar y consultar las intervenciones realizadas para evaluar la efectividad del mantenimiento.</td>
      <td>Given se ha realizado una intervención en la red. When el supervisor registra la acción. Then el sistema almacena el historial de mantenimiento</td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US20</td>
      <td>Visualización de indicadores clave</td>
      <td>Como supervisor, quiero visualizar indicadores clave del sistema para evaluar el estado general de la operación.</td>
      <td>Given el sistema procesa datos de monitoreo. When el supervisor accede al dashboard. Then el sistema muestra indicadores clave actualizados</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US21</td>
      <td>Visualización gráfica de datos</td>
      <td>Como usuario, quiero ver gráficos de los datos monitoreados para interpretar tendencias de manera clara.</td>
      <td>Given existen datos históricos de monitoreo. When el usuario accede a la sección de visualización. Then el sistema muestra los datos en formato gráfico</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US22</td>
      <td>Filtrado de información por zona y tiempo</td>
      <td>Como usuario, quiero filtrar los datos por zona y periodo de tiempo para analizar información específica.</td>
      <td>Given existen datos de monitoreo registrados. When el usuario aplica filtros por zona o tiempo. Then el sistema muestra la información correspondiente a los filtros seleccionados</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US23</td>
      <td>Visualización del estado general del sistema</td>
      <td>Como supervisor, quiero visualizar el estado general del sistema para identificar rápidamente situaciones críticas.</td>
      <td>Given el sistema consolida información de múltiples sensores. When el supervisor accede al dashboard principal. Then el sistema muestra un resumen del estado general de la red</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US24</td>
      <td>Personalización de vistas del dashboard</td>
      <td>Como usuario, quiero personalizar la visualización del dashboard para priorizar la información relevante para mi operación.</td>
      <td>Given el usuario accede a la configuración del dashboard. When selecciona los elementos que desea visualizar. Then el sistema guarda y aplica la configuración personalizada</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US25</td>
      <td>Identificación de agua reutilizable</td>
      <td>Como operador técnico, quiero identificar cuando el agua cumple parámetros adecuados para su reutilización para aprovechar el recurso disponible.</td>
      <td>Given el sistema monitorea parámetros de calidad del agua. When los valores cumplen los estándares definidos. Then el sistema identifica el agua como apta para reutilización</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US26</td>
      <td>Validación de condiciones de reutilización</td>
      <td>Como operador técnico, quiero validar que el agua cumpla condiciones específicas antes de su reutilización para garantizar su uso seguro.</td>
      <td>Given el sistema detecta agua potencialmente reutilizable. When se evalúan los parámetros definidos. Then el sistema confirma si el agua cumple con las condiciones requeridas</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US27</td>
      <td>Registro de volúmenes reutilizables</td>
      <td>Como operador técnico, quiero registrar el volumen de agua reutilizable para gestionar su disponibilidad.</td>
      <td>Given el agua ha sido validada como reutilizable. When el sistema procesa los datos. Then registra el volumen disponible para reutilización</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US28</td>
      <td>Gestión de disponibilidad de agua reutilizada</td>
      <td>Como operador, quiero visualizar la disponibilidad de agua reutilizable para planificar su uso en operaciones.</td>
      <td>Given existen volúmenes de agua reutilizable registrados. When el operador consulta la disponibilidad. Then el sistema muestra la cantidad de agua disponible</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US29</td>
      <td>Asignación de agua reutilizada a operaciones</td>
      <td>Como operador, quiero asignar agua reutilizable a procesos operativos para reducir el consumo de agua potable.</td>
      <td>Given existe agua disponible para reutilización. When el operador la asigna a una operación. Then el sistema registra la asignación realizada</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US30</td>
      <td>Seguimiento del uso de agua reutilizada</td>
      <td>Como supervisor, quiero hacer seguimiento del uso de agua reutilizada para evaluar el impacto en la operación.</td>
      <td>Given el sistema registra el uso de agua reutilizada. When el supervisor consulta la información. Then el sistema muestra el historial de utilización</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US31</td>
      <td>Generación de reportes operativos</td>
      <td>Como supervisor, quiero generar reportes operativos para evaluar el desempeño del sistema de monitoreo.</td>
      <td>Given el sistema almacena datos de monitoreo. When el supervisor solicita un reporte. Then el sistema genera un reporte con la información requerida</td>
      <td>EP07</td>
    </tr>
    <tr>
      <td>US32</td>
      <td>Análisis de tendencias de datos</td>
      <td>Como supervisor, quiero analizar tendencias en los datos para identificar patrones de comportamiento en la red.</td>
      <td>Given existen datos históricos registrados. When el supervisor analiza los datos. Then el sistema muestra tendencias en el comportamiento de los parámetros</td>
      <td>EP07</td>
    </tr>
    <tr>
      <td>US33</td>
      <td>Reporte de incidencias</td>
      <td>Como supervisor, quiero consultar reportes de incidencias para evaluar la frecuencia de eventos críticos en la red.</td>
      <td>Given el sistema registra alertas e incidencias. When el supervisor consulta el reporte. Then el sistema muestra el historial de eventos críticos</td>
      <td>EP07</td>
    </tr>
    <tr>
      <td>US34</td>
      <td>Reporte de impacto en reutilización de agua</td>
      <td>Como supervisor, quiero visualizar el impacto del uso de agua reutilizada para evaluar los beneficios operativos y ambientales.</td>
      <td>Given el sistema registra el uso de agua reutilizada. When el supervisor consulta el reporte de impacto. Then el sistema muestra indicadores relacionados al uso y ahorro generado</td>
      <td>EP07</td>
    </tr>
    <tr>
      <td>US35</td>
      <td>Visualización de información del producto</td>
      <td>Como visitante, quiero conocer la propuesta de valor del sistema para entender sus beneficios.</td>
      <td>Given el visitante accede a la landing page. When navega por la página. Then el sistema muestra información clara sobre la solución y sus beneficios</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US36</td>
      <td>Visualización de funcionalidades del sistema</td>
      <td>Como visitante, quiero visualizar las funcionalidades del sistema para comprender cómo resuelve el problema.</td>
      <td>Given el visitante accede a la landing page. When revisa la sección de funcionalidades. Then el sistema muestra las características principales del producto</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US37</td>
      <td>Acceso a información de contacto o interés</td>
      <td>Como visitante, quiero acceder a información de contacto para solicitar más información sobre el sistema.</td>
      <td>Given el visitante se encuentra en la landing page. When desea contactar o mostrar interés. Then el sistema proporciona un medio para establecer contacto</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US38</td>
      <td>Configuración de rangos de seguridad para pH</td>
      <td>Como operador técnico, quiero definir los límites superior e inferior de pH para detectar niveles de acidez o alcalinidad que puedan corroer la tubería o violar normativas ambientales.</td>
      <td>Given el operador se encuentra en el panel de "Configuración de Sensores Químicos", When eloperador ingresa un valor mínimo y un valor máximo. Then el sistema valida que el valor mínimo sea menor al máximo y guarda los umbrales.<br>
      Given el operador se encuentra en el panel de "Configuración de Sensores Químicos", When el operador ingresa un valor mínimo y un valor máximo. Then se activa una alerta visual si el sensor reporta valores fuera de ese rango.</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US39</td>
      <td>Configuración de límites de caudal para detección de fugas u obstrucciones.</td>
      <td>Como operador técnico, quiero establecer el flujo nominal y los márgenes de tolerancia para identificar fugas (caída de presión) o taponamientos (sobrepresión).</td>
      <td>Given el operador accede a la sección de "Parámetros Hidráulicos", When el operador define el umbral de "Flujo Crítico Bajo" (posible fuga) y "Flujo Crítico Alto" (obstrucción o sobrecarga). Then el sistema registra los valores en $L/s$ (litros por segundo).</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US40</td>
      <td>Configuración de niveles de alerta para gases inflamables/tóxicos.</td>
      <td>Como operador técnico, quiero definir la concentración máxima permitida de gases (como $H_2S$ o $CH_4$) para prevenir explosiones o intoxicaciones en la red.</td>
      <td>Given el operador está en el módulo de "Seguridad Atmosférica". When define el umbral de Pre-alarma y Alarma Crítica. Then el sistema guarda la configuración y asegura que estos valores no puedan ser desactivados sin una clave de supervisor. And al superar el umbral crítico, el sistema debe habilitar automáticamente el protocolo de ventilación (si está integrado).</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US41</td>
      <td>Monitoreo en tiempo real mediante mapa interactivo.</td>
      <td>Como supervisor, quiero visualizar la ubicación geográfica de todos los nodos de la red en un mapa para identificar rápidamente qué zonas presentan estados críticos (alerta/alarma).</td>
      <td>Given el supervisor registrado accede al mapa. When el sistema carga las coordenadas de los sensores IoT. Then se muestran marcadores con código de colores: verde (normal), amarillo (advertencia) y rojo (crítico).</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US42</td>
      <td>Consulta de gráficas de comportamiento temporal.</td>
      <td>Como supervisor, quiero consultar gráficas de tendencias de los sensores en rangos de tiempo específicos para detectar patrones de degradación en la calidad del agua.</td>
      <td>Given el supervisor selecciona un nodo o sector específico. When el supervisor filtra por un rango de fechas y un tipo de sensor. Then el sistema renderiza un gráfico de líneas que muestra la evolución del parámetro frente a los umbrales configurados.</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US43</td>
      <td>Consolidado de alertas operativas pendientes.</td>
      <td>Como supervisor, quiero ver un listado priorizado de todas las anomalías activas en la red para asignar equipos de mantenimiento de manera eficiente.</td>
      <td>Given que existen condiciones de sensores que superan los umbrales definidos en la configuración. When el supervisor accede al panel de alertas. Then el sistema muestra una tabla con: ID del sensor, ubicación, tipo de anomalía, y severidad.</td>
      <td>EP02</td>
    </tr>
  </tbody>
</table>
