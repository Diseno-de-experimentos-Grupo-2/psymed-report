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

| Hipótesis 1 | Cambio de color del botón de Log in a verde (Web) |
|-|-|
| Question |	¿El cambio del color del botón de “Iniciar Sesión” a verde ha incrementado la interacción y el número de inicios de sesión exitosos? |
| Data analyze|	Para este análisis se utilizó Google Analytics y Datadog RUM. Se realizaron 30 pruebas durante sesiones de usuario en la aplicación web. Después del cambio al color verde, se observó que la tasa de clic (CTR) al botón pasó de 12.4% a 15.1%, lo que representa un incremento del 21.7% en interacción. Además, los inicios de sesión exitosos aumentaron un 9.8% en relación con la semana previa. Esto sugiere que el nuevo color mejora la visibilidad y sensación de acción en el usuario. <br> <br> <p  align = "center"> <img width="250" height="250" alt="image" src="https://media.discordapp.net/attachments/1286768073453342767/1436762712334929960/content.png?ex=6910c90c&is=690f778c&hm=a8756d41424ff6325819d96f7ad95f326d05b5862c2e36910739d96d2de52c68&=&format=webp&quality=lossless"/> </p> |
| Hypothesis|	El cambio del botón a verde mejora la tasa de interacción y aumenta los inicios de sesión exitosos, debido a una mayor claridad visual y estímulo de acción.|

| Hipótesis 2 | Redirección inicial a registrar estado de salud (App móvil) |
|-|-|
| Question |	¿Enviar al usuario directamente a la vista de “Registrar estado de salud” mejora la frecuencia de registros realizados en la primera sesión? |
| Data analyze|	Para este análisis se utilizó Firebase Analytics. Se realizaron 50 pruebas de sesión en dispositivos móviles. Antes de la modificación, solo el 32% de los usuarios completaba un registro de estado en la primera sesión. Después de aplicar la redirección automática, la cifra aumentó al 56%, lo que representa un incremento del 24 puntos porcentuales y una mejora significativa en el engagement inicial. <br> <br> <p  align = "center"> <img width="250" height="250" alt="image" src="https://media.discordapp.net/attachments/1286768073453342767/1436802305927282789/vGPjBs3Lg888EBeeumlzJkzJ4sWLUqbNm2y22675cgjj8zAgQPTunXrNaoFaFgVpVItDwUDAADwqXDBBRfkwgsvTJJa144CaAgWcQcAAACg0ARYAAAAABSaAAsAAACAQhNgAQAAAFBoAiwAAAAACs2vEAIAAABQaGZgAQAAAFBoAiwAAAAACk2ABQAAAEChCbAAAAAAKDQBFgAAAACFJsACAAAAoNAEWAAAAAAUmgALAAAAgEITYAEAAABQaAIsAAAAAApNgAUAAABAoQmwAAAAACg0ARYAAAAAhSbAAgAAAKDQBFgAAAAAFJoACwAAAIBCE2ABAAAAUGgCLAAAAAAKTYAFAAAAQKEJsAAAAAAoNAEWAAAAAIUmwAIAAACg0ARYAAAAABSaAAsAAACAQhNgAQAAAFBoAiwAAAAACk2ABQAAAEChCbAAAAAAKDQBFgAAAACF9v8B3C4L27FCwWgAAAAASUVORK5CYII.png?ex=6910edec&is=690f9c6c&hm=6193d2d594c6a24022a81bc59ed51f672c99fb9f719b6861cef76c6026ebb334&=&format=webp&quality=lossless"/></p> |
| Hypothesis |	La redirección aumenta la participación en el registro de estado de salud y fortalece el vínculo inicial del usuario con la aplicación.|

| Hipótesis 3 | Imagen referencial de psicología en el dashboard del doctor (Web) |
|-|-|
| Question |	¿La inclusión de la imagen referencial mejora la comprensión visual del dashboard y aumenta la interacción con secciones relacionadas? |
| Data analyze|	Se utilizó Hotjar Heatmaps y Google Analytics para analizar la atención visual y el flujo de navegación. Después de 20 sesiones monitoreadas, se observó que el área donde se colocó la imagen recibió un 33% más de fijaciones visuales, y los clics hacia los recursos psicológicos aumentaron en 11.4%. Esto indica un estímulo visual efectivo.  <br> <br> <p  align = "center"> <img width="250" height="250" alt="image" src="https://github.com/user-attachments/assets/f081e919-aeb7-4e97-b45e-b4552a5aa5ba"/></p> |
|Hypothesis|	La imagen referencial mejora la orientación visual y aumenta la probabilidad de interacción con recursos psicológicos en el dashboard.|

| Hipótesis 4 | Imagen del logo en dashboard del paciente (Web) |
|-|-|
| Question |	¿La presencia del logo en el dashboard incrementa la percepción de identidad y confianza del usuario en la plataforma? |
| Data analyze|	Para este análisis se aplicó una encuesta in-app corta (N=28) y revisión de flujos mediante Hotjar. La percepción de confianza pasó de 3.8 a 4.4/5 en promedio. Además, la tasa de permanencia en la pantalla inicial aumentó 8.9%, indicando menor abandono inmediato. <br> <br> <p  align = "center"> <img width="250" height="250" alt="image" src="https://github.com/user-attachments/assets/e67d095c-d7f5-4a96-9b4c-6d6595d4fb27"/></p>|
|Hypothesis|	Incluir el logo refuerza la identidad visual y genera mayor confianza, lo que reduce el abandono al ingresar al dashboard.|

| Hipótesis 5 | Cambio de tema a morado pastel (App móvil) |
|-|-|
| Question |	¿El nuevo tema morado pastel mejora la satisfacción visual sin afectar la usabilidad general de la aplicación? |
| Data analyze|	Se utilizaron pruebas con Lighthouse Mobile y encuestas in-app de preferencia visual (N=31). La puntuación de satisfacción estética aumentó de 3.9 a 4.6/5. Las mediciones de performance se mantuvieron estables (puntaje de rendimiento entre 74-78, sin variaciones significativas). No se detectaron problemas de contraste según validación automática. <br> <br> <p  align = "center"> <img width="250" height="250" alt="image" src="https://github.com/user-attachments/assets/150d579b-3217-41c4-9cce-657e1a72ec01"/></p>|
|Hypothesis|	El nuevo tema aumenta la satisfacción visual del usuario sin comprometer accesibilidad ni rendimiento.|

### 8.2.2. Domain Business Metrics

| Métrica de Negocio |	Descripción|	Cómo se mide|	Objetivo de Mejora |
|--------------------|------------|-------------|--------------------|
|Tasa de Retención de Usuario|	Mide la cantidad de usuarios que vuelven a la aplicación después de utilizarla por primera vez.|	Usuarios activos semanales / usuarios registrados.|	Aumentar la retención al mejorar la experiencia visual y navegación.|
|Tasa de Compleción del Registro de Estado de Salud (móvil)|	Mide cuántos usuarios que entran efectivamente terminan registrando su estado de salud.	|Total de usuarios que inician sesión vs. los que completan la acción.	|Incrementar completitud gracias a la redirección directa.|
|Engagement en el Dashboard (web)|	Mide la interacción dentro de los paneles del doctor y paciente.|	Clics, tiempo en página, número de elementos consultados por sesión.|	Incrementar la interacción gracias a los elementos visuales agregados.|
|Tasa de Rebote en Login (web)|	Mide cuántos usuarios llegan al login pero se salen sin iniciar sesión.|	Sesiones que abandonan en login / sesiones totales en login.|	Disminuir el abandono gracias al botón más visible y atractivo.|
|Nivel de Satisfacción Visual|	Evalúa la percepción estética y usabilidad del diseño.|	Encuesta interna o puntuación post-sesión (1–5).|	Aumentar bienestar visual gracias al nuevo tema morado pastel.|
|Adopción del Tema (móvil)|	Mide cuántos usuarios mantienen el tema por defecto vs. cambios manuales (si aplica).	|Registro automático en preferencias de UI.	|Confirmar que el cambio de color es mejor aceptado visualmente.|

**Explicación del Impacto al Negocio**

- El cambio de color del botón de login influye directamente en la tasa de acceso, por lo que la tasa de rebote en login es clave.

- La redirección a “Registrar Estado de Salud” mejora la tarea principal del usuario móvil, entonces la tasa de completitud debe aumentar.

- Las imágenes agregadas en los dashboards fortalecen la identidad de la plataforma, lo que se refleja en engagement y tiempo en sesión.

- El tema morado pastel impacta la experiencia visual, lo cual afecta la percepción de facilidad de uso y satisfacción.

### 8.2.3. Measures.

1. Para medir el impacto del cambio de color del botón "Log in" a verde se puede considerar la tasa de clics (CTR) del botón y la tasa de conversión de inicio de sesión. Un aumento en CTR y en conversiones indicaría que el nuevo color mejora la visibilidad y la intención de inicio de sesión.

- Fuente de datos: Google Analytics / Mixpanel / eventos front (o Datadog RUM si usarás Datadog).

2. Para evaluar si el botón verde afecta la usabilidad, medir tiempo hasta el primer clic en la pantalla de login y tasa de rebote de la página de login. Menores tiempos y menor rebote indican mejor usabilidad.

- Fuente de datos: RUM (Real User Monitoring), logs de frontend.

3. Para validar la redirección en app móvil hacia "Registrar estado de salud" medir la tasa de éxito de redirección (porcentaje de sesiones donde la redirección ocurre correctamente) y la tasa de abandono después de la redirección. Una alta tasa de éxito y baja tasa de abandono indican flujo correcto y útil.

- Fuente de datos: Firebase Analytics / Mobile Analytics / eventos en app / Datadog Mobile RUM.

4. Medir completitud del formulario de estado de salud (porcentaje de usuarios que inician vs completan) tras la redirección. Aumentos significativos muestran que la redirección produce acciones esperadas.

- Fuente de datos: Backend logs, eventos de formulario.

5. Para la imagen referencial de psicología en dashboard de doctor, medir tiempo de carga de la vista y error rate de carga de la imagen. Si la imagen incrementa tiempos excesivos o provoca errores, debe optimizarse.

- Fuente de datos: Lighthouse / RUM / Datadog Synthetic & logs.

6. Evaluar engagement en dashboard de doctor (tiempo medio por sesión en dashboard, acciones por sesión) después de añadir la imagen. Un aumento sugiere que la imagen aporta valor informativo/estético.

- Fuente de datos: Analytics del dashboard.

7. Para la imagen del logo en dashboard de paciente, medir percepción/UX mediante una encuesta in-app (CSAT) y retención en la pantalla (tiempo promedio). Mejores puntuaciones y mayor tiempo apoyan la hipótesis de percepción positiva.

- Fuente de datos: Encuestas in-app + analytics.

8. Para el cambio del tema a morado pastel en versión móvil, medir NPS/CSAT en muestras de usuarios móviles y tasa de permanencia en la app tras la actualización de tema. Mejoras sugieren mayor satisfacción visual y usabilidad.

- Fuente de datos: Encuestas + Firebase / analytics.

9. Medir errores y crashes introducidos por los cambios (crash rate, exceptions por versión). Cualquier aumento requiere rollback/investigación.

- Fuente de datos: Sentry / Datadog APM / logs móviles.

10. Para todos los cambios visuales, medir funnel de conversión (p. ej. abrir app → ver login → iniciar sesión → completar acción) y comparar antes/después para ver dónde impactan los cambios.

- Fuente de datos: Eventos de producto / herramientas de analítica.

11. Medir tasa de adopción por cohorte: porcentaje de usuarios que usan la nueva funcionalidad (p. ej. usuarios móviles que son redirigidos) por cohortes diarias/semanales. Indica si la función se está usando con el tiempo.

- Fuente de datos: Cohort analysis en analytics/Firebase.

12. Medir retención (D1, D7, D30) de usuarios expuestos a los cambios vs no expuestos (A/B). Mayor retención sugiere efecto positivo a largo plazo.

- Fuente de datos: Analytics / A/B testing platform.

13. Medir tiempos de respuesta de backend relacionados con las nuevas acciones (p. ej. guardado del estado de salud). Aumentos pueden indicar cuello de botella.

- Fuente de datos: Datadog APM / logs de servidor.

14. Medir uso de recursos del frontend (CPU, memoria) y TTFB / LCP / CLS en páginas afectadas (login, dashboards). Valores estables/óptimos confirman que los cambios visuales no degradan performance.

- Fuente de datos: Lighthouse, Datadog RUM, Synthetics.

15. Medir tasa de errores de validación en formularios (por ejemplo, en registro de estado de salud). Un aumento puede significar problemas de UX o bugs en la redirección/flow.

- Fuente de datos: Backend logs, eventos de error.

16. Medir feedback cualitativo: número y sentimiento de comentarios/soporte relacionados con las nuevas features (tickets, reviews, encuestas). Complementa métricas cuantitativas.

- Fuente de datos: Sistema de tickets, Zendesk, comentarios en Play/App Store, encuestas in-app.

17. Medir eficacia del A/B test para cambios visuales: tamaño del efecto en métricas clave (CTR, conversión), p-value y confianza estadística. Decisión basada en umbral predefinido.

- Fuente de datos: Plataforma de A/B testing (Optimizely / Firebase A/B / herramienta interna).

18. Medir impacto en soporte/operaciones: número de incidencias generadas tras el deploy y tiempo medio de resolución (MTTR). Un aumento requiere ajuste de rollout o rollback.

- Fuente de datos: Datadog logs/alerts, sistema de incidencias.

19. Medir adopción por segmento (p. ej. nuevos usuarios vs recurrentes; Android vs iOS) para detectar diferencias de comportamiento e identificar optimizaciones específicas.

- Fuente de datos: Analytics segmentado.

20. Medir porcentaje de rollback o hotfixes necesarios tras la entrega y la frecuencia de despliegues correctivos. Alto porcentaje indica problemas en QA/pipeline.

- Fuente de datos: Registro de deployments / CI/CD pipeline logs (GitHub Actions, Jenkins, Datadog events).

### 8.2.4. Conditions.

**● Público Objetivo:**

El público objetivo de las pruebas serán usuarios activos de la plataforma, principalmente estudiantes y jóvenes adultos que ya utilizan o están familiarizados con la herramienta. La selección no estará limitada por ubicación, pero el piloto inicial se realizará con usuarios de Lima para facilitar observación y retroalimentación directa.

**● Entorno de Pruebas:**

Las pruebas se llevarán a cabo en un entorno controlado, utilizando versiones de prueba (staging) de la aplicación. Se monitoreará el rendimiento del sistema antes y después de habilitar las nuevas funciones para comparar resultados con claridad.

**● Usuarios Participantes:**

Se seleccionará un grupo reducido de usuarios piloto que utilizarán la plataforma con la nueva función habilitada (Vista de Ayuda y Crear Ubicación). Estos usuarios serán guiados y se les solicitará retroalimentación directa durante el periodo de pruebas.

**● Período de Evaluación:**

Las pruebas se realizarán durante un período de 2 a 4 semanas, tiempo suficiente para observar patrones de uso, identificar errores recurrentes y evaluar impacto en la experiencia del usuario y el rendimiento del sistema.

**● Control de Variables Externas:**

Se controlarán factores como horarios de alto tráfico, versiones de navegador, tipos de dispositivo y velocidad de red, para evitar que estos influyan en los resultados y permitir una medición precisa del desempeño real de la nueva funcionalidad.

**● Participación Activa de Usuarios:**

Se incentivará la participación activa mediante breves mensajes dentro de la aplicación, recordatorios y encuestas rápidas para recopilar retroalimentación sobre facilidad de uso, claridad de la función y utilidad percibida.

**● Consentimiento Informado:**

Los usuarios participantes serán informados previamente sobre los objetivos del experimento y el tipo de datos que se recolectarán (uso de la función, tiempos de interacción, niveles de satisfacción), asegurando su consentimiento voluntario.

**● Muestra Representativa:**

La muestra incluirá usuarios con distintos niveles de experiencia tecnológica (bajo, medio y alto), para evaluar si las funciones resultan igualmente accesibles para todos los perfiles de usuario.

**● Colaboración con Entornos Educativos y Grupos de Comunidad:**

En caso de ser necesario, se establecerán acuerdos con instituciones o comunidades estudiantiles para facilitar adopción, uso guiado y retroalimentación colectiva.

● Medición y Evaluación Continua:
Durante todo el período de pruebas, el desempeño de la aplicación será monitoreado en tiempo real mediante métricas como CPU usage, tasa de clics, tiempo de permanencia y tasa de éxito en la navegación. Los resultados se evaluarán semanalmente para decidir si se requieren ajustes, optimizaciones o cambios en la interfaz.

### 8.2.5. Scale Calculations and Decisions.

● Tamaño de la Muestra Piloto:

Antes de aplicar los cambios de manera definitiva en la plataforma, se seleccionará una muestra piloto de entre 20 y 50 usuarios activos que utilicen la aplicación de forma regular. Este grupo permitirá observar el comportamiento real de los usuarios frente a las funciones Crear Ubicación y Vista de Ayuda sin afectar a la totalidad de la comunidad.

● Pruebas en Pequeña Escala:

Las primeras pruebas se realizarán con grupos reducidos, preferiblemente usuarios que ya estén familiarizados con la interfaz. Esto permitirá identificar dificultades en la navegación, carga del sistema o confusión en la interacción antes de abrir la funcionalidad al resto de usuarios.

● Expansión Progresiva:

Si los resultados del piloto muestran mejoras en los indicadores clave (uso activo, menor tiempo de búsqueda, disminución en solicitudes de soporte), las funciones se extenderán progresivamente a más usuarios dentro de la misma plataforma. La expansión se realizará por etapas para evitar saturaciones o fallos en producción.

● Escalabilidad y Recursos Técnicos:

La decisión de escalar la implementación dependerá de:

- Capacidad del servidor para soportar el aumento de solicitudes.

- Carga promedio del CPU después de habilitar las funciones.

- Tasa de errores o cuellos de carga registrados.

- Disponibilidad de personal para soporte y monitoreo.

Si las métricas se mantienen dentro de los rangos esperados, se continuará con el despliegue de manera controlada.

● Monitoreo Continuo:

Durante el proceso de expansión se realizará un seguimiento constante de:

- Tiempo de respuesta de la aplicación.

- Porcentaje de uso de la nueva funcionalidad.

- Feedback reportado por los usuarios.

Esto permitirá actuar rápidamente ante posibles problemas de rendimiento o usabilidad.

● Evaluación de Resultados:

Los resultados obtenidos del piloto se compararán con las métricas iniciales (línea base) para evaluar si:

- La función realmente mejora la experiencia.

- Reduce la necesidad de soporte adicional.

- Aumenta la interacción y el tiempo útil dentro de la plataforma.

Solo si los resultados son positivos se procederá con la expansión total.

● Comunicación con Usuarios y Equipos:

Se informará a los usuarios sobre los cambios implementados, explicando su propósito y beneficios. Además, el equipo técnico y de soporte será preparado para responder dudas o incidencias durante la adopción.

● Retroalimentación de Usuarios:

La retroalimentación recopilada en cada fase será clave para decidir si:

- Se continúa avanzando con la expansión.

- Se realizan ajustes de diseño o experiencia.

Se reevalúa la función antes de una liberación completa.

### 8.2.6. Methods Selection.

Para la evaluación de las funciones implementadas, se seleccionarán métodos de experimentación que permitan medir el impacto de manera confiable y comparativa:

● Pruebas A/B:
Se utilizarán para comparar el comportamiento de los usuarios con y sin acceso a las funciones Crear Ubicación y Vista de Ayuda. Esto permitirá identificar si la nueva funcionalidad realmente mejora el uso y la interacción dentro de la plataforma.

● Pruebas de Grupo de Control:
Se definirá un grupo de usuarios que continuará utilizando la plataforma en su estado actual y otro grupo que utilizará las nuevas funciones. La comparación entre ambos permitirá atribuir cambios directamente a la nueva funcionalidad.

● Experimentación en Entorno Real:
Luego de validar la estabilidad en pruebas controladas, las funciones se habilitarán progresivamente a usuarios reales para observar su uso en el contexto cotidiano sin intervenciones artificiales.

La selección final de métodos dependerá de la viabilidad técnica, el tamaño de la muestra disponible y los objetivos específicos de cada funcionalidad en evaluación.

### 8.2.7. Data Analytics: Goals, KPIs and Metrics Selection.

Se establecerán indicadores y métricas para evaluar el desempeño y la adopción de las nuevas funciones:

**Objetivo General:**
Medir el impacto de Crear Ubicación y Vista de Ayuda en la participación del usuario, la eficiencia de navegación y la carga del sistema.

**KPIs Principales:**

- Tasa de Uso de la Función: Porcentaje de usuarios que utilizan las funciones nuevas frente al total de usuarios activos.

- Tiempo Promedio de Navegación: Tiempo utilizado para completar tareas comunes dentro de la plataforma.

- Reducción de Solicitudes de Soporte: Número de consultas dirigidas al soporte antes y después de la implementación.

- Carga Promedio del CPU: Nivel de consumo de recursos tras la habilitación de las nuevas funciones.

**Métricas Específicas:**

- Número de ubicaciones creadas por día/semana.

- Cantidad de veces que se abre la ventana Vista de Ayuda.

- Variación en el porcentaje de errores o caídas del sistema.

- Nivel de interacción por sesión (clics, vistas, rutas navegadas).

Estas métricas permitirán determinar si las funcionalidades están mejorando la experiencia de usuario y el rendimiento general del sistema.

### 8.2.8. Web and Mobile Tracking Plan.

Para asegurar la correcta recopilación de datos que respalde los experimentos, se implementará un plan de seguimiento unificado tanto en la versión web como móvil de la plataforma:

● Instrumentación de Eventos de Usuario:

Se definirán eventos clave como:

 - Crear una ubicación

 - Editar una ubicación

 - Abrir Vista de Ayuda

 - Tiempo dentro de la ventana de ayuda

 - Acciones posteriores a recibir ayuda

● Integración de Herramientas de Monitoreo:

Se utilizarán herramientas como:

 - Datadog para monitoreo de rendimiento, consumo de CPU y tiempo de respuesta.

 - Google Analytics o Mixpanel para rastrear interacciones del usuario.

 - Logging centralizado para registrar errores y acciones relevantes.

● Sincronización entre Web y Móvil:

Los mismos identificadores de usuario y los mismos eventos serán registrados en ambas plataformas para mantener coherencia en el análisis de datos.

● Control de Privacidad y Consentimiento:

Los usuarios serán informados sobre la recopilación de datos con fines de mejora de la experiencia y deberán otorgar consentimiento previo.

Este plan permitirá evaluar con precisión el impacto de cada cambio en el uso real de la plataforma.

## 8.3. Experimentation
### 8.3.1. To-Be User Stories.
### 8.3.2.To-Be Product Backlog
