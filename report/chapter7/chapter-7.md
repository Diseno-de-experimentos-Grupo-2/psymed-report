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

## 7.2 Cpntinuous Delivery
### 7.2.1 Tools and Practices.
### 7.2.2 Stages Deployment Pipeline Components.

## 7.3 Continuous deployment
### 7.3.1 Tool and Practices.
### 7.3.2 Production Deployment Pipeline Components.

Los elementos fundamentales de un pipeline orientado al despliegue en producción son los siguientes:

**a. Construcción (Build):** Se compila el código fuente y se generan los artefactos listos para ser distribuidos en el entorno productivo.

**b. Validación (Testing):** Se ejecutan pruebas automatizadas con el fin de asegurar que la aplicación cumple los criterios de calidad establecidos y que no se introducen fallos no previstos.

**c. Entorno de Preproducción (Staging):** Antes del despliegue definitivo, la solución se implementa en un ambiente intermedio para la realización de pruebas adicionales y validación por parte de un grupo reducido de usuarios.

**d. Implementación en Producción (Production Deployment):** Se lleva a cabo el despliegue automático de los artefactos en el entorno productivo.

**e. Supervisión Continua (Continuous Monitoring):** Una vez desplegada, la aplicación es monitoreada de manera constante para garantizar su rendimiento, disponibilidad y estabilidad, atendiendo incidentes en tiempo real.

**f. Reversión (Rollback):** Ante la detección de fallas críticas, el pipeline contempla mecanismos de reversión inmediata hacia una versión previa estable de la aplicación.
