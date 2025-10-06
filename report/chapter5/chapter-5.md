# Capítulo V: Product Implementation, Validation & Deployment

## 5.1 Software Configuration Management
En este apartado se describe el proceso mediante el cual se organiza, gestiona y controla la configuración del software y los cambios en el desarrollo del proyecto. El objetivo es garantizar que todos los integrantes del equipo trabajen bajo un mismo entorno, utilizando herramientas estandarizadas y metodologías que aseguren la trazabilidad, la calidad y la colaboración continua.
### 5.1.1. Software Development Environment Configuration.
**Requirements Management**
1.Requirements Management

Trello: Plataforma de gestión de proyectos basada en tableros Kanban. Será utilizada por el equipo de PsyMed para planificar, organizar y hacer seguimiento del trabajo, especialmente bajo metodologías ágiles (Scrum). Permite asignar responsables, definir prioridades y actualizar el estado de cada tarea en tiempo real, lo que mejora la visibilidad del progreso y la coordinación del equipo.

Ruta de referencia: https://trello.com/es

Tableros de la organización: https://trello.com/w/closedsource1/home




**Product UX/UI Design**

1. Figma: Herramienta colaborativa para el diseño de interfaces y prototipado. Se empleará en la construcción de los prototipos de la aplicación, tanto en su versión Desktop como en Mobile Web Browser. Facilita el diseño en equipo y permite iterar rápidamente en el aspecto visual antes del desarrollo.

Ruta de referencia: https://www.figma.com/login
2. Figma: Herramienta colaborativa para el diseño de interfaces y prototipado. Se empleará en la construcción de los prototipos de la aplicación, tanto en su versión Desktop como en Mobile Web Browser. Facilita el diseño en equipo y permite iterar rápidamente en el aspecto visual antes del desarrollo.

Ruta de referencia: https://www.figma.com/login

**Software Development**
1. WebStorm: Entorno de desarrollo integrado (IDE) especializado en tecnologías web. Ha sido elegido por su soporte avanzado para HTML, CSS, JavaScript y frameworks como React y Angular. Ofrece herramientas de refactorización, depuración, integración con Git y compatibilidad multiplataforma, lo que optimiza la productividad y estandariza el desarrollo del equipo.
   
   Ruta de referencia: https://www.jetbrains.com/webstorm/
   <br>

2. HTML5: Lenguaje de marcado utilizado para estructurar y presentar el contenido de la aplicación web. Servirá como base para la maquetación de la interfaz.
   
   Ruta de referencia: https://www.w3schools.com/html/html5_syntax.asp 
   <br>

3. CSS: Lenguaje de hojas de estilo en cascada para definir la presentación visual del contenido. En conjunto con HTML, permitirá dar estilo, diseño adaptable y coherencia visual a la aplicación.
   
   Ruta de referencia: https://google.github.io/styleguide/htmlcssguide.html
   <br>
   <br>

4. JavaScript: Lenguaje de programación dinámico y orientado a objetos. Se utilizará para el desarrollo de la lógica de la interfaz y la interacción del usuario con la aplicación.
   
   Ruta de referencia: https://developer.mozilla.org/es/docs/Web/JavaScript
   <br>
   <br>

5. Angular: Framework de JavaScript escrito en TypeScript. Será la principal tecnología para el desarrollo del front-end del proyecto PsyMed. Permite crear aplicaciones escalables, modulares y mantenibles. El código desarrollado se encuentra alojado en el repositorio correspondiente.
   
   Ruta de referencia: https://github.com/Diseno-de-experimentos-Grupo-2/psymed-frontend

 <br>

**Software Deployment**
1. Git: Sistema de control de versiones distribuido. Permitirá a los integrantes del equipo llevar un registro detallado de los cambios, gestionar ramas de desarrollo, y facilitar la integración de nuevas funcionalidades sin comprometer la estabilidad del proyecto.
   
   Ruta de referencia: https://git-scm.com/
   <br>
   <br>
   **Software Documentation and Project Management**
2. GitHub: Plataforma colaborativa en la nube para el alojamiento de repositorios Git. Será el medio oficial para la centralización del código, revisión de contribuciones y gestión de issues, además de permitir la integración con otras herramientas de desarrollo y CI/CD
   
   Ruta de referencia: https://github.com/


### 5.1.2. Source Code Management.
El proyecto adoptará las convenciones del modelo GitFlow para la gestión del control de versiones, utilizando GitHub como plataforma principal para alojar y organizar el código. GitFlow es un enfoque estructurado que facilita la colaboración en equipo, la integración de cambios y la gestión de múltiples versiones del software. Este modelo asegura que cada etapa de desarrollo esté debidamente aislada, probada y documentada antes de ser integrada en la rama principal.

A continuación, se detalla cómo se implementará este flujo de trabajo, junto con los enlaces a los repositorios donde se centralizan los entregables principales:

**Repositorio de GitHub:**
- Enlace para acceder a la [organización en GitHub](https://github.com/Diseno-de-experimentos-Grupo-2)
- Enlace para acceder al repositorio de la [Landing Page](https://github.com/Diseno-de-experimentos-Grupo-2/Landing-Page)
- Enlace para acceder al repositorio del [Reporte Final](https://github.com/Diseno-de-experimentos-Grupo-2/psymed-report)
- Enlace para acceder al repositorio del [Frontend Web](https://github.com/Diseno-de-experimentos-Grupo-2/psymed-frontend)
- Enlace para acceder al repositorio del [Frontend Móvil](https://github.com/Diseno-de-experimentos-Grupo-2/psymed-mobile-flutter)

**Flujo de trabajo GitFlow**

El flujo de trabajo se basará en el modelo propuesto por Vincent Driessen en "A successful Git branching model".

![GitFlowDiagram.png](../../assets/GitFlowDiagram.png)

**Estructura de branches (Ramas):**


1. **Master branch (Rama principal):** Contendrá únicamente versiones estables y listas para producción. Los cambios que lleguen aquí deberán haber pasado por pruebas y validaciones en develop y feature branches.

2. **Develop Branch (Rama de Desarrollo):** Funciona como la rama de integración, donde se combinan y prueban las nuevas funcionalidades antes de ser promovidas a master. Garantiza que el código en desarrollo se mantenga operativo y estable.

3. **Feature branch (Ramas de funcionalidad):** Cada nueva característica o mejora se desarrollará en una rama independiente creada a partir de develop. Una vez finalizada y probada, se fusionará nuevamente en develop.

Convención de nombres: feature/nombre-descriptivo.
Ejemplo: feature/bc-medication-management.

### 5.1.3. Source Code Style Guide & Conventions.
**HTML:** Para garantizar un código legible, mantenible y coherente, se seguirán las siguientes prácticas y guías de estilo:

1. Cerrar todos los elementos HTML: Por ejemplo, ```<p>Esto es un párrafo.</p>```
2. Siempre declarar el tipo de documento en la primera línea del documento, para
   HTML es "<!DOCTYPE html>”.
3. Escribir en una línea los comentarios cortos.
4. Utilizar comillas en caso de que los atributos contengan espacios entre sí.
5. Procurar especificar el texto alt y las dimensiones width y height de las imágenes, ya que de esta manera se facilitará la
   disponibilidad del contenido. Por ejemplo:   ```<img src="abc.img" alt="image name"  
   style="width:128px;height:128px">```
6. Se nos recomienda no usar el espacio al momento de utilizar los signos porque
   es más fácil de leerlo de esta forma.  
   <br>
   HTML: (https://www.w3schools.com/html/html5_syntax.asp)

**CSS:** Entre las prácticas empleadas se menciona:

1. Usar sangría de 2 espacios, evitando tabulaciones.
2. Escribir el código en minúsculas.
3. Eliminar espacios en blanco innecesarios.
4. Documentar el código mediante comentarios.
5. Utilizar nombres de clase descriptivos y significativos. 
   <br>

   CSS: (https://google.github.io/styleguide/htmlcssguide.html)



### 5.1.4. Software Deployment Configuration.
### Landing page deployment:
Para el despliegue de la Landing Page se utilizará GitHub Pages, siguiendo los pasos descritos a continuación:

1. Colocar los archivos de la página en la raíz del repositorio.
2. Nombrar los archivos de acuerdo a las convenciones: "index.html" para la landing page, "styles.css" para los estilos, "main.js" para los scripts, y una carpeta llamada "assets/images" para las imágenes.
3. Subir los archivos al repositorio mediante un commit.
4. Ir a Settings > Pages y seleccionar el branch main.
5. Definir la carpeta raíz (root) como fuente de la página.
6. Esperar que GitHub realice las validaciones necesarias.
7. Acceder al enlace generado para visualizar la página desplegada.

## GithubPages

![alt text](../../assets/GithubPages.png)
Una vez completado el despliegue, la landing page quedará publicada y accesible públicamente mediante el enlace: https://wx55-closed-source.github.io/landing-page/

## 5.2. Product Implementation & Deployment

### 5.2.1. Sprint 1

### 5.2.1.2. Sprint Backlog 1

<table>
<tr>
    <th colspan="3">Sprint #</th>
    <th colspan="10">Sprint 1</th>
</tr>
<tr>
    <td colspan="3">User Story</td>
    <td colspan="10">Work-Item/Task</td>
</tr>
<tr>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="3">Description</td>
    <td colspan="1">Estimation</td>
    <td colspan="2">Assigned To</td>
    <td colspan="1">Status (To-do / InProcess / To-Review / Done)</td>
</tr>
<tr>
    <td colspan="1">US01</td>
    <td colspan="2">Registro como profesional de la salud mental</td>
    <td colspan="1">EP01</td>
    <td colspan="2">Implementar módulo de registro de profesionales de salud mental</td>
    <td colspan="3">Desarrollar el formulario de registro con validaciones, manejo de errores (campos vacíos y correo duplicado) y conexión al backend para la creación de cuenta con rol profesional.</td>
    <td colspan="1">8</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US02</td>
    <td colspan="2">Inicio de Sesión como pacientes</td>
    <td colspan="1">EP02</td>
    <td colspan="2">Implementar módulo de inicio de sesión para pacientes</td>
    <td colspan="3">Crear la vista de login para pacientes, con validación de credenciales, manejo de errores de autenticación y flujo de recuperación de contraseña mediante correo electrónico.</td>
    <td colspan="1">6</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US03</td>
    <td colspan="2">Inicio de sesión como profesional de la salud mental</td>
    <td colspan="1">EP03</td>
    <td colspan="2">Implementar módulo de inicio de sesión para profesionales de salud mental</td>
    <td colspan="3">Desarrollar formulario de login con asignación de rol profesional, validación de credenciales, recuperación de contraseña y redirección al panel correspondiente.</td>
    <td colspan="1">6</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US04</td>
    <td colspan="2">Registro de información personal del paciente</td>
    <td colspan="1">EP04</td>
    <td colspan="2">Implementar registro de información personal del paciente</td>
    <td colspan="3">Crear formulario y servicio que permita al profesional registrar y guardar datos personales del paciente en la base de datos, mostrando validaciones y confirmación de guardado.</td>
    <td colspan="1">5</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US05</td>
    <td colspan="2">Vizualización del estado actual de ánimo del paciente</td>
    <td colspan="1">EP05</td>
    <td colspan="2">Implementar vista de visualización del estado de ánimo del paciente</td>
    <td colspan="3">Desarrollar interfaz que muestre el estado de ánimo actual y pasado del paciente, incluyendo manejo de casos sin registros.</td>
    <td colspan="1">6</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US06</td>
    <td colspan="2">Registro de estado de ánimo</td>
    <td colspan="1">EP06</td>
    <td colspan="2">Implementar registro y visualización de estado de ánimo del paciente</td>
    <td colspan="3">Crear formulario para que el paciente registre su estado emocional, y vista con historial cronológico o calendario de registros.</td>
    <td colspan="1">6</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US07</td>
    <td colspan="2">Registro de funciones biológicas</td>
    <td colspan="1">EP07</td>
    <td colspan="2">Implementar formulario de registro de funciones biológicas</td>
    <td colspan="3">Crear interfaz que permita registrar niveles de sueño, hambre, energía e hidratación (escala del 1 al 5) y guardar los datos en el backend.</td>
    <td colspan="1">5</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US08</td>
    <td colspan="2">Registro de medicamentos del paciente</td>
    <td colspan="1">EP08</td>
    <td colspan="2">Implementar registro de medicamentos del paciente</td>
    <td colspan="3">Permitir al profesional ingresar, editar y guardar medicamentos en el perfil del paciente, validando campos y mostrando mensajes de éxito o error.</td>
    <td colspan="1">6</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US09</td>
    <td colspan="2">Ver medicamentos</td>
    <td colspan="1">EP09</td>
    <td colspan="2">Implementar vista de medicamentos del paciente</td>
    <td colspan="3">Crear sección donde el paciente pueda ver los medicamentos recetados por su profesional, con detalles como dosis y frecuencia.</td>
    <td colspan="1">6</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US10</td>
    <td colspan="2">Creación de citas</td>
    <td colspan="1">EP10</td>
    <td colspan="2">Implementar módulo de creación de citas médicas</td>
    <td colspan="3">Permitir al profesional agendar nuevas citas asociadas a pacientes, especificando fecha, hora y motivo, con almacenamiento en la base de datos.</td>
    <td colspan="1">6</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US11</td>
    <td colspan="2">Ver citas médicas</td>
    <td colspan="1">EP11</td>
    <td colspan="2">Implementar vista de citas médicas para el paciente</td>
    <td colspan="3">Mostrar al paciente la lista de citas programadas con fecha, hora y detalles del profesional asignado.</td>
    <td colspan="1">4</td>
    <td colspan="2">Romina</td>
    <td colspan="1">Done</td>
</tr>
</table>

### 5.2.1.2. Implmented Landing Page Evidence.

La Landing Page fue hecho deploy a través de GitHub Pages, y se puede acceder a travéz de este enlace: https://diseno-de-experimentos-grupo-2.github.io/Landing-Page/

![alt text](../../assets/Landing1.png)
![alt text](../../assets/Landing2.png)
![alt text](../../assets/Landing3.png)
![alt text](../../assets/Landing4.png)
![alt text](../../assets/Landing5.png)
![alt text](../../assets/Landing6.png)
![alt text](../../assets/Landing7.png)
![alt text](../../assets/Landing8.png)

### 5.2.1.3. Implemented Frontend-Web Application Evidence.

El Frontend-Web se hizo deploy a través de , y se puede acceder desde el siguiente enlace: 

![alt text](../../assets/front-web-rol.png)
![alt text](../../assets/front-web-register.png)
![alt text](../../assets/front-web-login.png)

Paciente: 

![alt text](../../assets/sprint3/df19.jpeg)
![alt text](../../assets/front-web-patient-mood.png)
![alt text](../../assets/front-web-patient-biological-functions.png)
![alt text](../../assets/sprint3/df16.jpeg)

Profesional:

![alt text](../../assets/IMG-20240924-WA0029.jpg)
![alt text](../../assets/IMG-20240924-WA0030.jpg)
![alt text](../../assets/sprint3/df09.jpeg)

### 5.2.1.4. Implemented RESTful API and Severless Backend Evidence.
![alt text](../../assets/sprint4/backend_deployment.png)

### 5.2.1.6. RESTful API documentation.
Enlace al repositorio del Backend:https://github.com/Diseno-de-experimentos-Grupo-2/psymed-backend

Enlace del Backend deployment: https://psymed-production.up.railway.app

| **Endpoint**                                 | **Método** | **Descripción**                                    | **Parámetros**                      | **Respuesta**                                         | **Ejemplo**                                              |
|----------------------------------------------|------------|----------------------------------------------------|------------------------------------|--------------------------------------------------------|----------------------------------------------------------|
| `/api/v1/professional-profiles`              | POST       | Create a new professional profile                  | JSON Body - `CreateProfessionalProfileResource` | `201 Created` - Profile created<br>`400 Bad Request` - Invalid input | `{"name": "Dr. John Doe", "specialty": "Psychiatrist"}` |
| `/api/v1/professional-profiles/{profileId}`  | GET        | Retrieve a professional profile by its ID          | `{profileId} (Long)`               | `200 OK` - Profile found<br>`404 Not Found` - Profile not found | `{"id": 1, "name": "Dr. John Doe", "specialty": "Psychiatrist"}` |
| `/api/v1/patient-profiles`                     | POST       | Create a new patient profile                       | JSON Body - `CreatePatientProfileResource` | `201 Created` - Profile created<br>`400 Bad Request` - Invalid input | `{"name": "Jane Doe", "age": 30, "diagnosis": "Anxiety"}` |
| `/api/v1/patient-profiles/{profileId}`         | GET        | Retrieve a patient profile by its ID               | `{profileId} (Long)`               | `200 OK` - Profile found<br>`404 Not Found` - Profile not found | `{"id": 1, "name": "Jane Doe", "age": 30, "diagnosis": "Anxiety"}` |
| `/api/v1/patient-profiles`                     | GET        | Retrieve all patient profiles                      | N/A                                | `200 OK` - List of profiles                                | `[{"id": 1, "name": "Jane Doe"}, {"id": 2, "name": "John Doe"}]` |
| `/api/v1/patients/{patientId}/mood-states`               | POST       | Create a new mood state record for a patient            | `patientId (Long)`<br>JSON Body - `CreateMoodStateRecordResource` | `201 Created` - Mood state created<br>`400 Bad Request` - Invalid input | `{"date": "2024-11-17", "mood": "Happy", "notes": "Feeling great today!"}` |
| `/api/v1/patients/{patientId}/mood-states`               | GET        | Retrieve all mood states for a specific patient         | `patientId (Long)`                         | `200 OK` - List of mood states<br>`404 Not Found` - Patient not found  | `[{"id": 1, "date": "2024-11-17", "mood": "Happy", "notes": "Feeling great today!"}]` |
| `/api/v1/patients/{patientId}/biological-functions`       | POST       | Create a new biological function record for a patient     | `patientId (Long)`<br>JSON Body - `CreateBiologicalFunctionRecordResource` | `201 Created` - Biological function created<br>`400 Bad Request` - Invalid input | `{"date": "2024-11-17", "type": "Sleep", "value": "7 hours", "notes": "Slept well"}` |
| `/api/v1/patients/{patientId}/biological-functions`       | GET        | Retrieve all biological function records for a specific patient | `patientId (Long)`                         | `200 OK` - List of biological functions<br>`404 Not Found` - Patient not found  | `[{"id": 1, "date": "2024-11-17", "type": "Sleep", "value": "7 hours"}]` |
| `/api/v1/pills`                | POST        | Create a new medication                                 | JSON Body - `CreatePillResource`      | `201 Created` - Medication created<br>`400 Bad Request` - Invalid input<br>`404 Not Found` - Medication not found | `{"name": "Aspirin", "dosage": "500mg", "instructions": "Take one daily"}` |
| `/api/v1/pills`                | GET         | Retrieve all medications                                | N/A                                   | `200 OK` - List of medications<br>`404 Not Found` - No medications found    | `[{"id": 1, "name": "Aspirin", "dosage": "500mg"}]`       |
| `/api/v1/pills/{pillId}`       | DELETE      | Delete a medication by its ID                           | `pillId (Long)`                       | `200 OK` - Medication deleted<br>`404 Not Found` - Medication not found     | N/A                                                      |
| `/api/v1/accounts/{accountId}`       | GET        | Retrieve account details by account ID       | `accountId (Long)`           | `200 OK` - Account found<br>`404 Not Found` - Account not found | `{"id": 1, "username": "johndoe", "email": "johndoe@example.com"}` |
| `/api/v1/authentication/sign-in`         | POST       | Authenticate a user and generate a token               | JSON Body - `SignInResource`         | `200 OK` - User authenticated<br>`404 Not Found` - Invalid credentials | `{"username": "johndoe", "password": "password123"}`      |
| `/api/v1/authentication/sign-up`         | POST       | Register a new user account                            | JSON Body - `SignUpResource`         | `201 Created` - Account created<br>`400 Bad Request` - Invalid input | `{"username": "janedoe", "email": "janedoe@example.com", "password": "securePass!"}` |

---

### 5.2.1.7. Team Collaboration Insights.

Front-end Web Application: 



Back-end Web Application:


Mobile Application: 


