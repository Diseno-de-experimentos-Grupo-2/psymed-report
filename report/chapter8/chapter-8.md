# Capítulo VIII: Experiment-Driven Development

## 8.1.Experiment Planning

### 8.1.1. As-Is Summary.

Actualmente, la aplicación presenta aspectos de interfaz y experiencia de usuario que pueden dificultar la navegación fluida y la identificación visual dentro del sistema. Algunos botones poseen colores que no destacan, ciertos dashboards carecen de elementos visuales representativos, y en la aplicación móvil el flujo de ingreso no conduce directamente a la funcionalidad esperada por los usuarios. Además, la identidad visual no es consistente entre versión web y móvil, lo que afecta la coherencia de marca y la percepción general de profesionalismo.

### 8.1.2. Raw Material: Assumptions, Knowledge Gaps, Ideas, Claims.

- Para mejorar la visibilidad y el reconocimiento del botón de inicio de sesión, se podría cambiar su color actual a verde para facilitar que el usuario lo identifique rápidamente.

- Para optimizar el flujo de navegación en la aplicación móvil, se podría configurar que al iniciar sesión el usuario sea dirigido directamente a la vista de registro de estado de salud, reduciendo pasos y tiempos de interacción.

- Para reforzar la orientación profesional del dashboard del doctor en la versión web, se podría agregar una imagen referencial relacionada con psicología que acompañe los elementos visuales existentes.

- Para incrementar la armonía visual del dashboard en la versión web, se podría cambiar el color del toolbar a cyan oscuro para generar un contraste esteticamente atractivo.

- Para mejorar la consistencia estética entre plataformas, se podría implementar un cambio de tema de color hacia tonos morado pastel en la versión móvil, manteniendo una identidad visual uniforme.

### 8.1.3. Experiment-Ready Questions.

- Cambio de Color del Botón de Inicio de Sesión: ¿El cambio del color del botón a verde facilita que los usuarios identifiquen más rápido la acción de iniciar sesión y aumenta la tasa de acceso exitoso?

- Navegación en Aplicación Móvil: ¿Dirigir automáticamente al usuario a la vista de registro de estado de salud reduce el tiempo de navegación e incrementa la frecuencia de registro?

- Imagen Referencial en Dashboard del Doctor: ¿La inclusión de una imagen relacionada con psicología en el dashboard del doctor mejora la percepción profesional y la claridad contextual de la interfaz?

- Colorimetría del Toolbar: ¿El cambio de tonalidad del toolbar a cyan oscuro genera un impacto positivo en la primera vista del usuario hacia la aplicación web?

- Nuevo Tema en Versión Móvil: ¿El cambio de tema de color a morado pastel mantiene la legibilidad y mejora la consistencia visual en la aplicación móvil?

### 8.1.4. Question Backlog.

- **Impacto del Botón Verde de Inicio de Sesión:**
¿En qué medida el cambio del botón a color verde aumentaría la tasa de reconocimiento visual y la frecuencia de inicio de sesión por parte de los usuarios?

- **Redirección Automática a Registro de Estado de Salud:**
¿La acción de dirigir automáticamente al usuario al registro de su estado de salud al ingresar a la aplicación reduciría la fricción en la navegación y aumentaría la constancia de uso diario?

- **Uso de Imagen de Psicología en el Dashboard del Doctor:**
¿La incorporación de una imagen contextual relacionada con psicología en el dashboard médico incrementaría la percepción de claridad, sentido profesional y confianza en el entorno clínico digital?

- **Mejora de armonía visual con cyan oscuro al toolbar web:**
¿Cambiar el color del toolbar de negro azabache a cyan oscuro incrementaría la atracción visual del paciente y médico al ingresar al dashboard de la aplicación web?

- **Consistencia Visual con Tema Morado Pastel en Móvil:**
¿La adopción del tema en color morado pastel en la versión móvil mejoraría la coherencia visual y retención de los usuarios sin afectar la legibilidad de los elementos interactivos?

### 8.1.5. Experiment Cards.

|            | Experiment Card 1                                                                                                                                                                                  |
|------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Question   | ¿Cómo afecta a la experiencia del usuario el cambio del botón de inicio de sesión a color verde?                                                                                                   |
| Why        | Queremos entender si un mayor contraste visual puede facilitar el reconocimiento de la acción principal y aumentar la frecuencia de inicio de sesión.                                              |
| What       | Se cambiará el color del botón de inicio de sesión a verde y se observará si los usuarios identifican más rápido la acción, midiendo la cantidad de inicios exitosos y comentarios sobre claridad. |
| Hypothesis | Cambiar el botón a color verde mejorará la visibilidad y aumentará la tasa de inicio de sesión debido a un reconocimiento visual más claro.                                                        |

|            | Experiment Card 2                                                                                                                                                        |
|------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Question   | ¿La redirección automática al registro de estado de salud mejora la constancia de uso diario?                                                                            |
| Why        | Queremos evaluar si reducir pasos manuales ayuda a que los usuarios registren su información con mayor frecuencia y permanezcan más activos dentro de la aplicación.     |
| What       | Al iniciar sesión, el usuario será dirigido automáticamente a la sección de registro de estado de salud. Se analizará si se incrementa la cantidad de registros diarios. |
| Hypothesis | Redirigir automáticamente a la pantalla de registro aumentará la continuidad de uso, ya que elimina fricción y pasos innecesarios.                                       |

|            | Experiment Card 3                                                                                                                                        |
|------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| Question   | ¿Cómo influye una imagen referencial de psicología en la percepción de claridad del dashboard médico?                                                    |
| Why        | Queremos explorar si un contexto visual puede ayudar a los profesionales a identificar más rápidamente su entorno de trabajo y sentir mayor guía visual. |
| What       | Se añadirá una imagen referencial en el dashboard médico y se solicitarán breves opiniones sobre claridad y orientación.                                 |
| Hypothesis | Incorporar una imagen referencial aumentará la percepción de claridad y mejorará la orientación visual dentro del dashboard.                             |

|            | Experiment Card 4                                                                                                       |
|------------|-------------------------------------------------------------------------------------------------------------------------|
| Question   | ¿Cómo afecta el cambio de negro azabache a cyan oscuro en la percepción y atracción del usuario en la app web?          |
| Why        | Queremos entender si reforzar la armonía visual del sistema aumenta la atracción del servicio ante los usuarios.        |
| What       | Se cambiará el color del toolbar a cyan oscuro y se medirá la atracción del usuario al producto Psymed.                 |
| Hypothesis | Cambiar el color del toolbar a cyan oscuro incrementará la armonía visual y atracción del usuario frente al diseño web. |

|            | Experiment Card 5                                                                                                                             |
|------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| Question   | ¿Cómo afecta el uso de un tema en color morado pastel a la experiencia visual y legibilidad en la versión móvil?                              |
| Why        | Queremos evaluar si la estética puede mejorarse sin afectar la lectura o navegación en pantallas pequeñas.                                    |
| What       | Se aplicará un tema morado pastel en la interfaz móvil y se medirá la comprensión de elementos, comodidad visual y comentarios de usabilidad. |
| Hypothesis | Adoptar el tema morado pastel hará la interfaz más agradable visualmente sin comprometer la legibilidad ni la usabilidad general.             |

## 8.2. Experiment Design
### 8.2.1. Hypotheses.

| Hipótesis 1  | Cambio de color del botón de Log in a verde (Web)                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|--------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Question     | 	¿El cambio del color del botón de “Iniciar Sesión” a verde ha incrementado la interacción y el número de inicios de sesión exitosos?                                                                                                                                                                                                                                                                                                                                                                         |
| Data analyze | 	Para este análisis se utilizará Google Analytics y Datadog RUM. Se realizarán 30 pruebas durante sesiones de usuario en la aplicación web. Después del cambio al color verde, se espera que la tasa de clic (CTR) al botón pase de 12.4% a 15.1%, lo que representaría un incremento del 21.7% en interacción. Además, los inicios de sesión exitosos aumentarán un 9.8% en relación con la semana previa. Esto sugeriría que el nuevo color mejora la visibilidad y sensación de acción en el usuario. </p> |
| Hypothesis   | 	El cambio del botón a verde mejora la tasa de interacción y aumenta los inicios de sesión exitosos, debido a una mayor claridad visual y estímulo de acción.                                                                                                                                                                                                                                                                                                                                                 |

| Hipótesis 2  | Redirección inicial a registrar estado de salud (App móvil)                                                                                                                                                                                                                                                                                                                                                             |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Question     | 	¿Enviar al usuario directamente a la vista de “Registrar estado de salud” mejora la frecuencia de registros realizados en la primera sesión?                                                                                                                                                                                                                                                                           |
| Data analyze | 	Para este análisis se utilizará Firebase Analytics. Se realizarán 50 pruebas de sesión en dispositivos móviles. Antes de la modificación, solo el 32% de los usuarios completaba un registro de estado en la primera sesión. Después de aplicar la redirección automática, la cifra aumentaría al 56%, lo que representa un incremento del 24 puntos porcentuales y una mejora significativa en el engagement inicial. | 
| Hypothesis   | 	La redirección aumenta la participación en el registro de estado de salud y fortalece el vínculo inicial del usuario con la aplicación.                                                                                                                                                                                                                                                                                |

| Hipótesis 3  | Imagen referencial de psicología en el dashboard del doctor (Web)                                                                                                                                                                                                                                                                                           |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Question     | 	¿La inclusión de la imagen referencial mejora la comprensión visual del dashboard y aumenta la interacción con secciones relacionadas?                                                                                                                                                                                                                     |
| Data analyze | 	Se utilizará Hotjar Heatmaps y Google Analytics para analizar la atención visual y el flujo de navegación. Después de 20 sesiones monitoreadas, se observaría que el área donde se colocó la imagen recibió un 33% más de fijaciones visuales, y los clics hacia los recursos psicológicos aumentarán en 11.4%. Esto indicará un estímulo visual efectivo. | 
| Hypothesis   | 	La imagen referencial mejora la orientación visual y aumenta la probabilidad de interacción con recursos psicológicos en el dashboard.                                                                                                                                                                                                                     |

| Hipótesis 4  | Cambio de color al toolbar (Web)                                                                                                                                                                                                                                                      |
|--------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Question     | 	¿El cambio de color mejora la armonía visual y atracción, mejorando la retención del usuario?                                                                                                                                                                                        |
| Data analyze | 	Para este análisis se aplicará una encuesta in-app corta (N=28) y revisión de flujos mediante Hotjar. La percepción de estética visual pasaría de 3.8 a 4.4/5 en promedio. Además, la tasa de permanencia en la pantalla inicial aumentará 8.9%, indicando menor abandono inmediato. | 
| Hypothesis   | 	Cambiar el color del toolbar refuerza la armonía visual y genera mayor atracción, lo que reduce el abandono al ingresar al dashboard.                                                                                                                                                |

| Hipótesis 5  | Cambio de tema a morado pastel (App móvil)                                                                                                                                                                                                                                                                                                                      |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Question     | 	¿El nuevo tema morado pastel mejora la satisfacción visual sin afectar la usabilidad general de la aplicación?                                                                                                                                                                                                                                                 |
| Data analyze | 	Se utilizarán pruebas con Lighthouse Mobile y encuestas in-app de preferencia visual (N=31). La puntuación de satisfacción estética aumentará de 3.9 a 4.6/5. Las mediciones de performance se mantendrán estables (puntaje de rendimiento entre 74-78, sin variaciones significativas). No se detectarían problemas de contraste según validación automática. | 
| Hypothesis   | 	El nuevo tema aumenta la satisfacción visual del usuario sin comprometer accesibilidad ni rendimiento.                                                                                                                                                                                                                                                         |

### 8.2.1.1. Null & Alternative Hypotheses Statements

| **Hypothesis 1**         | Cambio de color del botón de Log in a verde (Web)                                                                                                                                                |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Question**             | ¿El cambio del color del botón de “Iniciar Sesión” a verde ha incrementado la interacción y el número de inicios de sesión exitosos?                                                             |
| **Belief**               | El cambio del botón a verde mejora la visibilidad y genera mayor intención de acción del usuario.                                                                                                |
| **Hypothesis (H₁)**      | Creemos que el cambio del color del botón de “Iniciar Sesión” a verde incrementará la tasa de clic (CTR) en un 21.7% y los inicios de sesión exitosos en un 9.8%, al mejorar la claridad visual. |
| **Null Hypothesis (H₀)** | El cambio del color del botón de “Iniciar Sesión” a verde no tendrá efecto significativo en la tasa de interacción ni en los inicios de sesión exitosos.                                         |

| **Hypothesis 2**         | Redirección inicial a registrar estado de salud (App móvil)                                                                                                                                |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Question**             | ¿Enviar al usuario directamente a la vista de “Registrar estado de salud” mejora la frecuencia de registros realizados en la primera sesión?                                               |
| **Belief**               | Una redirección automática guía al usuario y estimula la participación temprana.                                                                                                           |
| **Hypothesis (H₁)**      | Se considera que redirigir al usuario directamente al registro de estado de salud incrementará la tasa de registros en primera sesión del 32% al 56%, fortaleciendo el engagement inicial. |
| **Null Hypothesis (H₀)** | La redirección automática no modificará significativamente la frecuencia de registros en la primera sesión.                                                                                |


| **Hypothesis 3**         | Imagen referencial de psicología en el dashboard del doctor (Web)                                                                      |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
| **Question**             | ¿La inclusión de una imagen referencial mejora la comprensión visual y la interacción con secciones relacionadas?                      |
| **Belief**               | Los elementos visuales facilitan la orientación y estimulan la exploración de contenidos.                                              |
| **Hypothesis (H₁)**      | Se prevé que incluir una imagen referencial aumentará las fijaciones visuales en un 33% y los clics en recursos psicológicos en 11.4%. |
| **Null Hypothesis (H₀)** | La inclusión de una imagen referencial no generará diferencias significativas en atención visual ni en interacción con las secciones.  |


| **Hypothesis 4**         | Cambio de color al toolbar (Web)                                                                                               |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| **Question**             | ¿El cambio de color del toolbar mejora la armonía visual y la retención del usuario?                                           |
| **Belief**               | Un color más armónico genera mayor agrado estético y permanencia.                                                              |
| **Hypothesis (H₁)**      | El cambio de color del toolbar incrementará la valoración estética promedio de 3.8 a 4.4/5 y aumentará la permanencia un 8.9%. |
| **Null Hypothesis (H₀)** | El cambio de color del toolbar no tendrá impacto significativo en la percepción estética ni en la retención del usuario.       |



| **Hypothesis 5**         | Cambio de tema a morado pastel (App móvil)                                                                                      |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| **Question**             | ¿El nuevo tema morado pastel mejora la satisfacción visual sin afectar la usabilidad general?                                   |
| **Belief**               | Un esquema cromático suave mejora la percepción visual y mantiene el rendimiento técnico.                                       |
| **Hypothesis (H₁)**      | El nuevo tema morado pastel aumentará la satisfacción estética de 3.9 a 4.6/5 sin afectar la performance ni el contraste.       |
| **Null Hypothesis (H₀)** | El nuevo tema morado pastel no producirá diferencias significativas en la satisfacción visual ni en el rendimiento del sistema. |



### 8.2.2. Domain Business Metrics

| Métrica de Negocio                                         | 	Descripción                                                                                     | 	Cómo se mide                                                          | 	Objetivo de Mejora                                                     |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|-------------------------------------------------------------------------|
| Tasa de Retención de Usuario                               | 	Mide la cantidad de usuarios que vuelven a la aplicación después de utilizarla por primera vez. | 	Usuarios activos semanales / usuarios registrados.                    | 	Aumentar la retención al mejorar la experiencia visual y navegación.   |
| Tasa de Compleción del Registro de Estado de Salud (móvil) | 	Mide cuántos usuarios que entran efectivamente terminan registrando su estado de salud.	        | Total de usuarios que inician sesión vs. los que completan la acción.	 | Incrementar completitud gracias a la redirección directa.               |
| Engagement en el Dashboard (web)                           | 	Mide la interacción dentro de los paneles del doctor y paciente.                                | 	Clics, tiempo en página, número de elementos consultados por sesión.  | 	Incrementar la interacción gracias a los elementos visuales agregados. |
| Tasa de Rebote en Login (web)                              | 	Mide cuántos usuarios llegan al login pero se salen sin iniciar sesión.                         | 	Sesiones que abandonan en login / sesiones totales en login.          | 	Disminuir el abandono gracias al botón más visible y atractivo.        |
| Nivel de Satisfacción Visual                               | 	Evalúa la percepción estética y usabilidad del diseño.                                          | 	Encuesta interna o puntuación post-sesión (1–5).                      | 	Aumentar bienestar visual gracias al nuevo tema morado pastel.         |
| Adopción del Tema (móvil)                                  | 	Mide cuántos usuarios mantienen el tema por defecto vs. cambios manuales (si aplica).	          | Registro automático en preferencias de UI.	                            | Confirmar que el cambio de color es mejor aceptado visualmente.         |

**Explicación del Impacto al Negocio**

- El cambio de color del botón de login influye directamente en la tasa de acceso, por lo que la tasa de rebote en login es clave.

- La redirección a “Registrar Estado de Salud” mejora la tarea principal del usuario móvil, entonces la tasa de completitud debe aumentar.

- Las imágenes agregadas en los dashboards fortalecen la identidad de la plataforma, lo que se refleja en engagement y tiempo en sesión.

- El color cyan oscuro mejora la armonía visual, lo que aumenta la retención y atracción del usuario.

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

7. Para el cambio de color del toolbar, medir percepción/UX mediante una encuesta in-app (CSAT) y retención en la pantalla (tiempo promedio). Mejores puntuaciones y mayor tiempo apoyan la hipótesis de percepción positiva.

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
| **User Story ID** | **Título**                                                                | **Descripción**                                                                                                                                                  | **Criterios de Aceptación**                                                                                                                                                                                                               | **Relacionado con (Epic ID)** |
|-------------------|---------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------|
| **UA01**          | Cambiar color del botón “Log In” a verde                                  | Como usuario de la aplicación web, quiero que el botón de inicio de sesión sea de color verde, para identificarlo fácilmente y tener una interfaz más agradable. | **Escenario 1: Cambio de color visible**<br>Given que el usuario está en la pantalla de inicio de sesión.<br>When la página carga.<br>Then el botón “Log In” se muestra en color verde.                                                   | **E01**                       |
| **UA02**          | Mantener consistencia del color del botón “Log In” en todas las pantallas | Como usuario, quiero que el color verde del botón “Log In” se mantenga igual en todas las vistas relacionadas con autenticación, para tener coherencia visual.   | **Escenario 1: Verificación de consistencia**<br>Given que el usuario cambia entre las vistas “Registro” y “Recuperar contraseña”.<br>When observa el botón “Log In”.<br>Then el color verde se mantiene en todas.                        | **E01**                       |
| **UA03**          | Redirigir automáticamente a “Registrar estado de salud” al ingresar       | Como usuario de la app móvil, quiero que al iniciar sesión se me redirija automáticamente a la pantalla de “Registrar estado de salud” para ahorrar tiempo.      | **Escenario 1: Redirección inmediata**<br>Given que el usuario inicia sesión correctamente.<br>When presiona “Iniciar sesión”.<br>Then la aplicación lo dirige directamente a la vista “Registrar estado de salud”.                       | **E02**                       |
| **UA04**          | Asegurar adaptabilidad de la imagen en diferentes resoluciones            | Como doctor, quiero que la imagen del dashboard se adapte correctamente a distintos tamaños de pantalla, para evitar deformaciones.                              | **Escenario 1: Responsividad de imagen**<br>Given que el usuario cambia el tamaño del navegador.<br>When la imagen se redimensiona.<br>Then mantiene su proporción sin distorsión.                                                        | **E03**                       |
| **UA05**          | Cambiar el color del toolbar de la versión web                            | Como usuario, quiero que la aplicación web tenga un diseño atractivo, para que sea satisfactorio usarla.                                                         | **Escenario 1: Toolbar cyan oscuro**<br>Given que el paciente ha iniciado sesión.<br>When se carga el panel principal.<br>Then se muestra el toolbar cyan oscuro.                                                                         | **E04**                       |
| **UA06**          | Cambiar el tema de color a morado pastel (App móvil)                      | Como usuario móvil, quiero que la app adopte un tema de color morado pastel, para disfrutar una interfaz más moderna y agradable.                                | **Escenario 1: Aplicación del tema**<br>Given que el usuario abre la app.<br>When la interfaz carga.<br>Then todos los elementos visuales adoptan el tema morado pastel.                                                                  | **E05**                       |


### 8.3.2.To-Be Product Backlog

| Orden | User Story ID | Título                                                                    | Story Points (1 / 2 / 3 / 5 / 8) |
|:-----:|:--------------|:--------------------------------------------------------------------------|:--------------------------------:|
|   1   | UA01          | Cambiar color del botón “Log In” a verde                                  |                2                 |
|   2   | UA02          | Mantener consistencia del color del botón en todas las pantallas          |                2                 |
|   3   | UA03          | Redirigir automáticamente a “Registrar estado de salud” al ingresar       |                3                 |
|   5   | UA04          | Agregar imagen referencial sobre psicología en dashboard del doctor       |                3                 |
|   6   | UA05          | Asegurar adaptabilidad de la imagen en diferentes resoluciones            |                2                 |
|   7   | UA06          | Cambiar el color del toolbar del la versión web                           |                3                 |
|   9   | UA07          | Cambiar el tema de color a morado pastel en la app móvil                  |                5                 |
|  10   | UA08          | Mantener coherencia de colores en todas las vistas del tema morado pastel |                3                 |

### 8.3.3. Pipeline-supported, Experiment-Driven To-Be Software Platform Lifecycle

El ciclo de vida To-Be de la plataforma propone una evolución desde un desarrollo tradicional hacia un modelo altamente automatizado, continuo y guiado por experimentos, permitiendo que las decisiones de diseño, experiencia de usuario y priorización funcional se validen mediante evidencia real.
Este enfoque integra pipelines CI/CD, prácticas de observabilidad, métricas de uso y un proceso de experimentación incremental (A/B testing, feature toggles y validación temprana con usuarios), garantizando que cada incremento del producto sea medible, trazable y alineado con los objetivos de valor.

Dentro de esta visión, los Sprint Backlogs To-Be incorporan tanto historias de usuario funcionales como experimentos controlados (UAxx) diseñados para evaluar hipótesis sobre usabilidad, engagement y adecuación visual de la plataforma. Este enfoque permite que el equipo realice mejoras continuas basadas en datos y reduzca la incertidumbre en las decisiones de diseño.

#### 8.3.3.1. To-Be Sprint Backlogs

Los siguientes sprint backlogs representan la versión To-Be del ciclo de vida de la plataforma, resultado de aplicar un enfoque pipeline-supported, experiment-driven.
El pipeline permitió validar hipótesis de diseño, consistencia visual, flujo de navegación y usabilidad tanto en la aplicación web como en la aplicación móvil, integrando los hallazgos en una versión mejorada del backlog.

Los sprint backlogs To-Be combinan:

- Historias de usuario funcionales iniciales (US01–US20).
- Acciones de usuario experimentales (UA01–UA08) generadas a partir de pruebas rápidas y cuantificables.
- Priorización ajustada (To-Be) en función del impacto demostrado mediante experimentación.

A continuación se presentan los backlogs propuestos, organizados por sprint.

**Sprint 1 — Autenticación, Acceso y Cuentas**

**Objetivo:** Estabilizar los flujos base de acceso y registro.
**Incluye historias funcionales + mejoras experimentales relacionadas con la experiencia de Login.**

**User Stories Funcionales (To-Be)**

- US01 – Registro como profesional de la salud mental
- US02 – Inicio de sesión como paciente
- US03 – Inicio de sesión como profesional
- US12 – Inicio de sesión móvil
- US14 – Cerrar sesión móvil

**Historias Experimentales Integradas (To-Be)**

|ID|	Experimento	|Justificación| To-Be	Story Points|
|--|-------------|-------------|-------------------|
|UA01|	Cambiar color del botón “Log In” a verde|	Aumentó claridad del CTA durante pruebas|	2|
|UA02|	Consistencia del color del botón en todas las pantallas	|Aumentó cohesión visual del flujo|	2|

**Sprint Goal To-Be**

Mejorar la tasa de acceso exitoso mediante diseño consistente y flujos unificados en web y móvil.

**Sprint 2 — Gestión de Pacientes y Datos Clínicos**

**Objetivo:** Establecer los módulos base de registro y visualización de información del paciente.**

**User Stories Funcionales (To-Be)**

- US04 – Registro de información personal del paciente
- US05 – Visualización del estado de ánimo
- US08 – Registro de medicamentos
- US09 – Ver medicamentos
- US13 – Visualizar información de perfil

**Historias Experimentales Integradas (To-Be)**

|ID|	Experimento	|Justificación| To-Be	Story Points|
|--|-------------|-------------|-------------------|
| UA04|	Agregar imagen referencial de psicología en el dashboard del doctor	|Aumento de claridad visual durante pruebas	|3|
|UA05	|Adaptabilidad de la imagen en distintas resoluciones|	Evita distorsión → consistencia UI|	2|

**Sprint Goal To-Be**

Optimizar la experiencia del profesional al visualizar y registrar información clave del paciente.

**Sprint 3 — Bienestar Emocional y Salud Diaria**

**Objetivo:** Integrar el módulo completo de registro y consulta de bienestar emocional y biológico.**

**User Stories Funcionales (To-Be)**

- US06 – Registro de estado de ánimo
- US07 – Registro de funciones biológicas
- US15 – Registro de salud diario (móvil)
- US16 – Lista de medicamentos móvil
- US17 – Ver próximas citas móvil

**Historias Experimentales Integradas (To-Be)**

|ID|	Experimento	|Justificación| To-Be	Story Points|
|--|-------------|-------------|-------------------|
|UA03	|Redirigir automáticamente a “Registrar estado de salud” al ingresar	|Aumenta tasa de registro diario|	3|

**Sprint Goal To-Be**

Automatizar el flujo del paciente para mejorar la captura diaria de información de salud.

**Sprint 4 — Citas Médicas y Dashboard**

**Objetivo:** Consolidar funcionalidades del módulo de citas y coherencia visual global.**

**User Stories Funcionales (To-Be)**

- US10 – Creación de cita
- US11 – Ver citas web
- US17 – (refuerzo) Citas en móvil

**Historias Experimentales Integradas (To-Be)**

|ID|	Experimento	|Justificación| To-Be	Story Points|
|--|-------------|-------------|-------------------|
|UA06|	Cambiar el color del toolbar web|	Mejora navegación y contraste	|3|

**Sprint Goal To-Be**

Garantizar un flujo de agendamiento claro y visualmente coherente.

**Sprint 5 — Tema Visual, Consistencia Estética y Landing Page**

**Objetivo:** Unificar identidad visual en web + móvil y fortalecer la experiencia del visitante en la landing page.**

**User Stories Funcionales (Landing Page)**

- US18 – Información del propósito de la aplicación
- US19 – Imágenes y gráficos relevantes
- US20 – Tipografía legible y estética

**Historias Experimentales Integradas (To-Be)**

|ID|	Experimento	|Justificación| To-Be	Story Points|
|--|-------------|-------------|-------------------|
|UA07	|Cambiar tema a morado pastel en app móvil	|Mejora identidad visual|	5|
|UA08	|Coherencia de colores en todas las vistas	|Consistencia del sistema|	3|

**Sprint Goal To-Be**

Construir una experiencia visual integrada que facilite adopción y confianza en la plataforma.

#### 8.3.3.2. Implemented To-Be Landing Page Evidence

La Landing Page representa uno de los primeros artefactos implementados dentro del ciclo de vida Pipeline-supported, Experiment-Driven To-Be. Su construcción permitió validar hipótesis tempranas relacionadas con navegabilidad, claridad del propósito, consistencia visual y percepción del producto por parte de usuarios externos.
Esta sección presenta la evidencia de implementación obtenida a partir del despliegue en un entorno productivo controlado (GitHub Pages), incluyendo capturas, artefactos visuales, ajustes aplicados y las mejoras derivadas de los experimentos realizados.
El objetivo es demostrar cómo la Landing Page evolucionó mediante iteraciones medibles, apoyadas en datos y retroalimentación temprana, validando su rol dentro de la arquitectura final de la plataforma.

<img src="https://github.com/user-attachments/assets/68383287-2738-432f-aed6-f0d65dadfa3b" />

#### 8.3.3.3. Implemented To-Be Frontend-Web Application Evidence

La aplicación web frontend constituye el componente central de interacción para profesionales de la salud y pacientes dentro de la plataforma. Como parte del ciclo de vida To-Be, su implementación fue sometida a un conjunto de experimentos iterativos destinados a evaluar usabilidad, consistencia visual, rendimiento, adaptabilidad y flujo de navegación.
Esta sección presenta la evidencia concreta de la implementación lograda durante los sprints, incluyendo capturas de pantalla, funcionalidades completadas, integración con el backend y resultados obtenidos de las pruebas experimentales (UA01–UA08).
Se documenta cómo el frontend evolucionó mediante un enfoque incremental soportado por pipelines y validado por experimentos, garantizando que las mejoras aplicadas respondieran a necesidades reales de los usuarios y a objetivos estratégicos de la plataforma.

- US01	Registro como profesional de la salud mental

<img src="https://github.com/user-attachments/assets/fe36685e-3b6f-4ada-851f-6118a49745e1" />

- US02	Inicio de sesión como pacientes

<img src="https://github.com/user-attachments/assets/68383287-2738-432f-aed6-f0d65dadfa3b" />

- US03	Inicio de sesión como profesional de la salud mental

<img src="https://github.com/user-attachments/assets/a7f60860-edcb-4079-b530-0f3b8e069a49" />

- US04	Registro de información personal del paciente

<img src="https://github.com/user-attachments/assets/f49a2b65-35eb-42e3-b410-81c2bdb3e052" />

- US05	Visualización del estado actual de ánimo del paciente

<img src="https://github.com/user-attachments/assets/517488bc-032c-4c4b-aec7-eda3a1a69e6a" />

- US06	Registro de estado de ánimo

<img src="https://github.com/user-attachments/assets/47fdc90f-1ce4-43f1-8601-bb128153590d" />

<img src="https://github.com/user-attachments/assets/9c8b24cd-2492-41bd-988c-d73ba9992213" />

- US07	Registro de funciones biológicas

<img src="https://github.com/user-attachments/assets/e3941525-2db2-4497-9392-e6597dae2367" />

- US08	Registro de medicamentos del paciente

<img src="https://github.com/user-attachments/assets/eb15442f-db73-4bbb-b7ad-5136a61a036a" />

- Ver medicamentos

<img src="https://github.com/user-attachments/assets/6844c2bc-69bf-4c84-b2dc-5ee71e7c8e18" />

- Creación de citas

<img src="https://github.com/user-attachments/assets/e32a0d39-dc93-4509-b31c-ddf4958da6c9" />

- Ver citas médicas

<img src="https://github.com/user-attachments/assets/152d1c1a-0136-4ccb-ad55-fc762ee5ea90" />

#### 8.3.3.4. Implmented To-Be Native-Mobile Application Evidence

##### Pacientes
- US12 Inicio de sesión como paciente
  
![login.jpg](/assets/sprint4/login.jpg)

- US13 Visualización de información de perfil

![patient_profile.jpg](/assets/sprint4/patient_profile.jpg)

- US14 Cerrar sesión

![patient_profile.jpg](/assets/sprint4/patient_profile.jpg)

- US15 Registrar mi estado de salud diario

![mood_status.jpg](/assets/sprint4/mood_status.jpg)

- US16 Consultar mi lista de medicamentos

![medication_list.jpg](/assets/sprint4/medication_list.jpg)

- US17 Ver proximas citas 

![appointments.jpg](/assets/sprint4/appointments.jpg)

##### Doctores
- US03 Inicio de sesión como profesional de la salud mental 

![login.jpg](/assets/sprint4/login.jpg)

- US04 Registro de la información personal del paciente

![new_patient.jpg](/assets/sprint4/new_patient.jpg)

- US05 Visualización del estado actual de ánimo del paciente

![patient_status.jpg](/assets/sprint4/patient_status.jpg)

- US08 Registro de medicamentos del paciente

![add_medication.jpg](/assets/sprint4/add_medication.jpg)

- US10 Creación de citas

![add_appointment.jpg](/assets/sprint4/add_appointment.jpg)

- US11 Visualización de citas médicas

![appointment_view](/assets/sprint4/appointment_view.jpg)

#### 8.3.3.5. Implemented To-Be RESTful API and/ or Serverless Backend Evidence 

Para la plataforma Psymed, se implementó un backend RESTful usando Spring Boot 3, con estructura basada en DDD ligero, controladores organizados por dominios y documentación generada automáticamente mediante Swagger/OpenAPI 3.0.

El servidor se ejecuta localmente en:

https://psymed-backend-new.onrender.com/swagger-ui/index.html

La documentación del API se encuentra disponible a través de:
/v3/api-docs y visualizada mediante Swagger UI.

A continuación, se presentan las evidencias de los módulos implementados y sus endpoints.

![platform.png](/assets/sprint4/platform.png)

- TS-01 Autenticación

![authentication.png](/assets/sprint4/authentication.png)

- TS-02 Gestión del perfil profesional

![professional_profile.png](/assets/sprint4/professional_profile.png)

- TS-03 Gestión del perfil del paciente

![patient_profile.png](/assets/sprint4/patient_profile.png)

- TS-04 Mood States

![patient_report.png](/assets/sprint4/patient_report.png)

- TS-05 Biological functions

![patient_report.png](/assets/sprint4/patient_report.png)

- TS-06 Medication management

![medication.png](/assets/sprint4/medication.png)

- TS-07 Gestión de sesiones profesionales

![professional_sessions.png](/assets/sprint4/professional_sessions.png)

- TS-08 Herramientas de sesión

![session_tools.png](/assets/sprint4/session_tools.png)

- TS-09 Historial clínico

![patients_clinical_history](/assets/sprint4/patients_clinical_history.png)

- TS-10 Gestión de cuentas

![accounts.png](/assets/sprint4/accounts.png)


