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
#### 6.2.1.2. Code Quality & Code Security.
### 6.2.2. Reviews

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


### 6.3.2. Registro de Entrevistas.

Entrevistas a segmento profesionales:

- Entrevista 1:

![WhatsApp Image 2025-11-06 at 11 39 00 PM](https://github.com/user-attachments/assets/d236f0f9-7542-455b-a9d0-4742c60feb45)


| Nombre               | Karina          |
|----------------------|-----------------|
| Apellido             | Ramirez         |
| Edad                 | 51 años         |
| Distrito             | La Molina       |
| URL                  |                 |
| Inicio de entrevista |    |
| Fin de entrevista    |  |

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


| Nombre               | Hortensia            |
|----------------------|-----------------|
| Apellido             | Piedra Cáceres         |
| Edad                 | 36 años         |
| Distrito             | Arequipa       |
| URL                  |                 |
| Inicio de entrevista |    |
| Fin de entrevista    |  |

Resumen de entrevista:

La psicóloga clínica Hortensia Piedra Cáceres, residente en Arequipa, brindó una evaluación detallada de la plataforma Psymed, un sistema web y móvil diseñado para optimizar la gestión de pacientes, citas y seguimiento emocional y físico en el ámbito psicológico y psiquiátrico.

Desde el inicio, la entrevistada consideró que el proceso de inicio de sesión es claro y sencillo, permitiendo distinguir adecuadamente entre el acceso de pacientes y profesionales. En cuanto al registro de pacientes, sugirió incluir información adicional como la edad y antecedentes de terapia previa, para enriquecer la historia clínica inicial.

Respecto al módulo de citas, destacó su facilidad de uso y propuso añadir opciones que reflejen distintos tipos de atención, como evaluaciones psicológicas, entregas de informes, orientación vocacional o terapias grupales (DBT). También recomendó incorporar campos para registrar costos, paquetes de sesiones y reprogramaciones, ya que son aspectos frecuentes en la práctica clínica.

Sobre el seguimiento emocional y físico, valoró que el paciente pueda registrar su estado diario, pero sugirió incluir un campo de notas donde exprese la causa o contexto de sus emociones, facilitando el análisis posterior en sesión. Consideró apropiado mantener cierta separación entre la información del psicólogo y la del psiquiatra, por motivos de confidencialidad.

En el ámbito de la versión móvil, la psicóloga afirmó que sería útil para profesionales, especialmente para consultar citas y el progreso de sus pacientes. Recalcó la conveniencia de que los terapeutas puedan acceder también desde el celular, no solo desde la computadora.

En términos de diseño y usabilidad, propuso emplear colores cálidos (melón, beige, café claro) en lugar de tonos fríos o clínicos, con el fin de generar cercanía y evitar una estética hospitalaria. También sugirió incorporar pequeñas imágenes decorativas que aporten calidez visual.

Finalmente, consideró que SciMed respeta la privacidad del paciente, dado que el registro emocional es parte del proceso terapéutico. Recomendó agregar el motivo de consulta y un sistema para asignar tareas terapéuticas, donde el paciente pueda indicar si comprendió la actividad y cómo se sintió al realizarla.

Concluyó afirmando que la plataforma es intuitiva, funcional y pertinente para el trabajo psicológico, y que con las mejoras propuestas podría convertirse en una herramienta integral para la práctica clínica y el acompañamiento terapéutico.

Entrevistas a segmento pacientes:


### 6.3.3. Evaluacionessegún heurísticas.
## 6.4. Auditoría de Experiencias de Usuario.
### 6.4.1. Auditoría realizada.
#### 6.4.1.1. Información del grupo auditado.
#### 6.4.1.2. Cronograma de auditoría realizada.
#### 6.4.1.3. Contenido de auditoría realizada.
### 6.4.2. Auditoría recibida.
#### 6.4.2.1. Información del grupo auditor.
#### 6.4.2.2. Cronograma de auditoría recibida.
#### 6.4.2.3. Contenido de auditoría recibida.
#### 6.4.2.4. Resumen de modificaciones para subsanar hallazgos

