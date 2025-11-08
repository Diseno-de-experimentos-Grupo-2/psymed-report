# Capítulo VIII: Experiment-Driven Development

## 8.1.Experiment Planning

### 8.1.1. As-Is Summary.

Actualmente, la aplicación presenta aspectos de interfaz y experiencia de usuario que pueden dificultar la navegación fluida y la identificación visual dentro del sistema. Algunos botones poseen colores que no destacan, ciertos dashboards carecen de elementos visuales representativos, y en la aplicación móvil el flujo de ingreso no conduce directamente a la funcionalidad esperada por los usuarios. Además, la identidad visual no es consistente entre versión web y móvil, lo que afecta la coherencia de marca y la percepción general de profesionalismo.

### 8.1.2. Raw Material: Assumptions, Knowledge Gaps, Ideas, Claims.

- Para mejorar la visibilidad y el reconocimiento del botón de inicio de sesión, se podría cambiar su color actual a verde para facilitar que el usuario lo identifique rápidamente.

- Para optimizar el flujo de navegación en la aplicación móvil, se podría configurar que al iniciar sesión el usuario sea dirigido directamente a la vista de registro de estado de salud, reduciendo pasos y tiempos de interacción.

- Para reforzar la orientación profesional del dashboard del doctor en la versión web, se podría agregar una imagen referencial relacionada con psicología que acompañe los elementos visuales existentes.

- Para fortalecer la coherencia visual y la pertenencia del usuario en el dashboard del paciente en la versión web, se podría incorporar la imagen del logo institucional.

- Para mejorar la consistencia estética entre plataformas, se podría implementar un cambio de tema de color hacia tonos morado pastel en la versión móvil, manteniendo una identidad visual uniforme.

### 8.1.3. Experiment-Ready Questions.

- Cambio de Color del Botón de Inicio de Sesión: ¿El cambio del color del botón a verde facilita que los usuarios identifiquen más rápido la acción de iniciar sesión y aumenta la tasa de acceso exitoso?

- Navegación en Aplicación Móvil: ¿Dirigir automáticamente al usuario a la vista de registro de estado de salud reduce el tiempo de navegación e incrementa la frecuencia de registro?

- Imagen Referencial en Dashboard del Doctor: ¿La inclusión de una imagen relacionada con psicología en el dashboard del doctor mejora la percepción profesional y la claridad contextual de la interfaz?

- Imagen del Logo en Dashboard del Paciente: ¿Mostrar el logo institucional en el dashboard del paciente aumenta el sentido de pertenencia y confianza en la plataforma?

- Nuevo Tema en Versión Móvil: ¿El cambio de tema de color a morado pastel mantiene la legibilidad y mejora la consistencia visual en la aplicación móvil?

### 8.1.4. Question Backlog.

- **Impacto del Botón Verde de Inicio de Sesión:**
¿En qué medida el cambio del botón a color verde aumentaría la tasa de reconocimiento visual y la frecuencia de inicio de sesión por parte de los usuarios?

- **Redirección Automática a Registro de Estado de Salud:**
¿La acción de dirigir automáticamente al usuario al registro de su estado de salud al ingresar a la aplicación reduciría la fricción en la navegación y aumentaría la constancia de uso diario?

- **Uso de Imagen de Psicología en el Dashboard del Doctor:**
¿La incorporación de una imagen contextual relacionada con psicología en el dashboard médico incrementaría la percepción de claridad, sentido profesional y confianza en el entorno clínico digital?

- **Inclusión del Logo Institucional en el Dashboard del Paciente:**
¿Mostrar el logo institucional en el dashboard del paciente fortalecería la identidad de la plataforma y aumentaría la confianza y legitimidad del servicio?

- **Consistencia Visual con Tema Morado Pastel en Móvil:**
¿La adopción del tema en color morado pastel en la versión móvil mejoraría la coherencia visual y retención de los usuarios sin afectar la legibilidad de los elementos interactivos?

### 8.1.5. Experiment Cards.

|  | Experiment Card 1 |
|----|----|
| Question | ¿Cómo afecta a la experiencia del usuario el cambio del botón de inicio de sesión a color verde? |
| Why | Queremos entender si un mayor contraste visual puede facilitar el reconocimiento de la acción principal y aumentar la frecuencia de inicio de sesión. |
| What | Se cambiará el color del botón de inicio de sesión a verde y se observará si los usuarios identifican más rápido la acción, midiendo la cantidad de inicios exitosos y comentarios sobre claridad. |
| Hypothesis | Cambiar el botón a color verde mejorará la visibilidad y aumentará la tasa de inicio de sesión debido a un reconocimiento visual más claro.|

|  | Experiment Card 2 |
|----|----|
| Question | ¿La redirección automática al registro de estado de salud mejora la constancia de uso diario? |
| Why | Queremos evaluar si reducir pasos manuales ayuda a que los usuarios registren su información con mayor frecuencia y permanezcan más activos dentro de la aplicación. |
| What | Al iniciar sesión, el usuario será dirigido automáticamente a la sección de registro de estado de salud. Se analizará si se incrementa la cantidad de registros diarios. |
| Hypothesis | Redirigir automáticamente a la pantalla de registro aumentará la continuidad de uso, ya que elimina fricción y pasos innecesarios. |

|  | Experiment Card 3 |
|----|----|
| Question | ¿Cómo influye una imagen referencial de psicología en la percepción de claridad del dashboard médico? |
| Why | Queremos explorar si un contexto visual puede ayudar a los profesionales a identificar más rápidamente su entorno de trabajo y sentir mayor guía visual. |
| What | Se añadirá una imagen referencial en el dashboard médico y se solicitarán breves opiniones sobre claridad y orientación. |
| Hypothesis | Incorporar una imagen referencial aumentará la percepción de claridad y mejorará la orientación visual dentro del dashboard. |

|  | Experiment Card 4 |
|----|----|
| Question | ¿La inclusión del logo institucional en el dashboard del paciente fortalece la percepción de confianza? |
| Why | Queremos entender si reforzar la identidad visual del sistema aumenta la credibilidad del servicio ante los pacientes. |
| What | Se colocará el logo institucional en la parte superior del dashboard del paciente y se recogerá retroalimentación respecto a identidad y confianza. |
| Hypothesis | Agregar el logo institucional mejorará la percepción de confiabilidad y pertenencia del usuario respecto a la plataforma. |

|  | Experiment Card 5 |
|----|----|
| Question | ¿Cómo afecta el uso de un tema en color morado pastel a la experiencia visual y legibilidad en la versión móvil? |
| Why | Queremos evaluar si la estética puede mejorarse sin afectar la lectura o navegación en pantallas pequeñas. |
| What | Se aplicará un tema morado pastel en la interfaz móvil y se medirá la comprensión de elementos, comodidad visual y comentarios de usabilidad. |
| Hypothesis | Adoptar el tema morado pastel hará la interfaz más agradable visualmente sin comprometer la legibilidad ni la usabilidad general. |

## 8.2. Experiment Design
### 8.2.1. Hypotheses.
### 8.2.2. Domain Business Metrics
### 8.2.3. Measures.
### 8.2.4. Conditions.
### 8.2.5. Scale Calculations and Decisions.
### 8.2.6. Methods Selection.
### 8.2.7. Data Analytics: Goals, KPIs and Metrics Selection.
### 8.2.8. Web and Mobile Tracking Plan.
## 8.3. Experimentation
### 8.3.1. To-Be User Stories.
### 8.3.2.To-Be Product Backlog
