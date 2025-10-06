# UNIVERSIDAD PERUANA DE CIENCIAS APLICADAS

<p align="center">
  <img src="/assets/UPC_logo_transparente.png"  style="width:200px; height:auto;">
</p>

## <div style="text-align: center;"> Ingeniería de Software </div>
## <div style="text-align: center;"> Diseño de Experimentos de Ingeniería de Software</div>
## <div style="text-align: center;"> Nrc: 7508 </div>
## <div style="text-align: center;"> Docente: Julio Manuel Noriega Melendez </div>
## <div style="text-align: center;"> Informe TB1</div>
## <div style="text-align: center;"> Start up: CLOSED SOURCE </div>
## <div style="text-align: center;"> Product: PSYMED </div>

### <div style="text-align: center;"> INTEGRANTES:</div>
<div style="display: flex; justify-content: center;">
    <table>
      <thead>
        <tr>
          <th style="background-color: #333; color: #fff;">Apellidos y Nombres</th>
          <th style="background-color: #333; color: #fff;">Código de Alumno</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Asmad Padilla, Fátima</td>
          <td>U20221B490</td>
        </tr>
        <tr>
          <td>Nakasone Gomez, Marco</td>
          <td>U202210790</td>
        </tr>
        <tr>
          <td>Torres Flores, Paolo Alessandro</td>
          <td>U20221F613</td>
        </tr>
        <tr>
          <td>Maita Falckenheiner, Romina Guadalupe</td>
          <td>U202213765</td>
        </tr>
      </tbody>
    </table> 
</div>

<div style="text-align: center;"> Ciclo 2025-20 </div>

## Registro de Versiones del Informe

**Proyecto:** PSYMED – Informe TP
**Periodo de trabajo:** 04/09/2025 – 06/10/2025  
**Integrantes del equipo:**  
- **Paolo Torres** – Líder de UX / UI  
- **Romina Maita** – Desarrolladora Backend  
- **Fatima Asmad** – Desarrolladora Frontend  
- **Marco Nakasone** – Analista de Requerimientos  

---

## Historial de Versiones

| Versión |      Fecha | Responsable(s) | Descripción de cambios                                                                                                                                                          |
|--------:|-----------:|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|     0.1 | 04/09/2025 | Marco          | Creación de estructura inicial del documento y carátula. Agregado el índice general y capítulos preliminares.                                                                   |
|     0.2 | 05/09/2025 | Marco, Paolo   | Redacción de **Capítulo I: Introducción**, secciones 1.1 y 1.2. Incorporación de perfiles de la startup y proceso Lean UX.                                                      |
|     0.3 | 06/09/2025 | Marco          | Avance en 1.3 (Segmentos objetivo) y elaboración inicial del **Capítulo II: Requirements Elicitation & Analysis**.                                                              |
|     0.4 | 07/09/2025 | Marco, Paolo   | Inclusión de entrevistas: diseño y registro. Creación de User Personas, Task Matrix y Journey Mapping.                                                                          |
|     0.5 | 08/09/2025 | Paolo          | Desarrollo de Empathy Mapping, As-Is Scenario Mapping y Ubiquitous Language. Revisión general de redacción.                                                                     |
|     0.6 | 09/09/2025 | Romina, Fatima | Redacción de **Capítulo III: Requirements Specification**, incluyendo To-Be Scenarios, User Stories y Product Backlog.                                                          |
|     0.7 | 10/09/2025 | Paolo          | Avance de Impact Mapping. Inicio de **Capítulo IV: Product Design**, con Style Guidelines y Information Architecture.                                                           |
|     0.8 | 11/09/2025 | Paolo, Fatima  | Elaboración de Landing Page Wireframe y Mock-up. Desarrollo de Mobile Applications Wireframes y Wireflows.                                                                      |
|     0.9 | 12/09/2025 | Fatima, Romina | Creación de Web Applications Wireframes, Wireflows y Mock-ups. Adición de Domain-Driven Software Architecture (contexto y contenedores).                                        |
|     1.0 | 13/09/2025 | Romina         | Diseño de Class Diagrams, Class Dictionary y Database Diagram. Inicio de Capítulo V con Software Configuration Management.                                                      |
|     1.1 | 14/09/2025 | Todo el equipo | Revisión final, corrección de estilo y ortografía. Inclusión de evidencia de implementación (Landing, Frontend, Backend, API), bibliografía y anexos. Preparación para entrega. |

---


## Project Report Collaboration Insights
<img width="908" height="455" alt="image" src="https://github.com/user-attachments/assets/04cad86f-a510-4851-adff-0ccd40927754" />

# Contenido
## Tabla de Contenidos

### [Student Outcome](#student-outcome)
### [Part I: As-Is Software Project](#part-i-as-is-software-project)
### [Capítulo I: Introducción](#capítulo-i-introducción)
- [1.1. Startup Profile](#11-startup-profile)
    - [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
    - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
- [1.2. Solution Profile](#12-solution-profile)
    - [1.2.1. Antecedentes y problemática](#121-antecedentes-y-problemática)
    - [1.2.2. Lean UX Process](#122-lean-ux-process)
        - [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)
        - [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumptions)
        - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
        - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
- [1.3. Segmentos objetivo](#13-segmentos-objetivo)

### [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
- [2.1. Competidores](#21-competidores)
    - [2.1.1. Análisis competitivo](#211-análisis-competitivo)
    - [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
- [2.2. Entrevistas](#22-entrevistas)
    - [2.2.1. Diseño de entrevistas](#221-diseño-de-entrevistas)
    - [2.2.2. Registro de entrevistas](#222-registro-de-entrevistas)
    - [2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)
- [2.3. Needfinding](#23-needfinding)
    - [2.3.1. User Personas](#231-user-personas)
    - [2.3.2. User Task Matrix](#232-user-task-matrix)
    - [2.3.3. User Journey Mapping](#233-user-journey-mapping)
    - [2.3.4. Empathy Mapping](#234-empathy-mapping)
    - [2.3.5. As-is Scenario Mapping](#235-as-is-scenario-mapping)
- [2.4. Ubiquitous Language](#24-ubiquitous-language)

### [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
- [3.1. To-Be Scenario Mapping](#31-to-be-scenario-mapping)
- [3.2. User Stories](#32-user-stories)
- [3.3. Product Backlog](#33-product-backlog)
- [3.4. Impact Mapping](#34-impact-mapping)

### [Capítulo IV: Product Design](#capítulo-iv-product-design)
- [4.1. Style Guidelines](#41-style-guidelines)
    - [4.1.1. General Style Guidelines](#411-general-style-guidelines)
    - [4.1.2. Web Style Guidelines](#412-web-style-guidelines)
    - [4.1.3. Mobile Style Guidelines](#413-mobile-style-guidelines)
        - [4.1.3.1. iOS Mobile Style Guidelines](#4131-ios-mobile-style-guidelines)
        - [4.1.3.2. Android Mobile Style Guidelines](#4132-android-mobile-style-guidelines)
- [4.2. Information Architecture](#42-information-architecture)
    - [4.2.1. Organization Systems](#421-organization-systems)
    - [4.2.2. Labeling Systems](#422-labeling-systems)
    - [4.2.3. SEO Tags and Meta Tags](#423-seo-tags-and-meta-tags)
    - [4.2.4. Searching Systems](#424-searching-systems)
    - [4.2.5. Navigation Systems](#425-navigation-systems)
- [4.3. Landing Page UI Design](#43-landing-page-ui-design)
    - [4.3.1. Landing Page Wireframe](#431-landing-page-wireframe)
    - [4.3.2. Landing Page Mock-up](#432-landing-page-mock-up)
- [4.4. Mobile Applications UX/UI Design](#44-mobile-applications-uxui-design)
    - [4.4.1. Mobile Applications Wireframes](#441-mobile-applications-wireframes)
    - [4.4.2. Mobile Applications Wireflow Diagrams](#442-mobile-applications-wireflow-diagrams)
    - [4.4.3. Mobile Applications Mock-ups](#443-mobile-applications-mock-ups)
    - [4.4.4. Mobile Applications User Flow Diagrams](#444-mobile-applications-user-flow-diagrams)
- [4.5. Mobile Applications Prototyping](#45-mobile-applications-prototyping)
    - [4.5.1. Android Mobile Applications Prototyping](#451-android-mobile-applications-prototyping)
    - [4.5.2. iOS Mobile Applications Prototyping](#452-ios-mobile-applications-prototyping)
- [4.6. Web Applications UX/UI Design](#46-web-applications-uxui-design)
    - [4.6.1. Web Applications Wireframes](#461-web-applications-wireframes)
    - [4.6.2. Web Applications Wireflow Diagrams](#462-web-applications-wireflow-diagrams)
    - [4.6.3. Web Applications Mock-ups](#463-web-applications-mock-ups)
    - [4.6.4. Web Applications User Flow Diagrams](#464-web-applications-user-flow-diagrams)
- [4.7. Web Applications Prototyping](#47-web-applications-prototyping)
- [4.8. Domain-Driven Software Architecture](#48-domain-driven-software-architecture)
    - [4.8.1. Software Architecture Context Diagram](#481-software-architecture-context-diagram)
    - [4.8.2. Software Architecture Container Diagrams](#482-software-architecture-container-diagrams)
    - [4.8.3. Software Architecture Components Diagrams](#483-software-architecture-components-diagrams)
- [4.9. Software Object-Oriented Design](#49-software-object-oriented-design)
    - [4.9.1. Class Diagrams](#491-class-diagrams)
    - [4.9.2. Class Dictionary](#492-class-dictionary)
- [4.10. Database Design](#410-database-design)
    - [4.10.1. Relational/Non-Relational Database Diagram](#4101-relationalnon-relational-database-diagram)

### [Capítulo V: Product Implementation](#capítulo-v-product-implementation)
- [5.1. Software Configuration Management](#51-software-configuration-management)
    - [5.1.1. Software Development Environment Configuration](#511-software-development-environment-configuration)
    - [5.1.2. Source Code Management](#512-source-code-management)
    - [5.1.3. Source Code Style Guide & Conventions](#513-source-code-style-guide--conventions)
    - [5.1.4. Software Deployment Configuration](#514-software-deployment-configuration)
- [5.2. Product Implementation & Deployment](#52-product-implementation--deployment)
    - [5.2.1. Sprint Backlogs](#521-sprint-backlogs)
    - [5.2.2. Implemented Landing Page Evidence](#522-implemented-landing-page-evidence)
    - [5.2.3. Implemented Frontend-Web Application Evidence](#523-implemented-frontend-web-application-evidence)
    - [5.2.4. Acuerdo de Servicio - SaaS](#524-acuerdo-de-servicio---saas)
    - [5.2.5. Implemented Native-Mobile Application Evidence](#525-implemented-native-mobile-application-evidence)
    - [5.2.6. Implemented RESTful API and/or Serverless Backend Evidence](#526-implemented-restful-api-andor-serverless-backend-evidence)
    - [5.2.7. RESTful API documentation](#527-restful-api-documentation)
    - [5.2.8. Team Collaboration Insights](#528-team-collaboration-insights)
- [5.3. Video About-the-Product](#53-video-about-the-product)

### [Part II: Verification, Validation & Pipeline](#part-ii-verification-validation--pipeline)
### [Capítulo VI: Product Verification & Validation](#capítulo-vi-product-verification--validation)
- [6.1. Testing Suites & Validation](#61-testing-suites--validation)
    - [6.1.1. Core Entities Unit Tests](#611-core-entities-unit-tests)
    - [6.1.2. Core Integration Tests](#612-core-integration-tests)
    - [6.1.3. Core Behavior-Driven Development](#613-core-behavior-driven-development)
    - [6.1.4. Core System Tests](#614-core-system-tests)
- [6.2. Static testing & Verification](#62-static-testing--verification)
    - [6.2.1. Static Code Analysis](#621-static-code-analysis)
        - [6.2.1.1. Coding standard & Code conventions](#6211-coding-standard--code-conventions)
        - [6.2.1.2. Code Quality & Code Security](#6212-code-quality--code-security)
    - [6.2.2. Reviews](#622-reviews)
- [6.3. Validation Interviews](#63-validation-interviews)
    - [6.3.1. Diseño de Entrevistas](#631-diseño-de-entrevistas)
    - [6.3.2. Registro de Entrevistas](#632-registro-de-entrevistas)
    - [6.3.3. Evaluaciones según heurísticas](#633-evaluaciones-según-heurísticas)
- [6.4. Auditoría de Experiencias de Usuario](#64-auditoría-de-experiencias-de-usuario)
    - [6.4.1. Auditoría realizada](#641-auditoría-realizada)
        - [6.4.1.1. Información del grupo auditado](#6411-información-del-grupo-auditado)
        - [6.4.1.2. Cronograma de auditoría realizada](#6412-cronograma-de-auditoría-realizada)
        - [6.4.1.3. Contenido de auditoría realizada](#6413-contenido-de-auditoría-realizada)
    - [6.4.2. Auditoría recibida](#642-auditoría-recibida)
        - [6.4.2.1. Información del grupo auditor](#6421-información-del-grupo-auditor)
        - [6.4.2.2. Cronograma de auditoría recibida](#6422-cronograma-de-auditoría-recibida)
        - [6.4.2.3. Contenido de auditoría recibida](#6423-contenido-de-auditoría-recibida)
        - [6.4.2.4. Resumen de modificaciones para subsanar hallazgos](#6424-resumen-de-modificaciones-para-subsanar-hallazgos)

### [Capítulo VII: DevOps Practices](#capítulo-vii-devops-practices)
- [7.1. Continuous Integration](#71-continuous-integration)
    - [7.1.1. Tools and Practices](#711-tools-and-practices)
    - [7.1.2. Build & Test Suite Pipeline Components](#712-build--test-suite-pipeline-components)
- [7.2. Continuous Delivery](#72-continuous-delivery)
    - [7.2.1. Tools and Practices](#721-tools-and-practices)
    - [7.2.2. Stages Deployment Pipeline Components](#722-stages-deployment-pipeline-components)
- [7.3. Continuous Deployment](#73-continuous-deployment)
    - [7.3.1. Tools and Practices](#731-tools-and-practices)
    - [7.3.2. Production Deployment Pipeline Components](#732-production-deployment-pipeline-components)
- [7.4. Continuous Monitoring](#74-continuous-monitoring)
    - [7.4.1. Tools and Practices](#741-tools-and-practices)
    - [7.4.2. Monitoring Pipeline Components](#742-monitoring-pipeline-components)
    - [7.4.3. Alerting Pipeline Components](#743-alerting-pipeline-components)
    - [7.4.4. Notification Pipeline Components](#744-notification-pipeline-components)

### [Part III: Experiment-Driven Lifecycle](#part-iii-experiment-driven-lifecycle)
### [Capítulo VIII: Experiment-Driven Development](#capítulo-viii-experiment-driven-development)
- [8.1. Experiment Planning](#81-experiment-planning)
    - [8.1.1. As-Is Summary](#811-as-is-summary)
    - [8.1.2. Raw Material: Assumptions, Knowledge Gaps, Ideas, Claims](#812-raw-material-assumptions-knowledge-gaps-ideas-claims)
    - [8.1.3. Experiment-Ready Questions](#813-experiment-ready-questions)
    - [8.1.4. Question Backlog](#814-question-backlog)
    - [8.1.5. Experiment Cards](#815-experiment-cards)
- [8.2. Experiment Design](#82-experiment-design)
    - [8.2.1. Hypotheses](#821-hypotheses)
    - [8.2.2. Domain Business Metrics](#822-domain-business-metrics)
    - [8.2.3. Measures](#823-measures)
    - [8.2.4. Conditions](#824-conditions)
    - [8.2.5. Scale Calculations and Decisions](#825-scale-calculations-and-decisions)
    - [8.2.6. Methods Selection](#826-methods-selection)
    - [8.2.7. Data Analytics: Goals, KPIs and Metrics Selection](#827-data-analytics-goals-kpis-and-metrics-selection)
    - [8.2.8. Web and Mobile Tracking Plan](#828-web-and-mobile-tracking-plan)
- [8.3. Experimentation](#83-experimentation)
    - [8.3.1. To-Be User Stories](#831-to-be-user-stories)
    - [8.3.2. To-Be Product Backlog](#832-to-be-product-backlog)
    - [8.3.3. Pipeline-supported, Experiment-Driven To-Be Software Platform Lifecycle](#833-pipeline-supported-experiment-driven-to-be-software-platform-lifecycle)
        - [8.3.3.1. To-Be Sprint Backlogs](#8331-to-be-sprint-backlogs)
        - [8.3.3.2. Implemented To-Be Landing Page Evidence](#8332-implemented-to-be-landing-page-evidence)
        - [8.3.3.3. Implemented To-Be Frontend-Web Application Evidence](#8333-implemented-to-be-frontend-web-application-evidence)
        - [8.3.3.4. Implemented To-Be Native-Mobile Application Evidence](#8334-implemented-to-be-native-mobile-application-evidence)
        - [8.3.3.5. Implemented To-Be RESTful API and/or Serverless Backend Evidence](#8335-implemented-to-be-restful-api-andor-serverless-backend-evidence)
        - [8.3.3.6. Team Collaboration Insights](#8336-team-collaboration-insights)
    - [8.3.4. To-Be Validation Interviews](#834-to-be-validation-interviews)
        - [8.3.4.1. Diseño de Entrevistas](#8341-diseño-de-entrevistas)
        - [8.3.4.2. Registro de Entrevistas](#8342-registro-de-entrevistas)
- [8.4. Experiment Aftermath & Analysis](#84-experiment-aftermath--analysis)
    - [8.4.1. Analysis and Interpretation of Results](#841-analysis-and-interpretation-of-results)
    - [8.4.2. Re-scored and Re-prioritized Question Backlog](#842-re-scored-and-re-prioritized-question-backlog)
- [8.5. Continuous Learning](#85-continuous-learning)
    - [8.5.1. Shareback Session Artifacts: Learning Workflow](#851-shareback-session-artifacts-learning-workflow)
- [8.6. To-Be Software Platform Pre-launch](#86-to-be-software-platform-pre-launch)
    - [8.6.1. About-the-Product Intro Video](#861-about-the-product-intro-video)

### [Conclusiones](#conclusiones)
### [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)
### [Video App Validation](#video-app-validation)
### [Video About-the-Team](#video-about-the-team)
### [Bibliografía](#bibliografía)
### [Anexos](#anexos)


## Student Outcome

**ABET – EAC - Student Outcome 4**

**Criterio**: 

La capacidad de reconocer responsabilidades éticas y profesionales en situaciones de ingeniería y hacer juicios informados, que deben considerar el impacto de las soluciones de ingeniería en contextos globales, económicos, ambientales y sociales.En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 4.

| Criterio específico                                                                                                                                          | Acciones realizadas                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Conclusiones                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 4.c.1 Reconoce responsabilidad ética y profesional en situaciones de ingeniería de software                                                                  | **TB1:** Paolo participó en la redacción de *Startup Profile* y *Solution Profile*, garantizando que los problemas estuvieran sustentados en fuentes reales y entrevistas verificadas. Colaboró en la formulación de *Lean UX Problem Statements* basados en hallazgos objetivos. <br> **TP:** Participó en la validación del funcionamiento del sistema mediante pruebas unitarias con JUnit y pruebas funcionales con Selenium. Aseguró que la documentación técnica reflejara con precisión los resultados y los criterios de validación aplicados. <br><br> **TB1:** Fátima desarrolló las secciones de *Needfinding* (User Personas, Empathy Mapping, As-is Scenario Mapping) y colaboró en *Impact Mapping*, asegurando una representación fiel de los usuarios objetivo. <br> **TP:** Colaboró en la documentación de pruebas, garantizando la presentación completa y transparente de los resultados obtenidos con JUnit y Selenium. <br><br> **TB1:** Marco fue responsable del *Product Design* (Style Guidelines, Wireframes, Prototyping) y del *Database Design*, aplicando estándares de accesibilidad y usabilidad. <br> **TP:** Realizó pruebas automatizadas con JUnit y Selenium en los módulos de interfaz, documentando incidencias y correcciones. <br><br> **TB1:** Romina desarrolló el backend y frontend, junto con el diseño UX/UI, garantizando integridad de datos y usabilidad. <br> **TP:** Lideró las pruebas de integración con JUnit y Selenium, verificando la interacción entre componentes y documentando los resultados. | **TB1:** Paolo demostró responsabilidad profesional al validar información real y evitar suposiciones. <br> **TP:** Mantuvo una conducta ética al garantizar la veracidad y trazabilidad de las pruebas. <br><br> **TB1:** Fátima reflejó responsabilidad ética al priorizar necesidades reales de usuarios y evitar sesgos. <br> **TP:** Garantizó transparencia y mejora continua al registrar resultados sin omitir fallos. <br><br> **TB1:** Marco mostró responsabilidad profesional al asegurar accesibilidad, seguridad y usabilidad. <br> **TP:** Reafirmó su compromiso ético validando la funcionalidad y accesibilidad del diseño. <br><br> **TB1:** Romina asumió responsabilidad ética y profesional al garantizar la confiabilidad del sistema. <br> **TP:** Aseguró la integridad y calidad del software mediante pruebas exhaustivas y documentadas. |
| 4.c.2 Emite juicios informados considerando el impacto de las soluciones de ingeniería de software en contextos globales, económicos, ambientales y sociales | **TB1:** Paolo analizó competidores y definió estrategias de diferenciación mediante *Competitive Analysis* y tácticas de posicionamiento. <br> **TP:** Analizó los resultados de las pruebas considerando rendimiento y estabilidad del sistema. <br><br> **TB1:** Fátima construyó *User Journey Mapping* e *Impact Mapping*, evaluando el efecto del diseño en la experiencia y bienestar del usuario. <br> **TP:** Analizó cómo los resultados de las pruebas influían en la usabilidad y accesibilidad del sistema. <br><br> **TB1:** Marco evaluó escalabilidad, sostenibilidad y seguridad en *Product Implementation* y *Database Design*. <br> **TP:** Interpretó los resultados de las pruebas para optimizar la interfaz, el rendimiento y la escalabilidad. <br><br> **TB1:** Romina evaluó el impacto de sus decisiones en la escalabilidad y adaptabilidad del sistema. <br> **TP:** Analizó la estabilidad, seguridad y sostenibilidad del sistema tras las pruebas automatizadas.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | **TB1:** Paolo emitió juicios informados sobre el impacto económico y la sostenibilidad del producto. <br> **TP:** Priorizó la confiabilidad y sostenibilidad técnica del sistema. <br><br> **TB1:** Fátima consideró el impacto social y emocional del software en los usuarios. <br> **TP:** Relacionó la calidad técnica con la mejora de la experiencia y la estabilidad del sistema. <br><br> **TB1:** Marco emitió juicios informados sobre la privacidad y escalabilidad del sistema. <br> **TP:** Priorizó la eficiencia y adaptabilidad del sistema con base en los resultados de prueba. <br><br> **TB1:** Romina emitió juicios informados priorizando accesibilidad, eficiencia y sostenibilidad. <br> **TP:** Evaluó el impacto de las decisiones técnicas en la mejora continua y adaptabilidad del software.                                          |
