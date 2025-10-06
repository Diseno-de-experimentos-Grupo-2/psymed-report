# CAPÍTULO III: Requirements Specifications

## 3.1. To-Be Scenario Mapping.
### Segmento Profesionales:
![Professionals To-Be Scenario Mapping](../../assets/to-be-profesional.jpg)
### Segmento Pacientes:
![Pattients_TobeScenarioMapping](../../assets/to-be-paciente.jpg)
## 3.2. User Stories.
US01 - Registro como profesional de la salud mental
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US01</td>
<td>Profesional de la salud mental</td>
<td>8</td>
<td>EP01</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Registro como profesional de la salud mental</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como profesional de la salud mental, quiero registrarme con mis credenciales para poder acceder a las funcionalidades específicas y gestionar la información de mis pacientes.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Registro de datos exitoso</b>


Dado que el profesional de la salud mental ha completado todos los campos del formulario de registro,


Cuando hace clic al botón "Crear cuenta",


Entonces la cuenta se crea,


Y el profesional accede a la aplicación con el rol de profesional de la salud mental.</li>
<li><b>Escenario 2: Registro de datos incompleto</b>


Dado que el profesional de la salud mental no ha completado todos los campos del formulario de registro,


Cuando hace clic al botón "Crear cuenta",


Entonces la plataforma muestra un mensaje de error indicando qué campos faltan por completar.</li>
<li><b>Escenario 3: Registro con credenciales ya utilizadas</b>


Dado que el profesional de la salud mental ha completado todos los campos del formulario de registro usando un correo ya registrado,


Cuando hace clic al botón "Crear cuenta",


Entonces la plataforma muestra un mensaje de error indicando que el correo electrónico ya está en uso


Y sugiere recuperar la contraseña.</li>
</ul>
</td>
</tr>
</table>

US02 - Inicio de sesión como paciente
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US02</td>
<td>Paciente</td>
<td>8</td>
<td>EP01</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Inicio de sesión como paciente</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como paciente, quiero iniciar sesión en la plataforma para acceder a mi información personal y seguimiento de tratamiento.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Inicio de sesión exitoso</b>


Dado que el paciente ha ingresado su correo electrónico y contraseña correctamente,


Cuando hace clic en un botón de "Iniciar sesión",


Entonces accede a su cuenta


Y es dirigido a su panel de control personal con el rol de paciente.</li>
<li><b>Escenario 2: Contraseña incorrecta</b>


Dado que el paciente ha ingresado su correo y una contraseña incorrecta,


Cuando hace clic en un botón de "Iniciar sesión",


Entonces la plataforma muestra un mensaje de error indicando que la contraseña es incorrecta


Y ofrece la opción de restablecerla.</li>
<li><b>Escenario 3: Recuperación de contraseña</b>


Dado que el paciente ha olvidado su contraseña,


Cuando hace clic en un botón de "Olvidé mi contraseña",


Entonces la plataforma envía un enlace de restablecimiento de contraseña al correo electrónico registrado.</li>
</ul>
</td>
</tr>
</table>

US03 - Inicio de sesión como profesional de la salud mental
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US03</td>
<td>Profesional de la salud mental</td>
<td>8</td>
<td>EP01</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Inicio de sesión como profesional de la salud mental</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como profesional de la salud mental, quiero iniciar sesión en la plataforma para gestionar la información de mis pacientes y acceder a herramientas de seguimiento.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Inicio de sesión exitoso</b>


Dado que el profesional de la salud mental ha ingresado su correo electrónico y contraseña correctamente,


Cuando hace clic en un botón de "Iniciar sesión",


Entonces accede a su cuenta


Y es dirigido a su panel de control con acceso a herramientas avanzadas de gestión de pacientes y el rol de profesional de la salud.</li>
<li><b>Escenario 2: Contraseña incorrecta</b>


Dado que el profesional de la salud mental ha ingresado su correo y una contraseña incorrecta,


Cuando hace clic en un botón de "Iniciar sesión",


Entonces la plataforma muestra un mensaje de error indicando que la contraseña es incorrecta


Y ofrece la opción de restablecerla.</li>
<li><b>Escenario 3: Recuperación de contraseña</b>


Dado que el profesional de la salud mental ha olvidado su contraseña,


Cuando hace clic en un botón de "Olvidé mi contraseña",


Entonces la plataforma envía un enlace de restablecimiento de contraseña al correo electrónico registrado.</li>
</ul>
</td>
</tr>
</table>

US04 - Registro de información personal del paciente
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US04</td>
<td>Profesional de la salud mental</td>
<td>5</td>
<td>EP01</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Registro de información personal del paciente</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como profesional de la salud mental, quiero registrar la información personal del paciente para tener una referencia detallada y precisa de sus datos básicos en cada consulta.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Registro exitoso de información personal</b>


Dado que el profesional de la salud mental ha ingresado todos los datos del formulario de información personal del paciente,


Cuando hace clic en un botón de "Guardar",


Entonces la información personal del paciente se registra correctamente en la plataforma y está disponible para futuras consultas.</li>
<li><b>Escenario 2: Registro incompleto de información personal</b>


Dado que el profesional de la salud mental no ha ingresado todos los datos del formulario de información personal del paciente,


Cuando hace clic en un botón de "Guardar",


Entonces la plataforma muestra un mensaje de error indicando qué campos faltan por completar.</li>
</ul>
</td>
</tr>
</table>

US05 - Visualización del estado actual de ánimo del paciente
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US05</td>
<td>Profesional de la salud mental</td>
<td>3</td>
<td>EP02</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Visualización del estado actual de ánimo del paciente</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como profesional de la salud mental, quiero visualizar el estado de ánimo actual del paciente para evaluar su condición emocional.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Visualización del estado de ánimo</b>


Dado que el profesional de la salud mental ha accedido al perfil del paciente,


Cuando selecciona la opción de visualizar estados de ánimo,


Entonces la plataforma muestra el estado de ánimo del paciente que se registró el mismo día.</li>
<li><b>Escenario 2: Estados de ánimo no registrados</b>


Dado que el profesional de la salud mental ha accedido al perfil del paciente sin haber registrado ningún estado de ánimo del mismo,


Cuando selecciona la opción de visualizar estados de ánimo,


Entonces la plataforma no muestra los datos ingresados.</li>
</ul>
</td>
</tr>
</table>

US06 - Registro de estado de ánimo
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US06</td>
<td>Paciente</td>
<td>5</td>
<td>EP02</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Registro de estado de ánimo</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como paciente, quiero comunicarle a mi profesional mi estado de ánimo para ver mi estado actual.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Registro de emoción</b>


Dado que el paciente se encuentra en la sección de registros de estado emocional,


Cuando registra su estado de ánimo actual,


Entonces la plataforma debe actualizar su estado emocional en el perfil del paciente.</li>
<li><b>Escenario 2: Almacenamiento de estado de ánimo</b>


Dado que el paciente se encuentra en la sección de registros de estado emocional,


Y posee un registro con cada uno de los estados que ingresó con anterioridad,


Cuando ingresa al historial de estados de ánimo,


Entonces la plataforma debe mostrar un calendario con los estados del paciente a lo largo del tiempo.</li>
</ul>
</td>
</tr>
</table>

US07 - Registro de funciones biológicas
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US07</td>
<td>Paciente</td>
<td>5</td>
<td>EP02</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Registro de funciones biológicas</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como paciente, quiero registrar la calidad de mis funciones biológicas para que mi profesional conozca mi estado actual de salud.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Ingreso de funciones biológicas</b>


Dado que el paciente ha accedido a la sección de registro de funciones biológicas,


Cuando selecciona la opción de registrar funciones,


Entonces la plataforma debe permitir al paciente seleccionar su nivel de sueño, hambre, energía e hidratación en una escala del 1 al 5.</li>
</ul>
</td>
</tr>
</table>

US08 - Registro de medicamentos del paciente
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US08</td>
<td>Profesional de la salud mental</td>
<td>3</td>
<td>EP03</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Registro de medicamentos del paciente</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como profesional de la salud mental, quiero registrar los medicamentos del paciente para seguir adecuadamente su tratamiento farmacológico.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Registro exitoso de medicamentos</b>


Dado que el profesional de la salud mental ha ingresado todos los datos de los medicamentos de su paciente,


Cuando hace clic en un botón de "Guardar",


Entonces los datos del medicamento se registran correctamente en el sistema y se asocian al perfil del paciente.</li>
<li><b>Escenario 2: Registro incompleto de medicamentos</b>


Dado que el profesional de la salud mental no ha ingresado todos los datos de los medicamentos de su paciente,


Cuando hace clic en un botón de "Guardar",


Entonces la plataforma muestra un mensaje de error indicando los campos incompletos o incorrectos.</li>
</ul>
</td>
</tr>
</table>

US09 - Ver medicamentos
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US09</td>
<td>Paciente</td>
<td>3</td>
<td>EP03</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Ver medicamentos</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como paciente, quiero poder ver los medicamentos que mi profesional de salud mental ha asignado para poder estar pendiente de cuáles consumir.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Visualización de medicamentos</b>


Dado que el paciente entra a la plataforma


Cuando ingresa a la vista de medicamentos


Entonces puede ver todos los medicamentos recetados.</li>
</ul>
</td>
</tr>
</table>

US10 - Creación de citas
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US10</td>
<td>Profesional de la salud</td>
<td>2</td>
<td>EP04</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Creación de citas</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como profesional de la salud, quiero agendar las citas de mis pacientes.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Creación de nueva cita</b>


Dado que el profesional de salud entra a la plataforma


Cuando ingresa a la vista de citas sobre el perfil de un paciente


Entonces puede registrar una nueva cita.</li>
</ul>
</td>
</tr>
</table>

US11 - Ver citas médicas
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US11</td>
<td>Paciente</td>
<td>2</td>
<td>EP04</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Ver citas médicas</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como paciente, quiero poder ver las citas médicas programadas para poder saber qué días ir al consultorio del profesional de salud mental.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Visualización de citas</b>


Dado que el paciente entra a la plataforma


Cuando ingresa a la vista de citas


Entonces puede ver todas las citas programas y los detalles de hora y fecha.</li>
</ul>
</td>
</tr>
</table>

# Historias de usuario para la aplicación Móvil

US12 - Iniciar Sesión como Paciente
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US12</td>
<td>Paciente</td>
<td>8</td>
<td>EP01</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Iniciar Sesión como Paciente</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como Paciente, quiero poder iniciar sesión con mi usuario y contraseña para acceder a mi información personal y de salud dentro de la aplicación.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Inicio de Sesión Exitoso</b>


Dado que el Paciente está en la pantalla de "Bienvenido" e ingresa su Usuario y Contraseña correctos,


Cuando pulsa el botón "Iniciar Sesión",


Entonces el sistema valida las credenciales y el paciente es dirigido a la pantalla principal.</li>
<li><b>Escenario 2: Credenciales Inválidas</b>


Dado que el Paciente ingresa un Usuario o Contraseña incorrectos,


Cuando pulsa el botón "Iniciar Sesión",


Entonces el sistema no permite iniciar sesión


Y muestra un mensaje de error.</li>
<li><b>Escenario 3: Campos Vacíos</b>


Dado que el Paciente deja los campos de Usuario y/o Contraseña vacíos,


Cuando pulsa el botón "Iniciar Sesión",


Entonces el sistema no permite iniciar sesión


Y muestra un mensaje de error indicando qué campos faltan.</li>
</ul>
</td>
</tr>
</table>

US13 - Visualizar Información de Perfil
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US13</td>
<td>Paciente</td>
<td>3</td>
<td>EP01</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Visualizar Información de Perfil</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como Paciente, quiero poder ver mi información personal (Correo Electrónico, Dirección, ID de Paciente y ID de Profesional) en la sección "Mi Perfil" para confirmar que mis datos son correctos.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Visualización del Perfil</b>


Dado que estoy en la aplicación y navego a la pestaña "Profile",


Entonces veo mi Nombre completo,


Y veo mi Correo Electrónico asociado,


Y veo mi Dirección,


Y veo mi ID de Paciente y mi ID de Profesional asignados.</li>
</ul>
</td>
</tr>
</table>

US14 - Cerrar Sesión
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US14</td>
<td>Paciente</td>
<td>2</td>
<td>EP01</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Cerrar Sesión</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como Paciente, quiero poder cerrar mi sesión de forma segura desde la pantalla de Mi Perfil para proteger mi privacidad.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Cierre de Sesión Exitoso</b>


Dado que estoy en la pantalla "Mi Perfil" e he iniciado sesión,


Cuando pulso el botón "Cerrar Sesión",


Entonces la sesión actual se cierra exitosamente,


Y soy redirigido a la pantalla de Inicio de Sesión.</li>
</ul>
</td>
</tr>
</table>

US15 - Registrar Mi Estado de Salud Diario
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US15</td>
<td>Paciente</td>
<td>5</td>
<td>EP02</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Registrar Mi Estado de Salud Diario</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como Paciente, quiero poder registrar mi estado de salud diario (Mood, Hunger, Hydration, Sleep Quality, Energy Level) para llevar un seguimiento de mi bienestar.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Registro Exitoso de Datos de Salud</b>


Dado que estoy en la pestaña "Health" y no he completado el registro de hoy,


Cuando selecciono una opción para cada categoría (Mood, Hunger, Hydration, Sleep Quality, Energy Level) y pulso el botón de registro,


Entonces el sistema guarda el registro de ese día,


Y muestra un mensaje de confirmación.</li>
<li><b>Escenario 2: Reintento de Registro del Mismo Día</b>


Dado que ya he completado el registro de mi estado de salud hoy,


Cuando navego a la pestaña "Health",


Entonces veo un mensaje o un botón deshabilitado que indica "Ya registrado hoy", impidiendo un nuevo registro.</li>
</ul>
</td>
</tr>
</table>

US16 - Consultar Mi Lista de Medicamentos
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US16</td>
<td>Paciente</td>
<td>5</td>
<td>EP03</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Consultar Mi Lista de Medicamentos</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como Paciente, quiero poder ver la lista de medicamentos que tengo asignados para conocer el nombre, el motivo, la frecuencia (Intervalo) y la Cantidad de cada uno.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Visualización de Medicamentos</b>


Dado que estoy en la pestaña "Medication",


Entonces veo una lista de todos mis medicamentos,


Y para cada medicamento, se muestra el Motivo, el Intervalo, y la Cantidad.</li>
</ul>
</td>
</tr>
</table>

US17 - Ver Próximas Citas
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US17</td>
<td>Paciente</td>
<td>3</td>
<td>EP04</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Ver Próximas Citas</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como Paciente, quiero poder ver una lista de mis citas médicas próximas con sus detalles (fecha, hora, duración y profesional ID) para estar informado y planificar mi asistencia.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Visualización de Citas</b>


Dado que estoy en la pestaña de "Appointments",


Entonces veo la sección "Próximas Citas",


Y veo una lista de citas, donde cada una muestra la Fecha, la Hora, la Duración y el Profesional ID.</li>
<li><b>Escenario 2: Identificación de Cita de Hoy</b>


Dado que hay una cita programada para la fecha actual,


Entonces esta cita muestra una etiqueta distintiva con el texto "HOY".</li>
</ul>
</td>
</tr>
</table>

### Historias de Usuario de la Landing Page (US18 - US20)

US18 - Encontrar información del propósito de la aplicación
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US18</td>
<td>Visitante de la Landing Page</td>
<td>1</td>
<td>EP05</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Encontrar información del propósito de la aplicación</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como visitante de la Landing Page, quiero encontrar fácilmente la información que explique el propósito de la aplicación para comprender cómo puede ser útil para mí.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Visibilidad del propósito de la aplicación</b>


Dado que el visitante se encuentra en la landing page,


Cuando explora la página principal,


Entonces la landing page debe poseer información clara y concisa sobre el propósito de la aplicación.</li>
</ul>
</td>
</tr>
</table>

US19 - Visualización de imágenes y gráficos relevantes
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US19</td>
<td>Visitante de la Landing Page</td>
<td>1</td>
<td>EP05</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Visualización de imágenes y gráficos relevantes</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como visitante de la Landing Page, quiero que las imágenes y gráficos sean claros y visualmente atractivos para captar mi interés y comprender mejor el contenido.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Calidad de las imágenes</b>


Dado que el visitante se encuentra en la landing page,


Cuando explora la página principal,


Entonces la landing page debe presentar imágenes de alta calidad y relevantes que capten la atención del visitante.</li>
<li><b>Escenario 2: Relevancia de los gráficos</b>


Dado que el visitante se encuentra en la landing page,


Cuando se desplaza,


Entonces la landing page debe mostrar gráficos que ayuden al visitante a comprender el contenido.</li>
</ul>
</td>
</tr>
</table>

US20 - Tipografía cómoda y agradable estéticamente
<table>
<tr>
<th>Story ID</th>
<th>User</th>
<th>Priority</th>
<th>Epic</th>
</tr>
<tr>
<td>US20</td>
<td>Visitante de la Landing Page</td>
<td>1</td>
<td>EP05</td>
</tr>
<tr>
<th colspan="4">Title</th>
</tr>
<tr>
<td colspan="4">Tipografía cómoda y agradable estéticamente</td>
</tr>
<tr>
<th colspan="4">Description</th>
</tr>
<tr>
<td colspan="4">
Como visitante de la Landing Page, quiero que la tipografía de la misma sea legible y estéticamente agradable para facilitar la lectura y la navegación.
</td>
</tr>
<tr>
<th colspan="4">Acceptance Criteria</th>
</tr>
<tr>
<td colspan="4">
<ul>
<li><b>Escenario 1: Legibilidad de la tipografía</b>


Dado que el visitante se encuentra en la landing page,


Cuando se desplaza a través de la página principal,


Entonces la landing page debe poseer una tipografía clara y de un tamaño adecuado para facilitar la lectura.</li>
<li><b>Escenario 2: Consistencia en el estilo tipográfico</b>


Dado que el visitante se encuentra en la landing page,


Cuando cambia de sección,


Entonces la landing page debe mostrar un estilo tipográfico consistente para mantener la coherencia visual.</li>
</ul>
</td>
</tr>
</table>

**Spike Stories**

| ID	    | Título                                                                                                                                                                                                                              | 	Descripción                                                                                                                                                                                                                           | 	Criterios de aceptación                                                                                                                                                                                                                                                                                                           | 	Prioridad	 | EpicID |
|--------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------|--------|
| SP-01  | 	Investigación de bibliotecas de autenticación OAuth2                                                                                                                                                                               | 	Como desarrollador, quiero investigar bibliotecas de autenticación OAuth2 (Spring Security, Keycloak, Auth0) para determinar cuál es más adecuada para integrar con la plataforma.                                                    | 	Given que se identifican diferentes bibliotecas de autenticación OAuth2, When se evalúan criterios de compatibilidad, seguridad y facilidad de integración con el stack actual, Then se presenta un documento técnico con la recomendación de la librería a utilizar y un prototipo funcional mínimo que valide la autenticación. | 	Alta       | 	EP03  |
| SP-02  | 	Evaluación de frameworks para gráficos estadísticos                                                                                                                                                                                | 	Como desarrollador frontend, quiero investigar librerías de visualización (Chart.js, Recharts, D3.js) para seleccionar la más adecuada para representar datos de bienestar emocional.                                                 | 	Given que se prueban librerías de visualización, When se comparan en términos de rendimiento, personalización y soporte en Angular, Then se genera un documento con conclusiones y un prototipo funcional que muestre datos simulados del paciente.                                                                               | 	Media      | 	EP05  |
| SP-03  | 	Prueba de integración con servicios de notificaciones	                                                                                                                                                                             | Como desarrollador backend, quiero probar servicios de mensajería (Firebase, OneSignal, Web Push API) para definir la mejor opción para enviar recordatorios y alertas al paciente.                                                    | 	Given que se analizan servicios de notificaciones, When se evalúan costos, confiabilidad y facilidad de integración, Then se presenta un informe comparativo y un prototipo funcional de envío de notificación desde el backend.                                                                                                  | 	Alta       | 	EP07  |
| SP-04  | 	Investigación de métodos de cifrado para datos clínicos	Como desarrollador backend, quiero analizar técnicas de cifrado (AES, RSA, JWT) para asegurar la confidencialidad de los datos clínicos del paciente en tránsito y reposo. | 	Given que se identifican diferentes métodos de cifrado, When se prueban su implementación en un entorno de prueba, Then se entrega un documento con la recomendación técnica y un ejemplo funcional implementado en un microservicio. | 	Alta	                                                                                                                                                                                                                                                                                                                             | EP04        |
| SP-05  | 	Prueba de rendimiento de la API REST                                                                                                                                                                                               | 	Como equipo técnico, queremos realizar una prueba de carga sobre los endpoints más críticos para validar el rendimiento y detectar posibles cuellos de botella.                                                                       | 	Given que se identifican los endpoints más usados, When se ejecutan pruebas de carga con herramientas como JMeter o Postman, Then se entrega un reporte técnico con los resultados de rendimiento y recomendaciones de optimización.                                                                                              | 	Alta	      | EP04   |
| SP-06  | Evaluación de estrategias de almacenamiento para historiales clínicos                                                                                                                                                               | 	Como arquitecto de software, quiero evaluar la conveniencia entre bases de datos relacionales (PostgreSQL) y no relacionales (MongoDB) para almacenar los historiales clínicos del paciente.                                          | 	Given que se configuran entornos de prueba para ambas bases de datos, When se evalúan rendimiento, escalabilidad y facilidad de consulta, Then se genera un informe con la recomendación final basada en resultados empíricos.                                                                                                    | 	Media	     | EP04   |
| SP-07  | Validación de accesibilidad web (WCAG 2.1)	                                                                                                                                                                                         | Como diseñador UX/UI, quiero realizar una evaluación de accesibilidad de la landing page para asegurar el cumplimiento de las pautas WCAG 2.1 y mejorar la experiencia del usuario.                                                    | 	Given que se revisan los componentes principales de la landing page, When se validan contrastes, etiquetas alt, roles ARIA y navegación por teclado, Then se entrega un reporte con los hallazgos y un plan de mejoras de accesibilidad.	                                                                                         | Media       | 	EP01  |
| SP-08  | 	Evaluación de la viabilidad del módulo predictivo                                                                                                                                                                                  | 	Como equipo de desarrollo, queremos analizar la viabilidad de integrar un modelo predictivo de bienestar emocional basado en datos históricos del paciente.                                                                           | 	Given que se recopilan datasets de ejemplo, When se prueban modelos iniciales (regresión lineal, árbol de decisión), Then se entrega un documento técnico con resultados de precisión, requerimientos de datos y recomendaciones para su futura implementación.                                                                   | 	Baja       | 	EP05  |

## 3.3. Impact Mapping.
### Segmento profesionales:
![Professionals_](/assets/professionals_IM.jpeg)

### Segmento pacientes:
![Patients_impactmapping](/assets/patients_IM.jpeg)

## 3.4 Product Backlog.

| Order User Story | Título                                                  | Descripción                                                                                                                                                                                       | Story Points (Priority) |
|------------------|---------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------|
| 1                | Registro como profesional de la salud mental            | Como profesional de la salud mental quiero registrarme con mis credenciales para poder acceder a las funcionalidades específicas y gestionar la información de mis pacientes.                     | 8                       |
| 2                | Inicio de sesión como paciente                          | Como paciente, quiero iniciar sesión en la plataforma para acceder a mi información personal y seguimiento de tratamiento.                                                                        | 8                       |
| 3                | Inicio de sesión como profesional de la salud mental    | Como profesional de la salud mental, quiero iniciar sesión en la plataforma para gestionar la información de mis pacientes y acceder a herramientas de seguimiento.                               | 8                       |
| 4                | Iniciar Sesión como Paciente                            | Como Paciente, quiero poder iniciar sesión con mi usuario y contraseña para acceder a mi información personal y de salud dentro de la aplicación.                                                 | 8                       |
| 5                | Registro de información personal del paciente           | Como profesional de la salud mental, quiero registrar la información personal del paciente para tener una referencia detallada y precisa de sus datos básicos en cada consulta.                   | 5                       |
| 6                | Registro de estado de ánimo                             | Como paciente, quiero comunicarle a mi profesional mi estado de ánimo para ver mi estado actual.                                                                                                  | 5                       |
| 7                | Registro de funciones biológicas                        | Como paciente, quiero registrar la calidad de mis funciones biológicas para que mi profesional conozca mi estado actual de salud.                                                                 | 5                       |
| 8                | Registrar Mi Estado de Salud Diario                     | Como Paciente, quiero poder registrar mi estado de salud diario (Mood, Hunger, Hydration, Sleep Quality, Energy Level) para llevar un seguimiento de mi bienestar.                                | 5                       |
| 9                | Consultar Mi Lista de Medicamentos                      | Como Paciente, quiero poder ver la lista de medicamentos que tengo asignados para conocer el nombre, el motivo, la frecuencia (Intervalo) y la Cantidad de cada uno.                              | 5                       |
| 10               | Visualización de el estado actual de ánimo del paciente | Como profesional de la salud mental, quiero visualizar el estado de ánimo actual del paciente para evaluar su condición emocional.                                                                | 3                       |
| 11               | Registro de medicamentos del paciente                   | Como profesional de la salud mental, quiero registrar los medicamentos del paciente para seguir adecuadamente su tratamiento farmacológico.                                                       | 3                       |
| 12               | Ver medicamentos                                        | Como paciente quiero poder ver los medicamentos que mi profesional de salud mental ha asignado para poder estar pendiente de cuales consumir.                                                     | 3                       |
| 13               | Visualizar Información de Perfil                        | Como Paciente, quiero poder ver mi información personal (Correo Electrónico, Dirección, ID de Paciente y ID de Profesional) en la sección "Mi Perfil" para confirmar que mis datos son correctos. | 3                       |
| 14               | Ver Próximas Citas                                      | Como Paciente, quiero poder ver una lista de mis citas médicas próximas con sus detalles (fecha, hora, duración y profesional ID) para estar informado y planificar mi asistencia.                | 3                       |
| 15               | Creación de citas                                       | Como profesional de la salud quiero agendar las citas de mis pacientes.                                                                                                                           | 2                       |
| 16               | Ver citas médicas                                       | Como paciente quiero poder ver las citas médicas programadas para poder saber que días ir al consultorio del profesional de salud mental.                                                         | 2                       |
| 17               | Cerrar Sesión                                           | Como Paciente, quiero poder cerrar mi sesión de forma segura desde la pantalla de Mi Perfil para proteger mi privacidad.                                                                          | 2                       |
| 18               | Encontrar información del propósito de la aplicación    | Como visitante de la Landing Page, quiero encontrar fácilmente la información que explique el propósito de la aplicación para comprender cómo puede ser útil para mí.                             | 1                       |
| 19               | Visualización de imágenes y gráficos relevantes         | Como visitante de la Landing Page, quiero que las imágenes y gráficos sean claros y visualmente atractivos para captar mi interés y comprender mejor el contenido.                                | 1                       |
| 20               | Tipografía cómoda y agradable estéticamente             | Como visitante de la Landing Page, quiero que la tipografía de la misma sea legible y estéticamente agradable para facilitar la lectura y la navegación.                                          | 1                       |

