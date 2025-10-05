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


## 7.2 Cpntinuous Delivery
### 7.2.1 Tools and Practices.

**JUnit:** Es una herramienta ampliamente utilizada en entornos Java para la ejecución de pruebas unitarias. Su elección se debe a la necesidad de validar de manera automática y rápida el correcto funcionamiento de los componentes individuales del sistema. JUnit permite detectar errores en fases tempranas del desarrollo, lo que contribuye a mejorar la calidad del software y reducir costos de corrección en etapas posteriores. Además, se integra fácilmente en pipelines de CI/CD, facilitando su automatización.

**Selenium:** Se emplea para la automatización de pruebas integrales y funcionales a nivel de interfaz de usuario. Con Selenium es posible simular la interacción real de un usuario con la aplicación, verificando que el sistema responda adecuadamente a distintos escenarios. Esta práctica garantiza que las distintas partes del software trabajen de manera conjunta y que la experiencia del usuario final sea consistente.

En conjunto, el uso de JUnit y Selenium asegura que tanto la lógica interna como el comportamiento externo de la aplicación se validen continuamente, lo que mejora la confiabilidad del sistema en cada ciclo de entrega.

### 7.2.2 Stages Deployment Pipeline Components.

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
