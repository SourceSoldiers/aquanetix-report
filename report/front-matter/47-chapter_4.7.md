### 4.7. Software Object-Oriented Design

El desarrollo estructural de nuestra plataforma se fundamenta estrictamente en el paradigma orientado a objetos. Esta decisión metodológica nos brinda la capacidad de segmentar los distintos procesos del negocio hídrico garantizando una expansión futura sin fricciones. A través de la correcta aplicación del encapsulamiento para proteger la información corporativa, sumado a la herencia para jerarquizar nuestras entidades de monitoreo, diseñaremos componentes de software robustos, facilitando enormemente las labores de actualización técnica.

### 4.7.1. Class Diagrams

<div align="center"><img src="../assets/c4_diagrams/Diagrama_de_clase.png" width ="100%"></div>

### 4.7.2. Class Dictionary

#### Clase: Enterprise
Descripción: Representa a las organizaciones registradas en el sistema (EPS, Operadores de Residuos, Entidades Reguladoras). Es la raíz (Aggregate Root) que agrupa a usuarios, sensores y flota.
##### Atributos:
>* Id : int - Identificador único de la empresa.
>* Name : String - Nombre legal o razón social.
>* TaxId_RUC : String - Registro Único de Contribuyente.
##### Métodos:
>* CalculateFootprint() : decimal - Calcula la huella hídrica total consolidando los datos operativos.
>* UpgradePlan(newPlan: SubscriptionPlan) : void - Actualiza el plan de suscripción de la empresa.
#### Clase: User
Descripción: Entidad que representa a los actores que interactúan con el sistema (Ingenieros, Auditores, Administradores).
##### Atributos:
>* Id : int - Identificador único.
>* FullName : String - Nombre completo del usuario.
>* Email : String - Correo corporativo (usado para inicio de sesión).
>* PasswordHash : String - Contraseña encriptada (Privado por seguridad).
>* UserRole : Role - Enumeración que define los permisos del usuario.
##### Métodos:
>* Authenticate(password: String) : bool - Valida las credenciales de acceso.
UpdateLastLogin() : void - Registra la marca de tiempo del último acceso (Protegido).

#### Clase: Sensor
Descripción: Representa los dispositivos IoT físicos instalados en campo (pozas, tuberías) que miden variables en tiempo real.
##### Atributos:
>* Id : int - Identificador único.
>* Location : String - Ubicación física del sensor.
>* IsActive : bool - Indica si el sensor está transmitiendo actualmente.
>* Type : SensorType - Enumeración (Flujo, Ultrasonido, Turbidez).
##### Métodos:
>* RecordData(value: decimal) : TelemetryData - Recibe y persiste un nuevo dato de medición.
>* TriggerAlert(severity: AlertSeverity) : Alert - Genera una alerta interna si se supera un umbral (Privado).
  
#### Clase: Alert
Descripción: Almacena los eventos anómalos o críticos detectados por el sistema que requieren atención del Ingeniero Operativo.
##### Atributos:
>* Id : int - Identificador de la alerta.
>* Message : String - Descripción del problema (ej. "Posible desborde").
>* Severity : AlertSeverity - Nivel de gravedad (Bajo, Medio, Crítico).
>* IsResolved : bool - Bandera que indica si la incidencia ya fue atendida.
##### Métodos:
>* ResolveAlert(userId: int) : void - Cambia el estado de la alerta y registra qué usuario la solucionó.

#### Clase: WaterLog
Descripción: Entidad encargada de registrar los ingresos de agua (cisternas o red pública) para el control de la huella hídrica y la sostenibilidad financiera.
##### Atributos:
>* Id : int - Identificador del registro.
>* VolumeLiters : decimal - Cantidad de agua ingresada al sistema.
>* TotalCost : decimal - Costo monetario de la compra de agua (en Soles).
>* Source : String - Origen del recurso hídrico.
##### Métodos:
>* CalculateCostPerLiter() : decimal - Devuelve el costo unitario para generar métricas de eficiencia.

#### Clase: SubscriptionPlan
Descripción: Define los planes comerciales que determinan los límites operativos y costos para las empresas suscritas al sistema.
##### Atributos:
>* Id : int - Identificador del plan.
>* Name : String - Nombre comercial (Ej. "Plan Piloto", "Plan Integral").
>* MonthlyCost : decimal - Costo mensual de la licencia.
>* MaxSensors : int - Límite de dispositivos IoT permitidos.
##### Métodos:
>* VerifyLimit(currentSensors: int) : bool - Valida si la empresa puede registrar un sensor nuevo según su plan actual.
  
#### Clase: TelemetryData
Descripción: Almacena el historial continuo de lecturas enviadas por los sensores IoT en campo. Es una entidad de alto volumen de datos.
##### Atributos:
>* Id : long - Identificador de la lectura (BigInt debido al volumen).
>* Value : decimal - Valor numérico registrado (pH, %, litros).
>* Timestamp : DateTime - Fecha y hora exacta en la que el sensor capturó el dato.
##### Métodos:
>* ExportToCsv() : String - Genera un volcado de datos en formato CSV para que los auditores procesen la información externamente.
  
#### Interfaz: IAlertNotifier
Descripción: Contrato que define la estructura para servicios externos (como SendGrid o Twilio) encargados de enviar notificaciones push, SMS o correos electrónicos.
##### Métodos:
>* SendNotification(alertId: int, email: String) : bool - Ejecuta el envío de la alerta crítica al usuario correspondiente.
>* RegisterDeviceToken(token: String) : void - Registra el token del dispositivo móvil para habilitar notificaciones push.

#### Enumeración: Role
>* Descripción: Define los niveles de acceso y autorización dentro de la plataforma Aquanetix.
>* Valores: Admin, Engineer, Auditor.

#### Enumeración: SensorType
>* Descripción: Clasifica el tipo de hardware IoT desplegado en la infraestructura.
>* Valores: Ultrasonic (medición de nivel en pozas), Flow (caudal en tuberías), Turbidity (calidad del agua).

#### Enumeración: AlertSeverity
>* Descripción: Categoriza el nivel de urgencia de las incidencias operativas.
>* Valores: Low, Medium, Critical.


