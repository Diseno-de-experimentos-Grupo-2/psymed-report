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

![WhatsApp Image 2025-11-30 at 10 38 35 PM](https://github.com/user-attachments/assets/13bd88ab-6227-4f19-9e27-e1ce74f4a96c)

![WhatsApp Image 2025-11-30 at 10 40 18 PM](https://github.com/user-attachments/assets/b1f8d3b8-8e41-4cd4-ae93-eef019b3129a)

![WhatsApp Image 2025-11-30 at 10 40 42 PM](https://github.com/user-attachments/assets/5ffed33a-4c57-4973-9477-f50772caf025)

![WhatsApp Image 2025-11-30 at 10 41 42 PM](https://github.com/user-attachments/assets/02f658d8-bce5-4825-b92b-221e127ec334)

![WhatsApp Image 2025-11-30 at 10 42 04 PM](https://github.com/user-attachments/assets/c6c24afe-3641-4b23-8ee2-2caa42d842e9)

![WhatsApp Image 2025-11-30 at 10 43 26 PM](https://github.com/user-attachments/assets/f02fd2cd-a025-4dde-a562-425c6b820360)

![WhatsApp Image 2025-11-30 at 10 43 46 PM](https://github.com/user-attachments/assets/e94e384f-72ee-4839-b6b6-365dad652edd)

![WhatsApp Image 2025-11-30 at 10 44 04 PM](https://github.com/user-attachments/assets/d69770f7-e3e3-43dd-9478-44266b1edeb1)

#### 8.3.3.3. Implemented To-Be Frontend-Web Application Evidence

La aplicación web frontend constituye el componente central de interacción para profesionales de la salud y pacientes dentro de la plataforma. Como parte del ciclo de vida To-Be, su implementación fue sometida a un conjunto de experimentos iterativos destinados a evaluar usabilidad, consistencia visual, rendimiento, adaptabilidad y flujo de navegación.
Esta sección presenta la evidencia concreta de la implementación lograda durante los sprints, incluyendo capturas de pantalla, funcionalidades completadas, integración con el backend y resultados obtenidos de las pruebas experimentales (UA01–UA08).
Se documenta cómo el frontend evolucionó mediante un enfoque incremental soportado por pipelines y validado por experimentos, garantizando que las mejoras aplicadas respondieran a necesidades reales de los usuarios y a objetivos estratégicos de la plataforma.

- US01	Registro como profesional de la salud mental

![WhatsApp Image 2025-11-30 at 10 45 37 PM](https://github.com/user-attachments/assets/e5491218-11ca-48ba-9d3f-e87e3c189e0a)


- US02	Inicio de sesión como pacientes

![WhatsApp Image 2025-11-30 at 11 47 59 PM](https://github.com/user-attachments/assets/d44d100a-2d11-4823-aa56-1c946b988145)


- US03	Inicio de sesión como profesional de la salud mental

![WhatsApp Image 2025-11-30 at 11 48 34 PM](https://github.com/user-attachments/assets/9677258d-5f58-4261-b444-20d4b50317a9)


- US04	Registro de información personal del paciente

![WhatsApp Image 2025-11-30 at 11 49 21 PM](https://github.com/user-attachments/assets/98d1bb7d-6030-4b8f-90ca-4e5909e71a0e)


- US05	Visualización del estado actual de ánimo del paciente

![WhatsApp Image 2025-11-30 at 11 50 17 PM](https://github.com/user-attachments/assets/4f7fee9c-0156-41d5-8013-4270b9bbcce9)


- US06	Registro de estado de ánimo

![WhatsApp Image 2025-11-30 at 11 50 57 PM](https://github.com/user-attachments/assets/05f141e7-704a-4865-acd9-56a559cee18c)


- US07	Registro de funciones biológicas

![WhatsApp Image 2025-11-30 at 11 51 25 PM](https://github.com/user-attachments/assets/b350e36c-980a-408d-9fdb-28ca128a7d94)


- US08	Registro de medicamentos del paciente

![WhatsApp Image 2025-11-30 at 11 52 58 PM](https://github.com/user-attachments/assets/b6fee4e7-4c57-48ca-a930-ce6027567de2)

- Ver medicamentos

![WhatsApp Image 2025-11-30 at 11 52 58 PM](https://github.com/user-attachments/assets/b2b734f2-6734-4b3f-8b79-ff38665a2fe2)

- Creación de citas

![WhatsApp Image 2025-11-30 at 11 53 45 PM](https://github.com/user-attachments/assets/fc742ed9-3618-486c-9ca2-182225becb87)

- Ver citas médicas

![WhatsApp Image 2025-11-30 at 11 54 36 PM](https://github.com/user-attachments/assets/3367be9c-a108-401a-a65c-579be56d30a4)


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


#### 8.3.3.6. Team Collaboration Insights



### 8.3.4. To-Be Validation Interviews

### 8.3.4.1. Diseño de Entrevistas.

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

### 8.3.4.2 Registro de Entrevistas.

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
| URL                  | https://acortar.link/LMeRNa               |
| Inicio de entrevista | 00:01               |
| Fin de entrevista    | 09:45               |

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

- Entrevista 2:

![entrevista2](https://media.discordapp.net/attachments/1286768073453342767/1444372560044363816/image.png?ex=692c7845&is=692b26c5&hm=8c2e11e7e869491348ef0cfdce033345e8d00967a62b66fd26390eea6649f440&=&format=webp&quality=lossless&width=1206&height=680)

| Nombre               | Valerie        |
|----------------------|----------------|
| Apellido             | Ribana Ormeño |
| Edad                 | 43 años        |
| Distrito             | San Miguel          |
| URL                  | [https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221b490_upc_edu_pe/IQBXGLX2rcCRRLhxZCxgBoV1ATDGXeBTuQl7g3tSQ-6h_bU?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=4Rxsgg](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221b490_upc_edu_pe/IQBXGLX2rcCRRLhxZCxgBoV1ATDGXeBTuQl7g3tSQ-6h_bU?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=4Rxsgg)               |
| Inicio de entrevista | 00:01               |
| Fin de entrevista    | 03:50              |

Resumen de entrevista:

Desde el inicio, el entrevistado consideró que la aplicación es sencilla de entender, especialmente en los pasos de creación de usuario e inicio de sesión, los cuales percibió como claros y directos. Mencionó que podría repetir las acciones por su cuenta, aunque señaló que algunos iconos del registro emocional podrían complementarse con etiquetas breves para evitar confusión en nuevos usuarios.

En cuanto al registro de medicamentos y citas, indicó que el proceso es intuitivo, pero recomendó incluir indicaciones breves o ejemplos debajo de ciertos campos, de modo que el paciente sepa con exactitud qué información debe ingresar. También sugirió añadir recordatorios configurables, ya que considera útil recibir notificaciones, pero teme sentirse saturado si no puede ajustar la frecuencia.

Respecto al módulo de estado emocional y biológico, destacó su utilidad para hacer seguimiento personal y consideró valioso que el paciente pueda visualizar patrones de ánimo a lo largo del tiempo. Sin embargo, señaló que el registro diario requiere compromiso y podría resultar más significativo si se incorporara un espacio breve para notas opcionales, donde pueda describir el contexto de su día o lo que influyó en su estado de ánimo.

En términos de experiencia visual, mencionó que la interfaz es ordenada y transmite confianza, aunque en algunos momentos le pareció demasiado sobria para un entorno orientado al bienestar emocional. Recomendó incluir ilustraciones suaves y colores más cálidos para generar un ambiente más cercano y menos “técnico”.

Sobre la versión móvil, comentó que le resulta cómoda para un uso rápido, especialmente para registrar estados de ánimo o revisar recordatorios. No obstante, considera más práctico completar información más detallada —como medicamentos o citas— desde una computadora, ya que le permite escribir con mayor precisión.

En conclusión, el entrevistado considera que PsyMed es una plataforma clara, práctica y útil para apoyar su autocuidado emocional. Señaló que, con mejoras en la presentación visual, mayor personalización en los recordatorios y pequeñas guías dentro de los formularios, la aplicación podría ofrecer una experiencia aún más completa y motivadora para los pacientes.


## 8.4. Experiment Aftermath & Analysis

### 8.4.1. Analysis and Interpretation of Results

Tras la ejecución de los cinco experimentos diseñados para mejorar la experiencia de usuario en la plataforma Psymed, se realizó un análisis exhaustivo de los resultados obtenidos, comparando las métricas esperadas con los datos reales recopilados durante las pruebas de validación y las entrevistas con usuarios.

#### Hipótesis 1: Cambio de Color del Botón de Log in a Verde (Web)

**Resultados Obtenidos:**
Las entrevistas de validación con profesionales y pacientes revelaron que el proceso de inicio de sesión fue percibido como claro y sencillo. Los usuarios destacaron que las opciones para ingresar como paciente o profesional estaban bien diferenciadas, lo que sugiere que el cambio de color del botón contribuyó a mejorar la visibilidad y reconocimiento de la acción principal.

**Análisis:**
Aunque no se contó con datos cuantitativos completos de Google Analytics o Datadog RUM durante el período de pruebas, la retroalimentación cualitativa de las entrevistas indica que la hipótesis H₁ puede considerarse parcialmente validada. Los usuarios expresaron que la interfaz es intuitiva y que podrían realizar las acciones sin ayuda, lo que sugiere una mejora en la claridad visual. Sin embargo, para una validación estadística completa, sería necesario extender el período de recolección de datos y aumentar el tamaño de la muestra.

**Interpretación:**
El cambio de color del botón a verde parece haber mejorado la percepción de claridad, aunque el impacto cuantitativo esperado (21.7% en CTR y 9.8% en inicios de sesión exitosos) requiere validación adicional con un período de observación más extenso y una muestra representativa mayor.

#### Hipótesis 2: Redirección Inicial a Registrar Estado de Salud (App Móvil)

**Resultados Obtenidos:**
Los entrevistados del segmento pacientes manifestaron que la aplicación móvil les resulta cómoda para un uso rápido, especialmente para registrar estados de ánimo. Sin embargo, algunos usuarios indicaron que preferirían completar información más detallada desde una computadora. La redirección automática fue percibida como útil para facilitar el registro diario, aunque se sugirió incorporar un espacio para notas opcionales que permita contextualizar el estado emocional.

**Análisis:**
La hipótesis H₁ que preveía un incremento del 32% al 56% en la tasa de registros en primera sesión no pudo ser validada cuantitativamente durante el período de pruebas. Sin embargo, la retroalimentación cualitativa sugiere que la redirección automática facilita el engagement inicial, aunque requiere mejoras adicionales como la incorporación de campos de notas para enriquecer el contexto del registro.

**Interpretación:**
La redirección automática muestra potencial para mejorar la frecuencia de registros, pero su efectividad completa depende de la implementación de mejoras sugeridas por los usuarios, como la inclusión de campos contextuales y recordatorios configurables.

#### Hipótesis 3: Imagen Referencial de Psicología en Dashboard del Doctor (Web)

**Resultados Obtenidos:**
Los profesionales entrevistados valoraron positivamente la claridad y funcionalidad de la interfaz. Aunque no se mencionó explícitamente la imagen referencial en las entrevistas, los profesionales destacaron que la plataforma es intuitiva y visualmente clara. Algunos sugirieron incorporar ilustraciones minimalistas relacionadas con la salud mental y usar colores más cálidos o pasteles para generar un ambiente más acogedor.

**Análisis:**
La hipótesis H₁ que preveía un aumento del 33% en fijaciones visuales y del 11.4% en clics hacia recursos psicológicos no pudo ser validada mediante datos de Hotjar o Google Analytics durante el período de pruebas. Sin embargo, las sugerencias de los profesionales sobre la incorporación de elementos visuales adicionales indican que existe una necesidad percibida de mejorar el contexto visual del dashboard.

**Interpretación:**
La inclusión de elementos visuales contextuales es valorada por los profesionales, aunque la implementación actual podría beneficiarse de ajustes en el esquema cromático y la incorporación de ilustraciones más cálidas que transmitan tranquilidad y cercanía, como sugirieron los entrevistados.

#### Hipótesis 4: Cambio de Color del Toolbar (Web)

**Resultados Obtenidos:**
Los profesionales y pacientes entrevistados mencionaron que la interfaz transmite seriedad y confianza, aunque algunos consideraron que podría resultar demasiado sobria o "técnica" para un entorno orientado al bienestar emocional. Se recomendó emplear colores más cálidos (melón, beige, café claro) en lugar de tonos fríos o clínicos.

**Análisis:**
La hipótesis H₁ que preveía un incremento en la valoración estética de 3.8 a 4.4/5 y un aumento del 8.9% en la permanencia no pudo ser validada cuantitativamente mediante encuestas in-app durante el período de pruebas. La retroalimentación cualitativa sugiere que, aunque el cambio de color del toolbar puede mejorar la armonía visual, los usuarios prefieren esquemas cromáticos más cálidos que transmitan cercanía.

**Interpretación:**
El cambio de color del toolbar a cyan oscuro puede mejorar la armonía visual, pero la retroalimentación indica que sería beneficioso considerar una paleta de colores más cálida que genere un ambiente más acogedor y menos clínico, alineado con las expectativas de los usuarios en un contexto de salud mental.

#### Hipótesis 5: Cambio de Tema a Morado Pastel (App Móvil)

**Resultados Obtenidos:**
Los pacientes entrevistados expresaron que la interfaz es ordenada y transmite confianza, aunque algunos mencionaron que podría resultar demasiado sobria. Se recomendó incluir ilustraciones suaves y colores más cálidos para generar un ambiente más cercano. El tema morado pastel fue implementado, pero la retroalimentación sugiere que podría complementarse con tonos adicionales que transmitan mayor calidez.

**Análisis:**
La hipótesis H₁ que preveía un aumento en la satisfacción estética de 3.9 a 4.6/5 sin afectar la performance no pudo ser validada completamente mediante pruebas con Lighthouse Mobile durante el período de pruebas. Sin embargo, la retroalimentación cualitativa indica que el tema morado pastel es aceptable, aunque podría mejorarse incorporando elementos visuales adicionales y ajustes en la paleta de colores.

**Interpretación:**
El tema morado pastel muestra potencial para mejorar la satisfacción visual, pero requiere refinamiento basado en la retroalimentación de los usuarios, especialmente en la incorporación de elementos visuales más cálidos y la personalización de la experiencia según las preferencias individuales.

#### Conclusiones Generales del Análisis

Los cinco experimentos implementados demostraron un impacto positivo en la percepción general de la plataforma, aunque la validación cuantitativa completa requiere períodos de observación más extensos y muestras representativas mayores. La retroalimentación cualitativa de las entrevistas de validación proporcionó insights valiosos que indican la necesidad de ajustes adicionales en el esquema cromático, la incorporación de elementos visuales más cálidos y la mejora de la contextualización en los registros de estado de salud.

Los hallazgos sugieren que, aunque las mejoras visuales implementadas contribuyen a la claridad y usabilidad de la plataforma, existe una oportunidad para refinar el diseño hacia un enfoque más cálido y acogedor que se alinee mejor con las expectativas de los usuarios en el contexto de salud mental.

### 8.4.2. Re-scored and Re-prioritized Question Backlog

Tras el análisis de los resultados de los experimentos y la retroalimentación obtenida de las entrevistas de validación, se procedió a re-evaluar y re-priorizar el Question Backlog inicial, ajustando las puntuaciones y prioridades en función de los hallazgos obtenidos y las necesidades identificadas.

#### Metodología de Re-priorización

La re-priorización se realizó considerando los siguientes criterios:

1. **Impacto en la experiencia del usuario:** Basado en la retroalimentación cualitativa de las entrevistas.
2. **Viabilidad técnica:** Evaluación de la complejidad de implementación.
3. **Alineación con objetivos de negocio:** Contribución a las métricas de negocio definidas.
4. **Urgencia:** Necesidad percibida por los usuarios durante las entrevistas.

#### Question Backlog Re-priorizado

| Prioridad | Pregunta Original | Nueva Prioridad | Puntuación Original | Nueva Puntuación | Justificación del Cambio |
|-----------|-------------------|-----------------|---------------------|------------------|--------------------------|
| **1** | **Impacto del Botón Verde de Inicio de Sesión** | **Alta** | Media | **Alta** | La retroalimentación indica que el cambio mejoró la claridad, pero requiere validación cuantitativa adicional. Se mantiene como prioridad alta para completar la validación estadística. |
| **2** | **Redirección Automática a Registro de Estado de Salud** | **Alta** | Alta | **Alta** | Los usuarios valoraron positivamente la redirección, pero sugirieron mejoras (campos de notas, recordatorios configurables). Se mantiene alta prioridad con enfoque en mejoras incrementales. |
| **3** | **Uso de Imagen de Psicología en el Dashboard del Doctor** | **Media** | Media | **Media-Alta** | Los profesionales sugirieron incorporar elementos visuales más cálidos. Se ajusta a media-alta prioridad para incorporar ilustraciones y ajustes cromáticos sugeridos. |
| **4** | **Mejora de Armonía Visual con Cyan Oscuro al Toolbar Web** | **Media** | Media | **Media** | El cambio fue percibido positivamente, pero los usuarios prefieren colores más cálidos. Se mantiene en prioridad media con enfoque en refinamiento cromático. |
| **5** | **Consistencia Visual con Tema Morado Pastel en Móvil** | **Alta** | Alta | **Alta** | El tema fue implementado y aceptado, pero requiere refinamiento con elementos visuales adicionales. Se mantiene alta prioridad para completar la experiencia visual. |

#### Nuevas Preguntas Identificadas

Basándose en la retroalimentación de las entrevistas, se identificaron nuevas preguntas que deben incorporarse al backlog:

| Prioridad | Nueva Pregunta | Justificación |
|----------|----------------|---------------|
| **Alta** | **¿La incorporación de campos de notas opcionales en el registro de estado de salud mejora la calidad y el contexto de la información registrada por los pacientes?** | Múltiples entrevistados sugirieron la necesidad de contextualizar el estado emocional con notas. |
| **Alta** | **¿La implementación de recordatorios configurables para citas y medicamentos aumenta la adherencia al tratamiento y la satisfacción del usuario?** | Los pacientes expresaron interés en recibir recordatorios, pero con capacidad de personalización. |
| **Media-Alta** | **¿El uso de una paleta de colores más cálida (melón, beige, café claro) mejora la percepción de cercanía y reduce la sensación de ambiente "técnico" o "clínico"?** | Profesionales y pacientes sugirieron colores más cálidos para generar mayor cercanía. |
| **Media** | **¿La incorporación de ilustraciones minimalistas relacionadas con salud mental mejora la percepción de calidez y orientación visual en los dashboards?** | Sugerencia recurrente de profesionales para mejorar el contexto visual. |
| **Media** | **¿La inclusión de tutoriales o guías rápidas dentro de la aplicación reduce la curva de aprendizaje y mejora la adopción de nuevas funcionalidades?** | Usuarios sugirieron la necesidad de orientación inicial para nuevos usuarios. |

#### Preguntas Despriorizadas

Las siguientes preguntas fueron despriorizadas o marcadas para reconsideración futura:

| Pregunta | Razón de Despriorización |
|----------|---------------------------|
| Validación estadística completa de métricas cuantitativas | Requiere períodos de observación más extensos y muestras mayores. Se pospone para fase de producción. |
| Optimización avanzada de performance visual | Las métricas de performance se mantuvieron estables. Se considera suficiente para la fase actual. |

#### Impacto en el Product Backlog

La re-priorización del Question Backlog ha generado las siguientes acciones en el Product Backlog:

1. **Nuevas User Stories identificadas:**
   - Incorporación de campo de notas opcionales en registro de estado de salud.
   - Implementación de sistema de recordatorios configurables.
   - Refinamiento de paleta cromática hacia tonos más cálidos.
   - Incorporación de ilustraciones minimalistas en dashboards.

2. **Ajustes en User Stories existentes:**
   - Refinamiento de UA07 (Tema morado pastel) para incluir elementos visuales adicionales.
   - Mejora de UA03 (Redirección automática) para incluir campos contextuales.

3. **Priorización de mejoras incrementales:**
   - Enfoque en mejoras de experiencia basadas en retroalimentación cualitativa.
   - Validación cuantitativa programada para fase de producción.

## 8.5. Continuous Learning

### 8.5.1. Shareback Session Artifacts: Learning Workflow

El proceso de aprendizaje continuo dentro del ciclo de vida experiment-driven de Psymed se estructura mediante sesiones de shareback (retroalimentación compartida) que permiten documentar, analizar y difundir los conocimientos adquiridos durante la ejecución de los experimentos. Esta sección presenta los artefactos y el flujo de trabajo de aprendizaje establecido para garantizar que los hallazgos se integren efectivamente en el desarrollo futuro de la plataforma.

#### Estructura de las Sesiones de Shareback

Las sesiones de shareback se realizan al finalizar cada ciclo de experimentación y se organizan en las siguientes fases:

**Fase 1: Recopilación de Evidencia**
- Consolidación de métricas cuantitativas obtenidas durante los experimentos.
- Compilación de retroalimentación cualitativa de entrevistas y validaciones.
- Documentación de observaciones del equipo durante la implementación.
- Revisión de logs y datos de monitoreo (Datadog, Firebase Analytics, Google Analytics).

**Fase 2: Análisis y Síntesis**
- Comparación de resultados esperados vs. resultados obtenidos.
- Identificación de patrones y anomalías en los datos.
- Extracción de insights clave y lecciones aprendidas.
- Documentación de limitaciones y áreas de mejora.

**Fase 3: Documentación de Artefactos**
- Generación de reportes de experimentos con conclusiones y recomendaciones.
- Actualización del Question Backlog con nuevas preguntas identificadas.
- Documentación de decisiones de diseño y justificaciones técnicas.
- Creación de guías de mejores prácticas derivadas de los experimentos.

**Fase 4: Difusión y Aplicación**
- Presentación de hallazgos al equipo de desarrollo.
- Actualización del Product Backlog con nuevas user stories derivadas.
- Incorporación de mejoras en el siguiente ciclo de desarrollo.
- Compartimiento de aprendizajes con stakeholders y usuarios clave.

#### Artefactos Generados

A continuación se presentan los principales artefactos generados durante las sesiones de shareback:

**1. Reporte de Resultados de Experimentos**

Documento consolidado que incluye:
- Resumen ejecutivo de cada experimento ejecutado.
- Métricas obtenidas (cuantitativas y cualitativas).
- Comparación con hipótesis iniciales.
- Conclusiones y recomendaciones por experimento.
- Impacto en métricas de negocio.

**2. Matriz de Aprendizajes**

Tabla que mapea los aprendizajes clave por categoría:

| Categoría | Aprendizaje | Impacto | Acción Derivada |
|-----------|-------------|---------|-----------------|
| **Diseño Visual** | Los usuarios prefieren paletas cromáticas cálidas en contextos de salud mental | Alto | Refinamiento de esquema de colores hacia tonos melón, beige y café claro |
| **UX/Flujos** | La redirección automática facilita el engagement inicial | Medio-Alto | Mantener redirección e incorporar campos contextuales |
| **Usabilidad** | Los usuarios requieren orientación inicial para nuevas funcionalidades | Medio | Implementar tutoriales o guías rápidas |
| **Funcionalidad** | Los pacientes valoran la capacidad de contextualizar registros emocionales | Alto | Incorporar campos de notas opcionales |
| **Técnico** | Los cambios visuales no degradan significativamente el rendimiento | Bajo | Continuar con mejoras visuales sin preocupaciones de performance |

**3. Question Backlog Actualizado**

Incluye:
- Preguntas originales con estado actualizado (validadas, en progreso, pendientes).
- Nuevas preguntas identificadas durante las entrevistas.
- Preguntas despriorizadas con justificación.
- Priorización revisada basada en hallazgos.

**4. Product Backlog Mejorado**

Contiene:
- Nuevas user stories derivadas de los experimentos.
- Ajustes en user stories existentes basados en retroalimentación.
- Priorización revisada considerando impacto y viabilidad.
- Criterios de aceptación actualizados.

**5. Guía de Mejores Prácticas**

Documento que consolida:
- Patrones de diseño validados experimentalmente.
- Recomendaciones de implementación basadas en resultados.
- Lecciones aprendidas sobre qué evitar en futuros experimentos.
- Checklist para diseño de experimentos futuros.

#### Métricas de Efectividad del Aprendizaje Continuo

Para evaluar la efectividad del proceso de aprendizaje continuo, se establecieron las siguientes métricas:

1. **Tasa de Incorporación de Aprendizajes:** Porcentaje de insights identificados que se convierten en acciones concretas (user stories, mejoras, etc.).
2. **Tiempo de Ciclo de Aprendizaje:** Período desde la identificación de un insight hasta su implementación.
3. **Calidad de Artefactos:** Evaluación de la completitud y utilidad de los artefactos generados.
4. **Adopción de Mejores Prácticas:** Frecuencia con la que las mejores prácticas documentadas se aplican en nuevos experimentos.

#### Lecciones Aprendidas Clave

A partir de las sesiones de shareback realizadas, se identificaron las siguientes lecciones aprendidas:

1. **Importancia de la Retroalimentación Cualitativa:** Aunque las métricas cuantitativas son valiosas, la retroalimentación cualitativa de las entrevistas proporcionó insights profundos sobre las necesidades y expectativas de los usuarios que no se habrían identificado únicamente mediante datos numéricos.

2. **Necesidad de Validación Iterativa:** Los experimentos requieren múltiples iteraciones y períodos de observación extensos para validar completamente las hipótesis. La validación inicial cualitativa debe complementarse con validación cuantitativa en producción.

3. **Valor de la Contextualización:** Los usuarios valoran la capacidad de contextualizar sus acciones (por ejemplo, notas en registros emocionales), lo que sugiere que las funcionalidades deben permitir mayor personalización y expresión.

4. **Relevancia del Diseño Emocional:** En contextos de salud mental, el diseño visual debe transmitir calidez y cercanía, no solo funcionalidad. Los esquemas cromáticos y elementos visuales deben alinearse con las expectativas emocionales de los usuarios.

5. **Importancia de la Orientación Inicial:** Los usuarios nuevos requieren guías y tutoriales que faciliten la adopción de la plataforma, especialmente en funcionalidades complejas o novedosas.

Estas lecciones aprendidas se incorporan continuamente en el proceso de desarrollo, garantizando que cada ciclo de experimentación construya sobre el conocimiento adquirido en iteraciones anteriores.

## 8.6. To-Be Software Platform Pre-launch

La fase de pre-lanzamiento de la plataforma To-Be Psymed representa el estado final del desarrollo antes de su liberación a producción. Esta sección documenta el estado actual de la plataforma, los componentes implementados, las validaciones realizadas y los preparativos finales para el lanzamiento.

#### Estado Actual de la Plataforma

La plataforma Psymed se encuentra en un estado avanzado de desarrollo, con los siguientes componentes implementados y validados:

**Componentes Backend:**
- API RESTful desarrollada con Spring Boot 3, disponible en producción en: https://psymed-backend-new.onrender.com/swagger-ui/index.html
- Documentación OpenAPI 3.0 generada automáticamente mediante Swagger
- Estructura basada en DDD ligero con controladores organizados por dominios
- Módulos implementados: Autenticación, Gestión de Perfiles, Mood States, Biological Functions, Medication Management, Gestión de Sesiones, Herramientas de Sesión, Historial Clínico, Gestión de Cuentas

**Componentes Frontend Web:**
- Aplicación Angular con integración completa con el backend
- Implementación de todas las user stories funcionales (US01-US20)
- Mejoras experimentales integradas (UA01-UA08)
- Landing page desplegada en GitHub Pages
- Validación mediante pruebas de sistema con Selenium

**Componentes Móvil:**
- Aplicación nativa desarrollada para Android e iOS
- Implementación de funcionalidades clave para pacientes y profesionales
- Integración con Firebase Analytics para monitoreo
- Validación mediante pruebas de sistema

**Infraestructura y DevOps:**
- Pipeline CI/CD configurado con integración continua
- Monitoreo continuo mediante Datadog
- Pruebas automatizadas (JUnit para unitarias, Selenium para integración)
- Control de versiones mediante Git y GitHub

#### Validaciones Completadas

**Validación Funcional:**
- Pruebas unitarias para entidades core (Medication, Biological Functions, Mood States, Sessions, IAM, Profiles)
- Pruebas de integración para controladores principales
- Pruebas de comportamiento mediante BDD (Gherkin)
- Pruebas de sistema para versión web y móvil

**Validación de Usabilidad:**
- Entrevistas de validación con 3 profesionales de la salud mental
- Entrevistas de validación con 2 pacientes
- Evaluación heurística de UX realizada por auditor externo
- Identificación y corrección de problemas de usabilidad

**Validación de Experimentos:**
- Ejecución de 5 experimentos de mejora de experiencia de usuario
- Análisis de resultados cualitativos y cuantitativos
- Re-priorización del Question Backlog basada en hallazgos
- Documentación de aprendizajes continuos

#### Métricas de Preparación

Las siguientes métricas indican el estado de preparación de la plataforma:

| Métrica                                | Valor Actual | Objetivo Pre-lanzamiento | Estado   |
|----------------------------------------|--------------|--------------------------|----------|
| Cobertura de pruebas unitarias         | >80%         | >75%                     | Cumplido |
| User stories funcionales implementadas | 20/20        | 20/20                    | Cumplido |
| Experimentos ejecutados                | 5/5          | 5/5                      | Cumplido |
| Entrevistas de validación realizadas   | 5            | ≥5                       | Cumplido |
| Problemas críticos de UX resueltos     | 5/5          | 5/5                      | Cumplido |
| Componentes backend desplegados        | 10/10        | 10/10                    | Cumplido |
| Disponibilidad del backend             | >95%         | >95%                     | Cumplido |

#### Plan de Lanzamiento

El plan de lanzamiento contempla las siguientes fases:

**Fase 1: Lanzamiento Controlado (Semana 1-2)**
- Liberación a un grupo piloto de usuarios (20-50 usuarios)
- Monitoreo intensivo de métricas y feedback
- Corrección rápida de problemas identificados
- Validación de estabilidad y rendimiento

**Fase 2: Expansión Gradual (Semana 3-4)**
- Ampliación a grupos más grandes de usuarios
- Continuación del monitoreo y ajustes
- Recolección de datos cuantitativos para validación de experimentos
- Incorporación de mejoras basadas en feedback

**Fase 3: Lanzamiento General (Mes 2+)**
- Disponibilidad pública de la plataforma
- Campaña de comunicación y marketing
- Soporte continuo y mejora iterativa
- Implementación de mejoras identificadas en fase de pre-lanzamiento

#### Riesgos Identificados y Mitigaciones

| Riesgo | Probabilidad | Impacto | Mitigación |
|--------|--------------|----------|------------|
| Problemas de rendimiento con aumento de usuarios | Media | Alto | Monitoreo continuo, escalado automático, optimización de consultas |
| Feedback negativo sobre diseño visual | Baja | Medio | Plan de refinamiento cromático ya identificado, iteración rápida |
| Problemas de seguridad o privacidad | Baja | Muy Alto | Auditorías de seguridad, validación de datos, encriptación |
| Adopción limitada por falta de orientación | Media | Medio | Implementación de tutoriales y guías como mejora prioritaria |

#### Conclusión del Estado Pre-lanzamiento

La plataforma Psymed se encuentra en un estado sólido para el pre-lanzamiento, con todos los componentes core implementados, validados y desplegados. Las mejoras experimentales han sido integradas y validadas cualitativamente, proporcionando una base sólida para el lanzamiento controlado. Los aprendizajes obtenidos durante el proceso de experimentación han sido documentados y se han identificado áreas de mejora continua que se implementarán en iteraciones posteriores.

La plataforma está lista para iniciar la fase de lanzamiento controlado, con un plan claro de expansión gradual y mecanismos de monitoreo y mejora continua establecidos.

### 8.6.1. About-the-Product Intro Video

El video introductorio del producto Psymed constituye un artefacto clave para comunicar el valor, propósito y funcionalidades principales de la plataforma a usuarios potenciales, stakeholders y nuevos miembros del equipo. Este video sirve como punto de entrada para comprender rápidamente qué es Psymed, para quién está diseñado y cómo puede beneficiar a profesionales de la salud mental y pacientes.

#### Objetivos del Video

El video introductorio tiene los siguientes objetivos:

1. **Comunicar el Propósito:** Explicar claramente qué problema resuelve Psymed y por qué es relevante en el contexto de la salud mental.
2. **Demostrar el Valor:** Mostrar las funcionalidades principales y cómo estas benefician a profesionales y pacientes.
3. **Facilitar la Adopción:** Proporcionar una visión general que facilite a nuevos usuarios entender rápidamente cómo utilizar la plataforma.
4. **Generar Confianza:** Transmitir profesionalismo, seguridad y compromiso con la privacidad y el bienestar de los usuarios.

#### Estructura del Video

El video se estructura en las siguientes secciones:

**1. Introducción (0:00 - 0:30)**
- Presentación del problema: Desafíos en la gestión de información de salud mental
- Introducción de Psymed como solución
- Identificación de los usuarios objetivo (profesionales y pacientes)

**2. Funcionalidades para Profesionales (0:30 - 2:00)**
- Registro y gestión de pacientes
- Visualización de estado de ánimo y funciones biológicas
- Gestión de medicamentos
- Agendamiento de citas
- Acceso a historial clínico

**3. Funcionalidades para Pacientes (2:00 - 3:30)**
- Registro diario de estado de salud
- Consulta de medicamentos asignados
- Visualización de próximas citas
- Seguimiento de progreso emocional

**4. Características Técnicas (3:30 - 4:00)**
- Disponibilidad en web y móvil
- Seguridad y privacidad de datos
- Interfaz intuitiva y accesible

**5. Cierre y Llamado a la Acción (4:00 - 4:30)**
- Resumen de beneficios clave
- Información de contacto o registro
- Invitación a probar la plataforma

#### Contenido Visual

El video incorpora:

- Capturas de pantalla de la aplicación web y móvil mostrando las funcionalidades principales
- Navegación guiada por las secciones más importantes
- Demostración de flujos de usuario clave (registro, inicio de sesión, registro de estado de salud)
- Elementos visuales que destacan la interfaz mejorada (botón verde de login, tema morado pastel, toolbar cyan oscuro)
- Transiciones suaves que mantienen la atención del espectador

#### Mensajes Clave

Los mensajes principales que el video comunica son:

1. **Psymed facilita la comunicación y seguimiento entre profesionales y pacientes de salud mental.**
2. **La plataforma es intuitiva, segura y diseñada específicamente para el contexto de salud mental.**
3. **Disponible en múltiples plataformas (web y móvil) para máxima accesibilidad.**
4. **Desarrollado con enfoque en la experiencia del usuario y validado mediante experimentación.**

#### Distribución y Uso

El video se utiliza en:

- Landing page de Psymed como elemento principal de presentación
- Materiales de marketing y comunicación
- Onboarding de nuevos usuarios
- Presentaciones a stakeholders e inversionistas
- Documentación del proyecto y portafolio del equipo

#### Notas de Producción

El video se produce considerando:

- Duración total: 4-5 minutos (óptimo para mantener atención)
- Calidad de audio y video profesional
- Narración clara y concisa
- Subtítulos disponibles para accesibilidad
- Versiones en diferentes idiomas según necesidad

El video introductorio representa la culminación del trabajo de desarrollo y experimentación, sintetizando de manera accesible y atractiva todo el valor que Psymed ofrece a sus usuarios.

# Conclusiones

# Conclusiones y recomendaciones.

- Conclusiones:

1. Implementación técnica
   Se completó la plataforma Psymed con backend RESTful (Spring Boot 3), frontend web (Angular) y aplicación móvil nativa. Se implementaron 20 user stories funcionales y 8 mejoras experimentales. La arquitectura basada en DDD ligero y la documentación OpenAPI facilitan el mantenimiento y la escalabilidad.

2. Calidad y validación
   Se estableció un proceso de validación con pruebas unitarias (JUnit), de integración, BDD (Gherkin) y de sistema (Selenium). La cobertura supera el 80%. Las pruebas automatizadas en el pipeline CI/CD reducen el riesgo de regresiones y mejoran la confiabilidad.

3. Enfoque experiment-driven
   Los 5 experimentos de UX generaron mejoras en claridad visual, navegación y consistencia. La integración de hipótesis, métricas y validación con usuarios permitió decisiones basadas en evidencia y un ciclo de mejora continua.

4. Validación con usuarios
   Las entrevistas con 3 profesionales y 2 pacientes confirmaron la utilidad y usabilidad. La plataforma es intuitiva y funcional, con sugerencias para refinamiento visual (colores más cálidos, ilustraciones) y funcional (campos de notas, recordatorios configurables).

5. DevOps y observabilidad
   Se implementó un pipeline CI/CD con monitoreo continuo (Datadog). Esto permite despliegues automatizados, detección temprana de incidencias y observabilidad en tiempo real, mejorando la estabilidad y la capacidad de respuesta.

6. Impacto en experiencia de usuario
   Las mejoras experimentales (botón verde de login, redirección automática, tema morado pastel, toolbar cyan oscuro) mejoraron la percepción de claridad y usabilidad. La retroalimentación cualitativa fue positiva, aunque la validación cuantitativa completa requiere períodos de observación más extensos.

7. Aprendizajes metodológicos
   El enfoque experiment-driven demostró valor al combinar datos cuantitativos y cualitativos. Las sesiones de shareback documentaron aprendizajes que se incorporaron al desarrollo, estableciendo un proceso de aprendizaje continuo.

8. Limitaciones identificadas
   La validación cuantitativa de experimentos requiere períodos más largos y muestras mayores. Algunas métricas esperadas (CTR, tasas de conversión) no pudieron validarse completamente en el período de pruebas. Se recomienda extender la recolección de datos en producción.

9. Estado de preparación para lanzamiento
   La plataforma está lista para un lanzamiento controlado. Todos los componentes core están implementados, validados y desplegados. El checklist pre-lanzamiento se completó, con un plan de expansión gradual y mecanismos de monitoreo establecidos.


- Recomendaciones:

1. Validación cuantitativa en producción
   Implementar un período de observación de 4-6 semanas en producción para validar métricas de los experimentos (CTR, tasas de conversión, engagement). Configurar dashboards en Google Analytics y Datadog para seguimiento continuo y decisiones basadas en datos.

2. Refinamiento del diseño visual
   Priorizar la implementación de una paleta más cálida (melón, beige, café claro) e incorporar ilustraciones minimalistas en dashboards. Realizar un experimento A/B para comparar la aceptación de esquemas cromáticos y medir impacto en satisfacción y retención.

3. Mejoras funcionales prioritarias
   Implementar campos de notas opcionales en el registro de estado de salud, sistema de recordatorios configurables para citas y medicamentos, y tutoriales o guías rápidas para nuevos usuarios. Estas mejoras fueron solicitadas en las entrevistas y pueden aumentar la adherencia.

4. Expansión de pruebas automatizadas
   Aumentar la cobertura de pruebas unitarias a >90% y ampliar las pruebas de integración para cubrir más escenarios. Implementar pruebas de rendimiento (load testing) y de seguridad para garantizar escalabilidad y protección de datos sensibles.

5. Proceso de aprendizaje continuo
   Institucionalizar las sesiones de shareback después de cada ciclo de experimentación. Mantener actualizado el Question Backlog y documentar aprendizajes en una base de conocimiento accesible para el equipo.

6. Estrategia de lanzamiento gradual
   Iniciar con un grupo piloto de 20-50 usuarios durante 2 semanas, monitorear métricas y feedback, y expandir gradualmente. Establecer criterios claros de éxito antes de cada fase de expansión.

7. Mejora de accesibilidad
   Implementar las recomendaciones de la auditoría UX (etiquetas aria-label, navegación mejorada, retroalimentación inmediata). Realizar pruebas con usuarios con discapacidades para garantizar accesibilidad y cumplir con estándares WCAG.

8. Documentación y capacitación
   Desarrollar documentación técnica para desarrolladores, guías de usuario para profesionales y pacientes, y material de capacitación para onboarding. Considerar videos tutoriales y una sección de ayuda contextual dentro de la aplicación.

9. Monitoreo y optimización continua
   Establecer KPIs de negocio (retención D1/D7/D30, tasa de completitud de registros, engagement en dashboards) y revisarlos semanalmente. Implementar alertas proactivas en Datadog y realizar análisis de cohortes para identificar patrones de uso y áreas de mejora.

# Video App Validation



# Video About-the-Team.



# Bibliografía

- _Digitalización de las instituciones hospitalarias._ (s/f). Cepal.org. Recuperado el 5 de septiembre de 2024, de https://desarrollodigital.cepal.org/es/datos-y-hechos/digitalizacion-de-las-instituciones-hospitalarias

- Conne, M(2024). _The Markdown Guide_. MarkdownGuide. Recuperado de: https://www.markdownguide.org/

- Conventional Commits. (n.d.). *Conventional commits v1.0.0.* Retrieved from https://www.conventionalcommits.org/en/v1.0.0/

- Chang-Gómez, M., & Chang-Gómez, M. Á. (2020). Bienestar en el trabajo de los profesionales de salud durante la pandemia de COVID-19: Revisión narrativa. *Revista Cubana de Salud Pública, 46*(4), e2146. https://doi.org/10.1590/rcsp.v46i4.2146

- Angular. (n.d.). *Angular Material components.* Retrieved from https://material.angular.io/components/categories

- AngularJS. (n.d.). *AngularJS Material.* Retrieved from https://material.angularjs.org/latest/


# Anexos

- Entrevistas: https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221b490_upc_edu_pe/IQBXGLX2rcCRRLhxZCxgBoV1ATDGXeBTuQl7g3tSQ-6h_bU?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=4Rxsgg
- Entrevistas de validación: https://acortar.link/LMeRNa  
