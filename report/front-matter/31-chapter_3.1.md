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
      <td>EP001</td>
      <td>Configuración del sistema de monitoreo</td>
      <td>Permite definir parámetros, condiciones y configuraciones necesarias para el funcionamiento del monitoreo y la detección de anomalías en la red.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
      <tr>
      <td>EP002</td>
      <td>Monitoreo en tiempo real</td>
      <td>Permite visualizar datos de sensores IoT (pH, flujo y gases) en tiempo real para la supervisión de la red.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP003</td>
      <td>Gestión de alertas</td>
      <td>Permite detectar anomalías en los parámetros del agua y generar alertas automáticas para prevenir riesgos.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP004</td>
      <td>Mantenimiento preventivo</td>
      <td>Permite identificar patrones de fallas y zonas críticas para optimizar la planificación del mantenimiento.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP005</td>
      <td>Dashboard y visualización</td>
      <td>Permite visualizar información consolidada mediante gráficos e indicadores para la toma de decisiones.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP006</td>
      <td>Gestión de reutilización de agua</td>
      <td>Permite identificar, validar y gestionar el uso de agua tratada para su reutilización en procesos operativos.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP007</td>
      <td>Reportes y análisis</td>
      <td>Permite generar reportes históricos y métricas que apoyen la evaluación del desempeño del sistema.</td>
      <td>N/A</td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>EP008</td>
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
Cuando el visitante quiere solicitar una consultoría técnica.
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
      <td>US42</td>
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
      <td>US43</td>
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
      <td>US44</td>
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
      <td>US45</td>
      <td>Solicitud de demostración del sistema</td>
      <td>Como visitante corporativo interesado, quiero solicitar una demostración personalizada del ecosistema para observar cómo las funcionalidades de monitoreo y trazabilidad se adaptan a las necesidades específicas de mi organización.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el visitante ha evaluado la propuesta de valor y los beneficios en la landing page.
Cuando el visitante decide profundizar en el funcionamiento técnico y operativo de la plataforma.
Entonces el sistema proporciona un canal directo para manifestar el interés en una sesión demostrativa.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el visitante requiere una validación práctica de la herramienta.
Cuando el visitante interactúa con la opción de solicitar consultoría o demo.
Entonces el sistema captura la intención del usuario para facilitar la coordinación de una presentación detallada sobre las capacidades de inteligencia hídrica.
</td>
      <td>EP08</td>
    </tr>
    <tr>
      <td>US46</td>
      <td>Registro de usuarios</td>
      <td>Como nuevo usuario de la plataforma, quiero registrarme en ella ingresando mi nombre y contraseña, para crear una cuenta y poder acceder a las herramientas de monitoreo de agua.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el usuario está en la página de registro.
Cuando el usuario ingresa un nombre de usuario no registrado, y una contraseña.
Entonces el sistema debe redirigir al usuario a la pantalla de suscripción, para que elija un plan.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el usuario está en la página de registro.
Cuando ingresa un nombre de usuario que ya se encuentra registrado en el sistema.
Entonces el sistema debe mostrar un mensaje de error indicando que el correo ya está en uso.
</td>
      <td>EP009</td>
    </tr>
     <tr>
      <td>US47</td>
      <td>Inicio de sesión</td>
      <td>Como usuario registrado de Aquanetix, quiero iniciar sesión con mi correo y contraseña, para acceder de manera segura al dashboard.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el usuario se encuentra en la pantalla de inicio de sesión
Cuando ingresa con su nombre de usuario y contraseña correctos
Entonces el sistema debe redirigir al usuario a su panel de control.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que el usuario se encuentra en la pantalla de inicio de sesión
Cuando intenta ingresar con un nombre de usuario y/o contraseña incorrectos
Entonces el sistema debe mostrar un mensaje de error genérico, indicando que su nombre de usuario y/o contraseña son incorrectos.
</td>
      <td>EP009</td>
    </tr>
     <tr>
      <td>US48</td>
      <td>Cierre de sesión</td>
      <td>Como usuario autenticado, quiero cerrar mi sesión activa en la plataforma, para garantizar que nadie más pueda acceder a mis datos si dejo el dispositivo desatendido.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el usuario ha iniciado sesión y se encuentra navegando en la plataforma,
Cuando escoge la opción para cerrar sesión,
Entonces el sistema debe redirigir al usuario inmediatamente a la página pública de inicio de sesión,
Y bloquear cualquier intento posterior de navegación hacia rutas protegidas sin iniciar sesión de nuevo.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el usuario ha iniciado sesión y se encuentra navegando en la plataforma
Cuando escoge la opción para cerrar sesión.
Y el sistema intenta comunicarse con el backend para invalidar el token, pero la petición falla (por error 500 o falta de red)
Entonces el sistema debe borrar de todos modos el token del almacenamiento local (localStorage/sessionStorage) por seguridad
Y redirigir al usuario a la pantalla de inicio de sesión.
</td>
      <td>EP009</td>
    </tr>
     <tr>
      <td>US49</td>
      <td>Gestión de perfil del usuario.</td>
      <td>Como usuario autenticado, quiero acceder a una sección de perfil para ver y actualizar mis datos personales (nombre, apellido, teléfono), para mantener mi información de contacto actualizada dentro del sistema.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el usuario ha iniciado sesión y se encuentra en el dashboard principal,
Cuando hace clic en su avatar o en la opción "Mi Perfil" del menú de navegación,
Entonces el sistema debe redirigirlo a la vista de perfil de usuario.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el usuario se encuentra visualizando la pantalla de "Mi Perfil",
Cuando hace clic en el botón "Volver" o en el logotipo de Aquanetix en la barra superior,
Entonces el sistema debe redirigirlo de regreso al dashboard principal sin perder el estado de su sesión.
</td>
      <td>EP009</td>
    </tr>
    <tr>
      <td>US50</td>
      <td>Selección de plan de suscripción</td>
      <td>Como usuario recién registrado, quiero visualizar los planes de suscripción disponibles y seleccionar uno, para activar mi cuenta con las características de monitoreo y redistribución que mejor se adapten a mis necesidades.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el usuario acaba de completar su registro y se encuentra en la pantalla de "Selección de Plan",
Cuando selecciona uno de los planes disponibles y lo confirma,
Entonces el sistema debe asociar el plan elegido a su cuenta en la base de datos,
Y redirigir al usuario al dashboard principal con los accesos correspondientes a su nivel de suscripción.
<br><br>

<b>Criterio de aceptación 2:</b><br>
Dado que el usuario se encuentra visualizando la pantalla de su perfil,
Cuando intenta volver al dashboard,
Entonces el sistema debe redirigirlo de regreso al dashboard principal sin perder el estado de su sesión.
</td>
      <td>EP009</td>
    </tr>
    <tr>
      <td>T01</td>
      <td>Get-All-Devices</td>
      <td>Como desarrollador, quiero implementar un endpoint de tipo API REST con el método GET /api/devices, para proveer un listado centralizado en formato JSON con la información de todos los dispositivos de monitoreo hídrico que consumirá el frontend.</td>
      <td>
<b>Criterio de Aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/devices.
Cuando la base de datos responde correctamente (tenga o no registros almacenados).
Entonces el sistema debe retornar un código de estado 200 OK junto con el arreglo JSON correspondiente (con los datos de los dispositivos o vacío []).
        <br><br>
        
<b>Criterio de Aceptación 2:</b><br>
Dado que se invoca el endpoint /api/devices mediante una petición GET.
Cuando la base de datos no se encuentra disponible o el servidor experimenta una falla interna.
Entonces el sistema debe retornar un código de estado 500 Internal Server Error y registrar el error en los logs de la aplicación de forma segura.<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T02</td>
      <td>Get-Device-By-Id</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful GET /api/devices/{id}, para permitir la consulta individual de un dispositivo de monitoreo hídrico específico mediante su identificador único.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/devices/{id} enviando un ID válido y existente.
Cuando el sistema procesa la consulta en la base de datos.
Entonces el sistema debe retornar un código de estado 200 OK junto con el objeto JSON que contiene los detalles específicos de ese dispositivo.
        <br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se realiza una solicitud HTTP GET al endpoint /api/devices/{id} enviando un ID que no corresponde a ningún dispositivo registrado.
Cuando el sistema valida la inexistencia del recurso.
Entonces el sistema debe retornar un código de estado 404 Not Found acompañado de un mensaje JSON indicando que el dispositivo no fue localizado.<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T03</td>
      <td>Update-Device-Frequency</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful UPDATE /api/devices/{id}/frequency, para permitir la actualización remota de la frecuencia de transmisión de datos de un dispositivo de monitoreo específico.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP PATCH a /api/devices/{id}/frequency con un JSON que contiene el nuevo intervalo de tiempo válido.
Cuando el sistema actualiza exitosamente el parámetro en la base de datos.
Entonces el sistema debe retornar un código de estado 200 OK (o 204 No Content) confirmando que la frecuencia de transmisión se modificó correctamente.<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se envía una solicitud HTTP PATCH al endpoint pero con un valor de frecuencia negativo, vacío o en un formato de datos incorrecto.
Cuando el backend ejecuta las reglas de validación de negocio.
Entonces el sistema debe retornar un código de estado 400 Bad Request junto con un JSON que describa los errores de validación del payload.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T04</td>
      <td>Create-Device-Thresholds</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful POST /api/devices/{id}/thresholds, para registrar los umbrales de alerta mínimos y máximos asignados a las métricas de un dispositivo de monitoreo hídrico.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP POST a /api/devices/{id}/thresholds enviando un JSON con los límites de alerta estructurados correctamente.
Cuando el sistema procesa el almacenamiento de estos nuevos parámetros de control.
Entonces el sistema debe retornar un código de estado 201 Created junto con el objeto JSON de los umbrales creados y su respectivo identificador.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se realiza una solicitud POST al endpoint omitiendo campos obligatorios o definiendo un umbral mínimo mayor que el máximo.
Cuando el backend evalúa la integridad y lógica de los datos recibidos.
Entonces el sistema debe rechazar la operación retornando un código de estado 400 Bad Request.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T05</td>
      <td>Register-Devices-BC</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful POST /api/devices, para procesar el registro masivo o individual de nuevos dispositivos de monitoreo hídrico dentro de su respectivo contexto de negocio en la plataforma.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que una aplicación emisora envía una solicitud HTTP POST a /api/devices incluyendo los campos obligatorios del dispositivo (número de serie, modelo, etc.).
Cuando el backend verifica que el dispositivo no se encuentra duplicado y lo persiste en la base de datos de manera exitosa.
Entonces el sistema debe retornar un código de estado 201 Created y el recurso recién creado en el cuerpo de la respuesta.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se envía una solicitud HTTP POST para registrar un dispositivo cuyo identificador único o número de serie ya existe en el sistema.
Cuando el backend realiza la validación de unicidad en la persistencia.
Entonces el sistema debe prevenir la duplicación de datos retornando un código de estado 490 Conflict (o 400 Bad Request) informando la naturaleza del problema.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T06</td>
      <td>Get-All-Alerts</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful GET /api/alerts, para proveer un listado histórico y centralizado de todas las alertas generadas por el sistema de monitoreo hídrico.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/alerts.
Cuando la base de datos responde de manera correcta.
Entonces el sistema debe retornar un código de estado 200 OK junto con un arreglo JSON que contenga las alertas registradas (o vacío []).
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se invoca el endpoint /api/alerts mediante una petición GET.
Cuando ocurre un problema de conectividad interna con la base de datos o un timeout.
Entonces el sistema debe responder con un código de estado 500 Internal Server Error y registrar el error en los logs del servidor.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T07</td>
      <td>Get-Alerts-By-Device-Id</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful GET /api/devices/{deviceId}/alerts, para filtrar y recuperar únicamente las alertas que pertenecen a un dispositivo de monitoreo específico.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET a /api/devices/{deviceId}/alerts enviando un ID de dispositivo existente.
Cuando el backend procesa la consulta con la condición de filtrado.
Entonces el sistema debe retornar un código de estado 200 OK y el arreglo JSON con las alertas asociadas a ese dispositivo.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se realiza la solicitud HTTP GET especificando un deviceId que no está registrado en el sistema.
Cuando el backend valida la integridad estructural de los datos.
Entonces el sistema debe retornar un código de estado 404 Not Found informando que el dispositivo referenciado no existe.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T08</td>
      <td>Create-Alert</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful POST /api/alerts, para permitir que el motor de reglas o los servicios de monitoreo registren de forma automática una nueva alerta cuando se superen los umbrales definidos.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que el servicio emite una solicitud HTTP POST a /api/alerts con los datos obligatorios (dispositivo de origen, métrica excedida, timestamp).
Cuando el sistema procesa de manera correcta la inserción del registro.
Entonces el sistema debe retornar un código de estado 201 Created junto con el objeto de la alerta creada.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se realiza una solicitud POST al endpoint omitiendo parámetros críticos de la alerta (como el ID del dispositivo o la descripción).
Cuando el backend intercepta el payload y ejecuta la validación.
Entonces el sistema debe rechazar la petición retornando un código de estado 400 Bad Request.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T09</td>
      <td>Get-Alerts-By-Status</td>
      <td> Como desarrollador, quiero implementar el endpoint de la API RESTful GET /api/alerts?status={status}, para permitir al frontend filtrar las alertas del sistema de acuerdo a su estado actual (ej. Activa, Atendida, Resuelta).
</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que se realiza una solicitud HTTP GET a /api/alerts incluyendo un parámetro de estado válido (ej. status=active).
Cuando el backend procesa la consulta aplicando dicho criterio.
Entonces el sistema debe retornar un código de estado 200 OK junto con el listado JSON filtrado.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se invoca el endpoint enviando un estado que no coincide con los enumerados permitidos por el sistema (ej. status=desconocido).
Cuando el backend valida la consulta.
Entonces el sistema debe retornar un código de estado 400 Bad Request indicando el error de sintaxis en el parámetro.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T10</td>
      <td>Update-Alert</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful PUT /api/alerts/{id}, para actualizar de forma integral las propiedades o comentarios de gestión de una alerta en particular.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP PUT a /api/alerts/{id} enviando el payload completo modificado.
Cuando el sistema persiste los cambios del recurso en la base de datos de forma exitosa.
Entonces el sistema debe retornar un código de estado 200 OK (o 204 No Content) confirmando la actualización del recurso.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se procesa una solicitud PUT enviando datos inconsistentes o intentando alterar campos inmutables de la alerta histórica.
Cuando se ejecutan las reglas de negocio en el backend.
Entonces el sistema debe denegar la operación devolviendo un código de estado 400 Bad Request.
<br></td>
      <td>N/A</td>    
    </tr>
    <tr>
      <td>T11</td>
      <td>Get-Alert-By-Id</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful GET /api/alerts/{id}, para permitir la consulta individual y detallada de una alerta específica mediante su identificador único.
  </td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que se realiza una solicitud HTTP GET al endpoint /api/alerts/{id} enviando un ID válido y existente.
Cuando el sistema lee el registro desde la base de datos.
Entonces el sistema debe retornar un código de estado 200 OK acompañado del objeto JSON completo de la alerta.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se solicita una alerta mediante un ID inexistente en la persistencia.
Cuando se valida la ausencia del recurso.
Entonces el sistema debe retornar un código de estado 404 Not Found.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T12</td>
      <td>Register-Monitoring-BC</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful POST /api/monitoring-records, para procesar e ingresar las tramas de telemetría continuas recibidas desde los sensores (flujo, presión, etc.) en su respectivo contexto de negocio.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un dispositivo emisor envía un payload JSON válido con las lecturas capturadas al endpoint de monitoreo.
Cuando el sistema valida la estructura del mensaje y lo registra exitosamente en la persistencia temporal/histórica.
Entonces el sistema debe retornar un código de estado 201 Created confirmando la correcta recepción del paquete de telemetría.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se recibe una petición HTTP POST pero con una estructura JSON rota o con tipos de datos inválidos en las lecturas de los sensores.
Cuando el middleware de la API o el controlador validan el request.
Entonces el sistema debe descartar el paquete devolviendo un código de estado
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T13</td>
      <td>Get-Quality-Analysis-By-Id</td>
      <td> Como desarrollador, quiero implementar el endpoint de la API RESTful GET /api/quality-analyses/{id}, para permitir la consulta individual de un reporte técnico o análisis de calidad de agua específico mediante su identificador único.
    </td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/quality-analyses/{id} enviando un ID válido y existente.
Cuando el sistema procesa la consulta en la base de datos.
Entonces el sistema debe retornar un código de estado 200 OK junto con el objeto JSON que contiene los parámetros detallados del análisis de calidad.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se realiza una solicitud HTTP GET al endpoint /api/quality-analyses/{id} con un identificador que no está registrado.
Cuando el backend verifica la inexistencia del recurso.
Entonces el sistema debe retornar un código de estado 404 Not Found acompañado de un mensaje JSON estructurado.
<br></td>
      <td>N/A</td>
    </tr>
     <tr>
      <td>T14</td>
      <td>Get-All-Quality-Analyses</td>
      <td>Como Desarrollador, quiero implementar el endpoint de la API RESTful GET /api/quality-analyses, para proveer un listado histórico centralizado con todos los análisis de calidad de agua registrados en la plataforma.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/quality-analyses.
Cuando la base de datos responde correctamente a la consulta de registros.
Entonces el sistema debe retornar un código de estado 200 OK junto con un arreglo JSON que contenga los análisis almacenados (o vacío []).
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/quality-analyses.
Cuando la base de datos responde correctamente a la consulta de registros.
Entonces el sistema debe retornar un código de estado 200 OK junto con un arreglo JSON que contenga los análisis almacenados (o vacío []).
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T15</td>
      <td>Create-Quality-Analysis</td>
      <td>Como Developer, quiero implementar el endpoint de la API RESTful POST /api/quality-analyses, para registrar un nuevo reporte de parámetros químicos o físicos del agua evaluada en el sistema de monitoreo.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que una entidad autorizada envía una solicitud HTTP POST a /api/quality-analyses con un JSON válido que incluye las métricas requeridas (pH, turbidez, etc.).
Cuando el sistema valida y almacena exitosamente el registro en la base de datos.
Entonces el sistema debe retornar un código de estado 201 Created junto con el objeto JSON del reporte generado.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se realiza una solicitud POST omitiendo campos obligatorios o enviando valores fuera de los rangos físicos permitidos por las reglas del backend.
Cuando el controlador de la API procesa la validación del request.
Entonces el sistema debe rechazar la inserción devolviendo un código de estado 400 Bad Request.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T16</td>
      <td>Register-Dashboard-BC</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful POST /api/dashboard-metrics, para registrar, consolidar o recalcular los KPI generales (consumo, eficiencia, estado global) requeridos por el contexto de negocio del Dashboard.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un servicio interno realiza una solicitud HTTP POST a /api/dashboard-metrics con el consolidado periódico de datos hídricos.
Cuando el backend actualiza de forma correcta las proyecciones y resúmenes estadísticos en la persistencia del dashboard.
Entonces el sistema debe retornar un código de estado 201 Created o 200 OK confirmando la actualización del panel visual.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se envía una solicitud POST al endpoint pero con un formato corrupto o datos temporales desalineados.
Cuando el backend ejecuta las reglas de integridad del contexto del Dashboard.
Entonces el sistema debe prevenir el registro inconsistente retornando un código de estado 400 Bad Request.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T17</td>
      <td>Get-All-Water-Batches</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful GET /api/water-batches, para proveer un listado centralizado de todos los lotes de agua registrados para su monitoreo y distribución.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/water-batches.
Cuando la base de datos responde correctamente a la consulta de registros.
Entonces el sistema debe retornar un código de estado 200 OK junto con un arreglo JSON que contenga los lotes de agua (o vacío []).
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se invoca el endpoint /api/water-batches mediante una petición GET.
Cuando el servicio de base de datos experimenta un error de conexión interno.
Entonces el sistema debe responder con un código de estado 500 Internal Server Error.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T18</td>
      <td>Get-Water-Batch-By-Id</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful GET /api/water-batches/{id}, para permitir la consulta individual de un lote de agua específico mediante su identificador único.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/water-batches/{id} enviando un ID válido y existente.
Cuando el sistema procesa la consulta en la base de datos.
Entonces el sistema debe retornar un código de estado 200 OK junto con el objeto JSON que contiene los detalles del lote de agua.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se realiza una solicitud HTTP GET al endpoint con un identificador que no está registrado.
Cuando el backend verifica la inexistencia del recurso.
Entonces el sistema debe retornar un código de estado 404 Not Found.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T19</td>
      <td>Create-Water-Batch</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful POST /api/water-batches, para registrar un nuevo lote de agua con sus especificaciones de origen y volumen en el sistema.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que una entidad autorizada envía una solicitud HTTP POST a /api/water-batches con un JSON válido que incluye los campos obligatorios del lote.
Cuando el sistema almacena exitosamente el registro en la base de datos.
Entonces el sistema debe retornar un código de estado 201 Created junto con el objeto JSON del lote generado.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se realiza una solicitud POST omitiendo parámetros requeridos o enviando valores de volumen inconsistentes.
Cuando el backend procesa la validación del request.
Entonces el sistema debe rechazar la inserción devolviendo un código de estado 400 Bad Request.
<br></td>
      <td>N/A</td>
    </tr>
       <tr>
      <td>T20</td>
      <td>Update-Water-Batch</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful PUT /api/water-batches/{id}, para actualizar de forma integral las propiedades o el estado de un lote de agua específico.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP PUT a /api/water-batches/{id} enviando el payload completo modificado.
Cuando el sistema persiste los cambios del recurso en la base de datos de manera exitosa.
Entonces el sistema debe retornar un código de estado 200 OK (o 204 No Content).
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se envía una solicitud PUT con una estructura malformada o valores fuera de rango para el lote de agua.
Cuando el backend ejecuta las validaciones de negocio.
Entonces el sistema debe denegar la operación devolviendo un código de estado 400 Bad Request.
<br></td>
      <td>N/A</td>
    </tr>
       <tr>
      <td>T21</td>
      <td>Delete-Water-Batch</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful DELETE /api/water-batches/{id}, para remover (o dar de baja de forma lógica) un lote de agua del sistema mediante su identificador único.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP DELETE al endpoint /api/water-batches/{id} con un ID válido.
Cuando el backend procesa el borrado físico o el cambio de estado a inactivo en la persistencia.
Entonces el sistema debe retornar un código de estado 200 OK (o 240 No Content) confirmando la eliminación del recurso.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se intenta eliminar un lote de agua enviando un ID que ya no existe o nunca fue registrado.
Cuando el sistema comprueba la ausencia del registro.
Entonces el sistema debe retornar un código de estado 404 Not Found.
<br></td>
      <td>N/A</td>
    </tr>
    <tr>
      <td>T22</td>
      <td>Validate-Water-Batch</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful POST /api/water-batches/{id}/validate, para evaluar y certificar si un lote de agua cumple con las normas de calidad necesarias antes de autorizar su redistribución.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que se realiza una solicitud HTTP POST a /api/water-batches/{id}/validate con los datos de las pruebas de laboratorio o sensores.
Cuando los parámetros químicos y físicos evaluados cumplen rigurosamente con los rangos permitidos.
Entonces el sistema debe actualizar el estado del lote a "Validado/Aprobado" y retornar un código 200 OK.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se invoca el endpoint de validación pero los datos del payload indican que se excedieron los límites de contaminación permitidos.
Cuando el sistema procesa las reglas de control de calidad.
Entonces el sistema debe registrar el lote con estado "Rechazado" y retornar un código 200 OK (o 422 Unprocessable Entity) detallando las métricas fuera de norma.
<br></td>
      <td>N/A</td>
    </tr>
      <tr>
      <td>T23</td>
      <td>Register-Service-Design-BC</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful POST /api/service-designs, para registrar las configuraciones estructurales, topologías o especificaciones iniciales del servicio de distribución en su respectivo contexto de negocio.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que una aplicación emisora envía una solicitud HTTP POST a /api/service-designs con un payload JSON que define el diseño del servicio.
Cuando el backend valida que la topología y configuraciones cumplen con las reglas del contexto y las persiste de manera exitosa.
Entonces el sistema debe retornar un código de estado 201 Created junto con el recurso de configuración creado.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se envía un request POST intentando registrar un diseño de servicio con un identificador o versión que ya se encuentra activo en el sistema.
Cuando el backend realiza el control de duplicidad.
Entonces el sistema debe denegar el registro retornando un código de estado 490 Conflict (o 400 Bad Request).
<br></td>
      <td>N/A</td>
    </tr>
  <tr>
      <td>T24</td>
      <td>Get-Subscription-By-Id</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful GET /api/subscriptions/{id}, para permitir la consulta individual de los detalles y el estado de una suscripción específica mediante su identificador único.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/subscriptions/{id} enviando un ID válido y existente.
Cuando el sistema procesa la consulta en la base de datos.
Entonces el sistema debe retornar un código de estado 200 OK junto con el objeto JSON que contiene los datos de la suscripción (fechas, plan, estado).
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se realiza una solicitud HTTP GET al endpoint con un identificador que no está registrado.
Cuando el backend verifica la inexistencia del recurso.
Entonces el sistema debe retornar un código de estado 404 Not Found.
<br></td>
      <td>N/A</td>
    </tr>
      <tr>
      <td>T25</td>
      <td>Get-All-Subscriptions</td>
      <td>Como developer, quiero implementar el endpoint de la API RESTful GET /api/subscriptions, para proveer un listado centralizado con todas las suscripciones de los clientes registradas en la plataforma.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP GET al endpoint /api/subscriptions.
Cuando la base de datos responde correctamente a la consulta de registros.
Entonces el sistema debe retornar un código de estado 200 OK junto con un arreglo JSON que contenga las suscripciones (o vacío []).
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se invoca el endpoint /api/subscriptions mediante una petición GET.
Cuando el servicio de persistencia experimenta un error de conexión interno o un timeout.
Entonces el sistema debe responder con un código de estado 500 Internal Server Error.
<br></td>
      <td>N/A</td>
    </tr>
      <tr>
      <td>T26</td>
      <td>Update-Subscription</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful PUT /api/subscriptions/{id}, para permitir la actualización integral de los parámetros de una suscripción (como la renovación, cambio de plan o cancelación).</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que un componente autorizado realiza una solicitud HTTP PUT a /api/subscriptions/{id} enviando el payload completo modificado.
Cuando el sistema persiste los cambios en la base de datos de manera exitosa.
Entonces el sistema debe retornar un código de estado 200 OK (o 204 No Content) confirmando la modificación.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se envía una solicitud PUT con una estructura malformada o valores lógicos incorrectos (ej. fecha de fin anterior a la fecha de inicio).
Cuando el backend ejecuta las validaciones de negocio.
Entonces el sistema debe denegar la operación devolviendo un código de estado 400 Bad Request.
<br></td>
      <td>N/A</td>
    </tr>    
      <tr>
      <td>T27</td>
      <td>Register-Subscription-BC</td>
      <td>Como desarrollador, quiero implementar el endpoint de la API RESTful POST /api/subscriptions, para registrar la adquisición de una nueva suscripción corporativa en su respectivo contexto de negocio.</td>
      <td>
<b>Criterio de aceptación 1:</b><br>
Dado que una aplicación emisora envía una solicitud HTTP POST a /api/subscriptions incluyendo los campos obligatorios del plan y cliente.
Cuando el backend valida e inserta exitosamente la suscripción en la base de datos.
Entonces el sistema debe retornar un código de estado 201 Created junto con el recurso recién creado en el cuerpo de la respuesta.
<br><br>
        
<b>Criterio de aceptación 2:</b><br>
Dado que se procesa una solicitud POST omitiendo parámetros críticos del contrato de suscripción (como el identificador del cliente o el tipo de plan).
Cuando el middleware de la API intercepta y evalúa el request.
Entonces el sistema debe rechazar el registro retornando un código de estado 400 Bad Request.
<br></td>
      <td>N/A</td>
    </tr>
  </tbody>
</table>
