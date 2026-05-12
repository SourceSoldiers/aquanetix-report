# Capítulo III: Requirements Specification

## 3.1. User Stories

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
      <td>EP01</td>
      <td>Configuración del sistema de monitoreo</td>
      <td>Permite definir parámetros, condiciones y configuraciones necesarias para el funcionamiento del monitoreo y la detección de anomalías en la red.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
      <tr>
      <td>EP02</td>
      <td>Monitoreo en tiempo real</td>
      <td>Permite visualizar datos de sensores IoT (pH, flujo y gases) en tiempo real para la supervisión de la red.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP03</td>
      <td>Gestión de alertas</td>
      <td>Permite detectar anomalías en los parámetros del agua y generar alertas automáticas para prevenir riesgos.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP04</td>
      <td>Mantenimiento preventivo</td>
      <td>Permite identificar patrones de fallas y zonas críticas para optimizar la planificación del mantenimiento.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP05</td>
      <td>Dashboard y visualización</td>
      <td>Permite visualizar información consolidada mediante gráficos e indicadores para la toma de decisiones.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP06</td>
      <td>Gestión de reutilización de agua</td>
      <td>Permite identificar, validar y gestionar el uso de agua tratada para su reutilización en procesos operativos.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP07</td>
      <td>Reportes y análisis</td>
      <td>Permite generar reportes históricos y métricas que apoyen la evaluación del desempeño del sistema.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP08</td>
      <td>Landing Page informativa</td>
      <td>Permite presentar información del producto, beneficios y propuesta de valor a potenciales clientes.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
     <td>EP09</td>
      <td>Control de acceso por suscripción</td>
      <td>Maneja el acceso a los usuarios a la aplicación mediante una suscripción.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>US01</td>
      <td>Suscripción Automatizada y Control de Acceso</td>
      <td>Como operador técnico, quiero realizar el pago de mi suscripción mensual a través de una pasarela segura, para obtener acceso inmediato a los tableros de control y reportes de calidad del agua.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el operador registrado ha elegido una suscripción mensual.
Cuando el usuario ingresa una tarjeta válida y confirma la transacción a través de la pasarela de Stripe.
Entonces el sistema debe recibir la confirmación de pago y actualizar el estado del usuario a activo en la base de datos.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador registrado ha elegido una suscripción mensual.
Cuando el usuario ingresa una tarjeta inválida o la transacción es rechazada por la pasarela de pago.
Entonces el sistema debe mostrar un mensaje de error y mantener el estado del usuario como inactivo.
</td>
      <td>EP09</td>
    </tr>
    <tr>
      <td>US02</td>
      <td>Configuración de reglas de alerta</td>
      <td>Como operador técnico, quiero establecer condiciones de alerta para recibir notificaciones ante eventos críticos.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existen umbrales definidos en el sistema.
Cuando el operador configura una regla de alerta.
Entonces el sistema genera alertas cuando se cumplen las condiciones establecidas.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador intenta registrar una regla de alerta con valores inválidos o incompletos.
Cuando guarda la configuración.
Entonces el sistema debe mostrar un mensaje de error y evitar el registro de la regla.
</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US03</td>
      <td>Ajuste de frecuencia de monitoreo</td>
      <td>Como operador técnico, quiero definir la frecuencia de captura de datos de los sensores para optimizar el monitoreo.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema cuenta con sensores activos.
Cuando el operador establece la frecuencia de monitoreo.
Entonces el sistema aplica la periodicidad configurada para la recolección de datos.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador modifica la frecuencia de monitoreo.
Cuando la configuración es guardada correctamente.
Entonces el sistema actualiza automáticamente la periodicidad para los sensores asociados.
</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US04</td>
      <td>Configuración de visualización del monitoreo</td>
      <td>Como usuario, quiero configurar la visualización de los datos para facilitar el análisis de la información.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el usuario accede a la configuración de visualización.
Cuando selecciona los datos que desea visualizar.
Entonces el sistema muestra la información según la configuración definida.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el usuario visualiza información de monitoreo.
Cuando selecciona distintos tipos de datos o parámetros.
Entonces el sistema permite alternar entre las diferentes vistas de información disponibles.
</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US05</td>
      <td>Visualización de datos en tiempo real</td>
      <td>Como operador técnico, quiero visualizar los datos de pH, flujo y gases en tiempo real para supervisar el estado de la red.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema recibe datos de sensores activos.
Cuando el operador accede al módulo de monitoreo.
Entonces el sistema muestra una tabla con el identificador del sensor, tipo, valor actual y estado operativo en tiempo real.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que un sensor cambia su condición operativa.
Cuando el sistema actualiza los datos de monitoreo.
Entonces el estado visual del sensor debe reflejarse mediante indicadores de color como Normal, Advertencia o Alerta.
</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US06</td>
      <td>Monitoreo por zona crítica</td>
      <td>Como operador técnico, quiero consultar los datos de monitoreo por zona para identificar áreas con mayor riesgo operativo.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existen sensores asociados a distintas zonas de la red.
Cuando el operador selecciona una zona específica.
Entonces el sistema muestra los datos correspondientes a dicha zona.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador consulta una zona crítica.
Cuando existen múltiples sensores registrados en dicha zona.
Entonces el sistema organiza y muestra la información según los sensores asociados.
</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US07</td>
      <td>Identificación de variaciones anómalas</td>
      <td>Como operador técnico, quiero detectar variaciones anómalas en los parámetros monitoreados para actuar antes de que ocurra una falla.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema monitorea continuamente los valores de los sensores.
Cuando se detecta una variación fuera de los rangos establecidos.
Entonces el sistema marca el evento como anomalía.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el sistema identifica una anomalía en los parámetros monitoreados.
Cuando el operador revisa el evento detectado.
Entonces el sistema muestra información detallada sobre el sensor y el valor fuera del rango permitido.
</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US08</td>
      <td>Renovación automática de suscripción</td>
      <td>Como usuario, quiero que el sistema gestione la renovación automática de mi suscripción, para evitar interrupciones en el monitoreo de mis sensores y en la programación de mis pedidos de agua.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el cliente tiene una suscripción activa con la opción de renovación automática habilitada.
Cuando el sistema detecta que faltan 24 horas para el vencimiento del periodo contratado.
Entonces el sistema debe realizar el cobro automático a través de Stripe y extender la vigencia del servicio.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el pago de renovación automática es rechazado.
Cuando el sistema intenta procesar el cobro.
Entonces el sistema notifica al usuario sobre el error y mantiene el estado pendiente de renovación.
</td>
      <td>EP09</td>
    </tr>
    <tr>
      <td>US09</td>
      <td>Actualización automática de datos</td>
      <td>Como operador técnico, quiero que los datos del monitoreo se actualicen automáticamente para mantener información vigente durante la supervisión.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema recibe nuevos datos de sensores.
Cuando la información cambia.
Entonces el sistema actualiza los valores mostrados sin intervención manual.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador se encuentra visualizando el panel de monitoreo.
Cuando el sistema recibe nuevas lecturas.
Entonces los datos deben refrescarse automáticamente sin necesidad de recargar la página.
</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US10</td>
      <td>Consulta de historial reciente de monitoreo</td>
      <td>Como operador técnico, quiero revisar el historial reciente de los sensores para comparar cambios en el comportamiento de la red.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema almacena registros recientes de monitoreo.
Cuando el operador consulta el historial de un sensor o zona.
Entonces el sistema muestra los datos registrados en el periodo reciente.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador visualiza el historial de monitoreo.
Cuando selecciona un sensor específico.
Entonces el sistema presenta la información ordenada cronológicamente.
</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US11</td>
      <td>Generación automática de alertas</td>
      <td>Como operador técnico, quiero que el sistema genere alertas automáticas cuando detecte valores críticos para actuar oportunamente ante riesgos en la red.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema monitorea datos de pH, flujo y gases.
Cuando un valor supera los umbrales configurados.
Entonces el sistema genera una alerta automáticamente.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que se genera una alerta crítica.
Cuando el operador accede al módulo de alertas.
Entonces el sistema muestra la severidad, ubicación y sensor asociado al evento.
</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US12</td>
      <td>Clasificación de alertas por nivel de riesgo</td>
      <td>Como operador técnico, quiero que las alertas se clasifiquen según su nivel de riesgo para priorizar la atención de incidencias.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema detecta una anomalía.
Cuando genera la alerta correspondiente.
Entonces el sistema la clasifica según el nivel de riesgo definido.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que existen alertas con distintos niveles de riesgo.
Cuando el operador visualiza las incidencias.
Entonces el sistema diferencia visualmente cada alerta mediante etiquetas o colores.
</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US13</td>
      <td>Consulta de alertas activas</td>
      <td>Como supervisor, quiero consultar las alertas activas para identificar rápidamente los eventos que requieren atención inmediata.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existen alertas generadas en el sistema.
Cuando el supervisor consulta las alertas activas.
Entonces el sistema muestra únicamente las alertas que se encuentran vigentes.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor accede al panel de alertas.
Cuando existen incidencias activas registradas.
Entonces el sistema muestra información como severidad, sensor asociado y ubicación de la anomalía.
</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US14</td>
      <td>Registro del historial de alertas</td>
      <td>Como supervisor, quiero acceder al historial de alertas para analizar incidentes previos y mejorar la toma de decisiones operativas.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema genera alertas durante la operación.
Cuando el supervisor consulta el historial.
Entonces el sistema muestra el registro de alertas emitidas anteriormente.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor revisa el historial de alertas.
Cuando selecciona una incidencia específica.
Entonces el sistema muestra los detalles y la fecha del evento registrado.
</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US15</td>
      <td>Marcado de alertas atendidas</td>
      <td>Como operador técnico, quiero marcar alertas como atendidas para llevar control sobre las incidencias resueltas en la red.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existe una alerta activa en el sistema.
Cuando el operador registra su atención.
Entonces el sistema actualiza el estado de la alerta como atendida.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que una alerta fue marcada como atendida.
Cuando el supervisor consulta el historial de incidencias.
Entonces el sistema muestra el estado actualizado de la alerta.
</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US16</td>
      <td>Identificación de zonas críticas</td>
      <td>Como operador técnico, quiero identificar zonas con mayor riesgo de fallas para priorizar acciones de mantenimiento.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema analiza datos históricos de monitoreo.
Cuando detecta patrones de riesgo en una zona.
Entonces el sistema identifica dicha zona como crítica.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que existen múltiples zonas monitoreadas.
Cuando el sistema identifica áreas críticas.
Entonces estas se resaltan visualmente para facilitar su priorización.
</td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US17</td>
      <td>Recomendación de mantenimiento preventivo</td>
      <td>Como operador técnico, quiero recibir recomendaciones de mantenimiento para prevenir fallas en la red.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema detecta condiciones de riesgo.
Cuando analiza tendencias en los datos.
Entonces el sistema genera recomendaciones de mantenimiento.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador consulta las recomendaciones generadas.
Cuando accede al detalle de mantenimiento.
Entonces el sistema muestra la zona afectada y la acción sugerida.
</td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US18</td>
      <td>Programación de intervenciones</td>
      <td>Como supervisor, quiero programar intervenciones de mantenimiento para organizar las actividades operativas.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existe una zona identificada como crítica.
Cuando el supervisor agenda una intervención.
Entonces el sistema registra la programación del mantenimiento.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que una intervención fue programada.
Cuando el supervisor consulta el calendario operativo.
Entonces el sistema muestra la fecha y detalles de la actividad registrada.
</td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US19</td>
      <td>Seguimiento de mantenimiento realizado</td>
      <td>Como supervisor, quiero registrar y consultar las intervenciones realizadas para evaluar la efectividad del mantenimiento.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que se ha realizado una intervención en la red.
Cuando el supervisor registra la acción.
Entonces el sistema almacena el historial de mantenimiento.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que existen mantenimientos registrados.
Cuando el supervisor consulta el historial.
Entonces el sistema muestra las intervenciones realizadas junto con su fecha y descripción.
</td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US20</td>
      <td>Visualización de indicadores clave</td>
      <td>Como supervisor, quiero visualizar indicadores clave del sistema para evaluar el estado general de la operación.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema procesa datos de monitoreo.
Cuando el supervisor accede al dashboard.
Entonces el sistema muestra indicadores clave actualizados.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor visualiza el dashboard principal.
Cuando se cargan los datos operativos.
Entonces el sistema presenta métricas como sensores activos, alertas críticas, volumen tratado y eficiencia del sistema.
</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US21</td>
      <td>Visualización gráfica de datos</td>
      <td>Como usuario, quiero ver gráficos de los datos monitoreados para interpretar tendencias de manera clara.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existen datos históricos de monitoreo.
Cuando el usuario accede a la sección de visualización.
Entonces el sistema muestra los datos en formato gráfico.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el usuario consulta una gráfica.
Cuando selecciona distintos parámetros monitoreados.
Entonces el sistema actualiza dinámicamente la representación visual de los datos.
</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US22</td>
      <td>Filtrado de información por zona y tiempo</td>
      <td>Como usuario, quiero filtrar los datos por zona y periodo de tiempo para analizar información específica.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existen datos de monitoreo registrados.
Cuando el usuario aplica filtros por zona o tiempo.
Entonces el sistema muestra la información correspondiente a los filtros seleccionados.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el usuario modifica los filtros de visualización.
Cuando selecciona una nueva zona o rango temporal.
Entonces el sistema actualiza automáticamente los resultados mostrados.
</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US23</td>
      <td>Visualización del estado general del sistema</td>
      <td>Como supervisor, quiero visualizar el estado general del sistema para identificar rápidamente situaciones críticas.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema consolida información de múltiples sensores.
Cuando el supervisor accede al dashboard principal.
Entonces el sistema muestra un resumen del estado general de la red.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor consulta el estado general del sistema.
Cuando existen incidencias o anomalías activas.
Entonces el sistema destaca visualmente los puntos que requieren atención inmediata.
</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US24</td>
      <td>Personalización de vistas del dashboard</td>
      <td>Como usuario, quiero personalizar la visualización del dashboard para priorizar la información relevante para mi operación.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el usuario accede a la configuración del dashboard.
Cuando selecciona los elementos que desea visualizar.
Entonces el sistema guarda y aplica la configuración personalizada.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el usuario personaliza el dashboard.
Cuando vuelve a ingresar al sistema.
Entonces el sistema mantiene las preferencias de visualización previamente configuradas.
</td>
      <td>EP05</td>
    </tr>
    <tr>
      <td>US25</td>
      <td>Identificación de agua reutilizable</td>
      <td>Como operador técnico, quiero identificar cuando el agua cumple parámetros adecuados para su reutilización para aprovechar el recurso disponible.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema monitorea parámetros de calidad del agua.
Cuando los valores cumplen los estándares definidos.
Entonces el sistema identifica el agua como apta para reutilización.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador consulta el estado del agua monitoreada.
Cuando el sistema detecta parámetros dentro de los rangos permitidos.
Entonces el sistema muestra visualmente la condición de agua reutilizable.
</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US26</td>
      <td>Validación de condiciones de reutilización</td>
      <td>Como operador técnico, quiero validar que el agua cumpla condiciones específicas antes de su reutilización para garantizar su uso seguro.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema detecta agua potencialmente reutilizable.
Cuando se evalúan los parámetros definidos.
Entonces el sistema confirma si el agua cumple con las condiciones requeridas.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador revisa las condiciones de reutilización.
Cuando algún parámetro no cumple los estándares establecidos.
Entonces el sistema indica que el agua no es apta para reutilización.
</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US27</td>
      <td>Registro de volúmenes reutilizables</td>
      <td>Como operador técnico, quiero registrar el volumen de agua reutilizable para gestionar su disponibilidad.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el agua ha sido validada como reutilizable.
Cuando el sistema procesa los datos.
Entonces registra el volumen disponible para reutilización.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que existen volúmenes de agua reutilizable registrados.
Cuando el operador consulta la información disponible.
Entonces el sistema muestra el volumen actualizado registrado en el sistema.
</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US28</td>
      <td>Gestión de disponibilidad de agua reutilizada</td>
      <td>Como operador, quiero visualizar la disponibilidad de agua reutilizable para planificar su uso en operaciones.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existen volúmenes de agua reutilizable registrados.
Cuando el operador consulta la disponibilidad.
Entonces el sistema muestra la cantidad de agua disponible.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador visualiza la disponibilidad de agua reutilizada.
Cuando existen cambios en los volúmenes registrados.
Entonces el sistema actualiza automáticamente la información mostrada.
</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US29</td>
      <td>Asignación de agua reutilizada a operaciones</td>
      <td>Como operador, quiero asignar agua reutilizable a procesos operativos para reducir el consumo de agua potable.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existe agua disponible para reutilización.
Cuando el operador la asigna a una operación.
Entonces el sistema registra la asignación realizada.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador consulta las asignaciones realizadas.
Cuando existen operaciones registradas.
Entonces el sistema muestra el volumen asignado y la operación correspondiente.
</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US30</td>
      <td>Seguimiento del uso de agua reutilizada</td>
      <td>Como supervisor, quiero hacer seguimiento del uso de agua reutilizada para evaluar el impacto en la operación.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema registra el uso de agua reutilizada.
Cuando el supervisor consulta la información.
Entonces el sistema muestra el historial de utilización.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor revisa el historial de uso de agua reutilizada.
Cuando selecciona un registro específico.
Entonces el sistema muestra detalles relacionados con el volumen utilizado y la fecha de operación.
</td>
      <td>EP06</td>
    </tr>
    <tr>
      <td>US31</td>
      <td>Generación de reportes operativos</td>
      <td>Como supervisor, quiero generar reportes operativos para evaluar el desempeño del sistema de monitoreo.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema almacena datos de monitoreo.
Cuando el supervisor solicita un reporte.
Entonces el sistema genera un reporte con la información requerida.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor genera un reporte operativo.
Cuando finaliza el procesamiento de datos.
Entonces el sistema permite visualizar o exportar el reporte generado.
</td>
      <td>EP07</td>
    </tr>
    <tr>
      <td>US32</td>
      <td>Análisis de tendencias de datos</td>
      <td>Como supervisor, quiero analizar tendencias en los datos para identificar patrones de comportamiento en la red.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existen datos históricos registrados.
Cuando el supervisor analiza los datos.
Entonces el sistema muestra tendencias en el comportamiento de los parámetros.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor consulta tendencias históricas.
Cuando selecciona un parámetro específico.
Entonces el sistema presenta variaciones y patrones de comportamiento en el tiempo.
</td>
      <td>EP07</td>
    </tr>
    <tr>
      <td>US33</td>
      <td>Reporte de incidencias</td>
      <td>Como supervisor, quiero consultar reportes de incidencias para evaluar la frecuencia de eventos críticos en la red.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema registra alertas e incidencias.
Cuando el supervisor consulta el reporte.
Entonces el sistema muestra el historial de eventos críticos.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor visualiza el reporte de incidencias.
Cuando existen eventos registrados.
Entonces el sistema organiza la información según fecha, severidad y ubicación.
</td>
      <td>EP07</td>
    </tr>
    <tr>
      <td>US34</td>
      <td>Reporte de impacto en reutilización de agua</td>
      <td>Como supervisor, quiero visualizar el impacto del uso de agua reutilizada para evaluar los beneficios operativos y ambientales.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el sistema registra el uso de agua reutilizada.
Cuando el supervisor consulta el reporte de impacto.
Entonces el sistema muestra indicadores relacionados al uso y ahorro generado.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor analiza el impacto de reutilización.
Cuando accede al reporte correspondiente.
Entonces el sistema presenta métricas ambientales y operativas relacionadas con el ahorro de agua.
</td>
      <td>EP07</td>
    </tr>
    <tr>
      <td>US35</td>
      <td>Visualización de información del producto</td>
      <td>Como visitante, quiero conocer la propuesta de valor del sistema para entender sus beneficios.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el visitante accede a la landing page.
Cuando navega por la sección principal del sitio.
Entonces el sistema muestra información clara sobre la propuesta de valor y los beneficios de Aquanetix.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el visitante explora la landing page.
Cuando interactúa con las secciones de solución y beneficios.
Entonces el sistema presenta información organizada mediante tarjetas y llamadas a la acción visuales.
</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US36</td>
      <td>Visualización de funcionalidades del sistema</td>
      <td>Como visitante, quiero visualizar las funcionalidades del sistema para comprender cómo resuelve el problema.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el visitante accede a la landing page.
Cuando revisa la sección de funcionalidades.
Entonces el sistema muestra las principales capacidades del ecosistema Aquanetix.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el visitante visualiza las funcionalidades del sistema.
Cuando explora las tarjetas informativas.
Entonces el sistema presenta características como monitoreo IoT, cumplimiento normativo y trazabilidad.
</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US37</td>
      <td>Acceso a información de contacto o interés</td>
      <td>Como visitante, quiero acceder a información de contacto para solicitar más información sobre el sistema.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el visitante se encuentra en la landing page.
Cuando desea contactar o mostrar interés.
Entonces el sistema proporciona un medio para establecer contacto.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el visitante revisa la sección final de la landing page.
Cuando selecciona el botón “Agendar Consultoría Técnica” o “Solicitar Demo”.
Entonces el sistema dirige al usuario hacia el canal de contacto correspondiente.
</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US38</td>
      <td>Configuración de rangos de seguridad para pH</td>
      <td>Como operador técnico, quiero definir los límites superior e inferior de pH para detectar niveles de acidez o alcalinidad que puedan corroer la tubería o violar normativas ambientales.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el operador se encuentra en el panel de "Configuración de Sensores Químicos".
Cuando el operador ingresa un valor mínimo y un valor máximo.
Entonces el sistema valida que el valor mínimo sea menor al máximo y guarda los umbrales.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el operador se encuentra en el panel de "Configuración de Sensores Químicos".
Cuando el operador ingresa un valor mínimo y un valor máximo.
Entonces se activa una alerta visual si el sensor reporta valores fuera de ese rango.
</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US39</td>
      <td>Configuración de límites de caudal para detección de fugas u obstrucciones.</td>
      <td>Como operador técnico, quiero establecer el flujo nominal y los márgenes de tolerancia para identificar fugas (caída de presión) o taponamientos (sobrepresión).</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el operador accede a la sección de "Parámetros Hidráulicos".
Cuando el operador define el umbral de "Flujo Crítico Bajo" (posible fuga) y "Flujo Crítico Alto" (obstrucción o sobrecarga).
Entonces el sistema registra los valores en L/s (litros por segundo).
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que existen límites de caudal configurados en el sistema.
Cuando los sensores detectan valores fuera de los márgenes establecidos.
Entonces el sistema genera una alerta indicando una posible fuga u obstrucción.
</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US40</td>
      <td>Configuración de niveles de alerta para gases inflamables/tóxicos.</td>
      <td>Como operador técnico, quiero definir la concentración máxima permitida de gases (como $H_2S$ o $CH_4$) para prevenir explosiones o intoxicaciones en la red.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el operador está en el módulo de "Seguridad Atmosférica".
Cuando define el umbral de Pre-alarma y Alarma Crítica.
Entonces el sistema guarda la configuración y asegura que estos valores no puedan ser desactivados sin una clave de supervisor.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que los sensores detectan concentraciones de gases superiores al umbral crítico configurado.
Cuando el sistema procesa los valores registrados.
Entonces se activa automáticamente el protocolo de ventilación, si este se encuentra integrado.
</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US41</td>
      <td>Monitoreo en tiempo real mediante mapa interactivo.</td>
      <td>Como supervisor, quiero visualizar la ubicación geográfica de todos los nodos de la red en un mapa para identificar rápidamente qué zonas presentan estados críticos (alerta/alarma).</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el supervisor registrado accede al mapa.
Cuando el sistema carga las coordenadas de los sensores IoT.
Entonces se muestran marcadores con código de colores: verde (normal), amarillo (advertencia) y rojo (crítico).
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el supervisor visualiza el mapa interactivo.
Cuando selecciona un marcador correspondiente a un sensor.
Entonces el sistema muestra información detallada sobre el estado y los parámetros monitoreados de dicho nodo.
</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US42</td>
      <td>Consulta de gráficas de comportamiento temporal.</td>
      <td>Como supervisor, quiero consultar gráficas de tendencias de los sensores en rangos de tiempo específicos para detectar patrones de degradación en la calidad del agua.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el supervisor selecciona un nodo o sector específico.
Cuando el supervisor filtra por un rango de fechas y un tipo de sensor.
Entonces el sistema renderiza un gráfico de líneas que muestra la evolución del parámetro frente a los umbrales configurados.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el sistema muestra una gráfica de comportamiento temporal.
Cuando un parámetro supera los umbrales establecidos.
Entonces el sistema resalta visualmente los puntos críticos dentro de la gráfica.
</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US43</td>
      <td>Consolidado de alertas operativas pendientes.</td>
      <td>Como supervisor, quiero ver un listado priorizado de todas las anomalías activas en la red para asignar equipos de mantenimiento de manera eficiente.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que existen condiciones de sensores que superan los umbrales definidos en la configuración.
Cuando el supervisor accede al panel de alertas.
Entonces el sistema muestra una tabla con: ID del sensor, ubicación, tipo de anomalía y severidad.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que existen múltiples alertas activas registradas en el sistema.
Cuando el supervisor visualiza el consolidado de alertas.
Entonces el sistema organiza las anomalías según su nivel de severidad para facilitar la priorización de atención.
</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US44</td>
      <td>Navegación de contenido</td>
      <td>Como visitante, quiero disponer de puntos de acceso directo a las secciones clave de la página para localizar rápidamente la información que es de mi interés sin realizar un recorrido lineal.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el visitante desea explorar un tema específico (como la solución o los beneficios).
Cuando elige una sección en el sistema de navegación de la Landing Page.
Entonces el sistema lo posiciona de manera inmediata en la sección correspondiente.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que el visitante se encuentra en cualquier sección de la página.
Cuando el visitante desea cambiar de sección.
Entonces el visitante puede elegir otra sección sin tener que volver al inicio.

</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US45</td>
      <td>Comprensión del problema</td>
      <td>Como visitante corporativo, quiero conocer el problema a enfrentar para comprender mejor el enfoque de la solución.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el visitante está navegando por la Landing Page.
Cuando consulta la información sobre el problema a enfrentar.
Entonces el sistema presenta con sustento estadístico el desafío de la brecha hídrica que está presente.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el visitante ha revisado las cifras del déficit de saneamiento.
Cuando analiza el impacto de la falta de visibilidad operativa en la gestión de recursos.
Entonces el sistema establece una conexión directa entre la problemática expuesta y la necesidad de una transformación digital para democratizar el acceso al agua segura.

</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US46</td>
      <td>Acceso a información de respaldo y transparencia</td>
      <td>Como visitante, quiero disponer de un espacio con referencias institucionales y legales para validar la formalidad del proyecto y conocer mis derechos como usuario.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el visitante desea conocer el marco legal del sitio.
Cuando consulta la información de cierre de la página.
Entonces el sistema ofrece acceso a las políticas de privacidad, términos de servicio y compromisos de sostenibilidad de la organización.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el visitante ha revisado las cifras del déficit de saneamiento.
Cuando analiza el impacto de la falta de visibilidad operativa en la gestión de recursos.
Entonces el sistema muestra la identificación de la empresa como desarrolladores y la marca de propiedad intelectual correspondiente al año 2026.
</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US47</td>
      <td>Solicitud de demostración del sistema</td>
      <td>Como visitante corporativo interesado, quiero solicitar una demostración personalizada del ecosistema para observar cómo las funcionalidades de monitoreo y trazabilidad se adaptan a las necesidades específicas de mi organización.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el visitante ha evaluado la propuesta de valor y los beneficios en la landing page.
Cuando decide profundizar en el funcionamiento técnico y operativo de la plataforma.
Entonces el sistema proporciona un canal directo para manifestar el interés en una sesión demostrativa.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el visitante requiere una validación práctica de la herramienta.
Cuando interactúa con la opción de solicitar consultoría o demo.
Entonces el sistema captura la intención del usuario para facilitar la coordinación de una presentación detallada sobre las capacidades de inteligencia hídrica.
</td>
      <td>EP08</td>
    </tr>
  </tbody>
</table>
