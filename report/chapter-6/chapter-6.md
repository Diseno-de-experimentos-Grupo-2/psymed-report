# Capítulo VI: Product Verification & Validation

## 6.1. Testing Suites & Validation
En esta sección se describen las pruebas realizadas para verificar y validar el producto desarrollado, asegurando que cumple con los requisitos especificados y funciona correctamente en diferentes escenarios. Se detallan las pruebas unitarias, de integración, de comportamiento y del sistema.

## 6.1.1. Core Entities Unit Tests.

Los Core Entities Unit Tests se centran en verificar la funcionalidad de las entidades principales del sistema PSYMED. Estas pruebas aseguran que las entidades individuales funcionan correctamente de manera aislada, sin depender de otras partes del sistema.

El backedn de PSYMED está desarrollado en Java utilizando el framework Spring Boot, y las pruebas unitarias se implementan utilizando JUnit y Mockito. A continuación, se describen algunas de las pruebas unitarias realizadas para las entidades principales del sistema.

- Bounded context Medication:
  ```getId() test```
  
<img src="https://github.com/user-attachments/assets/2de3127d-060d-4520-b793-06ba056bf2eb" />

```getName() test```

<img src="https://github.com/user-attachments/assets/f92236ee-8b37-489e-b95c-b261ad93b30d" />


```getDescription()```

<img src="https://github.com/user-attachments/assets/7900ac5a-792f-4cf0-b6d2-4453e142f6fc" />


```getPatientId()```

<img src="https://github.com/user-attachments/assets/25d56c1c-5d80-4284-be05-c56e6b32e890" />


```getInterval()```

<img src="https://github.com/user-attachments/assets/360f0a66-0a0d-4cee-a8f5-b996bf418183" />

```getQuantity()```

<img src="https://github.com/user-attachments/assets/74f89ce1-8f84-4448-a9f6-62ebeef77a1b" />


Pruebas unitarias para validar ingreso de registro de funciones biológicas del paciente

Los únicos valores permitidos son del 0 al 5

```Hydration```

<img src="https://github.com/user-attachments/assets/1886452d-4c5d-4871-9bc6-f6b76987a7a9" />

```Hunger```

<img src="https://github.com/user-attachments/assets/7b49227f-0088-474d-ba23-81ae1f35513b" />


```Sleep```

<img src="https://github.com/user-attachments/assets/392de06c-0650-4bc5-b7af-732a935f295f" />


```Energy```

<img src="https://github.com/user-attachments/assets/22e7d689-1e1a-43b1-838c-3bc7f5ab0219" />


- Mood status:

Pruebas unitarias para validar ingreso de registro del estado de ánimo del paciente

<img src="https://github.com/user-attachments/assets/4f3bef8f-8d78-43b3-9d20-5a96e4acf7e9" />

- Session class

Esta prueba unitaria valída que las citas no se pueden crear en el pasado o en el futuro.

<img src="https://github.com/user-attachments/assets/33b739cc-5381-4b70-bb3f-e2f95126237d" />


- Session Command Service

Esta prueba unitaria utiliza

<img src="https://github.com/user-attachments/assets/1873802e-3139-4295-845b-76a411bb0aba" />


También se valida que las citas deben ser en el futuro

<img src="https://github.com/user-attachments/assets/7ba02f31-8e84-445c-9aa2-af7064242c21" />


ProfessionalSessionController:
No se pueden crear citas sin el id del paciente

<img src="https://github.com/user-attachments/assets/ea4bb53b-3728-4627-85aa-6e21dc9a0c29" />

De la misma manera no se puede crear una sesión sin el profesional de salud:

<img src="https://github.com/user-attachments/assets/c71ae864-90a4-40dc-a302-7da43904c1de" />

Tampoco se pueden crear sesiones con más de un médico

<img src="https://github.com/user-attachments/assets/c43d3995-094c-401f-b97a-537d7b7e95cb" />

<img src="https://github.com/user-attachments/assets/e39501da-dcf0-4cc4-b3c5-1914550e288d" />

IAM:

Validar creación de cuentas de acuerdo al rol del usuario (profesional o paciente)

<img src="https://github.com/user-attachments/assets/9c9d1ce6-a219-4eb6-be9a-b136aed9ed37" />

Profiles:

Solo se aceptan direcciones sin comas por reglas de negocio

<img src="https://github.com/user-attachments/assets/1b767a7a-fd21-45ae-a019-eea3a0803665" />

## 6.1.2. Core Integration Tests.

Esta seccion describe las pruebas de integración realizadas en funcionalidades Core del negocio.

Resultado al usar ```mvn test```

Prueba integral

<img src="https://github.com/user-attachments/assets/3f1effbc-d85c-4237-8226-1374470f5774" />


- PillController Test

<img src="https://github.com/user-attachments/assets/d9727712-89eb-4af7-82ee-41b8c8876297" />


- Biological Function Controller:

<img src="https://github.com/user-attachments/assets/7f4e6c09-3ed2-498a-84e8-c57bf31f3134" />


- MoodState Controller

<img src="https://github.com/user-attachments/assets/532f5bfa-2cc7-429a-8a29-bf2fb0059903" />


- SessionReservationController

<img src="https://github.com/user-attachments/assets/9009ee96-5b50-4e9f-ab06-b05626fb0dae" />


- IAM:

<img src="https://github.com/user-attachments/assets/e090e41a-9a12-40f9-aa79-4a656823c545" />

Solo debe retornar una cuenta cuando se verifica que esta existe

<img src="https://github.com/user-attachments/assets/7fa62fd8-26b1-4cc8-928e-2d72f060becd" />


Authentication Controller Test

Se verifica la cuenta cuando el usuario hace sign in exitosamente

<img src="https://github.com/user-attachments/assets/b7ccd37f-3d58-43db-b013-e7afa9c1914a" />


## 6.1.3. Core Behavior-Driven Development

En esta sección se describen las pruebas de desarrollo guiado por comportamiento (BDD) realizadas para validar las funcionalidades principales del sistema PSYMED.
Se usa lenguaje Gherkin para definir los escenarios de prueba de manera clara y comprensible para todos los miembros del equipo, incluyendo desarrolladores, testers y stakeholders.

Estos archivos se encuentran en el repositorio: https://github.com/Diseno-de-experimentos-Grupo-2/psymed-features.git

<img src="https://github.com/user-attachments/assets/2e0164f1-835f-4911-adba-6312333119bd" />

A continuación, se presentan los archivos de características (feature files) que agrupan las historias de usuario relacionadas:

# Archivo: EP01_Acceso_y_Perfil.feature

Feature: Gestión de Acceso y Perfil de Usuarios
Como usuario (profesional de la salud mental o paciente),
Quiero registrarme, iniciar sesión y ver mi perfil,
Para poder acceder a las funcionalidades y validar mi información.

Background:
Given el usuario no está autenticado

# Historia de Usuario US01 y US03: Registro e Inicio de Sesión (Profesional)
@EP01 @Autenticacion @Profesional
Scenario Outline: Registro e Inicio de Sesión de Profesional
Given el profesional de la salud mental está en la página de Registro
When completa todos los campos del formulario de registro con entradas <validez>
And pulsa el botón "Crear cuenta"
Then el sistema debería mostrar el resultado <resultado_registro>
And el profesional debería ser dirigido a <pagina_destino>

    Examples:
      | validez | resultado_registro | pagina_destino |
      | válida  | la cuenta se crea  | el panel de control con rol de profesional |
      | incompleta | un mensaje de error indicando campos faltantes | la página de Registro |
      | con credenciales ya usadas | un mensaje de error indicando que el correo ya está en uso | la página de Registro |

# Historia de Usuario US02 y US12: Inicio de Sesión (Paciente)
@EP01 @Autenticacion @Paciente
Scenario Outline: Inicio de Sesión de Paciente
Given el paciente está en la pantalla "Bienvenido" e ingresa credenciales <validez_login>
When pulsa el botón "Iniciar Sesión"
Then el sistema debería validar las credenciales con <resultado_login>
And el paciente debería ser dirigido a <pagina_destino_login>

    Examples:
      | validez_login | resultado_login | pagina_destino_login |
      | correctas | éxito | la pantalla principal con rol de paciente |
      | incorrectas | un mensaje de error de contraseña incorrecta | la pantalla de Inicio de Sesión |
      | campos vacíos | un mensaje de error de campos incompletos | la pantalla de Inicio de Sesión |

# Historias US02 y US03: Recuperación de Contraseña
@EP01 @Autenticacion @Recuperacion
Scenario: Solicitud de Recuperación de Contraseña
Given el usuario (paciente o profesional) ha olvidado su contraseña
When hace clic en el botón "Olvidé mi contraseña"
Then la plataforma envía un enlace de restablecimiento al correo electrónico registrado.

# Historia de Usuario US04: Registro de Datos Personales del Paciente (Profesional)
@EP01 @GestionDatos @Profesional
Scenario Outline: Registro de Información Personal del Paciente
Given el profesional de la salud mental está en el formulario de registro de información personal del paciente
When ingresa los datos de forma <estado_datos>
And hace clic en el botón "Guardar"
Then el sistema <accion_sistema>

    Examples:
      | estado_datos | accion_sistema |
      | completa | registra la información correctamente y la hace disponible para consultas. |
      | incompleta | muestra un mensaje de error indicando qué campos faltan por completar. |

# Historia de Usuario US13: Visualizar Información de Perfil (Paciente)
@EP01 @Perfil @Paciente
Scenario: Visualización de Información de Perfil
Given estoy en la aplicación y navego a la pestaña "Profile"
Then veo mi Nombre completo
And veo mi Correo Electrónico asociado
And veo mi Dirección
And veo mi ID de Paciente y mi ID de Profesional asignados

# Historia de Usuario US14: Cerrar Sesión (Paciente)
@EP01 @Autenticacion @Paciente
Scenario: Cerrar Sesión de Forma Segura
Given estoy en la pantalla "Mi Perfil" y he iniciado sesión
When pulso el botón "Cerrar Sesión"
Then la sesión actual se cierra exitosamente
And soy redirigido a la pantalla de Inicio de Sesión


2. Funcionalidades de Seguimiento de Salud (EP02_Seguimiento_Salud.feature)
   Este archivo agrupa las historias relacionadas con el registro y la visualización del estado emocional y biológico del paciente (US05, US06, US07, US15).

# Archivo: EP02_Seguimiento_Salud.feature

Feature: Registro y Visualización del Estado de Salud
Como paciente, quiero registrar mi estado emocional y biológico,
Y como profesional, quiero visualizar esta información,
Para evaluar el bienestar y el progreso del paciente.

# Historia de Usuario US06, US07 y US15: Registro Diario de Salud (Paciente)
@EP02 @Paciente @Registro
Scenario Outline: Registro del Estado de Salud Diario
Given el paciente se encuentra en la sección/pestaña "Health"
When registra su estado de ánimo actual
And selecciona su nivel de sueño, hambre, energía e hidratación en una escala del 1 al 5
Then la plataforma debe <resultado>

    Examples:
      | resultado |
      | actualizar su estado emocional en el perfil del paciente. |
      | guardar el registro de ese día y mostrar un mensaje de confirmación. |

@EP02 @Paciente @Registro
Scenario: Reintento de Registro en el Mismo Día
Given el paciente ya ha completado el registro de su estado de salud hoy
When navega a la pestaña "Health"
Then ve un mensaje o un botón deshabilitado que indica "Ya registrado hoy", impidiendo un nuevo registro.

# Historia de Usuario US06: Historial de Estados de Ánimo (Paciente)
@EP02 @Paciente @Historial
Scenario: Visualización del Historial de Estados de Ánimo
Given el paciente se encuentra en la sección de registros de estado emocional
And posee un registro con cada uno de los estados que ingresó con anterioridad
When ingresa al historial de estados de ánimo
Then la plataforma debe mostrar un calendario con los estados del paciente a lo largo del tiempo.

# Historia de Usuario US05: Visualización del Estado de Ánimo (Profesional)
@EP02 @Profesional @Visualizacion
Scenario Outline: Visualización del Estado de Ánimo del Paciente
Given el profesional de la salud mental ha accedido al perfil del paciente
When selecciona la opción de visualizar estados de ánimo
Then la plataforma <muestra_datos>

    Examples:
      | muestra_datos |
      | muestra el estado de ánimo del paciente que se registró el mismo día. |
      | no muestra los datos ingresados si no hay registros recientes. |
3. Funcionalidades de Medicamentos (EP03_Medicamentos.feature)
   Este archivo aborda la prescripción y el seguimiento del tratamiento farmacológico (US08, US09, US16).


# Archivo: EP03_Medicamentos.feature

Feature: Gestión y Consulta de Medicamentos
Como profesional de la salud, quiero registrar la medicación,
Y como paciente, quiero poder consultarla,
Para seguir adecuadamente el tratamiento farmacológico.

# Historia de Usuario US08: Registro de Medicamentos (Profesional)
@EP03 @Profesional @Registro
Scenario Outline: Registro de Medicamentos Asignados
Given el profesional de la salud mental ha ingresado los datos de los medicamentos de su paciente de forma <estado_datos>
When hace clic en un botón de "Guardar"
Then la plataforma <accion_plataforma>

    Examples:
      | estado_datos | accion_plataforma |
      | completa | registra los datos del medicamento correctamente y los asocia al perfil del paciente. |
      | incompleta | muestra un mensaje de error indicando los campos incompletos o incorrectos. |

# Historia de Usuario US09 y US16: Consulta de Lista de Medicamentos (Paciente)
@EP03 @Paciente @Consulta
Scenario: Visualización de Lista de Medicamentos
Given el paciente entra a la plataforma e ingresa a la pestaña "Medication"
When ingresa a la vista de medicamentos
Then puede ver una lista de todos los medicamentos recetados
And para cada medicamento, se muestra el Motivo, el Intervalo (frecuencia) y la Cantidad.
4. Funcionalidades de Citas (EP04_Citas.feature)
   Este archivo se enfoca en el agendamiento y la visualización de las citas médicas (US10, US11, US17).


# Archivo: EP04_Citas.feature

Feature: Gestión de Citas Médicas
Como profesional, quiero agendar citas,
Y como paciente, quiero ver mi agenda,
Para planificar y asegurar la asistencia a las sesiones.

# Historia de Usuario US10: Creación de Citas (Profesional)
@EP04 @Profesional @Agenda
Scenario: Creación de una Nueva Cita
Given el profesional de salud entra a la plataforma
When ingresa a la vista de citas sobre el perfil de un paciente
Then puede registrar una nueva cita, incluyendo fecha, hora y duración.

# Historia de Usuario US11 y US17: Visualización de Citas (Paciente)
@EP04 @Paciente @Agenda
Scenario: Visualización de Próximas Citas Médicas
Given el paciente entra a la plataforma y navega a la vista de citas
When ingresa a la vista de citas
Then puede ver la sección "Próximas Citas"
And ve una lista de citas, donde cada una muestra la Fecha, la Hora, la Duración y el Profesional ID.

@EP04 @Paciente @Agenda
Scenario: Identificación de Cita Programada para Hoy
Given el paciente está visualizando su lista de Próximas Citas
And hay una cita programada para la fecha actual
Then esta cita debe mostrar una etiqueta distintiva con el texto "HOY".

5. Funcionalidades de Landing Page (EP05_Landing_Page.feature)
   Este archivo contiene las historias relacionadas con la experiencia del visitante y la presentación inicial de la aplicación (US18, US19, US20).


## Archivo: EP05_Landing_Page.feature

Feature: Experiencia del Visitante en la Landing Page
Como visitante de la Landing Page,
Quiero ver información clara y un diseño atractivo,
Para comprender rápidamente el valor de la aplicación y facilitar mi lectura.

Background:
Given el visitante se encuentra en la landing page
When explora la página principal

# Historia de Usuario US18: Propósito y Contenido
@EP05 @Contenido @Comunicacion
Scenario: Claridad del Propósito de la Aplicación
Then la landing page debe poseer información clara y concisa que explique el propósito de la aplicación.

# Historia de Usuario US19: Elementos Visuales
@EP05 @Diseño @Visual
Scenario: Calidad y Relevancia de Imágenes y Gráficos
Then la landing page debe presentar imágenes de alta calidad y relevantes que capten la atención del visitante
And la landing page debe mostrar gráficos que ayuden al visitante a comprender el contenido.

# Historia de Usuario US20: Tipografía y Legibilidad
@EP05 @Diseño @Legibilidad
Scenario: Consistencia y Comodidad de la Tipografía
Then la landing page debe poseer una tipografía clara y de un tamaño adecuado para facilitar la lectura
And la landing page debe mostrar un estilo tipográfico consistente para mantener la coherencia visual.


## 6.1.4. Core System Tests.

A continuación, se presentan las pruebas del sistema realizadas para validar la funcionalidad completa de PSYMED. Para ello se utilizó la herramienta Selenium, que permite automatizar las pruebas de la interfaz de usuario y simular interacciones reales con el sistema.

Cada prueba está validada por los user stories:

### Versión Web

- US01	Registro como profesional de la salud mental

Como profesional de la salud mental quiero registrarme con mis credenciales para poder acceder a las funcionalidades específicas y gestionar la información de mis pacientes.

<img src="https://github.com/user-attachments/assets/fe36685e-3b6f-4ada-851f-6118a49745e1" />

- US02	Inicio de sesión como pacientes

Como paciente, quiero iniciar sesión en la plataforma para acceder a mi información personal y seguimiento de tratamiento.

<img src="https://github.com/user-attachments/assets/68383287-2738-432f-aed6-f0d65dadfa3b" />

- US03	Inicio de sesión como profesional de la salud mental

Como profesional de la salud mental, quiero iniciar sesión en la plataforma para gestionar la información de mis pacientes y acceder a herramientas de seguimiento.

<img src="https://github.com/user-attachments/assets/a7f60860-edcb-4079-b530-0f3b8e069a49" />

- US04	Registro de información personal del paciente

Como profesional de la salud mental, quiero registrar la información personal del paciente para tener una referencia detallada y precisa de sus datos básicos en cada consulta.

<img src="https://github.com/user-attachments/assets/f49a2b65-35eb-42e3-b410-81c2bdb3e052" />

- US05	Visualización del estado actual de ánimo del paciente

Como profesional de la salud mental, quiero visualizar el estado de ánimo actual del paciente para evaluar su condición emocional.

<img src="https://github.com/user-attachments/assets/517488bc-032c-4c4b-aec7-eda3a1a69e6a" />

- US06	Registro de estado de ánimo

Como paciente, quiero comunicarle a mi profesional mi estado de ánimo para ver mi estado actual.

<img src="https://github.com/user-attachments/assets/47fdc90f-1ce4-43f1-8601-bb128153590d" />

Solo puede registrarse el estado de ánimo una vez al día

<img src="https://github.com/user-attachments/assets/9c8b24cd-2492-41bd-988c-d73ba9992213" />

- US07	Registro de funciones biológicas

Como paciente, quiero registrar la calidad de mis funciones biológicas para que mi paciente conozca mi estado actual de salud.

<img src="https://github.com/user-attachments/assets/e3941525-2db2-4497-9392-e6597dae2367" />


- US08	Registro de medicamentos del paciente

Como profesional de la salud mental, quiero registrar los medicamentos del paciente para seguir adecuadamente su tratamiento farmacológico

<img src="https://github.com/user-attachments/assets/eb15442f-db73-4bbb-b7ad-5136a61a036a" />


- Ver medicamentos

Como paciente quiero poder ver los medicamentos que mi profesional de salud mental ha asignado para poder estar pendiente de cuales consumir

<img src="https://github.com/user-attachments/assets/6844c2bc-69bf-4c84-b2dc-5ee71e7c8e18" />


- Creación de citas

Como profesional de la salud quiero agendar las citas de mis pacientes

<img src="https://github.com/user-attachments/assets/e32a0d39-dc93-4509-b31c-ddf4958da6c9" />


- Ver citas médicas

Como paciente quiero poder ver las citas médicas programadas para poder saber que días ir al consultorio del profesional de salud mental

<img src="https://github.com/user-attachments/assets/152d1c1a-0136-4ccb-ad55-fc762ee5ea90" />


### Versión Móvil

- US12	Iniciar Sesión como Paciente:

Como Paciente, quiero poder iniciar sesión con mi usuario y contraseña para acceder a mi información personal y de salud dentro de la aplicación.

<img src="https://github.com/user-attachments/assets/010d7484-3461-4c85-9c71-dd3627833d7a" />


- US13	Visualizar Información de Perfil:

Como Paciente, quiero poder ver mi información personal (Correo Electrónico, Dirección, ID de Paciente y ID de Profesional) en la sección "Mi Perfil" para confirmar que mis datos son correctos.

<img src="https://github.com/user-attachments/assets/927737b9-901f-4ff8-9ad9-f3570ce4748a" />

- US14	Cerrar Sesión:

Como Paciente, quiero poder cerrar mi sesión de forma segura desde la pantalla de Mi Perfil para proteger mi privacidad.

<img src="https://github.com/user-attachments/assets/dfda97a6-4b69-4b7e-8d0f-f3b95ec0d5a3" />

- US15	Registrar Mi Estado de Salud Diario:

Como Paciente, quiero poder registrar mi estado de salud diario (Mood, Hunger, Hydration, Sleep Quality, Energy Level) para llevar un seguimiento de mi bienestar.

<img src="https://github.com/user-attachments/assets/af11c2dd-44f5-4ea9-bb85-423d60b159a2" />


- US16	Consultar Mi Lista de Medicamentos:

Como Paciente, quiero poder ver la lista de medicamentos que tengo asignados para conocer el nombre, el motivo, la frecuencia (Intervalo) y la Cantidad de cada uno.

<img src="https://github.com/user-attachments/assets/79b82a41-10cb-42f4-9c8d-d341a9850327" />

- US17	Ver Próximas Citas:
  Como Paciente, quiero poder ver una lista de mis citas médicas próximas con sus detalles (fecha, hora, duración y profesional ID) para estar informado y planificar mi asistencia.
  
<img src="https://github.com/user-attachments/assets/bdff83fc-5368-4bba-8f72-09d30fdea540" />


## 6.2. Static testing & Verification
## 6.2.1. Static Code Analysis
#### 6.2.1.1. Coding standard & Code conventions.

En el código desarrollado se emplearon los lenguajes Java y TypeScript, aplicando sus respectivos estándares de 
codificación. Para Java, se siguieron las convenciones definidas por la Google Java Style Guide, garantizando una 
estructura clara, legible y coherente en nombres, formato y documentación. En el caso de TypeScript, utilizado 
dentro del framework Angular, se aplicaron las recomendaciones de la Angular Style Guide y las reglas de ESLint, 
asegurando buenas prácticas en la organización de archivos, nomenclatura y consistencia del código.

#### 6.2.1.2. Code Quality & Code Security.

En el desarrollo del proyecto se aplicaron prácticas de control de calidad y seguridad del código tanto en **Java** como en **TypeScript (Angular)**.  
Para evaluar la calidad del código, se consideraron métricas de complejidad, duplicación y mantenibilidad, empleando herramientas como  **ESLint**, que permitió detectar y corregir inconsistencias según los estándares de codificación definidos (*Google Java Style Guide* y *Angular Style Guide*).

En cuanto a la seguridad, se realizó la verificación de posibles vulnerabilidades comunes, como **inyecciones SQL**, y **manejo inseguro de datos sensibles**, asegurando que el código mantuviera altos niveles de **robustez**, **integridad** y **protección** frente a amenazas.

### 6.2.2. Reviews

Se realizó una revisión exhaustiva del código desarrollado en **Java** y **TypeScript (Angular)** con el 
objetivo de asegurar la correcta implementación de las buenas prácticas previamente mencionadas en cuanto a 
**calidad** y **seguridad**. Estas revisiones permitieron verificar el cumplimiento de los estándares de codificación,
así como la adecuada gestión de la **complejidad**, **mantenibilidad** y la mitigación de 
vulnerabilidades como **inyecciones SQL**, y manejo de datos sensibles.

## 6.3. Validation Interviews.
### 6.3.1. Diseño de Entrevistas.

Preguntas para segmento profesionales:

- ¿Qué tan fácil te resultó entender cómo crear un nuevo usuario o iniciar sesión?

- ¿Te pareció intuitivo el proceso para registrar un paciente o ingresar medicamentos/citas?

- ¿Hubo algún momento en el video en el que te sentiste confundido o perdiste el hilo de lo que pasaba?

- Si tuvieras que hacer tú mismo las acciones que mostró el video (crear usuario, registrar medicamento, etc.), ¿crees que podrías hacerlo sin ayuda?

- ¿Qué mejorarías para que la app sea más fácil de usar?

- ¿Te resultó clara la parte del registro del estado emocional y biológico?

- ¿Crees que esta app te ayudaría a estar más consciente del estado del paciente?

- ¿Cómo te sentiste al ver la app? (por ejemplo: tranquilo, confundido, interesado, indiferente)

- ¿Sientes que la app respeta la privacidad y la sensibilidad de la información de salud mental?

Preguntas para segmento pacientes:

- ¿Qué tan fácil te resultó entender cómo crear un nuevo usuario o iniciar sesión?

- ¿Te pareció intuitivo el proceso para registrar un paciente o ingresar medicamentos/citas?

- ¿Hubo algún momento en el video en el que te sentiste confundido o perdiste el hilo de lo que pasaba?

- Si tuvieras que hacer tú mismo las acciones que mostró el video (crear usuario, registrar medicamento, etc.), ¿crees que podrías hacerlo sin ayuda?

- ¿Qué mejorarías para que la app sea más fácil de usar?

- ¿Te resultó clara la parte del registro del estado emocional y biológico?

- ¿Te gustaría recibir recordatorios de tus citas o medicamentos?

- ¿Te sentirías cómodo registrando tu estado de ánimo todos los días?

- ¿Crees que esta app te ayudaría a estar más consciente de tu salud mental?

- ¿Cómo te sentiste al ver la app? (por ejemplo: tranquilo, confundido, interesado, indiferente)

- ¿Sientes que la app respeta la privacidad y la sensibilidad de la información de salud mental?

- ¿Qué tan confiable te parece el sistema para manejar información médica?

### 6.3.2. Registro de Entrevistas.

Entrevistas a segmento profesionales:

- Entrevista 1:

![WhatsApp Image 2025-11-06 at 11 39 00 PM](https://github.com/user-attachments/assets/d236f0f9-7542-455b-a9d0-4742c60feb45)


| Nombre               | Karina    |
|----------------------|-----------|
| Apellido             | Ramirez   |
| Edad                 | 51 años   |
| Distrito             | La Molina |
| URL                  | https://acortar.link/W1pxX8           |
| Inicio de entrevista | 00:01           |
| Fin de entrevista    | 20:35          |

Resumen de entrevista:

La psicoterapeuta Karina Ramírez Sedano brindó una evaluación detallada de la plataforma PSYMED, destinada a facilitar la gestión de pacientes, sesiones, tareas y seguimiento emocional y físico por parte de psicólogos y psiquiatras.

Desde el inicio, la entrevistada consideró que la interfaz de registro de pacientes es clara y funcional, ya que permite recopilar los datos básicos necesarios para abrir una historia clínica y comenzar el seguimiento del tratamiento. Destacó que el sistema facilita la organización inicial y constituye un filtro adecuado para el trabajo terapéutico.

Respecto al módulo de citas, indicó que la aplicación resulta sencilla de usar y adaptable a las dinámicas de sesión, que suelen durar entre 45 y 50 minutos. Apreció que la agenda pueda registrar sesiones semanales y que el sistema no permita programar fechas anteriores, lo cual refuerza la coherencia del registro.

En cuanto al seguimiento emocional del paciente, valoró la idea de que el usuario registre su estado diario, aunque advirtió que en casos clínicos como la depresión los cambios podrían no reflejar una mejora inmediata. Señaló que esta función debe servir como apoyo complementario, más que como indicador clínico determinante.

Sobre la vista de datos físicos y medicamentos, consideró que es útil para psiquiatras y que los psicólogos podrían beneficiarse de tener acceso limitado a esta información. No obstante, enfatizó la importancia de garantizar la privacidad, proponiendo que la aplicación incluya un espacio exclusivo para el profesional, donde se guarden notas confidenciales, protegidas mediante cifrado o acceso restringido.

En términos de usabilidad, Karina Ramírez afirmó que la plataforma es intuitiva y visualmente clara. Recomendó incorporar tonos pastel y colores suaves, que transmitan tranquilidad y cercanía. También sugirió que las sesiones o tareas aparezcan estructuradas como “libretos digitales”, simulando los cuadernos que usan los pacientes en terapia presencial.

Sobre la versión móvil, opinó que es conveniente contar con ambas opciones (web y móvil), ya que los psicoterapeutas suelen trabajar virtualmente con computadoras, mientras que los pacientes usan más el teléfono.

Finalmente, consideró que la plataforma favorece la conciencia emocional del paciente y facilita el seguimiento terapéutico. Recalcó la necesidad de mantener altos estándares de seguridad y confidencialidad, especialmente en la información compartida entre distintos profesionales de salud. Concluyó destacando que el proyecto es innovador, funcional y de gran utilidad para el ámbito psicológico y psiquiátrico.

- Entrevista 2:

![WhatsApp Image 2025-11-08 at 12 04 54 PM](https://github.com/user-attachments/assets/b29e3748-54f2-481f-bfca-aa277d20838a)


| Nombre               | Hortensia      |
|----------------------|----------------|
| Apellido             | Piedra Cáceres |
| Edad                 | 36 años        |
| Distrito             | Arequipa       |
| URL                  | https://acortar.link/xlvlUg               |
| Inicio de entrevista | 00:01               |
| Fin de entrevista    | 17:05               |

Resumen de entrevista:

La psicóloga clínica Hortensia Piedra Cáceres, residente en Arequipa, brindó una evaluación detallada de la plataforma Psymed, un sistema web y móvil diseñado para optimizar la gestión de pacientes, citas y seguimiento emocional y físico en el ámbito psicológico y psiquiátrico.

Desde el inicio, la entrevistada consideró que el proceso de inicio de sesión es claro y sencillo, permitiendo distinguir adecuadamente entre el acceso de pacientes y profesionales. En cuanto al registro de pacientes, sugirió incluir información adicional como la edad y antecedentes de terapia previa, para enriquecer la historia clínica inicial.

Respecto al módulo de citas, destacó su facilidad de uso y propuso añadir opciones que reflejen distintos tipos de atención, como evaluaciones psicológicas, entregas de informes, orientación vocacional o terapias grupales (DBT). También recomendó incorporar campos para registrar costos, paquetes de sesiones y reprogramaciones, ya que son aspectos frecuentes en la práctica clínica.

Sobre el seguimiento emocional y físico, valoró que el paciente pueda registrar su estado diario, pero sugirió incluir un campo de notas donde exprese la causa o contexto de sus emociones, facilitando el análisis posterior en sesión. Consideró apropiado mantener cierta separación entre la información del psicólogo y la del psiquiatra, por motivos de confidencialidad.

En el ámbito de la versión móvil, la psicóloga afirmó que sería útil para profesionales, especialmente para consultar citas y el progreso de sus pacientes. Recalcó la conveniencia de que los terapeutas puedan acceder también desde el celular, no solo desde la computadora.

En términos de diseño y usabilidad, propuso emplear colores cálidos (melón, beige, café claro) en lugar de tonos fríos o clínicos, con el fin de generar cercanía y evitar una estética hospitalaria. También sugirió incorporar pequeñas imágenes decorativas que aporten calidez visual.

Finalmente, consideró que SciMed respeta la privacidad del paciente, dado que el registro emocional es parte del proceso terapéutico. Recomendó agregar el motivo de consulta y un sistema para asignar tareas terapéuticas, donde el paciente pueda indicar si comprendió la actividad y cómo se sintió al realizarla.

Concluyó afirmando que la plataforma es intuitiva, funcional y pertinente para el trabajo psicológico, y que con las mejoras propuestas podría convertirse en una herramienta integral para la práctica clínica y el acompañamiento terapéutico.

- Entrevista 3:

![WhatsApp Image 2025-11-09 at 2 11 16 PM](https://github.com/user-attachments/assets/4bbee769-9e23-43ea-b749-1a0a2063e341)

| Nombre               | Valerie        |
|----------------------|----------------|
| Apellido             | Hikaru Ouchida |
| Edad                 | 29 años        |
| Distrito             | Lince          |
| URL                  |                |
| Inicio de entrevista |                |
| Fin de entrevista    |                |

Resumen de entrevista:

Desde el inicio, consideró que el diseño es intuitivo y de fácil uso, destacando la claridad del proceso de inicio de sesión y registro de profesionales. En cuanto al registro de pacientes, recomendó añadir la edad y el motivo de consulta, ya que estos datos permiten contextualizar los casos y facilitan la organización de la información clínica.

Respecto al módulo de citas, coincidió con la necesidad de incluir campos adicionales, como el tipo de sesión (terapia o seguimiento), frecuencia semanal o mensual, número de sesiones y reprogramaciones, lo cual permitiría un control más preciso del tratamiento.

En relación con el seguimiento emocional y físico, consideró muy útil que los pacientes puedan registrar su estado de ánimo diario, aunque subrayó que este módulo requiere compromiso por parte del paciente. Sugirió incorporar un espacio para notas, donde puedan expresar el contexto o las razones detrás de su estado emocional, favoreciendo así el análisis terapéutico.

Sobre la versión móvil, indicó que, por su estilo de trabajo, le resulta más práctico el acceso desde computadora o laptop, ya que facilita la redacción y el registro de información profesional, aunque valoró la utilidad de la aplicación móvil para pacientes.

En cuanto al diseño visual, opinó que la interfaz transmite seriedad, pero podría resultar demasiado médica. Propuso añadir ilustraciones minimalistas relacionadas con la salud mental y usar colores más cálidos o pasteles (como crema o café claro), con el fin de generar un entorno más acogedor y menos clínico.

En conclusión, la psicóloga consideró que la plataforma SciMed es funcional, clara y pertinente para la práctica clínica, y que con pequeñas mejoras en la presentación visual y la ampliación de ciertos campos, podría convertirse en una herramienta integral para el seguimiento terapéutico y la organización profesional.

Entrevistas a segmento pacientes:

![alt text](/assets/sprint4/entrevista-marco.png)

| Nombre               | Eiji                                                                                                                                                                                                                                                                                                                   |
|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Apellido             | Nakamurakari                                                                                                                                                                                                                                                                                                           |
| Edad                 | 21 años                                                                                                                                                                                                                                                                                                                |
| Distrito             | Pueblo Libre                                                                                                                                                                                                                                                                                                           |
| URL                  | https://upcedupe-my.sharepoint.com/:v:/g/personal/u202210790_upc_edu_pe/EXtAaJUAdK9EuGCCPjmhy7ABrB7VkCpccKvAT9yPiWNc1A?e=P4FBzj&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D |
| Inicio de entrevista | 20:59                                                                                                                                                                                                                                                                                                                  |
| Fin de entrevista    | 21:09                                                                                                                                                                                                                                                                                                                  |

Resumen de la entrevista:

El participante consideró que la aplicación es fácil de usar y comprender, destacando que las opciones para ingresar como paciente o profesional están bien diferenciadas. Sin embargo, sugirió incluir un texto explicativo o guía breve inicial para mejorar la orientación del usuario.

Mencionó que podría realizar las acciones del video sin ayuda, ya que la interfaz es intuitiva, aunque recomendó incorporar tutoriales o mensajes guía dentro de la app para facilitar aún más el uso a nuevos usuarios.

Entre las mejoras propuestas, señaló la necesidad de mensajes de confirmación más visibles, campos con ejemplos o autocompletado, y una guía rápida que oriente los primeros pasos del usuario.

El entrevistado afirmó que le gustaría recibir recordatorios de citas y medicamentos, considerando esta función esencial para garantizar el seguimiento del tratamiento. También indicó que se sentiría cómodo registrando su estado de ánimo diariamente, sobre todo si el proceso fuera visual e interactivo (por ejemplo, con iconos o colores).

Finalmente, expresó que la aplicación ayudaría a mejorar la conciencia sobre su salud mental, ya que permite observar la evolución del bienestar emocional y físico a lo largo del tiempo, fomentando una mejor comunicación con los profesionales de salud y un mayor autocuidado.


### 6.3.3. Evaluaciones según heurísticas.

#### **UX Heuristics & Principles Evaluation**
#### **Usability – Inclusive Design – Information Architecture**

**CARRERA:** Ingeniería de Software  <br>
**CURSO:** Diseño de Experimentos de Ingeniería de Software  <br>
**NRC:** 7508<br>
**PROFESORES:** Julio Manuel Noriega Melendez<br>
**AUDITOR:** Paolo Torres <br>
**CLIENTE(S):** Grupo Go6U<br>

---

#### **SITE o APP A EVALUAR:**
**Psymed** – Aplicación para profesionales de la salud mental y pacientes que facilita la gestión de procesos interactivos entre ambos.

---

#### **TAREAS A EVALUAR:**
El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:

1. Registro de paciente
2. Registro de profesional de la salud mental
3. Inicio de sesión y acceso al panel principal
4. Agendar una cita terapéutica
5. Enviar mensaje al terapeuta o paciente
6. Registrar notas o avances de sesión
7. Visualizar historial clínico
8. Cancelar o reprogramar una cita

No están incluidas en esta versión de la evaluación las siguientes tareas:

1. Generar reportes estadísticos de sesiones
2. Configurar recordatorios automáticos por correo o SMS
3. Integrar pagos en línea
4. Exportar historial clínico a otros formatos
5. Funcionalidades de supervisión entre terapeutas

---

#### **ESCALA DE SEVERIDAD:**

| Nivel | Descripción                                                                                                                                       |
|-------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| **1** | Problema superficial: puede ser fácilmente superado por el usuario o ocurre con muy poca frecuencia. No requiere corrección inmediata.            |
| **2** | Problema menor: ocurre con cierta frecuencia o genera confusión leve. Se recomienda corregir en una futura iteración.                             |
| **3** | Problema mayor: ocurre frecuentemente o impide al usuario completar una tarea sin ayuda. Debe corregirse con prioridad alta.                      |
| **4** | Problema muy grave: impide completamente el uso de la herramienta o compromete la experiencia del usuario. Debe corregirse antes del lanzamiento. |

---

#### **TABLA RESUMEN:**

| # | Problema                                                                                       | Escala de severidad | Heurística / Principio violado                |
|---|------------------------------------------------------------------------------------------------|---------------------|-----------------------------------------------|
| 1 | No existe un botón claro para regresar al panel principal desde la vista de historial clínico. | 3                   | Usability: Libertad y control del usuario     |
| 2 | Los íconos de funciones no tienen etiquetas textuales para lectores de pantalla.               | 2                   | Inclusive Design: Experiencias comparables    |
| 3 | La jerarquía visual de la sección de mensajes no resalta las conversaciones activas.           | 2                   | Information Architecture: Is it usable?       |
| 4 | Al registrar una cita, no se muestra retroalimentación inmediata tras confirmar.               | 3                   | Usability: Visibilidad del estado del sistema |
| 5 | El botón “Cancelar cita” está demasiado próximo al botón “Guardar cambios”.                    | 3                   | Usability: Prevención de errores              |

---

## 6.4. Auditoría de Experiencias de Usuario.
### 6.4.1. Auditoría realizada.
#### 6.4.1.1. Información del grupo auditado.

- Nombre del grupo: Go6U
- Integrantes: Paolo Torres, Romina Maita, Marco Nakasone, Fátima Asmad.
- Producto: Psymed

#### 6.4.1.2. Cronograma de auditoría realizada.

La auditoría se realizó el 09 de noviembre de 2025, durante la semana de 11 del curso.

#### 6.4.1.3. Contenido de auditoría realizada.

### **Evaluación del desempeño del equipo – Proyecto Psymed**

Durante el desarrollo del proyecto **Psymed**, perteneciente a la startup **Go6U**, se evidenció un desempeño sólido y comprometido por parte de todos los integrantes del equipo, tanto en la entrega **TP** como en la entrega **TB1**. Cada miembro asumió responsabilidades específicas que contribuyeron al cumplimiento de los objetivos propuestos dentro del curso **Diseño de Experimentos de Ingeniería de Software**.

La **líder de equipo**, **Romina Guadalupe Maita Falckenheiner**, demostró un alto nivel de organización y liderazgo técnico. Participó activamente en el desarrollo de las *user stories*, la realización de entrevistas y el desarrollo del backend móvil, cumpliendo con todas sus responsabilidades en los plazos establecidos. Su desempeño sobresaliente se reflejó en una calificación máxima, evidenciando un control adecuado de los entregables y una gestión efectiva de la coordinación del grupo.

**Paolo Torres Flores** destacó por su trabajo en la elaboración del *product backlog*, las *user stories* y el desarrollo del *frontend móvil*. Además, participó en el análisis competitivo y en la definición de estrategias y tácticas de posicionamiento. Cumplió de manera oportuna con todas sus asignaciones, mostrando claridad metodológica y consistencia en la documentación de los entregables, lo cual le permitió obtener también la máxima calificación.

Por su parte, **Marco Nakasone Gómez** se encargó del desarrollo de artefactos clave para la fase de diseño, como el *Impact Map*, el *To-Be Scenario Mapping*, la *User Task Matrix* y los *Drivers de propósito y constraint*. Su trabajo evidenció un dominio de las herramientas analíticas y una comprensión profunda del modelo de interacción entre usuarios dentro del contexto de Psymed, cumpliendo con cada actividad dentro de los plazos establecidos.

Finalmente, **Fátima Andrea Asmad Padilla** tuvo un rol fundamental en la revisión y documentación del proyecto, aportando a las correcciones y adaptaciones de capítulos previos y en la elaboración completa del capítulo 7. Su participación fue constante y rigurosa, cumpliendo con todas las entregas dentro de los plazos establecidos y manteniendo la coherencia entre los apartados técnicos y teóricos del informe.

En síntesis, los resultados obtenidos en ambos reportes reflejan un equipo altamente colaborativo, disciplinado y orientado al logro. Todos los integrantes cumplieron sus funciones con eficiencia y compromiso, alcanzando calificaciones equivalentes a **20 sobre 20** en cada una de las entregas. Esto evidencia una gestión integral del proyecto, caracterizada por la responsabilidad individual, la comunicación efectiva y la alineación con los objetivos técnicos y metodológicos del curso.


### 6.4.2. Auditoría recibida.
#### 6.4.2.1. Información del grupo auditor.

Se realizó una auditoría de experiencia de usuario a la aplicación Psymed, llevada a cabo por el auditor Paolo Torres, como parte del grupo Go6U. El objetivo de esta auditoría fue evaluar la usabilidad, el diseño inclusivo y la arquitectura de la información de la aplicación, identificando áreas de mejora para optimizar la experiencia del usuario tanto para profesionales de la salud mental como para pacientes.

#### 6.4.2.2. Cronograma de auditoría recibida.

La auditoría se realizó el 09 de noviembre de 2025, durante la semana de 11 del curso.

#### 6.4.2.3. Contenido de auditoría recibida.

#### **UX Heuristics & Principles Evaluation**
#### **Usability – Inclusive Design – Information Architecture**

**CARRERA:** Ingeniería de Software  <br>
**CURSO:** Diseño de Experimentos de Ingeniería de Software  <br>
**NRC:** 7508 <br>
**PROFESORES:** Julio Manuel Noriega Melendez<br>
**AUDITOR:** Paolo Torres <br>
**CLIENTE(S):** Grupo Go6U<br>

---

#### **SITE o APP A EVALUAR:**
**Psymed** – Aplicación para profesionales de la salud mental y pacientes que facilita la gestión de procesos interactivos entre ambos.

---

#### **TAREAS A EVALUAR:**
El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:

1. Registro de paciente
2. Registro de profesional de la salud mental
3. Inicio de sesión y acceso al panel principal
4. Agendar una cita terapéutica
5. Enviar mensaje al terapeuta o paciente
6. Registrar notas o avances de sesión
7. Visualizar historial clínico
8. Cancelar o reprogramar una cita

No están incluidas en esta versión de la evaluación las siguientes tareas:

1. Generar reportes estadísticos de sesiones
2. Configurar recordatorios automáticos por correo o SMS
3. Integrar pagos en línea
4. Exportar historial clínico a otros formatos
5. Funcionalidades de supervisión entre terapeutas

---

#### **ESCALA DE SEVERIDAD:**

| Nivel | Descripción                                                                                                                                       |
|-------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| **1** | Problema superficial: puede ser fácilmente superado por el usuario o ocurre con muy poca frecuencia. No requiere corrección inmediata.            |
| **2** | Problema menor: ocurre con cierta frecuencia o genera confusión leve. Se recomienda corregir en una futura iteración.                             |
| **3** | Problema mayor: ocurre frecuentemente o impide al usuario completar una tarea sin ayuda. Debe corregirse con prioridad alta.                      |
| **4** | Problema muy grave: impide completamente el uso de la herramienta o compromete la experiencia del usuario. Debe corregirse antes del lanzamiento. |

---

#### **TABLA RESUMEN:**

| # | Problema                                                                                       | Escala de severidad | Heurística / Principio violado                |
|---|------------------------------------------------------------------------------------------------|---------------------|-----------------------------------------------|
| 1 | No existe un botón claro para regresar al panel principal desde la vista de historial clínico. | 3                   | Usability: Libertad y control del usuario     |
| 2 | Los íconos de funciones no tienen etiquetas textuales para lectores de pantalla.               | 2                   | Inclusive Design: Experiencias comparables    |
| 3 | La jerarquía visual de la sección de mensajes no resalta las conversaciones activas.           | 2                   | Information Architecture: Is it usable?       |
| 4 | Al registrar una cita, no se muestra retroalimentación inmediata tras confirmar.               | 3                   | Usability: Visibilidad del estado del sistema |
| 5 | El botón “Cancelar cita” está demasiado próximo al botón “Guardar cambios”.                    | 3                   | Usability: Prevención de errores              |

---

#### **DESCRIPCIÓN DE PROBLEMAS:**

#### **PROBLEMA #1: No existe un botón claro para regresar al panel principal desde la vista de historial clínico**
**Severidad:** 3  
**Heurística violada:** Usabilidad – Libertad y control del usuario  
**Problema:**  
Cuando el usuario revisa el historial clínico, no dispone de una opción visible que le permita regresar fácilmente al panel principal. Esto genera confusión y obliga a usar el navegador para retroceder, afectando la fluidez de la navegación.

**Recomendación:**  
Incorporar un botón “Volver al panel” o un ícono de navegación persistente en la interfaz, que permita retornar fácilmente sin perder el contexto actual.

---

#### **PROBLEMA #2: Los íconos de funciones no tienen etiquetas textuales para lectores de pantalla**
**Severidad:** 2  
**Heurística violada:** Inclusive Design – Proporciona experiencias comparables  
**Problema:**  
Algunos íconos, como el de mensajes o configuración, carecen de atributos `aria-label` o texto alternativo, lo que dificulta la interacción para usuarios con discapacidad visual.

**Recomendación:**  
Agregar etiquetas accesibles (`aria-label` o `alt`) a todos los elementos interactivos para garantizar compatibilidad con tecnologías de asistencia.

---

#### **PROBLEMA #3: La jerarquía visual de la sección de mensajes no resalta las conversaciones activas**
**Severidad:** 2  
**Heurística violada:** Information Architecture – Is it usable?  
**Problema:**  
La interfaz de mensajes no diferencia visualmente las conversaciones activas de las archivadas, dificultando la búsqueda y seguimiento de pacientes.

**Recomendación:**  
Aplicar un esquema visual claro (colores, tipografía o etiquetas) que distinga estados de conversación y facilite la navegación.

---

#### **PROBLEMA #4: Al registrar una cita, no se muestra retroalimentación inmediata tras confirmar**
**Severidad:** 3  
**Heurística violada:** Usabilidad – Visibilidad del estado del sistema  
**Problema:**  
Luego de presionar “Confirmar cita”, el sistema no muestra un mensaje o indicador que confirme la acción, generando incertidumbre sobre si la cita fue registrada correctamente.

**Recomendación:**  
Incluir una notificación visual o sonora (por ejemplo, un mensaje de éxito o un ícono animado) que confirme la creación de la cita.

---

#### **PROBLEMA #5: El botón “Cancelar cita” está demasiado próximo al botón “Guardar cambios”**
**Severidad:** 3  
**Heurística violada:** Usabilidad – Prevención de errores  
**Problema:**  
La cercanía entre ambos botones aumenta el riesgo de cancelación accidental, especialmente en pantallas táctiles o móviles.

**Recomendación:**  
Separar ambos botones con espacio suficiente o colores contrastantes para minimizar errores involuntarios.

---

**Versión del documento:** V1.0  
**Puntaje total:** 20


#### 6.4.2.4. Resumen de modificaciones para subsanar hallazgos

Tras la evaluación heurística realizada en **Psymed**, se efectuaron una serie de modificaciones destinadas a mejorar la **usabilidad**, **accesibilidad** y **arquitectura de la información** de la aplicación.

Entre los principales ajustes se implementaron las siguientes acciones:

- **Navegación mejorada:** Se añadió un botón visible para regresar al panel principal desde todas las vistas, garantizando mayor control y libertad de navegación.
- **Accesibilidad reforzada:** Se incorporaron etiquetas `aria-label` y textos alternativos a los íconos y elementos interactivos para asegurar compatibilidad con lectores de pantalla.
- **Jerarquía visual optimizada:** Se rediseñó la sección de mensajes, destacando las conversaciones activas mediante colores y tipografía diferenciada.
- **Retroalimentación inmediata:** Se implementaron notificaciones visuales y mensajes de confirmación al registrar o modificar citas, mejorando la visibilidad del estado del sistema.
- **Prevención de errores:** Se reajustó la ubicación y el diseño de los botones “Cancelar cita” y “Guardar cambios” para evitar cancelaciones accidentales.

Estas modificaciones fortalecen la experiencia del usuario al interactuar con **Psymed**, promoviendo una interfaz más intuitiva, segura y alineada con los principios de diseño centrado en el usuario.
