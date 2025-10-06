# Capítulo VI: Product Verification & Validation

## 6.1. Testing Suites & Validation
En esta sección se describen las pruebas realizadas para verificar y validar el producto desarrollado, asegurando que cumple con los requisitos especificados y funciona correctamente en diferentes escenarios. Se detallan las pruebas unitarias, de integración, de comportamiento y del sistema.

## 6.1.1. Core Entities Unit Tests.

Los Core Entities Unit Tests se centran en verificar la funcionalidad de las entidades principales del sistema PSYMED. Estas pruebas aseguran que las entidades individuales funcionan correctamente de manera aislada, sin depender de otras partes del sistema.

El backedn de PSYMED está desarrollado en Java utilizando el framework Spring Boot, y las pruebas unitarias se implementan utilizando JUnit y Mockito. A continuación, se describen algunas de las pruebas unitarias realizadas para las entidades principales del sistema.

- Bounded context Medication:
  ```getId() test```

![image 2.png](../../image%202.png)

```getName() test```

![image 3.png](../../image%203.png)

```getDescription()```

![image 4.png](../../image%204.png)

```getPatientId()```

![image 5.png](../../image%205.png)

```getInterval()```

![image 6.png](../../image%206.png)

```getQuantity()```

![image 7.png](../../image%207.png)


Pruebas unitarias para validar ingreso de registro de funciones biológicas del paciente

Los únicos valores permitidos son del 0 al 5

```Hydration```

![image 11.png](../../image%2011.png)

```Hunger```

![image 12.png](../../image%2012.png)

```Sleep```

![image 13.png](../../image%2013.png)

```Energy```

![image 14.png](../../image%2014.png)

- Mood status:

Pruebas unitarias para validar ingreso de registro del estado de ánimo del paciente

![image 15.png](../../image%2015.png)


- Session class

Esta prueba unitaria valída que las citas no se pueden crear en el pasado o en el futuro.

![image 19.png](../../image%2019.png)

- Session Command Service

Esta prueba unitaria utiliza

![image 20.png](../../image%2020.png)



También se valida que las citas deben ser en el futuro

![image 22.png](../../image%2022.png)

ProfessionalSessionController:
No se pueden crear citas sin el id del paciente

![image 23.png](../../image%2023.png)

De la misma manera no se puede crear una sesión sin el profesional de salud:

![image 24.png](../../image%2024.png)

Tampoco se pueden crear sesiones con más de un médico

![image 25.png](../../image%2025.png)

![image 26.png](../../image%2026.png)

IAM:

Validar creación de cuentas de acuerdo al rol del usuario (profesional o paciente)

![image 27.png](../../image%2027.png)


Profiles:

Solo se aceptan direcciones sin comas por reglas de negocio

![image 31.png](../../image%2031.png)

## 6.1.2. Core Integration Tests.

Esta seccion describe las pruebas de integración realizadas en funcionalidades Core del negocio.

Resultado al usar ```mvn test```

Prueba integral

![image 9.png](../../image%209.png)

- PillController Test

![image 10.png](../../image%2010.png)

- Biological Function Controller:

![image 17.png](../../image%2017.png)

- MoodState Controller

![image 18.png](../../image%2018.png)

- SessionReservationController

![image 21.png](../../image%2021.png)


- IAM:

![image 28.png](../../image%2028.png)

Solo debe retornar una cuenta cuando se verifica que esta existe

![image 29.png](../../image%2029.png)


Authentication Controller Test

Se verifica la cuenta cuando el usuario hace sign in exitosamente

![image 30.png](../../image%2030.png)

## 6.1.3. Core Behavior-Driven Development

En esta sección se describen las pruebas de desarrollo guiado por comportamiento (BDD) realizadas para validar las funcionalidades principales del sistema PSYMED.
Se usa lenguaje Gherkin para definir los escenarios de prueba de manera clara y comprensible para todos los miembros del equipo, incluyendo desarrolladores, testers y stakeholders.

Estos archivos se encuentran en el repositorio: https://github.com/Diseno-de-experimentos-Grupo-2/psymed-features.git

![img.png](img.png)

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


- US02	Inicio de sesión como pacientes

Como paciente, quiero iniciar sesión en la plataforma para acceder a mi información personal y seguimiento de tratamiento.


- US03	Inicio de sesión como profesional de la salud mental

Como profesional de la salud mental, quiero iniciar sesión en la plataforma para gestionar la información de mis pacientes y acceder a herramientas de seguimiento.


- US04	Registro de información personal del paciente

Como profesional de la salud mental, quiero registrar la información personal del paciente para tener una referencia detallada y precisa de sus datos básicos en cada consulta.


- US05	Visualización del estado actual de ánimo del paciente

Como profesional de la salud mental, quiero visualizar el estado de ánimo actual del paciente para evaluar su condición emocional.


- US06	Registro de estado de ánimo

Como paciente, quiero comunicarle a mi profesional mi estado de ánimo para ver mi estado actual.


- US07	Registro de funciones biológicas

Como paciente, quiero registrar la calidad de mis funciones biológicas para que mi paciente conozca mi estado actual de salud.


- US08	Registro de medicamentos del paciente

Como profesional de la salud mental, quiero registrar los medicamentos del paciente para seguir adecuadamente su tratamiento farmacológico


- Ver medicamentos

Como paciente quiero poder ver los medicamentos que mi profesional de salud mental ha asignado para poder estar pendiente de cuales consumir


- Creación de citas

Como profesional de la salud quiero agendar las citas de mis pacientes


- Ver citas médicas

Como paciente quiero poder ver las citas médicas programadas para poder saber que días ir al consultorio del profesional de salud mental


### Versión Móvil

- US12	Iniciar Sesión como Paciente:

Como Paciente, quiero poder iniciar sesión con mi usuario y contraseña para acceder a mi información personal y de salud dentro de la aplicación.



- US13	Visualizar Información de Perfil:

Como Paciente, quiero poder ver mi información personal (Correo Electrónico, Dirección, ID de Paciente y ID de Profesional) en la sección "Mi Perfil" para confirmar que mis datos son correctos.



- US14	Cerrar Sesión:

Como Paciente, quiero poder cerrar mi sesión de forma segura desde la pantalla de Mi Perfil para proteger mi privacidad.



- US15	Registrar Mi Estado de Salud Diario:

Como Paciente, quiero poder registrar mi estado de salud diario (Mood, Hunger, Hydration, Sleep Quality, Energy Level) para llevar un seguimiento de mi bienestar.



- US16	Consultar Mi Lista de Medicamentos:

Como Paciente, quiero poder ver la lista de medicamentos que tengo asignados para conocer el nombre, el motivo, la frecuencia (Intervalo) y la Cantidad de cada uno.



- US17	Ver Próximas Citas:
  Como Paciente, quiero poder ver una lista de mis citas médicas próximas con sus detalles (fecha, hora, duración y profesional ID) para estar informado y planificar mi asistencia.