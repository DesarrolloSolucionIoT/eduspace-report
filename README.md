<div align="center">

![Logo UPC](https://upload.wikimedia.org/wikipedia/commons/f/fc/UPC_logo_transparente.png)

**Universidad Peruana de Ciencias Aplicadas**

**Facultad de Ingeniería**

**Curso:** 1ASI0572 – Desarrollo de Soluciones IoT

**NRC:** 6776

**Nombre del profesor:** Marco Antonio León Baca

---

## Informe de Trabajo Final

**Nombre de la startup:** BetterClass

**Nombre del producto:** EduSpace

---
**Integrantes:**

| Código | Apellidos y Nombres |
|--------|---------------------|
| u202310877| Alva Abanto, Luis Andrés |
| u20191e414| Antayhua Castillo, Josué Oscar |
| u202110385 | Loli Ramirez, Camila Cristina |
| u202220528 | Torres García, Andrés Alberto |
| u202312504 | Yalán Zhang, Angie Christina |

**Lima - abril 2026**

</div>

---

## Registro de Versiones del Informe

| Versión | Fecha | Autor | Descripción de modificación |
|---------|-------|-------|-----------------------------|
| 1.0 | 11/04/2026 | Equipo | Creación del informe. |

---

## Project Report Collaboration Insights

URL del repositorio del Project Report en GitHub: [https://github.com/DesarrolloSolucionIoT/eduspace-report](https://github.com/DesarrolloSolucionIoT/eduspace-report)


---

## Contenido

- [Registro de Versiones del Informe](#registro-de-versiones-del-informe)
- [Project Report Collaboration Insights](#project-report-collaboration-insights)
- [Student Outcome](#student-outcome)
- [Capítulo I: Introducción](#capítulo-i-introducción)
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
- [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
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
  - [2.4. Big Picture EventStorming](#24-big-picture-eventstorming)
  - [2.5. Ubiquitous Language](#25-ubiquitous-language)
- [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
  - [3.1. User Stories](#31-user-stories)
  - [3.2. Impact Mapping](#32-impact-mapping)
  - [3.3. Product Backlog](#33-product-backlog)
- [Capítulo IV: Solution Software Design](#capítulo-iv-solution-software-design)
  - [4.1. Strategic-Level Domain-Driven Design](#41-strategic-level-domain-driven-design)
    - [4.1.1. Design-Level EventStorming](#411-design-level-eventstorming)
      - [4.1.1.1. Candidate Context Discovery](#4111-candidate-context-discovery)
      - [4.1.1.2. Domain Message Flows Modeling](#4112-domain-message-flows-modeling)
      - [4.1.1.3. Bounded Context Canvases](#4113-bounded-context-canvases)
    - [4.1.2. Context Mapping](#412-context-mapping)
    - [4.1.3. Software Architecture](#413-software-architecture)
      - [4.1.3.1. Software Architecture System Landscape Diagram](#4131-software-architecture-system-landscape-diagram)
      - [4.1.3.2. Software Architecture Context Level Diagrams](#4132-software-architecture-context-level-diagrams)
      - [4.1.3.3. Software Architecture Container Level Diagrams](#4133-software-architecture-container-level-diagrams)
      - [4.1.3.4. Software Architecture Deployment Diagrams](#4134-software-architecture-deployment-diagrams)
  - [4.2. Tactical-Level Domain-Driven Design](#42-tactical-level-domain-driven-design)
    - [4.2.X. Bounded Context: \<Nombre\>](#42x-bounded-context-nombre)
      - [4.2.X.1. Domain Layer](#42x1-domain-layer)
      - [4.2.X.2. Interface Layer](#42x2-interface-layer)
      - [4.2.X.3. Application Layer](#42x3-application-layer)
      - [4.2.X.4. Infrastructure Layer](#42x4-infrastructure-layer)
      - [4.2.X.5. Bounded Context Software Architecture Component Level Diagrams](#42x5-bounded-context-software-architecture-component-level-diagrams)
      - [4.2.X.6. Bounded Context Software Architecture Code Level Diagrams](#42x6-bounded-context-software-architecture-code-level-diagrams)
        - [4.2.X.6.1. Bounded Context Domain Layer Class Diagrams](#42x61-bounded-context-domain-layer-class-diagrams)
        - [4.2.X.6.2. Bounded Context Database Design Diagram](#42x62-bounded-context-database-design-diagram)
- [Conclusiones](#conclusiones)
- [Bibliografía](#bibliografía)
- [Anexos](#anexos)

---

## Student Outcome

El curso contribuye al cumplimiento del Student Outcome ABET:

**ABET – EAC - Student Outcome 5:** La capacidad de funcionar efectivamente en un equipo cuyos miembros juntos proporcionan liderazgo, crean un entorno de colaboración e inclusivo, establecen objetivos, planifican tareas y cumplen objetivos.

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 5.

| Criterio específico | Acciones realizadas | Conclusiones |
|---------------------|---------------------|--------------|
| Trabaja en equipo para proporcionar liderazgo en forma conjunta | \<Apellido, Nombre\> **AV1** \<descripción de acciones\> | \<Conclusiones grupales\> |
| Crea un entorno colaborativo e inclusivo, establece metas, planifica tareas y cumple objetivos. | \<Apellido, Nombre\> **AV1** \<descripción de acciones\> | \<Conclusiones grupales\> |

---

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

EduSolutions es una startup enfocada en el desarrollo de soluciones tecnológicas innovadoras para el sector educativo. Su objetivo es mejorar el manejo integral de espacios educativos en institutos que cuentan con grandes infraestructuras.

En este contexto, surge la creación de la aplicación EduSpace, una aplicación que facilita la coordinación del personal y fortalece la comunicación entre trabajadores y supervisores.

EduSpace permite registrar y gestionar cada ambiente educativo, incluyendo aulas, su aforo y el docente responsable, así como ambientes deportivos y su equipamiento. La plataforma también gestiona los datos de los trabajadores, como docentes y personal de limpieza, facilitando la reasignación de responsabilidades en caso de ausencias.

Asimismo, cuenta con la interacción de sensores IoT para el monitoreo del entorno, permitiendo detectar la presencia de personas, temperatura, humedad, y automatizar el control de la iluminación. Esto contribuye a una gestión más eficiente y sostenible de recursos.

De esta manera, EduSpace permite a las instituciones educativas optimizar su eficiencia operativa, mejorar el uso de recursos y fortalecer su gestión interna.

**Misión:** Brindar soluciones tecnológicas y sostenibles que optimicen la gestión de espacios y recursos en instituciones educativas, mejorando su eficiencia operativa mediante herramientas digitales e integración de IoT.

**Visión:** Liderar en el rubro de servicios educativos en Latinoamérica con nuestra startup por ofrecer soluciones sostenibles y accesibles, destacando por la innovación en la gestión inteligente de espacios.


### 1.1.2. Perfiles de integrantes del equipo

| Foto del Participante                                                                                                                                                                                     | Nombres y Apellidos           | Código de Estudiante | Descripción de Carrera | Resumen de Conocimientos y Habilidades                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------|----------------------|------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [![Andrés Torres](https://github.com/DesarrolloSolucionIoT/report/raw/main/assets/chapter1/team/andres.jpeg)](https://github.com/DesarrolloSolucionIoT/report/blob/main/assets/chapter1/team/andres.jpeg) | Andrés Alberto Torres García  | u202220528           | Ingeniería de Software | Hola, soy Andrés Alberto Torres García, tengo 20 años y curso el séptimo ciclo de Ingeniería de Software. Me apasiona la tecnología y siempre busco entender cómo funcionan las cosas, lo que me ha permitido adquirir experiencia en C++, Python, JavaScript y TypeScript, así como en el desarrollo de aplicaciones web con Next.js, TailwindCSS y Firebase, bases de datos como MySQL, MongoDB y Firestore, y el uso de herramientas como Docker y GitHub. Además, el fútbol es otra de mis grandes pasiones, disciplina que me ha enseñado valores como el trabajo en equipo, la perseverancia y la constancia, que aplico también en mi vida académica y profesional. |
| [![Camila Loli](assets/chapter-I/CamilaLoli.jpg)                                                                                                                                                          | Camila Cristina Loli Ramirez  | u202110385           | Ingeniería de Software | Soy Camila Cristina Loli Ramirez, tengo 21 años y soy estudiante de la carrera Ingeniería de Software. Mi carrera se basa en los conocimientos y técnicas científicas para crear un programa informático. Tengo experiencia con el trabajo en equipo, creación de proyectos y creación de programas básicos. Aportaré al equipo mi creatividad, compromiso de trabajo en equipo, puntualidad y responsabilidad. Me comprometo a trabajar constantemente para mejorar nuestro proyecto y a generar un entorno de trabajo sano con mi grupo.                                                                                                                                 |
|                                                                                                                                                                                                           | Josué Oscar Antayhua Castillo | u20191e414           | Ingeniería de Software |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|                                                                                                                                                                                                           | Luis Andrés Alva Abanto       | u202310877           | Ingeniería de Software |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|                                                                                                                                                                                                           | Angie Christina Yalán Zhang   | u202312504           | Ingeniería de Software |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

Según el equipo de Expertos en Educación de la Universidad Internacional de Valencia (2025), en Perú, la gestión educativa enfrenta varios obstáculos que incluyen factores económicos, tecnológicos y organizacionales. Estas limitaciones impactan de manera negativa la infraestructura y la disponibilidad de recursos dentro de las instituciones educativas, lo que dificulta su adecuada administración.

Asimismo, el reducido uso de tecnologías en los procesos de gestión impide alcanzar niveles óptimos de eficiencia administrativa (Diaz, 2023). Diferentes estudios mencionan que la integración de herramientas tecnológicas permite optimizar procesos, mejorar la toma decisiones y fortalece la coordinación entre los trabajadores del entorno educativo (Valencia & Almeida, 2024).

Respecto al nivel organizacional, según Córdova Negrete et al. (2025) evidencian que las instituciones educativas presentan ineficiencias en sus procesos administrativos y limitaciones en su capacidad de respuesta. Estas condiciones generan problemas en la gestión de espacios, recursos y personal, lo que afecta la eficiencia operativa.

En consecuencia de la falta de una gestión apropiada, también hay diferentes problemas en el uso de recursos como la energía. El consumo eléctrico puede representar entre el 20% y 30% de los costos operativos en instituciones educativas (Birimisa, 2025), esto causa que haya una falta de control adecuado que perjudica tanto el aspecto financiero como el ambiental.

Además, la ausencia de sistemas de monitoreo impide regular de forma adecuada factores ambientales como la temperatura y la humedad dentro de los espacios educativos (aulas, laboratorios, entre otros). Estas condiciones pueden afectar el bienestar de los usuarios, generando riesgos para la salud, como problemas respiratorios o estrés térmico.

En este contexto, se identifica como problemática principal la gestión ineficiente de los espacios educativos y la falta de sistemas integrados que permitan una coordinación efectiva del personal, el monitoreo en tiempo real y la optimización de los recursos dentro de instituciones educativas con infraestructuras complejas.

Para analizar con más detalle los antecedentes y problemáticas, se realizó con anticipación la técnica 5 ‘W’s & 2 ‘H’s:

- ### _WHAT?_

El problema que se ha identificado es la gestión ineficiente de los espacios educativos con grandes infraestructuras. Estas organizaciones manejan múltiples espacios y recursos, lo que dificulta mantener un control adecuado sobre su disponibilidad y uso. Por consecuencia, esto ocasiona problemas de comunicación entre los empleados, retrasos en la toma de decisiones y dificultades para gestionar cambios o incidencias en tiempo real.

- ### _WHEN?_

La problemática surge cuando las instituciones experimentan un crecimiento o complejidad en su operación diaria, esto dificulta la gestión eficiente de sus espacios, personal y recursos. Esta situación se vuelve más crítica en situaciones como la planificación de nuevos semestres, la coordinación de actividades entre diferentes ambientes, la gestión de ausencias de personal, o cuando se enfrentan a la necesidad de automatizar procesos administrativos para mantener la eficiencia y evitar errores.

- ### _WHERE?_

Esta problemática ocurre dentro de instituciones educativas como universidades, colegios e institutos, especialmente en aquellos entornos que cuentan con múltiples espacios como aulas, laboratorios, bibliotecas y áreas deportivas. Es en estos contextos que la división de recursos y la falta de un sistema centralizado dificultan la gestión y coordinación diaria.

- ### _WHY?_

La causa principal del problema radica en la falta de integración y automatización en la gestión de los espacios y recursos. Muchas instituciones dependen de procesos manuales o sistemas desarticulados, esto genera una comunicación deficiente entre áreas, retrasos en la toma de decisiones y dificultades para coordinar al personal y los recursos disponibles.

- ### _WHO?_

En la problemática abordada, los afectados son los docentes, personal administrativo, y otros miembros del equipo de una institución educativa, quienes dependen de la organización de espacios y recursos para desarrollar sus tareas. La falta de coordinación impacta en su desempeño y en la eficiencia de las operaciones realizadas en la institución.

- ### _HOW?_

Este problema puede abordarse mediante la implementación de una solución tecnológica centralizada que permita gestionar de manera eficiente los espacios, recursos y personal. El uso de herramientas digitales facilitaría la automatización de procesos, mejora en la comunicación interna y monitoreo en tiempo real de los ambientes educativos.

- ### _HOW MUCH?_
El consumo energético de instituciones educativos puede representar entre el 20% y 30% de sus costos operativos (Birimisa, 2025), lo que evidencia que una gestión ineficiente de los recursos puede generar un impacto económico significativo.

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

#### 1.2.2.2. Lean UX Assumptions

#### 1.2.2.3. Lean UX Hypothesis Statements

#### 1.2.2.4. Lean UX Canvas

## 1.3. Segmentos objetivo

---

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores

### 2.1.1. Análisis competitivo

### 2.1.2. Estrategias y tácticas frente a competidores

## 2.2. Entrevistas

### 2.2.1. Diseño de entrevistas

### 2.2.2. Registro de entrevistas

### 2.2.3. Análisis de entrevistas

## 2.3. Needfinding

### 2.3.1. User Personas

### 2.3.2. User Task Matrix

### 2.3.3. User Journey Mapping

### 2.3.4. Empathy Mapping

## 2.4. Big Picture EventStorming

## 2.5. Ubiquitous Language

---

# Capítulo III: Requirements Specification

## 3.1. User Stories

| Epic / Story ID | Título | Descripción | Criterios de Aceptación | Relacionado con (Epic ID) |
|-----------------|--------|-------------|------------------------|--------------------------|
| | | | | |

## 3.2. Impact Mapping

## 3.3. Product Backlog

| # Orden | User Story ID | Título | Descripción | Story Points (1/2/3/5/8) |
|---------|--------------|--------|-------------|--------------------------|
| | | | | |

---

# Capítulo IV: Solution Software Design

## 4.1. Strategic-Level Domain-Driven Design

### 4.1.1. Design-Level EventStorming

#### 4.1.1.1. Candidate Context Discovery

#### 4.1.1.2. Domain Message Flows Modeling

#### 4.1.1.3. Bounded Context Canvases

### 4.1.2. Context Mapping

### 4.1.3. Software Architecture

#### 4.1.3.1. Software Architecture System Landscape Diagram

#### 4.1.3.2. Software Architecture Context Level Diagrams

#### 4.1.3.3. Software Architecture Container Level Diagrams

#### 4.1.3.4. Software Architecture Deployment Diagrams

## 4.2. Tactical-Level Domain-Driven Design

### 4.2.X. Bounded Context: \<Nombre\>

#### 4.2.X.1. Domain Layer

#### 4.2.X.2. Interface Layer

#### 4.2.X.3. Application Layer

#### 4.2.X.4. Infrastructure Layer

#### 4.2.X.5. Bounded Context Software Architecture Component Level Diagrams

#### 4.2.X.6. Bounded Context Software Architecture Code Level Diagrams

##### 4.2.X.6.1. Bounded Context Domain Layer Class Diagrams

##### 4.2.X.6.2. Bounded Context Database Design Diagram

---

# Conclusiones

## Conclusiones y recomendaciones

---

# Bibliografía

---

# Anexos

## Anexo A: Estructura para la sección Student Outcome

## Anexo B: Videos de Exposiciones

| Entrega | Título | URL |
|---------|--------|-----|
| AV1 | | |
