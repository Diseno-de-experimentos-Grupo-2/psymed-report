# Capítulo VII: DevOpsPractices
## 7.1 Continuous Integration
### 7.1.1 Tools and Practices.

#### Herramientas:

- Git como sistema de control de versiones distribuido.
- Repositorio centralizado en GitHub.
  
#### Prácticas:

- Realizar commits frecuentes y bien documentados.
- Uso de ramas (main, develop) siguiendo Git Flow o un flujo simplificado.
- Revisión de código mediante pull requests o merge requests.
- Integración de cambios frecuentes para evitar conflictos y asegurar la trazabilidad.

<img width="1125" height="417" alt="image" src="https://github.com/user-attachments/assets/95b60fd6-67b9-4674-bcf9-13df4818aa0d" />

### 7.1.2 Build & Test Suite Pipelines Components.

Dentro del pipeline de integración continua se incorporaron pruebas automatizadas en diferentes niveles para asegurar la calidad del software. En particular, se empleó JUnit para la ejecución de pruebas unitarias, verificando el correcto funcionamiento de componentes individuales de la aplicación. Asimismo, se utilizó Selenium para la realización de pruebas integrales, con el fin de validar la interacción entre módulos y garantizar la experiencia del usuario en un entorno simulado.

<img width="224" height="224" alt="image" src="https://github.com/user-attachments/assets/c7180300-7de5-44c9-b902-00d44b0c89a4" />   <img width="220" height="230" alt="image" src="https://github.com/user-attachments/assets/0a66b4a1-b6e2-432c-af83-44b5406c648c" />


## 7.2 Continuous Delivery
### 7.2.1 Tools and Practices.

**JUnit:** Es una herramienta ampliamente utilizada en entornos Java para la ejecución de pruebas unitarias. Su elección se debe a la necesidad de validar de manera automática y rápida el correcto funcionamiento de los componentes individuales del sistema. JUnit permite detectar errores en fases tempranas del desarrollo, lo que contribuye a mejorar la calidad del software y reducir costos de corrección en etapas posteriores. Además, se integra fácilmente en pipelines de CI/CD, facilitando su automatización.

**Selenium:** Se emplea para la automatización de pruebas integrales y funcionales a nivel de interfaz de usuario. Con Selenium es posible simular la interacción real de un usuario con la aplicación, verificando que el sistema responda adecuadamente a distintos escenarios. Esta práctica garantiza que las distintas partes del software trabajen de manera conjunta y que la experiencia del usuario final sea consistente.

En conjunto, el uso de JUnit y Selenium asegura que tanto la lógica interna como el comportamiento externo de la aplicación se validen continuamente, lo que mejora la confiabilidad del sistema en cada ciclo de entrega.

### 7.2.2 Stages Deployment Pipeline Components.

El pipeline de Continuous Delivery se estructura en diferentes etapas que permiten validar la calidad y preparación del software antes de su liberación en producción:

**- Stage 1:** Compilación y Construcción (Build). El código fuente es compilado y se generan los artefactos listos para ser evaluados.

**- Stage 2:** Pruebas Unitarias (JUnit). Se ejecutan pruebas automatizadas con JUnit para validar el correcto funcionamiento de los componentes individuales de la aplicación.

**- Stage 3:** Pruebas Integrales (Selenium). Se aplican pruebas de integración y funcionalidad mediante Selenium, simulando la interacción de los usuarios con la interfaz.

**- Stage 4:** Entorno de Preproducción (Staging). Los artefactos validados se despliegan en un entorno intermedio para su verificación en condiciones similares a producción.

**- Stage 5:** Validación por Usuarios (UAT). Se permite la revisión por parte de usuarios o stakeholders clave antes de la liberación final.

**- Stage 6:** Preparación de Release. Se genera la versión final lista para producción, empaquetada y versionada según los lineamientos establecidos.

## 7.3 Continuous deployment

El Continuous Deployment consiste en la capacidad de publicar de forma continua y completamente automatizada nuevas versiones del software directamente en el entorno de producción. Bajo este enfoque, cada modificación realizada al código atraviesa un proceso de validación y pruebas automatizadas; en caso de superar satisfactoriamente dichas verificaciones, la aplicación es desplegada de manera inmediata sin requerir intervención manual. Este mecanismo posibilita una entrega ágil y frecuente de nuevas funcionalidades y correcciones, favoreciendo la rápida evolución del sistema y la respuesta oportuna a las necesidades de los usuarios.

### 7.3.1 Tool and Practices.

Dentro del enfoque de Continuous Deployment se consideran diversas herramientas y prácticas esenciales para garantizar la confiabilidad y la automatización del proceso:

**a. Sistema de Control de Versiones:** Se emplea Git como herramienta principal para gestionar y dar seguimiento a los cambios en el código fuente.

**b. Automatización de Pruebas:** Se implementan pruebas automatizadas —unitarias, de integración y de regresión— con el objetivo de verificar la calidad del software antes de su liberación.

**c. Entornos Consistentes:** Se mantienen entornos de desarrollo y prueba que reproducen de forma cercana las condiciones del entorno productivo, reduciendo riesgos durante el despliegue.

**d. Pipeline de Despliegue Automatizado:** Se define un flujo de despliegue que contempla fases como compilación, pruebas, despliegue en staging y despliegue en producción.

**e. Supervisión y Retroalimentación:** Se incorporan mecanismos de monitoreo y registro (logging) que permiten observar el rendimiento y la estabilidad de la aplicación en tiempo real, facilitando la detección temprana de incidencias y la toma de decisiones rápidas.

### 7.3.2 Production Deployment Pipeline Components.

Los elementos fundamentales de un pipeline orientado al despliegue en producción son los siguientes:

**a. Construcción (Build):** Se compila el código fuente y se generan los artefactos listos para ser distribuidos en el entorno productivo.

**b. Validación (Testing):** Se ejecutan pruebas automatizadas con el fin de asegurar que la aplicación cumple los criterios de calidad establecidos y que no se introducen fallos no previstos.

**c. Entorno de Preproducción (Staging):** Antes del despliegue definitivo, la solución se implementa en un ambiente intermedio para la realización de pruebas adicionales y validación por parte de un grupo reducido de usuarios.

**d. Implementación en Producción (Production Deployment):** Se lleva a cabo el despliegue automático de los artefactos en el entorno productivo.

**e. Supervisión Continua (Continuous Monitoring):** Una vez desplegada, la aplicación es monitoreada de manera constante para garantizar su rendimiento, disponibilidad y estabilidad, atendiendo incidentes en tiempo real.

**f. Reversión (Rollback):** Ante la detección de fallas críticas, el pipeline contempla mecanismos de reversión inmediata hacia una versión previa estable de la aplicación.

## 7.4. Continuous Monitoring

El Continuous Monitoring se refiere a la supervisión constante del comportamiento, rendimiento y disponibilidad de la aplicación una vez desplegada, con el fin de detectar incidentes de manera temprana y garantizar su correcto funcionamiento en el entorno productivo. Esta práctica forma parte esencial del ciclo DevOps, ya que permite obtener retroalimentación continua sobre el estado del sistema y facilita la toma de decisiones rápidas para mantener la calidad del servicio.

### 7.4.1. Tools and Practices

Para el monitoreo continuo de la aplicación en producción se utiliza Datadog, una plataforma unificada que permite observar métricas, logs y trazas en tiempo real. Esto facilita la detección temprana de incidencias y el análisis del rendimiento del sistema.

**Herramienta Principal:**

- **Datadog**: Plataforma de observabilidad que integra monitoreo de infraestructura, análisis de logs, trazabilidad de servicios y generación de alertas en un solo entorno.

**Prácticas Aplicadas:**

- Configuración de métricas de uso de recursos (CPU, memoria, latencia, throughput).
- Recolección centralizada de logs para diagnóstico y auditoría.
- Definición de paneles de visualización (dashboards) para el análisis continuo.
- Establecimiento de umbrales y reglas automáticas de alertas.
- Revisión periódica de tendencias para mejorar rendimiento y estabilidad.

### 7.4.2. Monitoring Pipeline Components

El pipeline de monitoreo continuo con Datadog se organiza en las siguientes etapas:

|Etapa	| Descripción |
|-------|-------------|
| Instrumentación	| La aplicación es configurada para enviar métricas y logs hacia Datadog.|
| Recolección |	Datadog recibe datos en tiempo real desde la aplicación y la infraestructura.|
| Procesamiento y Análisis |	Los datos se clasifican automáticamente y se correlacionan entre servicios.|
| Visualización	| Se construyen dashboards en Datadog para observar el rendimiento del sistema.|
| Evaluación Continua |	Se revisan métricas e indicadores clave para detectar anomalías o degradaciones.|
