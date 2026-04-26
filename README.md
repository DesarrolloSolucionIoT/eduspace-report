<div align="center">

![Logo UPC](https://upload.wikimedia.org/wikipedia/commons/f/fc/UPC_logo_transparente.png)

**Universidad Peruana de Ciencias Aplicadas**

**Facultad de Ingeniería**

**Curso:** 1ASI0572 – Desarrollo de Soluciones IoT

**NRC:** 6776

**Nombre del profesor:** Marco Antonio León Baca

---

## Informe de Trabajo Final

**Nombre de la startup:** EduSolutions

**Nombre del producto:** EduSpace

---

**Integrantes:**

| Código     | Apellidos y Nombres            |
| ---------- | ------------------------------ |
| u202310877 | Alva Abanto, Luis Andrés       |
| u20191e414 | Antayhua Castillo, Josué Oscar |
| u202110385 | Loli Ramirez, Camila Cristina  |
| u202220528 | Torres García, Andrés Alberto  |
| u202312504 | Yalán Zhang, Angie Christina   |

**Lima - abril 2026**

</div>

---

## Registro de Versiones del Informe

| Versión | Fecha      | Autor          | Descripción de modificación                                                                       |
| ------- | ---------- | -------------- | ------------------------------------------------------------------------------------------------- |
| 1.0     | 11/04/2026 | Equipo         | Creación del informe.                                                                             |
| 1.1     | 25/04/2026 | Andrés Torres  | Se redactó la sección 4.2.5 (Tactical-Level DDD) del Bounded Context IoT Monitoring.             |
| 1.2     | 25/04/2026 | Andrés Torres  | Se redactaron las secciones 4.2.1, 4.2.2, 4.2.3 y 4.2.4 del Tactical-Level DDD. Se alineó el motor de base de datos a MySQL en 4.2.5. |

---

## Project Report Collaboration Insights

URL del repositorio del Project Report en GitHub: [https://github.com/DesarrolloSolucionIoT/eduspace-report](https://github.com/DesarrolloSolucionIoT/eduspace-report)

---

## Contenido

- [Capítulo I: Introducción](#capítulo-i-introducción)
  - [1.1. Startup Profile](#11-startup-profile)
    - [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
    - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
  - [1.2. Solution Profile](#12-solution-profile)
    - [1.2.1. Antecedentes y problemática](#121-antecedentes-y-problemática)
    - [1.2.2. Lean UX Process](#122-lean-ux-process)
      - [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)
        - [**a. DOMAIN**](#a-domain)
        - [**b. CUSTOMER SEGMENTS**](#b-customer-segments)
        - [**c. PAIN POINTS**](#c-pain-points)
        - [**d. GAP**](#d-gap)
        - [**e. VISION/STRATEGY**](#e-visionstrategy)
        - [**f. INITIAL SEGMENT**](#f-initial-segment)
      - [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumptions)
      - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
      - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
  - [1.3. Segmentos objetivo](#13-segmentos-objetivo)
- [Capítulo II: Requirements Elicitation \& Analysis](#capítulo-ii-requirements-elicitation--analysis)
  - [2.1. Competidores](#21-competidores)
    - [2.1.1. Análisis competitivo](#211-análisis-competitivo)
    - [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
      - [**Frente a las fortalezas de los competidores**](#frente-a-las-fortalezas-de-los-competidores)
        - [**Fortalezas de Smart Campus IoT:**](#fortalezas-de-smart-campus-iot)
        - [**Estrategias**](#estrategias)
        - [**Tácticas**](#tácticas)
      - [**Frente a las debilidades de los competidores**](#frente-a-las-debilidades-de-los-competidores)
        - [**Debilidades de Smart Campus IoT:**](#debilidades-de-smart-campus-iot)
        - [**Estrategias**](#estrategias-1)
        - [**Tácticas**](#tácticas-1)
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
    - [4.2.1. Bounded Context: IAM & Profile Management](#421-bounded-context-iam--profile-management)
      - [4.2.1.1. Domain Layer](#4211-domain-layer)
      - [4.2.1.2. Interface Layer](#4212-interface-layer)
      - [4.2.1.3. Application Layer](#4213-application-layer)
      - [4.2.1.4. Infrastructure Layer](#4214-infrastructure-layer)
    - [4.2.2. Bounded Context: Space & Resource Management](#422-bounded-context-space--resource-management)
      - [4.2.2.1. Domain Layer](#4221-domain-layer)
      - [4.2.2.2. Interface Layer](#4222-interface-layer)
      - [4.2.2.3. Application Layer](#4223-application-layer)
      - [4.2.2.4. Infrastructure Layer](#4224-infrastructure-layer)
    - [4.2.3. Bounded Context: Reservation & Scheduling](#423-bounded-context-reservation--scheduling)
      - [4.2.3.1. Domain Layer](#4231-domain-layer)
      - [4.2.3.2. Interface Layer](#4232-interface-layer)
      - [4.2.3.3. Application Layer](#4233-application-layer)
      - [4.2.3.4. Infrastructure Layer](#4234-infrastructure-layer)
    - [4.2.4. Bounded Context: Breakdown Management](#424-bounded-context-breakdown-management)
      - [4.2.4.1. Domain Layer](#4241-domain-layer)
      - [4.2.4.2. Interface Layer](#4242-interface-layer)
      - [4.2.4.3. Application Layer](#4243-application-layer)
      - [4.2.4.4. Infrastructure Layer](#4244-infrastructure-layer)
    - [4.2.5. Bounded Context: IoT Monitoring](#425-bounded-context-iot-monitoring)
      - [4.2.5.1. Domain Layer](#4251-domain-layer)
      - [4.2.5.2. Interface Layer](#4252-interface-layer)
      - [4.2.5.3. Application Layer](#4253-application-layer)
      - [4.2.5.4. Infrastructure Layer](#4254-infrastructure-layer)
- [Conclusiones](#conclusiones)
  - [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)
- [Bibliografía](#bibliografía)
- [Anexos](#anexos)
  - [Anexo A: Estructura para la sección Student Outcome](#anexo-a-estructura-para-la-sección-student-outcome)
  - [Anexo B: Videos de Exposiciones](#anexo-b-videos-de-exposiciones)

---

## Student Outcome

El curso contribuye al cumplimiento del Student Outcome ABET:

**ABET – EAC - Student Outcome 5:** La capacidad de funcionar efectivamente en un equipo cuyos miembros juntos proporcionan liderazgo, crean un entorno de colaboración e inclusivo, establecen objetivos, planifican tareas y cumplen objetivos.

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 5.

| Criterio específico                                                                             | Acciones realizadas                                      | Conclusiones              |
| ----------------------------------------------------------------------------------------------- | -------------------------------------------------------- | ------------------------- |
| Trabaja en equipo para proporcionar liderazgo en forma conjunta                                 | \<Apellido, Nombre\> **AV1** \<descripción de acciones\> | \<Conclusiones grupales\> |
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
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------- | -------------------- | ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
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

En el estado actual de la gestión administrativa en centros educativos con grandes infraestructuras es deficiente. En ambos segmentos, es complicado seguir un orden de procesos, ya que los procesos administrativos suelen depender de métodos manuales o sistemas desintegrados. Esto dificulta la coordinación del personal, el control de la disponibilidad de los espacios y correcta gestión de recursos.

Esta situación se ve agravada por la falta de herramientas tecnológicas accesibles que permitan monitorear en tiempo real el uso de los ambientes educativos, y factores relevantes como el consumo energético y las condiciones ambientales dentro de las aulas, bibliotecas, laboratorios, entre otros.

En consecuencia, las instituciones sufren de diferentes problemas, como retrasos en la forma de decisiones, uso ineficiente de recursos, aumento en costos operativos y una limitada capacidad de respuesta ante incidentes.

¿Cómo podríamos mejorar la gestión y monitoreo de espacios educativos para optimizar el uso de recursos, reducir costos operativos y elevar la eficiencia en la coordinación del personal?

##### **a. DOMAIN**

Gestión de espacios educativos y recursos en instituciones con infraestructuras complejas que requieren coordinación eficiente del personal, control de ambientes y optimización del uso de recursos.

##### **b. CUSTOMER SEGMENTS**

Administradores de instituciones educativas y docentes y auxiliares que gestionan múltiples espacios físicos y necesitan mejorar su organización y control.

##### **c. PAIN POINTS**

- Coordinación ineficaz del personal entre diferentes espacios.
- Comunicación deficiente entre trabajadores y supervisores.
- Procesos administrativos manuales y propensos a errores.
- Dificultad en el seguimiento y mantenimiento de equipos e inventarios.
- Falta de disponibilidad y uso de os espacios educativos.

##### **d. GAP**

No existe una solución integrada que permita centralizar la gestión de espacios, recursos y personal, y monitorear en tiempo real el uso de los ambientes educativos, esto limita la eficiencia operativa de las instituciones.

##### **e. VISION/STRATEGY**

Desarrollar una plataforma integral que permita facilitar la gestión eficiente de espacios educativos, automatizar tareas administrativas, mejorar la comunicación y coordinación del personal y el monitoreo en tiempo real de recursos, esto contribuye a un funcionamiento más eficiente y sostenible.

##### **f. INITIAL SEGMENT**

Las grandes instituciones educativas que enfrentan problemas en la coordinación de espacios y la administración de personal están buscando una solución digital para optimizar estos procesos.

#### 1.2.2.2. Lean UX Assumptions

Business Assumptions: 

- **Creemos que nuestros usuarios necesitan** una manera eficiente de gestionar los espacios educativos, recursos y personal en instituciones con múltiples ambientes.
- **Estas necesidades se pueden resolver con** una aplicación móvil centralizada que permita automatizar procesos, mejorar la coordinación interna y monitorear en tiempo real el uso de los espacios.
- **Nuestros clientes iniciales son** docentes de instituciones educativas y personal administrativo que buscan optimizar sus procesos.
- **El valor #1 que un cliente requiere de nuestro servicio** es optimizar el uso de espacios y recursos, para evitar ineficiencias en el funcionamiento de la institución.
- **El cliente también puede obtener estos beneficios adicionales** mejorar la comunicación entre el personal, reducción de errores administrativos, ahorro en el consumo energético.
- **Adquiriremos a nuestros clientes a través** campañas de marketing digital, demostraciones en línea y referencias de clientes existentes.
- **Haremos dinero a través** de la venta d planes de suscripción adaptados a las necesidades de las instituciones educativas.
- **Nuestra competencia de mercado** serán aplicaciones de gestión educativa tradicionales que no integran monitoreo en tiempo real ni automatización avanzada de recursos.
- **Los venceremos debido** a la integración de monitoreo en tiempo real, automatización de procesos y optimización del uso de recursos mediante tecnologías IoT.
- **Nuestros mayores riesgos son** que las instituciones educativas no perciban un valor claro en la adopción de una nueva plataforma, que el plan de suscripción no se ajuste a sus necesidades.
- **Resolveremos esto mediante** el desarrollo del producto, nuestra prioridad es entender las necesidades de los usuarios y proveer una solución tecnológica, que sea intuitiva de utilizar.
- **Sabremos que hemos tenido éxito cuando uno de estos cambios en el comportamiento de nuestro cliente:** El usuario logra gestionar la asignación de espacios y recursos en menor tiempo, reduzcan errores en la coordinación de actividades y utilicen activamente el sistema para monitorear el ambiente de las aulas.
- **Qué otras suposiciones tenemos que, de probarse falsas pueden causar que nuestro proyecto fracase:** suponer que los segmentos objetivos prefieren mantener el uso de sistemas manuales para monitorear los ambientes y recursos disponibles.

**Business Outcomes:** 

- Mejorar la eficiencia operativa de las instituciones educativas un 25% en sus primeros 4 meses de uso del sistema.
- Se espera que al menos el 30% de nuestros clientes nos recomienden a otras instituciones dentro de los primeros 6 meses.
- Ofrecer la aplicación en múltiples idiomas incrementará la base de usuarios en un 25% en los primeros seis meses, permitiendo que más instituciones educativas de diferentes regiones utilicen la plataforma y contribuyendo a un crecimiento anual del 15%
-  Crear interfaz fácil de usar y visualmente atractiva que retenga al menos el 50% de usuarios después de los primeros 7 meses.
- Conseguir que más del 65% de usuarios pague la suscripción (anual o mensual) ofrecida. 

**User Assumptions:** 

**¿Quiénes serán nuestros usuarios?** 

Nuestros usuarios principales son: 

- Docentes y auxiliares entre las edades de 22 a 65 años que buscan una solución que facilite el monitoreo de ambientes y mejore la comunicación con los administradores.
- Administradores de instituciones educativas entre 35 a 60 años que necesitan una herramienta que permita gestionar eficazmente los espacios y recursos.

**¿Dónde encaja nuestro producto en su vida o trabajo?** 

El producto se adapta al trabajo diario de los usuarios, facilitando la gestión de ambientes, equipos y recursos del centro educativo, y mejorando la comunicación entre el personal.

**¿Qué problemas tiene nuestro producto y cómo se pueden resolver?** 

La falta de control sobre los espacios educativos, la comunicación ineficiente y la ausencia de monitoreo en tiempo real.

**¿Cómo y cuándo es usado nuestro producto?** 

EduSolutions se utiliza de forma diaria para gestionar la asignación de espacios, coordinar actividades y monitorear el estado de los ambientes educativos.

**¿Qué características son importantes?** 

Acceso en tiempo real, facilidad de uso, centralización de información y automatización de procesos.

**¿Cómo debe verse y comportarse nuestro producto?** 

El producto debe de ser intuitivo, rápido, disponible durante el horario laboral, y accesible desde distintos dispositivos, lo que permitirá una gestión eficiente sin complejidad técnica.

**El valor principal que un usuario quiere obtener de nuestra funcionalidad es:**

- Mejora en la gestión de los espacios y recursos, junto con una comunicación más eficiente entre los trabajadores.

**Los usuarios también pueden obtener estos beneficios adicionales:**

- Acceso rápido a la información en cualquier momento y desde cualquier dispositivo.

**El mayor riesgo para el usuario es:**

- Que la aplicación no se adapte correctamente a diferentes dispositivos o que no facilite la comunicación interna como se espera.

**User Outcomes:**

- Acceso a Notificaciones y Actualizaciones: Al implementar un sistema de notificaciones, se espera que el 80% de los usuarios reciban y respondan a los eventos y cambios importantes en la aplicación dentro de las primeras 24 horas. Esto mejorará su capacidad de gestionar tareas en tiempo real, optimizando su productividad en un 15%.
- Reducción del Tiempo de Familiarización: Una interfaz intuitiva y fácil de usar reducirá el tiempo de familiarización de los usuarios en un 30%, permitiendo que al menos el 90% de ellos dominen las funcionalidades básicas en menos de una semana sin necesidad de capacitaciones adicionales.
- Mejora en el Control de Inventarios: Con la introducción de funciones para registrar y gestionar el inventario de equipos y recursos, se espera que los usuarios logren un aumento del 25% en el control y monitoreo de sus recursos. Esto resultará en una mejora de la productividad en un 20%, al optimizar el uso de los recursos disponibles en los centros educativos.

**Features Assumptions:**

- Acceso a Notificaciones y Actualizaciones:
  - Sistema de Notificaciones en Tiempo Real: Implementar una funcionalidad que envíe notificaciones automáticas sobre eventos importantes y cambios en la aplicación, permitiendo a los usuarios reaccionar rápidamente. Esto ayudará a que el 80% de los usuarios estén al tanto de las actualizaciones dentro de las primeras 24 horas.
- Reducción del Tiempo de Familiarización:
  - Interfaz Intuitiva y Fácil de Usar: Desarrollar una interfaz que sea simple e intuitiva, reduciendo el tiempo de aprendizaje en un 30%. Se espera que el 90% de los usuarios puedan dominar las funciones principales en menos de una semana sin necesidad de capacitación adicional.
- Mejora en el Control de Inventarios:
  - Gestión de Inventarios de Recursos: Crear una funcionalidad que permita a los usuarios registrar y gestionar el inventario de equipos y recursos en su centro educativo. Esto incrementará el control y monitoreo de los recursos en un 25%, mejorando la productividad en un 20% al optimizar el uso de los mismos.

* Monitoreo del ambiente mediante IoT:
  - Incorporación de sensores que permitan detectar la presencia de personas, así como medir la temperatura y humedad en los ambientes educativos.

#### 1.2.2.3. Lean UX Hypothesis Statements

- Nosotros creemos que los usuarios necesitan una aplicación que les permita gestionar los espacios de su centro educativo de manera eficiente. Sabremos que es verdad cuando al menos el 50% de usuarios adquiera los planes de suscripción durante el primer mes.
- Nosotros creemos que al contar con una interfaz intuitiva, visualmente atractiva y sea fácil de usar reducirá la tasa de abandono del sistema. Sabremos que es verdad cuando al menos el 70% de los usuarios continúen utilizando la plataforma después del primer mes.
- Nosotros creemos que el monitoreo en tiempo real mediante tecnologías IoT (presencia, temperatura, humedad y consumo energético) aportará valor a los usuarios en la gestión de los espacios. Sabremos que es verdad cuando los usuarios utilicen activamente estas funcionalidades y las consideren relevantes en la toma de decisiones operativas.

#### 1.2.2.4. Lean UX Canvas

![Lean UX Canvas](assets/chapter-I/lean-ux-canvas.png)

## 1.3. Segmentos objetivo

Nuestra aplicación se enfoca en optimizar la gestión de espacios educativos y la coordinación del personal a través de una plataforma integral. EduSpace facilita la grabación de aulas, espacios deportivos y entornos personales, y permite una gestión detallada de los recursos. Además, automatiza la nómina y proporciona un control completo del inventario de equipos y recursos con valoraciones contables. Los usuarios capturan información sobre sus actividades y necesidades operativas para mejorar la eficiencia y la comunicación. Así, nuestros segmentos objetivo serán los siguientes:

**Administradores de instituciones educativas**

- Edad: 35 a 60 años
- Perfil: Directivos, coordinadores académicos, personal administrativo encargados de la gestión operativo de institución educativa.
- Uso de tecnología: Intermedio
- Necesidad principal: Optimizar la gestión de espacios, recursos y personal de manera centralizada.
- Beneficios buscados: Tener mayor control operativo, reducción de errores, ahorro de tiempo y mejora en la toma de decisiones.

**Características demográficas:** Profesionales entre 35 a 60 años, de género masculino y femenino, con formación en gestión educativa, administración o especialidades afines, que trabajan solamente en instituciones educativas.

**Características geográficas:** Principalmente ubicados en zonas urbanas de Perú, especialmente Lima Metropolitana, donde existen instituciones educativas con infraestructuras grandes y complejas.

**Docentes y auxiliares**

- Edad: 22 a 65 años
- Perfil: Profesores y personal de apoyo que utilizan los espacios educativos de las instituciones donde trabajan para desarrollar sus actividades diarias.
- Uso de tecnología: Básico a intermedio
- Necesidad principal: Acceder rápidamente a información sobre la disponibilidad de espacios y coordinar actividades sin complicaciones.
- Beneficios buscados: Acceso rápido a la información sobre los recursos y espacios disponibles, mejor comunicación y menos errores en la asignación de espacios.

**Características demográficas:** Profesionales del sector educativo entre 22 a 65 años, de género masculino y femenino, con formación académica en sus respectivas disciplinas (ciencias, literatura, entre otros), con experiencia en enseñanza.

**Características geográficas:** Principalmente ubicados en instituciones educativas con infraestructura compleja de zonas urbanas o semiurbanas de Perú, especialmente Lima Metropolitana.

---

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores

### 2.1.1. Análisis competitivo

El análisis competitivo permite identificar las soluciones existentes que abordan el monitoreo de espacios, consumo energético y condiciones ambientales mediante tecnologías IoT. A partir de este análisis, se evalúan plataformas como Siemens, Cisco, Honeywell y Spacewell, las cuales ofrecen soluciones avanzadas orientadas a entornos corporativos.

<table border="1" cellpadding="10" cellspacing="0" style="margin-left: auto; margin-right: auto;">
  <tr>
    <th colspan="7">Competitive Analysis Landscape</th>
  </tr>
  <tr>
    <td colspan="2" rowspan="2">¿Por qué llevar a cabo este análisis?</td>
    <td colspan="5">¿Cómo se posicionan las soluciones actuales de monitoreo inteligente de espacios frente a una propuesta enfocada en el entorno educativo, y qué oportunidades existen para diferenciarse mediante especialización y analítica en tiempo real?</td>
  </tr>
  <tr>
    <td colspan="5">Identificar cómo las soluciones actuales de smart buildings gestionan espacios, energía y monitoreo, y determinar cómo una solución enfocada en entornos educativos puede diferenciarse mediante especialización, accesibilidad y lógica académica.</td>
  </tr>
  <tr>
   <td colspan="2">Nombre y logo</td>
    <td style="text-align: center;">EduSpace<br> <img src="https://github.com/user-attachments/assets/aa72b842-fa31-4a24-b10b-7d3444705e3d" alt="logo-eduspace" width="50"/>  </td>
    <td style="text-align: center;">Siemens Smart Infrastructure<br> <img src="https://github.com/user-attachments/assets/1ff299ad-8e8f-4c1d-aa55-7c1ad7fd085c" alt="logo-siemens" width="50"/> </td>
    <td style="text-align: center;">Cisco Spaces<br> <img src="https://github.com/user-attachments/assets/d0ed6004-fbc8-4252-8b82-0b329cd4e83a" alt="logo-cisco" width="50"/> </td>
    <td style="text-align: center;">Honeywell Building Tech <img src="https://github.com/user-attachments/assets/a25810df-41e8-41f5-879c-5ebe228763c0" alt="logo-honeywell" width="50"/> </td>
    <td style="text-align: center;">Spacewell<br> <img src="https://github.com/user-attachments/assets/a25810df-41e8-41f5-879c-5ebe228763c0" alt="logo-spacewell" width="50"/> </td> 
  </tr>
  <tr>
    <td rowspan="2">Perfil</td>
    <td>Overview</td>
    <td>Plataforma IoT enfocada en instituciones educativas que monitorea ocupación, ambiente y consumo energético en aulas, generando analítica y alertas en tiempo real</td>
    <td>Ecosistema integral de automatización de edificios inteligentes que incluye energía, seguridad, climatización y analítica avanzada</td>
    <td>Plataforma de analítica de espacios basada en ubicación mediante WiFi, enfocada en comportamiento de usuarios</td>
    <td>Plataforma de gestión de edificios que integra monitoreo ambiental, energía, seguridad y automatización</td>
    <td>Plataforma de facility management que optimiza el uso de espacios de trabajo mediante IoT, sensores y analítica</td>
  </tr>
  <tr>
    <td>Ventaja competitiva ¿Qué valor ofrece a los clientes?</td>
    <td>Especialización en educación + integración con horarios académicos + modelo accesible + lógica de scoring y alertas inteligentes</td>
    <td>Alta precisión, confiabilidad y soluciones completas a gran escala</td>
    <td>Analítica avanzada de ocupación con mapas de calor y comportamiento</td>
    <td>Integración completa de sistemas físicos del edificio + experiencia industrial</td>
    <td>Enfoque en optimización de espacios de trabajo + integración de datos IoT + enfoque en experiencia del usuario</td>
  </tr>
  <tr>
    <td rowspan="2">Perfil de Marketing</td>
    <td>Mercado objetivo</td>
    <td>Instituciones educativas con grandes y pequeñas infraestructuras que buscan optimizar la gestión de sus espacios y recursos.</td>
    <td>Grandes empresas e instituciones que buscan centralizar la gestión de sus instalaciones con un enfoque en sostenibilidad.</td>
    <td>Empresas, retail, oficinas corporativas, que requieren soluciones fáciles de usar para la gestión de instalaciones.</td>
    <td>Grandes instituciones y empresas que necesitan una solución completa para la gestión de sus instalaciones y recursos.</td>
    <td>Industrias, edificios comerciales, hospitales</td>
  </tr>
  <tr>
    <td>Estrategias de marketing</td>
    <td>Marketing dirigido a administradores de grandes y de pequeñas instituciones educativas, destacando la eficiencia y el control exhaustivo de recursos.</td>
    <td>Enfoque en la sostenibilidad y la eficiencia, con campañas dirigidas a administradores de instalaciones y responsables de sostenibilidad.</td>
    <td>Enfoque en la simplicidad y efectividad, con marketing dirigido a usuarios que buscan facilidad de uso en la gestión de instalaciones.</td>
    <td>Posicionamiento como solución de analítica inteligente basada en datos</td>
    <td>Campañas dirigidas a grandes organizaciones que necesitan una solución robusta y completa para la gestión de sus instalaciones.</td>
  </tr>
  <tr>
    <td rowspan="3">Perfil de Producto</td>
    <td>Productos & Servicios</td>
    <td>Monitoreo de aulas, dashboard en tiempo real, sistema de alertas, score de eficiencia, analítica histórica, integración con backend académico</td>
    <td>Automatización HVAC, control energético, seguridad, analítica avanzada, mantenimiento predictivo.</td>
    <td>Mapas de calor, conteo de personas, analítica de comportamiento, optimización de espacios</td>
    <td>Control de climatización, energía, seguridad, monitoreo ambiental, mantenimiento</td>
    <td>Gestión de espacios, sensores de ocupación, reservas de espacios, analítica de uso, facility management</td>
  </tr>
  <tr>
    <td>Precios & Costos</td>
    <td>Planes de suscripción, basados en la escala de la institución educativa y el número de funcionalidades utilizadas. </td>
    <td>Precios basados en suscripciones, ajustados según la cantidad de instalaciones y funcionalidades requeridas.</td>
    <td>Planes de suscripción con diferentes niveles de servicio, ajustados según el tamaño de la institución y sus necesidades.</td>
    <td>Precios altos por la adquisición de licencias e implementación de insfraestructuras.</td>
    <td>Precios personalizados basados en la escala y complejidad de la implementación para grandes organizaciones.</td>
  </tr>
  <tr>
    <td>Canales de distribución (Web y/o Móvil)</td>
    <td>Plataforma web y aplicación móvil.</td>
    <td>Plataforma web con soporte para aplicaciones móviles y monitoreo en tiempo real.</td>
    <td>Plataforma SaaS basada en cloud</td>
    <td>Soluciones empresariales personalizadas</td>
    <td>Plataforma SaaS (web) + integraciones empresariales</td>
  </tr>
  <tr>
    <td rowspan="5">Analisis SWOT</td>
  </tr>
 <tr>
    <td>Fortalezas</td>
    <td>Enfoque educativo; bajo costo; integración con horarios, aulas y docentes; dashboard con alertas y score; fácil adaptación a universidades/colegios.</td>
    <td>Marca global; alta confiabilidad; soluciones completas; gran experiencia en automatización.</td>
    <td>Analítica avanzada de ocupación; mapas de calor; uso de infraestructura WiFi existente.</td>
    <td>Experiencia industrial; integración de energía, seguridad y ambiente; soluciones robustas.</td>
    <td>Fuerte en gestión de espacios; usa IoT y analítica; modelo SaaS; enfoque en experiencia de usuario.</td>
  </tr>
  <tr>
    <td>Debilidades</td>
    <td>Menor precisión frente a soluciones industriales; dependencia de sensores básicos; requiere validación en campo; menor reputación inicial.</td>
    <td>Costos muy altos; implementación compleja; poco enfoque específico en educación.</td>
    <td>Depende de red WiFi robusta; menor enfoque en variables ambientales; no especializado en aulas.</td>
    <td>Alto costo; instalación compleja; enfoque generalista, no educativo.</td>
    <td>Orientado a oficinas/coworking; requiere integración empresarial; costo elevado para instituciones pequeñas.</td>
  </tr>
  <tr>
    <td>Oportunidades</td>
    <td>Crecimiento de smart campus; transformación digital educativa; optimización de aulas; integración futura con IA y predicción de uso.</td>
    <td>Expansión de smart buildings y smart cities; demanda de eficiencia energética.</td>
    <td>Mayor interés por analítica de espacios e híbrido laboral; expansión a campus.</td>
    <td>Crecimiento de edificios sostenibles e inteligentes; mantenimiento predictivo.</td>
    <td>Crecimiento del trabajo híbrido; demanda de optimización de espacios; posible expansión a educación.</td>
  </tr>
  <tr>
    <td>Amenazas</td>
    <td>Grandes empresas pueden adaptar sus soluciones al sector educativo; presupuestos limitados; resistencia al cambio tecnológico.</td>
    <td>Startups más económicas y especializadas; soluciones modulares más accesibles.</td>
    <td>Competidores IoT más completos; privacidad de datos de ubicación.</td>
    <td>Soluciones ágiles más baratas; adopción lenta por costos altos.</td>
    <td>Soluciones especializadas en educación; competidores con hardware más económico; barreras de adopción por costo.</td>
  </tr>
</table>

### 2.1.2. Estrategias y tácticas frente a competidores

Con base en el análisis competitivo realizado, se identificaron las principales fortalezas, debilidades, oportunidades y amenazas de las soluciones actuales en el ámbito de smart buildings y gestión de espacios, como Siemens, Cisco Spaces, Honeywell y Spacewell. Este análisis permite definir un conjunto de estrategias y tácticas que orienten a Smart Campus IoT a posicionarse como una solución diferenciada, accesible y especializada en el sector educativo.

A continuación, se detallan las estrategias y tácticas propuestas:

#### **Frente a las fortalezas de los competidores**

Los competidores analizados destacan por:

- Alto nivel de automatización y precisión en sus sistemas
- Soluciones integrales a gran escala (energía, seguridad, infraestructura)
- Amplia experiencia y posicionamiento en el mercado
- Uso de tecnologías avanzadas como IA, Big Data y analítica predictiva

##### **Fortalezas de Smart Campus IoT:**

- Especialización en el sector educativo
- Integración con procesos académicos (aulas, horarios, docentes)
- Bajo costo de implementación
- Flexibilidad y escalabilidad modular
- Enfoque en analítica aplicada a la toma de decisiones académicas

##### **Estrategias**

- Diferenciar la propuesta mediante un enfoque específico en educación.
- Posicionar la solución como una herramienta de gestión académica basada en datos.
- Priorizar la simplicidad y accesibilidad frente a soluciones complejas y costosas.

##### **Tácticas**

- Desarrollar dashboards orientados a indicadores académicos (uso de aulas, eficiencia).
- Comunicar el valor del sistema en términos de mejora del aprendizaje y optimización de recursos.
- Implementar módulos iniciales simples que puedan escalar progresivamente.

#### **Frente a las debilidades de los competidores**

Se identificaron las siguientes debilidades en los competidores:

- Alto costo de implementación
- Complejidad técnica e infraestructura pesada
- Falta de enfoque en el sector educativo
- Limitada adaptación a procesos académicos específicos

##### **Debilidades de Smart Campus IoT:**

- Menor precisión frente a soluciones industriales
- Dependencia de sensores de bajo costo
- Limitada validación en escenarios reales

##### **Estrategias**

- Aprovechar la falta de especialización educativa de los competidores.
- Enfocar la solución en necesidades concretas de instituciones educativas.
- Diseñar un sistema fácil de implementar y mantener.

##### **Tácticas**

- Desarrollar funcionalidades específicas como monitoreo por horario académico y score de aula.
- Realizar pilotos en instituciones educativas para validar el sistema.
- Optimizar el uso de sensores accesibles manteniendo precisión suficiente para el contexto educativo.

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

Para comprender el dominio del negocio de EduSpace en su totalidad, el equipo llevó a cabo una sesión de Big Picture EventStorming de manera colaborativa. El objetivo principal fue identificar los eventos de dominio más relevantes del sistema, mapear a los actores involucrados y descubrir los bounded contexts de forma natural a partir del flujo de eventos.

La sesión se desarrolló de forma remota utilizando LucidChart como herramienta de trabajo colaborativo. El proceso siguió las siguientes etapas:

1. **Exploración caótica:** Cada miembro del equipo colocó libremente todos los Domain Events que consideró relevantes para el negocio de EduSpace, sin ningún orden establecido. Se utilizaron sticky notes naranjas siguiendo la convención estándar de EventStorming.
2. **Ordenamiento cronológico:** Una vez generados los eventos, el equipo los ordenó en una línea de tiempo de izquierda a derecha, agrupándolos según su secuencia natural dentro del flujo del negocio.
3. **Identificación de actores y sistemas externos:** Se asoció a cada evento el actor que lo origina, ya sea una persona (Admin o Teacher) o un sistema externo (ESP32, Edge API, Web API), utilizando sticky notes amarillas para personas y rojas para sistemas.
4. **Identificación de hotspots:** El equipo marcó con sticky notes rosas los puntos de duda, conflicto o incertidumbre que requieren decisiones de diseño o aclaraciones futuras.
5. **Descubrimiento de Bounded Contexts:** Finalmente, se agruparon los eventos relacionados en bounded contexts, delimitados con rectángulos punteados. Este paso permitió identificar las fronteras naturales del dominio y sirvió como base para el diseño estratégico del sistema.

Como resultado de la sesión se identificaron seis bounded contexts: Identity & Access Management, Profile Management, Space & Resource Management, Reservation & Scheduling, Breakdown Management y el nuevo IoT Monitoring, incorporado para soportar el monitoreo en tiempo real de condiciones ambientales y ocupación de aulas mediante dispositivos IoT.

A continuación se presenta el diagrama resultante de la sesión:

![Big Picture Event Storming](/assets/images/big-picture-event-storming.png)

## 2.5. Ubiquitous Language

---

# Capítulo III: Requirements Specification

## 3.1. User Stories

| Epic / Story ID | Título | Descripción | Criterios de Aceptación | Relacionado con (Epic ID) |
| --------------- | ------ | ----------- | ----------------------- | ------------------------- |
|                 |        |             |                         |                           |

## 3.2. Impact Mapping

## 3.3. Product Backlog

| # Orden | User Story ID | Título | Descripción | Story Points (1/2/3/5/8) |
| ------- | ------------- | ------ | ----------- | ------------------------ |
|         |               |        |             |                          |

---

# Capítulo IV: Solution Software Design

## 4.1. Strategic-Level Domain-Driven Design

En este capítulo, el equipo presenta las decisiones de diseño estratégico para la solución EduSpace IoT, aplicando los principios de Domain-Driven Design (DDD). El objetivo de este nivel de diseño es identificar y definir los bounded contexts que conforman el sistema, comprender cómo interactúan entre sí y establecer una arquitectura clara que soporte tanto las funcionalidades existentes de gestión de espacios como las nuevas capacidades de monitoreo IoT. Las secciones a continuación abarcan las sesiones de Design-Level EventStorming, el proceso de Candidate Context Discovery, el modelado de Domain Message Flows, los Bounded Context Canvases, el Context Mapping y los diagramas de Arquitectura de Software.

### 4.1.1. Design-Level EventStorming

Tomando como base el Big Picture EventStorming realizado en el Capítulo II, el equipo llevó a cabo una serie de sesiones de Design-Level EventStorming con el objetivo de modelar cada bounded context con mayor nivel de detalle. A diferencia de la sesión de Big Picture, que se enfocó en comprender el dominio del negocio a alto nivel, el Design-Level EventStorming profundiza en la mecánica interna de cada contexto, incorporando Commands, Aggregates, Policies y Read Models junto a los Domain Events.

Las sesiones se realizaron de forma colaborativa utilizando LucidChart como herramienta de modelado, y abarcaron los seis bounded contexts identificados durante la sesión de Big Picture: Identity & Access Management, Space & Resource Management, Reservation & Scheduling, Breakdown Management y el nuevo contexto de IoT Monitoring. Se prestó especial atención al contexto de IoT Monitoring, al ser la incorporación principal de esta iteración e introducir nuevos actores como el dispositivo ESP32 y el Edge API.

A continuación se presentan los diagramas resultantes para cada bounded context.

![Design Level Event Storming](/assets/images/design-level-event-storming.png)

#### 4.1.1.1. Candidate Context Discovery

A partir del Design-Level EventStorming realizado, el equipo llevó a cabo el proceso de Candidate Context Discovery con el objetivo de identificar y delimitar los bounded contexts del sistema. Para ello se aplicó la técnica look-for-pivotal-events, que consiste en identificar los eventos clave del negocio que marcan cambios de estado significativos entre diferentes partes del proceso, y que naturalmente señalan las fronteras entre contextos.

Como resultado del análisis, se identificaron seis bounded contexts. A continuación se presenta cada uno con su justificación:

| #   | Bounded Context                           | Eventos pivote que delimitan su frontera                                                                | Justificación                                                                                                                                                                                                                                                                                                                                                                                                                           |
| --- | ----------------------------------------- | ------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | **Identity, Access & Profile Management** | `AdminAccountCreated`, `TeacherAccountCreated`, `SessionStarted`                                        | Agrupa todo lo relacionado con la autenticación, control de acceso y gestión de perfiles de usuario. Es el contexto de entrada obligatorio para cualquier usuario y concentra tanto las credenciales de acceso como la información personal asociada a cada cuenta.                                                                                                                                                                     |
| 2   | **Space & Resource Management**           | `ClassroomRegistered`, `SharedAreaRegistered`, `ResourceAddedToClassroom`, `TeacherAssignedToClassroom` | Agrupa la configuración y administración de todos los espacios físicos e inventario de recursos de la institución. Es el contexto core del negocio original.                                                                                                                                                                                                                                                                            |
| 3   | **Reservation & Scheduling**              | `SharedAreaReserved`, `ReservationConfirmed`, `MeetingScheduled`, `TeacherInvitedToMeeting`             | Gestiona la planificación y reserva de espacios compartidos y reuniones. Se separa de Space & Resource Management porque opera sobre disponibilidad y tiempo, no sobre el registro de espacios.                                                                                                                                                                                                                                         |
| 4   | **Breakdown Management**                  | `BreakdownReported`, `ReportStatusUpdated`                                                              | Concentra el ciclo de vida completo de los reportes de averías, desde su creación por un docente hasta su resolución por el administrador.                                                                                                                                                                                                                                                                                              |
| 5   | **IoT Monitoring**                        | `SensorReadingCaptured`, `EnvironmentalThresholdExceeded`, `OccupancyStatusChanged`, `AlertGenerated`   | Contexto nuevo incorporado en esta iteración. Gestiona la captura, procesamiento y visualización de datos provenientes de los dispositivos IoT instalados en las aulas, así como la generación de alertas automáticas. Se delimita como contexto independiente debido a que introduce nuevos actores (ESP32, Edge API), un flujo de datos completamente distinto al resto del sistema y requisitos técnicos propios del mundo embebido. |

#### 4.1.1.2. Domain Message Flows Modeling

En esta sección el equipo modeló los flujos de mensajes entre los bounded contexts identificados, con el objetivo de visualizar cómo colaboran entre sí para resolver los casos de negocio más importantes del sistema. Para ello se aplicó la técnica de Domain Storytelling, que permite representar de forma narrativa y visual cómo los actores, los sistemas y los bounded contexts se comunican e intercambian información a través de work objects (documentos, datos o mensajes).

Se modelaron los siguientes casos de negocio, seleccionados por su relevancia e impacto en el sistema:

1. Registro de un docente y acceso a la plataforma
2. Reserva de un espacio compartido por un docente
3. Monitoreo IoT y generación de alertas

A continuación se presentan los diagramas de Domain Storytelling para cada caso:

**Caso 1: Registro de docentes y acceso a plataforma**

Este flujo modela cómo el administrador registra la cuenta de un nuevo docente en el sistema y cómo este último accede a la plataforma. El bounded context de Identity, Access & Profile Management es el único involucrado, al ser el responsable tanto de la creación de cuentas como de la autenticación. El administrador envía las credenciales del docente al sistema, que confirma el registro. Posteriormente, el docente inicia sesión con sus credenciales y el sistema le carga el dashboard correspondiente a su rol.

![Domain Message Flow Model 1](/assets/images/message-flow1.png)

**Caso 2: Reserva de espacio compartido**

Este flujo ilustra la colaboración entre los bounded contexts de Reservation & Scheduling y Space & Resource Management. El docente consulta la disponibilidad de un espacio compartido, el sistema le retorna el calendario de disponibilidad, y el docente realiza la solicitud de reserva. Para confirmarla, Reservation & Scheduling consulta los datos del espacio a Space & Resource Management, que le responde con la información necesaria. Finalmente, el sistema confirma la reserva al docente.

![Domain Message Flow Model 2](/assets/images/message-flow2.png)

**Caso 3: Monitoreo IoT y generación de alertas**

Este flujo modela el nuevo proceso incorporado en esta iteración. El dispositivo ESP32 captura lecturas de los sensores y las envía al Edge API, que las procesa y las reenvía al bounded context de IoT Monitoring. Este contexto evalúa internamente los umbrales configurados y, en caso de detectar una condición anormal, genera una alerta que notifica al bounded context de Identity, Access & Profile Management para que informe a los usuarios correspondientes. Adicionalmente, tanto administradores como docentes pueden consultar el dashboard de IoT Monitoring para visualizar el estado ambiental de las aulas en tiempo real.

![Domain Message Flow Model 3](/assets/images/message-flow3.png)

#### 4.1.1.3. Bounded Context Canvases

Con el fin de detallar el diseño de cada bounded context identificado durante las sesiones de EventStorming, el equipo elaboró un Bounded Context Canvas por cada contexto, siguiendo la estructura propuesta por el DDD Crew (V4). Este artefacto permite documentar de forma estructurada la descripción del contexto, su clasificación estratégica, el lenguaje ubicuo específico, las decisiones de negocio clave y los flujos de comunicación entrante y saliente con otros colaboradores del sistema.

Los canvases se presentan en orden de importancia para el negocio, comenzando por el contexto core de la nueva iteración IoT y continuando con los contextos de soporte existentes.

A continuación se presentan los cinco Bounded Context Canvases elaborados:

**Iot Monitoring**

![Bounded Context Canvas IoT Monitoring](/assets/images/context-canvas-iot-monitoring.png)

**Space & Resource Management**

![Bounded Context Canvas Space and Resource Management](/assets/images/context-canvas-space-resource-management.png)

**Reservation & Scheduling**

![Bounded Context Canvas Reservation & Scheduling](/assets/images/context-canvas-reservation-scheduling.png)

**Breakdown Management**

![Bounded Context Canvas Breakdown Management](/assets/images/context-canvas-breakdown-management.png)

**IAM & Profile Management**

![Bounded Context Canvas IAM & Profile Management](/assets/images/context-canvas-iam-profile-management.png)

### 4.1.2. Context Mapping

En esta sección el equipo elaboró el Context Map de la plataforma EduSpace IoT, con el objetivo de visualizar las relaciones estructurales entre los bounded contexts identificados y definir los patrones de integración que gobiernan dichas relaciones. Para ello se analizaron las dependencias entre contextos identificadas durante las sesiones de EventStorming y los Bounded Context Canvases, evaluando alternativas de integración y seleccionando los patrones más adecuados según la naturaleza de cada relación.

Los patrones de relación entre Bounded Contexts aplicados en este Context Map son los siguientes:

- Customer/Supplier (C/S): El contexto downstream (customer) depende del contexto upstream (supplier). El supplier define la interfaz y el customer la consume.
- Conformist (CF): El contexto downstream adopta el modelo del upstream sin modificaciones, adaptándose completamente a él.
- Anti-Corruption Layer (ACL): El contexto downstream traduce el modelo del upstream a través de una capa de traducción para proteger su propio modelo de dominio.

A continuación se presenta el diagrama de Context Mapping resultante:

![Context Map](/assets/images/context-map_ContextMap.png)

### 4.1.3. Software Architecture

Para la representación de la arquitectura de software de la plataforma EduSpace IoT, el equipo aplicó el modelo C4 (Context, Container, Component, Code), utilizando Structurizr DSL como herramienta de modelado. Este modelo permite describir la arquitectura en diferentes niveles de abstracción, facilitando la comunicación entre los distintos stakeholders del proyecto. A continuación se presentan los diagramas correspondientes a los niveles de System Landscape, System Context, Container y Deployment.

#### 4.1.3.1. Software Architecture System Landscape Diagram

El diagrama de System Landscape presenta una visión general del ecosistema de la plataforma EduSpace IoT, mostrando el sistema principal en relación con los actores que lo utilizan y los sistemas externos con los que interactúa. En este nivel de abstracción, el sistema se representa como una caja única sin detallar su estructura interna.

Los actores identificados son el Administrador, responsable de la gestión institucional y la configuración del monitoreo IoT, y el Docente, quien utiliza la plataforma para reservar espacios, reportar averías y consultar el estado ambiental de las aulas. El único sistema externo con el que interactúa EduSpace IoT es SendGrid, servicio de entrega de correos electrónicos utilizado para el envío de notificaciones y verificaciones a los usuarios.

![System Landscape Diagram Key](/assets/images/c4-system-landscape-key.png)

![System Landscape Diagram](/assets/images/c4-system-landscape.png)

#### 4.1.3.2. Software Architecture Context Level Diagrams

El diagrama de System Context profundiza en las relaciones directas entre la plataforma EduSpace IoT, sus usuarios y los sistemas externos. A diferencia del System Landscape, este diagrama se centra exclusivamente en el sistema principal y sus interacciones inmediatas.

Dado que EduSpace IoT es una plataforma independiente que no se integra con otros sistemas institucionales externos más allá de SendGrid, el diagrama de System Context coincide con el System Landscape en términos de elementos representados. Esta situación es consistente con el alcance del proyecto, que no contempla integraciones con sistemas de gestión universitaria externos como ERP o SIS institucionales.

![System Context Diagram Key](/assets/images/c4-system-context-key.png)

![System Context Diagram](/assets/images/c4-system-context.png)

#### 4.1.3.3. Software Architecture Container Level Diagrams

El diagrama de Containers desglosa la estructura interna de la plataforma EduSpace IoT, mostrando los contenedores de software que la componen, sus responsabilidades y las relaciones entre ellos. Este nivel de abstracción permite visualizar las principales decisiones tecnológicas y la distribución de responsabilidades entre los distintos componentes del sistema.

La plataforma está compuesta por los siguientes contenedores: la Landing Page como sitio web estático, la Web Application como SPA desarrollada en Vue.js, la Mobile Application desarrollada en Flutter, el Web API como backend RESTful desarrollado en ASP.NET Core que implementa la lógica de negocio de todos los bounded contexts, el Edge API desarrollado en Flask que actúa como intermediario entre los dispositivos IoT y el Web API, la Embedded Application en MicroPython que corre directamente en el ESP32, la Base de Datos principal en PostgreSQL y la Edge Database en SQLite para el almacenamiento local en el Edge API.

![Container Diagram Key](/assets/images/c4-container-key.png)

![Container Diagram](/assets/images/c4-container.png)

#### 4.1.3.4. Software Architecture Deployment Diagrams

El diagrama de Deployment muestra cómo los contenedores de la plataforma EduSpace IoT se distribuyen en la infraestructura de despliegue. Este diagrama refleja las decisiones de infraestructura tomadas para el entorno de producción del proyecto.

La Landing Page se despliega en GitHub Pages por su naturaleza estática y gratuidad. La Web Application se despliega en Netlify, plataforma que ofrece despliegue continuo desde GitHub. La Mobile Application se distribuye mediante Firebase App Distribution para pruebas en dispositivos físicos. El Web API, el Edge API, la Edge Database y la Base de Datos PostgreSQL se despliegan en Railway, plataforma de hosting en la nube que permite gestionar múltiples servicios en un mismo entorno. Finalmente, la Embedded Application reside directamente en el microcontrolador ESP32, instalado físicamente en el aula monitoreada.

![Deplyment Diagram Key](/assets/images/c4-deployment-key.png)

![Deployment Diagram](/assets/images/c4-deployment.png)

## 4.2. Tactical-Level Domain-Driven Design

En este capítulo el equipo presenta el diseño táctico de la solución EduSpace IoT, aplicando los principios y patrones de Domain-Driven Design a nivel de bounded context. Para cada contexto delimitado identificado en la sección 4.1 se describe el conjunto de clases que lo componen, organizadas en cuatro capas: Domain Layer, Interface Layer, Application Layer e Infrastructure Layer. Este nivel de diseño permite establecer con precisión las responsabilidades de cada componente del sistema, las invariantes del dominio y los mecanismos de comunicación entre capas, proporcionando una base sólida para la implementación posterior.

La numeración de los bounded contexts en esta sección sigue el orden de importancia estratégica definido durante el proceso de diseño estratégico. El contexto de IoT Monitoring recibe el número 4.2.5 por tratarse del quinto contexto en dicho ordenamiento, siendo al mismo tiempo el de mayor novedad en esta iteración del proyecto al incorporar la capa IoT de la solución.

### 4.2.1. Bounded Context: IAM & Profile Management

El contexto de IAM & Profile Management concentra la responsabilidad de autenticación, autorización y gestión del ciclo de vida de los perfiles de usuario en la plataforma EduSpace IoT. Es el punto de entrada que toda sesión de usuario debe atravesar antes de acceder a cualquier otro contexto, y es el custodio de la identidad tanto de administradores como de docentes. Internamente se compone de dos sub-dominios coordinados mediante una ACL bidireccional: el sub-dominio **IAM** (Identity & Access Management), que gobierna credenciales, roles y el flujo de autenticación de dos factores por correo electrónico; y el sub-dominio **Profiles**, que gestiona los datos personales y la vinculación entre una cuenta de sistema y el perfil de persona que la representa. IAM expone la fachada `IIamContextFacade` (operación `CreateAccount`) para que Profiles pueda aprovisionar cuentas en nombre de un nuevo usuario. Profiles, a su vez, expone `IProfilesContextFacade` (operaciones `ValidateTeacherProfileIdExistence` y `ValidateAdminProfileIdExistence`) para que otros bounded contexts puedan verificar la existencia de un perfil sin acceder directamente a su modelo.

La incorporación del aggregate `VerificationCode` constituyó la adición propia de esta iteración IoT: el flujo de autenticación pasó de una verificación directa de credenciales a un proceso de dos pasos en el que el sistema emite un código numérico de seis dígitos con expiración de diez minutos y lo entrega al usuario mediante correo electrónico antes de emitir el JWT de sesión.

#### 4.2.1.1. Domain Layer

El Domain Layer de este bounded context define las reglas de identidad y de composición de perfiles que ninguna otra capa debe vulnerar: qué constituye una cuenta válida, cuáles son los roles posibles del sistema, cuándo un código de verificación puede considerarse vigente, y cuál es la estructura mínima que un perfil de administrador o docente debe satisfacer. Esta capa es independiente de toda infraestructura y publica los contratos de repositorio que la Infrastructure Layer debe implementar.

Los aggregates centrales de IAM son `Account`, que porta las credenciales hasheadas y el rol del usuario, y `VerificationCode`, incorporado en la iteración actual para soportar el flujo 2FA. En el sub-dominio Profiles, la clase base `Profile` concentra los datos comunes de persona (nombre, información privada y referencia a la cuenta), de la cual heredan los aggregates concretos `AdminProfile` y `TeacherProfile`; este último extiende el modelo con el atributo `AdministratorId`, que establece la relación de supervisión entre ambos roles. Los value objects `ProfileName`, `ProfilePrivateInformation` y `AccountId` encapsulan invariantes de composición y evitan la exposición de primitivos en las firmas del modelo.

| Clase | Tipo | Responsabilidad |
| --- | --- | --- |
| `Account` | Aggregate Root | Gestiona las credenciales de acceso al sistema. Atributos: `Id`, `Username`, `PasswordHash` (serializado con `[JsonIgnore]`), `Role` (ERoles). Expone métodos `UpdateUsername`, `UpdatePasswordHash` y `GetRole`. |
| `VerificationCode` | Aggregate Root (adición IoT) | Representa el código numérico de 6 dígitos generado durante el flujo 2FA por email. Atributos: `Id`, `AccountId` (FK), `Code`, `ExpirationDate`, `IsUsed`. Vinculado a `Account` mediante navegación. Su ciclo de vida comienza al iniciarse sesión y concluye al ser consumido (`IsUsed = true`) o al vencer `ExpirationDate`. |
| `AdminProfile` | Aggregate Root | Perfil de administrador. Hereda de `Profile`. Implementa `Update(UpdateAdminProfileCommand)` para actualizar `ProfileName` y `ProfilePrivateInformation`. |
| `TeacherProfile` | Aggregate Root | Perfil de docente. Hereda de `Profile`. Añade `AdministratorId` (int) que establece la relación de supervisión. Implementa `Update(UpdateTeacherProfileCommand)`. |
| `Profile` | Entity (clase base) | Base abstracta con los datos comunes de persona: `ProfileName`, `ProfilePrivateInformation`, `AccountId`. Implementa `IEntityWithCreatedUpdatedDate` para campos de auditoría `CreatedAt` / `UpdatedAt`. Expone propiedades de lectura `ProfileFullName`, `ProfileEmail` y `ProfileDni`. |
| `ERoles` | Value Object (enum) | Define los dos roles posibles del sistema: `RoleAdmin` y `RoleTeacher`. |
| `ProfileName` | Value Object (record) | Encapsula `FirstName`, `LastName` y la propiedad calculada `FullName`. |
| `ProfilePrivateInformation` | Value Object (record) | Encapsula `Email`, `Dni`, `Address`, `Phone`. Expone `ObtainEmail` y `ObtainDni` como accesores explícitos. |
| `AccountId` | Value Object (record) | Envoltorio de `int Id` que referencia la cuenta IAM desde el modelo de Profiles. Evita el uso de primitivos en las asociaciones cross-aggregate. |
| `IAccountRepository` | Repository Interface | Contrato para persistir y consultar `Account`. Operaciones: `AddAsync`, `FindByUsername`, `ExistsByUsername`, `FindByIdAsync`. |
| `ITeacherProfileRepository` | Repository Interface | Contrato para persistir y consultar `TeacherProfile`. Operaciones: `AddAsync`, `ListAsync`, `FindByIdAsync`, `FindAllTeachersByAdministratorIdAsync`, `ExistsByTeacherProfileId`, `Update`, `Remove`. |
| `IAdminProfileRepository` | Repository Interface | Contrato para persistir y consultar `AdminProfile`. Operaciones: `AddAsync`, `ListAsync`, `FindByIdAsync`, `ExistsByAdminProfileId`, `Update`, `Remove`. |
| `GetAllTeachersByAdministratorIdQuery` | Query | Definida en Domain para recuperar los docentes supervisados por un administrador dado. En la iteración actual esta query no es manejada por ningún command/query service expuesto en la Interface Layer; su lógica equivalente es resuelta directamente por `TeacherProfileRepository.FindAllTeachersByAdministratorIdAsync()`. |

#### 4.2.1.2. Interface Layer

La Interface Layer de este bounded context expone tres conjuntos de endpoints REST. El primero, `AuthenticationController`, gestiona el flujo completo de autenticación de dos factores: registro de cuenta, inicio de sesión con emisión del código de verificación, y validación del código con retorno del JWT y el perfil completo del usuario. Los controladores de Profiles, `AdministratorProfilesController` y `TeachersProfilesController`, exponen operaciones CRUD sobre los perfiles de ambos roles. Esta capa no contiene lógica de dominio: su responsabilidad se limita a traducir los cuerpos HTTP en resources, delegar a la Application Layer y construir la respuesta adecuada.

Los assemblers de transformación (sufijo `FromResourceAssembler` y `FromEntityAssembler`) separan el modelo de transporte del modelo de dominio, siguiendo el patrón de ensamblado explícito adoptado en todo el Web API.

| Clase | Tipo | Endpoints / Operaciones |
| --- | --- | --- |
| `AuthenticationController` | Controller | `POST /api/v1/authentication/sign-up` — crea una cuenta de sistema (requiere autenticación de administrador). `POST /api/v1/authentication/sign-in` — valida credenciales y envía el código 2FA al correo del perfil asociado; responde con mensaje de confirmación. `POST /api/v1/authentication/verify-code` — valida el código recibido, marca el `VerificationCode` como usado y retorna un `AuthenticatedAccountResource` con el JWT, el `profileId`, y los datos cruzados del perfil (aulas y reuniones para docentes). |
| `AdministratorProfilesController` | Controller | `POST /api/v1/administrator-profiles` — crea un perfil de administrador y aprovisiona su cuenta IAM vía ACL. `GET /api/v1/administrator-profiles` — lista todos los perfiles de administrador. `GET /api/v1/administrator-profiles/{administratorId}` — obtiene un perfil por ID. `PUT /api/v1/administrator-profiles/{administratorId}` — actualiza nombre e información privada. `DELETE /api/v1/administrator-profiles/{administratorId}` — elimina el perfil. |
| `TeachersProfilesController` | Controller | `POST /api/v1/teachers-profiles` — crea un perfil de docente y aprovisiona su cuenta IAM vía ACL. `GET /api/v1/teachers-profiles` — lista todos los perfiles de docentes. `GET /api/v1/teachers-profiles/{teacherId}` — obtiene un perfil por ID. `PUT /api/v1/teachers-profiles/{teacherId}` — actualiza nombre e información privada. `DELETE /api/v1/teachers-profiles/{teacherId}` — elimina el perfil. |
| `SignUpResource` / `SignUpCommandFromResourceAssembler` | Resource / Assembler | Transporta `username`, `password` y `role` para el registro. |
| `SignInResource` / `SignInCommandFromResourceAssembler` | Resource / Assembler | Transporta `username` y `password` para el inicio de sesión. |
| `VerifyCodeResource` / `VerifyCodeCommandFromResourceAssembler` | Resource / Assembler | Transporta `username` y `code` para la verificación 2FA. |
| `AuthenticatedAccountResource` / `AuthenticatedAccountResourceFromEntityAssembler` | Resource / Assembler | Respuesta completa del flujo de verificación: `id`, `username`, `role`, `token`, `profileId`, datos de perfil (docente o administrador), aulas y reuniones asociadas. |
| `AccountResource` / `AccountResourceFromEntityAssembler` | Resource / Assembler | Representación simple de una cuenta (sin token); usada para consultas internas. |
| `CreateAdminProfileResource` / `CreateAdminProfileCommandFromResourceAssembler` | Resource / Assembler | Transporta los datos de creación de perfil de administrador (`firstName`, `lastName`, `email`, `dni`, `address`, `phone`, `password`). |
| `CreateTeacherProfileResource` / `CreateTeacherProfileCommandFromResourceAssembler` | Resource / Assembler | Transporta los datos de creación de perfil de docente, incluyendo `administratorId`. |
| `UpdateAdminProfileResource` / `UpdateAdminProfileCommandFromResourceAssembler` | Resource / Assembler | Transporta campos actualizables del perfil de administrador. |
| `UpdateTeacherProfileResource` / `UpdateTeacherProfileCommandFromResourceAssembler` | Resource / Assembler | Transporta campos actualizables del perfil de docente. |
| `AdminProfileResource` / `AdminProfileResourceFromEntityAssembler` | Resource / Assembler | Representación de lectura del perfil de administrador. |
| `TeacherProfileResource` / `TeacherProfileResourceFromEntityAssembler` | Resource / Assembler | Representación de lectura del perfil de docente. |
| `IIamContextFacade` / `IamContextFacade` | ACL (saliente de Profiles) | Interfaz + implementación que expone `CreateAccount(username, password, role)`. Consumida por `AdminProfileCommandService` y `TeacherProfileCommandService` para aprovisionar la cuenta IAM al crear un perfil. |
| `IProfilesContextFacade` / `ProfilesContextFacade` | ACL (saliente de IAM) | Interfaz + implementación que expone `ValidateTeacherProfileIdExistence(id)` y `ValidateAdminProfileIdExistence(id)`. Consumida por otros bounded contexts para verificar la existencia de un perfil sin acoplar sus modelos. |

#### 4.2.1.3. Application Layer

La Application Layer orquesta los flujos de proceso sin contener reglas de dominio propias. Los command services del sub-dominio IAM coordinan el ciclo de autenticación de dos pasos: `AccountCommandService` es el servicio central y maneja los tres comandos del flujo de autenticación. El manejo de `SignInCommand` genera el `VerificationCode`, lo persiste y delega el envío del correo al outbound service `IEmailService`. El manejo de `VerifyCodeCommand` valida el código, genera el JWT y realiza una orquestación de aplicación cross-BC: consulta `ITeacherProfileRepository` y `IAdminProfileRepository` para resolver el perfil asociado a la cuenta, y —para cuentas con rol `RoleTeacher`— invoca adicionalmente `IClassroomQueryService` y `IMeetingQueryService` de otros bounded contexts para componer la respuesta completa de sesión. Esta decisión concentra la carga de inicialización de sesión en un único punto, retornando una tupla de siete elementos que la Interface Layer serializa directamente en el `AuthenticatedAccountResource`.

En el sub-dominio Profiles, los command services `AdminProfileCommandService` y `TeacherProfileCommandService` coordinan las operaciones CRUD y la creación de cuenta IAM mediante la ACL `IExternalIamService`. Los query services `AdminProfileQueryService` y `TeacherProfileQueryService` resuelven las consultas de solo lectura expuestas en los controllers. Cabe señalar que `TeacherProfileQueryService` implementa la interfaz `ITeacherQueryService` —cuyo nombre omite el sufijo `Profile` respecto a su implementación— y que `GetAllTeachersByAdministratorIdQuery`, definida en el Domain Layer, no cuenta con un handler en esta capa; la funcionalidad equivalente se resuelve directamente en el repositorio.

| Clase | Tipo | Responsabilidad |
| --- | --- | --- |
| `AccountCommandService` | Command Service | Implementa `IAccountCommandService`. Maneja `SignUpCommand` (crea `Account` con contraseña hasheada), `SignInCommand` (valida credenciales, genera y persiste `VerificationCode`, envía código por email vía `IEmailService`) y `VerifyCodeCommand` (valida código, genera JWT, resuelve perfil y datos asociados, retorna tupla cross-BC). |
| `AccountQueryService` | Query Service | Implementa `IAccountQueryService`. Maneja `GetAccountByIdQuery` y `GetAccountByUsernameQuery` delegando a `IAccountRepository`. |
| `AdminProfileCommandService` | Command Service | Implementa `IAdminProfileCommandService`. Maneja `CreateAdministratorProfileCommand` (crea `AdminProfile` y aprovisiona cuenta IAM vía `IExternalIamService`), `UpdateAdminProfileCommand` y `DeleteAdminProfileCommand`. |
| `TeacherProfileCommandService` | Command Service | Implementa `ITeacherProfileCommandService`. Maneja `CreateTeacherProfileCommand`, `UpdateTeacherProfileCommand` y `DeleteTeacherProfileCommand`, con aprovisionamiento de cuenta IAM análogo al del servicio de administrador. |
| `AdminProfileQueryService` | Query Service | Implementa `IAdminProfileQueryService`. Maneja `GetAllAdministratorsProfileQuery` y `GetAdministratorProfileByIdQuery`. |
| `TeacherProfileQueryService` | Query Service | Implementa `ITeacherQueryService`. Maneja `GetAllTeachersProfileQuery` y `GetTeacherProfileByIdQuery`. La interfaz que implementa (`ITeacherQueryService`) presenta un nombre inconsistente respecto a su implementación; se considera una deuda de nomenclatura de la iteración actual. |
| `IEmailService` | Outbound Service (interfaz) | Contrato del servicio de envío de correo electrónico. Método: `SendEmailAsync(to, subject, body)`. Consumida por `AccountCommandService` para la entrega del código 2FA. |
| `IHashingService` | Outbound Service (interfaz) | Contrato del servicio de hashing. Métodos: `HashPassword(password)` y `VerifyPassword(password, hash)`. Consumida por `AccountCommandService` durante el registro y el inicio de sesión. |
| `ITokenService` | Outbound Service (interfaz) | Contrato del servicio de generación y validación de JWT. Métodos: `GenerateToken(account)` y `ValidateToken(token)`. Consumida por `AccountCommandService` y por el middleware de autorización. |
| `IExternalIamService` | Outbound Service / ACL (interfaz, sub-dominio Profiles) | Contrato que Profiles usa para invocar la creación de cuenta en IAM sin depender directamente de su modelo. Método: `CreateAccount(username, password, role)`. |
| `ExternalIamService` | Outbound Service / ACL (implementación) | Implementación de `IExternalIamService`. Invoca `IIamContextFacade.CreateAccount` para aprovisionar la cuenta IAM desde el sub-dominio Profiles. |

#### 4.2.1.4. Infrastructure Layer

La Infrastructure Layer provee las implementaciones concretas de los contratos definidos en el Domain Layer, utilizando Entity Framework Core como ORM sobre una base de datos MySQL 8.0, consistente con la decisión de infraestructura adoptada para todo el Web API de la plataforma EduSpace IoT. Los repositorios heredan de `BaseRepository<T>` y acceden al `AppDbContext` compartido en `Shared/Infrastructure/Persistence/EFC/Configuration/`, el cual centraliza los `DbSet` de todos los bounded contexts y aplica convenciones de nomenclatura en snake_case mediante Humanizer. Los repositorios de `TeacherProfile` y `AdminProfile` sobreescriben `ListAsync()` para incluir la carga explícita del value object `AccountId` mediante `.Include(p => p.AccountId)`, necesaria para resolver la vinculación entre el perfil y la cuenta IAM durante el flujo de autenticación.

El adaptador `TokenService` implementa la generación y validación de JWT mediante `JsonWebTokenHandler` (Microsoft.IdentityModel). La configuración de validación establece `ValidateIssuer = false` y `ValidateAudience = false`, con expiración de siete días y sin mecanismo de refresh; esta configuración responde a las decisiones de implementación del ciclo académico actual. Para el envío de correo electrónico, la infraestructura registra condicionalmente dos implementaciones de `IEmailService` según el entorno de ejecución: `MockEmailService` en desarrollo (registra el código en el log sin enviar ningún correo) y `EmailService` en producción (integración con SendGrid API mediante HTTPS, configurada vía variables de entorno `SENDGRID_API_KEY` y `SMTP_USER`). El servicio de hashing `HashingService` encapsula BCrypt.Net para la generación y verificación de contraseñas.

| Clase | Tipo | Tecnología / Responsabilidad |
| --- | --- | --- |
| `AccountRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `IAccountRepository`. Extiende `BaseRepository<Account>`. Añade `FindByUsername` (consulta LINQ por `Username`) y `ExistsByUsername` (verificación de unicidad). |
| `TeacherProfileRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `ITeacherProfileRepository`. Extiende `BaseRepository<TeacherProfile>`. Sobreescribe `ListAsync()` con `.Include(p => p.AccountId)`. Añade `FindAllTeachersByAdministratorIdAsync(id)` para filtrar docentes por administrador, y `ExistsByTeacherProfileId(id)` para validación ACL. |
| `AdminProfileRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `IAdminProfileRepository`. Extiende `BaseRepository<AdminProfile>`. Sobreescribe `ListAsync()` con `.Include(p => p.AccountId)`. Añade `ExistsByAdminProfileId(id)` para validación ACL. |
| `AppDbContext` | DbContext (compartido) | Entity Framework Core. Contexto compartido con todos los bounded contexts del API, ubicado en `Shared/Infrastructure/Persistence/EFC/Configuration/`. Define los `DbSet` para `Account`, `VerificationCode`, `AdminProfile`, `TeacherProfile` y otras entidades del sistema. Aplica convenciones snake_case mediante Humanizer. |
| `TokenService` | External Adapter (JWT) | Microsoft.IdentityModel.JsonWebTokens + HMAC SHA256. Implementa `ITokenService`. Genera tokens firmados con expiración de 7 días. Valida tokens con `ValidateIssuer = false` y `ValidateAudience = false`. Sin mecanismo de refresh en la implementación actual. |
| `HashingService` | External Adapter (BCrypt) | BCrypt.Net. Implementa `IHashingService`. Encapsula `HashPassword` y `VerifyPassword` para el ciclo de vida de contraseñas de `Account`. |
| `EmailService` | External Adapter (SendGrid — producción) | SendGrid API (HTTPS). Implementa `IEmailService`. Registrado condicionalmente en entorno de producción. Lee `SENDGRID_API_KEY`, `SMTP_USER` y `SENDGRID_FROM_NAME` de las variables de entorno. Envía el correo con el código 2FA al usuario durante el flujo `SignInCommand`. |
| `MockEmailService` | External Adapter (mock — desarrollo) | ILogger. Implementa `IEmailService`. Registrado condicionalmente en entorno de desarrollo. No realiza envíos reales; registra destinatario, asunto y cuerpo del correo mediante `ILogger<MockEmailService>` para facilitar la verificación del flujo durante el desarrollo local. |
| `RequestAuthorizationMiddleware` | Middleware (Pipeline) | Middleware de autorización basado en el atributo `[Authorize]` / `[AllowAnonymous]`. Invoca `ITokenService.ValidateToken` en cada solicitud para extraer el `accountId` del JWT y lo inyecta en el contexto HTTP. Los endpoints marcados con `[AllowAnonymous]` omiten esta validación (usados en `sign-in` y `verify-code`). |

### 4.2.2. Bounded Context: Space & Resource Management

El contexto de Space & Resource Management concentra la responsabilidad sobre la gestión de los espacios físicos del establecimiento educativo: aulas (Classroom), recursos materiales asociados a ellas (Resource) y áreas comunes disponibles para toda la institución (SharedArea). Este bounded context actúa como el registro canónico del inventario espacial de la plataforma EduSpace IoT: cualquier otro contexto que necesite validar la existencia de un aula debe consultarlo a través de su fachada ACL pública, y el propio contexto valida la identidad del docente responsable de cada aula mediante una consulta al bounded context Profiles. Los eventos de dominio identificados durante el Design-Level EventStorming que delimitan este contexto son `ClassroomCreated`, `ClassroomUpdated`, `ClassroomDeleted`, `ResourceCreated`, `ResourceUpdated`, `ResourceDeleted`, `SharedAreaCreated`, `SharedAreaUpdated` y `SharedAreaDeleted`; sin embargo, en la implementación actual estos eventos no se materializan como objetos de dominio explícitos, dado que el equipo optó por una coordinación directa entre capas vía servicios de comando y consulta.

El contexto interactúa con dos vecinos inmediatos: recibe llamadas entrantes desde BreakdownManagement (que necesita confirmar que el aula afectada por una avería existe) y emite llamadas salientes hacia Profiles (para verificar que el docente asignado a un aula tiene un perfil registrado). Ambas interacciones se canalizan exclusivamente a través de interfaces ACL, respetando el principio de autonomía de bounded context.

#### 4.2.2.1. Domain Layer

El Domain Layer del contexto Space & Resource Management encapsula las reglas de negocio relativas a la creación y modificación de espacios físicos. Las invariantes principales son: el nombre de un `Classroom` no puede estar duplicado en el sistema; la asignación de un docente a un aula requiere que ese docente exista en el bounded context Profiles (validación inyectada mediante `Func<int, bool>`); y un `Resource` solo puede pertenecer a un `Classroom` existente. Las interfaces de repositorio abstraen la persistencia de cada aggregate, permitiendo que la Infrastructure Layer provea implementaciones concretas sin contaminar el dominio.

Como decisión técnica complementaria, el equipo introdujo tres mixins de auditoría —`ClassroomAudit`, `ResourceAudit` y `SharedAreaAudit`— que encapsulan los campos `CreatedAt` y `UpdatedAt` requeridos por la librería `EntityFrameworkCore.CreatedUpdatedDate`. `ClassroomAudit` y `ResourceAudit` implementan la interfaz `IEntityWithCreatedUpdatedDate`, lo que habilita el poblado automático de fechas por parte del interceptor de EF Core. `SharedAreaAudit` declara las mismas columnas pero no implementa dicha interfaz, lo que constituye una inconsistencia menor de implementación: los campos están presentes en el esquema pero el interceptor no los pobla automáticamente para ese aggregate. El contexto no publica Domain Events.

Los Commands y Queries se definen dentro del propio Domain Layer en las carpetas `Domain/Model/Commands` y `Domain/Model/Queries`, siguiendo la convención del proyecto de mantener los mensajes junto al modelo que los consume.

| Clase | Tipo | Responsabilidad |
| --- | --- | --- |
| `Classroom` | Aggregate Root | Representa un aula del establecimiento. Atributos: `Id`, `Name`, `Description`, `TeacherId` (Value Object), colección de navegación `Resources`. Expone `UpdateTeacherId(int? teacherId, Func<int, bool> verifyProfile)` como mecanismo de validación inyectada al momento de actualizar el docente responsable. Sus propiedades utilizan `private set`. |
| `Resource` | Aggregate Root | Representa un recurso físico asociado a un aula. Atributos: `Id`, `Name`, `KindOfResource`, `ClassroomId` (FK), `Classroom` (navigation property). Sus propiedades utilizan `private set` excepto `Id` que usa `set` por requerimiento de EF Core. |
| `SharedArea` | Aggregate Root | Representa un área común de la institución. Atributos: `Id`, `Name`, `Capacity`, `Description`. A diferencia de `Classroom` y `Resource`, todas sus propiedades utilizan `public set`. |
| `TeacherId` | Value Object | Record C# que encapsula el identificador de un docente. Atributo: `TeacherIdentifier: int`. |
| `ClassroomAudit` | Mixin de auditoría | Implementa `IEntityWithCreatedUpdatedDate`. Declara `CreatedDate` (`CreatedAt`) y `UpdatedDate` (`UpdatedAt`) como `DateTimeOffset?`. Habilita el poblado automático de fechas vía interceptor EF Core. |
| `ResourceAudit` | Mixin de auditoría | Implementa `IEntityWithCreatedUpdatedDate`. Mismo comportamiento que `ClassroomAudit`. |
| `SharedAreaAudit` | Mixin de auditoría | No implementa `IEntityWithCreatedUpdatedDate`. Declara `CreatedDate` y `UpdatedDate` con las mismas columnas que los otros mixins, pero el interceptor no las pobla automáticamente. |
| `IClassroomRepository` | Repository Interface | Contrato de persistencia para `Classroom`. Operaciones: `AddAsync`, `FindByIdAsync`, `ListAsync`, `FindByTeacherIdAsync`, `ExistsByNameAsync`, `ExistsByClassroomId`, `Update`, `Remove`. |
| `IResourceRepository` | Repository Interface | Contrato de persistencia para `Resource`. Operaciones: `AddAsync`, `FindByIdAsync`, `ListAsync`, `FindByClassroomIdAsync`, `ExistsByNameAsync`, `Update`, `Remove`. |
| `ISharedAreaRepository` | Repository Interface | Contrato de persistencia para `SharedArea`. Operaciones: `AddAsync`, `FindByIdAsync`, `ListAsync`, `Update`, `Remove`. |
| `CreateClassroomCommand` | Command | Comando para crear un `Classroom`. Campos: `Name`, `Description`, `TeacherId`. |
| `UpdateClassroomCommand` | Command | Comando para actualizar un `Classroom`. Incluye `ClassroomId` como identificador de la instancia a modificar. |
| `DeleteClassroomCommand` | Command | Comando para eliminar un `Classroom` por su `ClassroomId`. |
| `CreateResourceCommand` | Command | Comando para crear un `Resource`. Campos: `Name`, `KindOfResource`, `ClassroomId`. |
| `UpdateResourceCommand` | Command | Comando para actualizar un `Resource`. Incluye `Id` como identificador de la instancia a modificar. |
| `DeleteResourceCommand` | Command | Comando para eliminar un `Resource` por su `ResourceId`. |
| `CreateSharedAreaCommand` | Command | Comando para crear un `SharedArea`. Campos: `Name`, `Capacity`, `Description`. |
| `UpdateSharedAreaCommand` | Command | Comando para actualizar un `SharedArea`. Incluye `Id` como identificador de la instancia a modificar. |
| `DeleteSharedAreaCommand` | Command | Comando para eliminar un `SharedArea` por su `Id`. |
| `GetClassroomByIdQuery` | Query | Consulta de un `Classroom` por su `ClassroomId`. |
| `GetAllClassroomsQuery` | Query | Consulta del listado completo de aulas. |
| `GetAllClassroomsByTeacherIdQuery` | Query | Consulta de aulas filtradas por `TeacherId`. |
| `GetResourceByIdQuery` | Query | Consulta de un `Resource` por su `Id`. |
| `GetAllResourcesQuery` | Query | Consulta del listado completo de recursos. |
| `GetAllResourcesByClassroomIdQuery` | Query | Consulta de recursos pertenecientes a un aula específica. |
| `GetSharedAreaByIdQuery` | Query | Consulta de un `SharedArea` por su `Id`. |
| `GetAllSharedAreasQuery` | Query | Consulta del listado completo de áreas comunes. |

#### 4.2.2.2. Interface Layer

La Interface Layer del contexto Space & Resource Management expone tres conjuntos de endpoints REST que constituyen los puntos de entrada HTTP al bounded context. `ClassroomsController` gestiona el ciclo de vida completo de las aulas; `ResourcesController` administra los recursos físicos bajo una ruta anidada en el aula propietaria (`/api/v1/classrooms/{classroomId}/resources`); y `SharedAreaController` cubre las áreas comunes. Esta capa traduce las solicitudes HTTP en comandos o consultas, delega su ejecución íntegramente a la Application Layer y serializa la respuesta. No contiene reglas de dominio. Los assembladores de transformación (`*Assembler`) desacoplan la representación HTTP (Resources DTOs) del modelo de dominio.

Adicionalmente, esta capa aloja la fachada ACL de entrada `SpacesAndResourceManagementFacade`, que expone al bounded context BreakdownManagement el contrato `ValidateClassroomIdExistence(int classroomId)` sin revelar el modelo interno del contexto.

| Clase | Tipo | Endpoints / Operaciones |
| --- | --- | --- |
| `ClassroomsController` | Controller (`/api/v1/classrooms`) | `GET /api/v1/classrooms` — lista todas las aulas. `GET /api/v1/classrooms/{id}` — obtiene un aula por su Id. `GET /api/v1/classrooms/teachers/{teacherId}` — lista aulas por docente. `POST /api/v1/classrooms/teachers/{teacherId}` — crea un aula asignando un docente responsable. `PUT /api/v1/classrooms/{id}` — actualiza nombre, descripción y docente de un aula. `DELETE /api/v1/classrooms/{id}` — elimina un aula. |
| `ResourcesController` | Controller (`/api/v1/classrooms/{classroomId}/resources`) | `GET .../resources` — lista recursos del aula. `GET .../resources/{resourceId}` — obtiene un recurso validando pertenencia al aula. `POST .../resources` — crea un recurso asociado al aula. `PUT .../resources/{resourceId}` — actualiza nombre, tipo y aula de un recurso. `DELETE .../resources/{resourceId}` — elimina un recurso. |
| `SharedAreaController` | Controller (`/api/v1/shared-area`) | `GET /api/v1/shared-area` — lista todas las áreas comunes. `GET /api/v1/shared-area/{id}` — obtiene un área por su Id. `POST /api/v1/shared-area` — crea un área común. `PUT /api/v1/shared-area/{id}` — actualiza nombre, capacidad y descripción. `DELETE /api/v1/shared-area/{id}` — elimina un área común. |
| `ClassroomResource` | Resource (DTO de salida) | Representación JSON de un `Classroom` para respuestas GET/POST/PUT. |
| `CreateClassroomResource` | Resource (DTO de entrada) | Payload de creación de aula (sin Id, sin TeacherId — llega por ruta). |
| `UpdateClassroomResource` | Resource (DTO de entrada) | Payload de actualización de aula. |
| `ResourceResource` | Resource (DTO de salida) | Representación JSON de un `Resource`. |
| `CreateResourceResource` | Resource (DTO de entrada) | Payload de creación de recurso. |
| `UpdateResourceResource` | Resource (DTO de entrada) | Payload de actualización de recurso. |
| `SharedAreaResource` | Resource (DTO de salida) | Representación JSON de un `SharedArea`. |
| `CreateSharedAreaResource` | Resource (DTO de entrada) | Payload de creación de área común. |
| `UpdateSharedAreaResource` | Resource (DTO de entrada) | Payload de actualización de área común. |
| `ClassroomResourceFromEntityAssembler` | Assembler | Convierte una entidad `Classroom` en `ClassroomResource`. |
| `CreateClassroomCommandFromResourceAssembler` | Assembler | Convierte `CreateClassroomResource` + `teacherId` de ruta en `CreateClassroomCommand`. |
| `UpdateClassroomCommandFromResourceAssembler` | Assembler | Convierte `UpdateClassroomResource` + `id` de ruta en `UpdateClassroomCommand`. |
| `ResourceResourceFromEntityAssembler` | Assembler | Convierte una entidad `Resource` en `ResourceResource`. |
| `CreateResourceCommandFromResourceAssembler` | Assembler | Convierte `CreateResourceResource` + `classroomId` de ruta en `CreateResourceCommand`. |
| `UpdateResourceCommandFromResourceAssembler` | Assembler | Convierte `UpdateResourceResource` + `resourceId` de ruta en `UpdateResourceCommand`. |
| `SharedAreaResourceFromEntityAssembler` | Assembler | Convierte una entidad `SharedArea` en `SharedAreaResource`. |
| `CreateSharedAreaCommandFromResourceAssembler` | Assembler | Convierte `CreateSharedAreaResource` en `CreateSharedAreaCommand`. |
| `UpdateSharedAreaCommandFromResourceAssembler` | Assembler | Convierte `UpdateSharedAreaResource` + `id` de ruta en `UpdateSharedAreaCommand`. |
| `ISpacesAndResourceManagementFacade` | ACL Interface (inbound) | Contrato expuesto a BreakdownManagement BC. Operación: `ValidateClassroomIdExistence(int classroomId): bool`. |
| `SpacesAndResourceManagementFacade` | ACL Service (inbound) | Implementación de `ISpacesAndResourceManagementFacade`. Delega a `IClassroomRepository.ExistsByClassroomId`. |

#### 4.2.2.3. Application Layer

La Application Layer orquesta los flujos de proceso del bounded context sin contener reglas de dominio propias. Esta capa contiene los command services y query services que coordinan la interacción entre el Domain Layer y la Infrastructure Layer. Los command services reciben comandos provenientes de la Interface Layer, aplican validaciones de integridad (existencia de entidades relacionadas, unicidad de nombres) y delegan las operaciones de escritura en los repositorios del dominio. Los query services atienden consultas de solo lectura, delegando directamente en las operaciones de lectura de los repositorios. Dado que el contexto no publica Domain Events, no existen event handlers ni policies en esta capa.

Cabe destacar que `ClassroomCommandService` recibe por inyección de dependencias a `IExternalProfileService` —el adaptador ACL saliente hacia Profiles BC— y lo utiliza tanto en la creación de aulas (verificación directa previa a la persistencia) como en la actualización (pasado como `Func<int, bool>` al método `Classroom.UpdateTeacherId`). Esta decisión desacopla la lógica de validación externa del aggregate, manteniendo al aggregate libre de dependencias hacia infraestructura.

| Clase | Tipo | Responsabilidad |
| --- | --- | --- |
| `ClassroomCommandService` | Command Service | Implementa `IClassroomCommandService`. Maneja `CreateClassroomCommand` (verifica TeacherId vía `IExternalProfileService`, verifica unicidad de nombre, persiste el aggregate), `UpdateClassroomCommand` (carga, actualiza campos y delega la validación del docente como `Func<int, bool>` a `Classroom.UpdateTeacherId`) y `DeleteClassroomCommand` (carga y elimina). |
| `ResourceCommandService` | Command Service | Implementa `IResourceCommandService`. Maneja `CreateResourceCommand` (verifica existencia del aula asociada, verifica unicidad de nombre, persiste), `UpdateResourceCommand` (carga y actualiza campos) y `DeleteResourceCommand` (carga y elimina). |
| `SharedAreaCommandService` | Command Service | Implementa `ISharedAreaCommandService`. Maneja `CreateSharedAreaCommand`, `UpdateSharedAreaCommand` y `DeleteSharedAreaCommand` sobre el aggregate `SharedArea`. |
| `ClassroomQueryService` | Query Service | Implementa `IClassroomQueryService`. Maneja `GetClassroomByIdQuery`, `GetAllClassroomsQuery` y `GetAllClassroomsByTeacherIdQuery` delegando en `IClassroomRepository`. |
| `ResourceQueryService` | Query Service | Implementa `IResourceQueryService`. Maneja `GetResourceByIdQuery`, `GetAllResourcesQuery` y `GetAllResourcesByClassroomIdQuery` delegando en `IResourceRepository`. |
| `SharedAreaQueryService` | Query Service | Implementa `ISharedAreaQueryService`. Maneja `GetSharedAreaByIdQuery` y `GetAllSharedAreasQuery` delegando en `ISharedAreaRepository`. |
| `IExternalProfileService` | ACL Interface (outbound) | Contrato del adaptador saliente hacia Profiles BC. Operación: `VerifyProfile(int profileId): bool`. |
| `ExternalProfileService` | ACL Service (outbound) | Implementación de `IExternalProfileService`. Delega en `IProfilesContextFacade.ValidateTeacherProfileIdExistence`, el contrato que el bounded context Profiles expone hacia sus consumidores. |

#### 4.2.2.4. Infrastructure Layer

La Infrastructure Layer del contexto Space & Resource Management provee las implementaciones concretas de los contratos definidos en el Domain Layer, utilizando Entity Framework Core como ORM sobre una base de datos MySQL, de manera consistente con la decisión de infraestructura adoptada para el Web API de la plataforma EduSpace IoT (véase sección 4.1.3.3). Las implementaciones de repositorio extienden la clase base `BaseRepository<T>` del proyecto compartido y traducen las operaciones de dominio en consultas LINQ sobre el `AppDbContext`.

Como nota técnica relevante, los tres aggregates de este bounded context —`Classroom`, `Resource` y `SharedArea`— no se registran mediante propiedades `DbSet<T>` explícitas en `AppDbContext`. En su lugar, son descubiertos y configurados a través del método `OnModelCreating` mediante la API de configuración fluida de Entity Framework Core, siguiendo la misma convención aplicada en todos los contextos del proyecto. Las convenciones de nomenclatura en snake_case se aplican automáticamente a través de Humanizer.

| Clase | Tipo | Tecnología / Responsabilidad |
| --- | --- | --- |
| `ClassroomRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `IClassroomRepository`. Extiende `BaseRepository<Classroom>`. Operaciones propias: `FindByTeacherIdAsync` (filtra por `TeacherId.TeacherIdentifier`), `ExistsByNameAsync`, `ExistsByClassroomId`, `ExistsByClassroomName`. Sobrescribe `FindByIdAsync` y `ListAsync`. |
| `ResourceRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `IResourceRepository`. Extiende `BaseRepository<Resource>`. Gestiona la persistencia y consulta de instancias de `Resource`, incluyendo filtrado por `ClassroomId`. |
| `SharedAreaRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `ISharedAreaRepository`. Extiende `BaseRepository<SharedArea>`. Gestiona la persistencia y consulta de instancias de `SharedArea`. |
| `AppDbContext` | DbContext (compartido) | Entity Framework Core. Los aggregates `Classroom`, `Resource` y `SharedArea` se configuran mediante `OnModelCreating` (sin `DbSet<T>` explícito). Las relaciones, índices, conversiones de tipo y los mixins de auditoría (`ClassroomAudit`, `ResourceAudit`, `SharedAreaAudit`) se configuran en este método usando la API fluida. |

### 4.2.3. Bounded Context: Reservation & Scheduling

El contexto de Reservation & Scheduling concentra toda la responsabilidad relacionada con la planificación temporal de las actividades académicas de la institución: la creación y gestión de reuniones (meetings) entre administradores y docentes en aulas específicas, y la reserva de áreas comunes (shared areas) por parte de los docentes para uso no curricular. Este bounded context es el guardián de las invariantes de solapamiento horario y disponibilidad de espacio; ningún otro contexto puede crear o modificar bloques de tiempo sin pasar por sus contratos de dominio.

En la implementación actual del Web API, este bounded context se materializa en dos sub-módulos físicos: `ReservationScheduling/`, que contiene el aggregate `Meeting` bajo el namespace `FULLSTACKFURY.EduSpace.API.ReservationScheduling.*`, y `Reservations/`, que contiene el aggregate `Reservation`. Este segundo sub-módulo declara sus capas de Domain, Application e Infrastructure bajo el namespace `FULLSTACKFURY.EduSpace.API.EventsScheduling.*` por una decisión histórica de organización; sus contratos REST sí utilizan el namespace `Reservations.Interface.REST`. El equipo prevé reconciliar la nomenclatura física en una iteración posterior. Estratégicamente, ambos sub-módulos forman un único bounded context unificado en el modelo de dominio (véase sección 4.1), dado que comparten la misma política de negocio central: garantizar que ningún espacio o docente quede asignado a dos eventos simultáneos en el mismo rango horario.

#### 4.2.3.1. Domain Layer

El Domain Layer del contexto Reservation & Scheduling encapsula las reglas de negocio que gobiernan la asignación de tiempo sobre espacios y personas: qué constituye un bloque horario válido, cuándo existe un conflicto de ocupación, y cómo se registra la participación de un docente en una reunión. Esta capa es completamente independiente de la infraestructura y define los contratos que las capas superiores deben respetar a través de interfaces de repositorio y servicios de dominio.

El aggregate `Meeting` (sub-módulo `ReservationScheduling/`) representa una reunión programada por un administrador en un aula concreta para uno o más docentes. Gestiona su propia colección de participantes a través de la entidad `MeetingSession` y expone operaciones de negocio para añadir o remover docentes, validando la ausencia de conflictos horarios antes de persistir el cambio. El aggregate `Reservation` (sub-módulo `Reservations/`) representa la reserva de un área común por parte de un docente; incorpora en sí mismo la lógica de verificación de disponibilidad mediante el método `CanReserve`, que evalúa solapamientos contra las reservas existentes del área en el mismo día. Ambos aggregates comparten una invariante de negocio idéntica para las ventanas horarias: inicio anterior al fin, duración máxima de dos horas, y franja permitida entre las 07:00 y las 20:00 horas.

| Clase | Tipo | Responsabilidad / Atributos clave |
| --- | --- | --- |
| `Meeting` | Aggregate Root | Representa una reunión programada por un administrador en un aula. Atributos: `Id`, `Title`, `Description`, `Date` (DateOnly), `StartTime` (TimeOnly), `EndTime` (TimeOnly), `AdministratorId`, `ClassroomId`. Expone `AddTeacherToMeeting` y `RemoveTeacherFromMeeting` sobre la colección `MeetingParticipants`. Implementado como clase parcial distribuida en `Meeting.cs` y `MeetingManagement.cs`. |
| `Reservation` | Aggregate Root | Representa la reserva de un área común por un docente. Atributos: `Id`, `Title`, `ReservationDate`, `AreaId`, `TeacherId`. Contiene el método de dominio `CanReserve(IEnumerable<Reservation>)` que valida la ausencia de solapamiento horario contra reservas existentes. |
| `MeetingSession` | Entity | Entidad de unión entre `Meeting` y un docente participante. Atributos: `MeetingId`, `TeacherId`, referencias de navegación a `Meeting` y `TeacherProfile` (del BC Profiles). |
| `MeetingAudit` | Audit Class | Clase de trazabilidad de cambios sobre reuniones. Atributos: `MeetingAuditId` (Guid), `MeetingId` (Guid), `Action`, `ActionPerformedBy`, `CreatedDate`, `UpdatedDate`, `PreviousState`, `NewState`. |
| `MeetingDate` | Value Object | Encapsula el rango temporal de una reunión con invariantes estrictas: inicio ≠ fin, inicio < fin, ninguno de los dos en el pasado, duración máxima de 2 horas, franja horaria entre 07:00 y 20:00. Atributos: `Start` (DateTime), `End` (DateTime). |
| `ReservationDate` | Value Object | Encapsula el rango temporal de una reserva de área común. Comparte las mismas invariantes que `MeetingDate`. Atributos: `Start` (DateTime), `End` (DateTime). Implementado como `record`. |
| `Teacher` | Value Object | Representa los datos identificatorios de un docente en el contexto de una reunión. Atributos: `Id` (int), `FirstName` (string), `LastName` (string). |
| `AdministratorId` | Value Object | Envuelve el identificador del administrador que programa la reunión. Atributo: `AdministratorIdentifier` (int). |
| `ClassroomId` | Value Object | Envuelve el identificador del aula asignada a la reunión. Atributo: `ClassroomIdentifier` (int). |
| `AreaId` | Value Object | Envuelve el identificador del área común reservada. Atributo: `Identifier` (int). |
| `TeacherId` (ReservationScheduling) | Value Object | Envuelve el identificador del docente en el contexto del sub-módulo Meeting. |
| `TeacherId` (Reservations) | Value Object | Envuelve el identificador del docente en el contexto del sub-módulo Reservation. Atributo: `TeacherIdentifier` (int). |
| `IMeetingRepository` | Repository Interface | Contrato para persistir y consultar `Meeting`. Operaciones: `AddAsync`, `FindByIdAsync` (con participantes), `ListAsync`, `FindAllByAdminIdAsync`, `FindAllByTeacherIdAsync`, `Remove`, `Update`. |
| `IReservationRepository` | Repository Interface | Contrato para persistir y consultar `Reservation`. Operaciones: `AddAsync`, `FindByIdAsync`, `ListAsync`, `FindAllByAreaIdAsync`, `FindAllByAreaIdMonthAndDayAsync`, `Remove`, `Update`. |
| `IMeetingCommandService` | Domain Service Interface | Contrato de operaciones de escritura sobre `Meeting`: crear, actualizar, eliminar, añadir/remover participante. |
| `IMeetingQueryService` | Domain Service Interface | Contrato de consultas sobre `Meeting`: por Id, por administrador, por docente, listado general. |
| `IReservationCommandService` | Domain Service Interface | Contrato de operaciones de escritura sobre `Reservation`: crear, actualizar, eliminar. |
| `IReservationQueryService` | Domain Service Interface | Contrato de consultas sobre `Reservation`: por Id, por área, por área/mes/día, listado general. |
| `IExternalClassroomService` | ACL Interface (outbound) | Contrato interno del sub-módulo Meeting para validar la existencia de un aula contra el BC Spaces & Resource Management. |
| `IRExternalProfileService` | ACL Interface (outbound) | Contrato interno del sub-módulo Meeting para validar la existencia de administradores y docentes contra el BC Profiles. |
| `IExternalProfileService` | ACL Interface (outbound) | Contrato interno del sub-módulo Reservation para validar la existencia de un docente contra el BC Profiles. |

#### 4.2.3.2. Interface Layer

La Interface Layer del contexto Reservation & Scheduling expone tres controladores REST que sirven como puertos de entrada al bounded context. `MeetingsController` atiende el ciclo de vida completo de las reuniones; `MeetingParticipantsController` gestiona exclusivamente la asignación y remoción de docentes participantes en una reunión existente; y `ReservationsController` atiende el ciclo de vida de las reservas de áreas comunes. Los controladores delegan la totalidad de la lógica de negocio hacia la Application Layer y se limitan a la traducción entre representaciones HTTP y comandos o consultas de dominio mediante los ensambladores del paquete `Transform`.

Cada controlador utiliza el patrón Resource/Assembler: los recursos de entrada (`CreateMeetingResource`, `UpdateMeetingResource`, `CreateReservationResource`, `UpdateReservationResource`) son mapeados a comandos de dominio por los `CommandFromResourceAssembler` correspondientes, mientras que los aggregates resultantes son proyectados a recursos de salida (`MeetingResource`, `ReservationResource`) por los `EntityFromAssembler` respectivos.

| Clase | Tipo | Endpoints / Operaciones |
| --- | --- | --- |
| `MeetingsController` | Controller | `POST /api/v1/administrators/{administratorId}/classrooms/{classroomId}/meetings` — crea una reunión en un aula para un administrador. `GET /api/v1/meetings` — lista todas las reuniones. `GET /api/v1/teachers/{teacherId}/meetings` — lista reuniones de un docente. `GET /api/v1/meetings/{id}` — obtiene una reunión por Id. `PUT /api/v1/meetings/{id}` — actualiza una reunión. `DELETE /api/v1/meetings/{id}` — elimina una reunión. |
| `MeetingParticipantsController` | Controller | `POST /api/v1/meetings/{meetingId}/teachers/{teacherId}` — agrega un docente a la lista de participantes de una reunión. `DELETE /api/v1/meetings/{meetingId}/teachers/{teacherId}` — remueve un docente de la lista de participantes. |
| `ReservationsController` | Controller | `POST /api/v1/teachers/{teacherId}/areas/{areaId}/reservations` — crea una reserva de área común. `GET /api/v1/reservations` — lista todas las reservas. `GET /api/v1/areas/{areaId}/reservations` — lista reservas de un área. `GET /api/v1/reservations/{id}` — obtiene una reserva por Id. `PUT /api/v1/reservations/{id}` — actualiza una reserva. `DELETE /api/v1/reservations/{id}` — elimina una reserva. |

#### 4.2.3.3. Application Layer

La Application Layer orquesta los flujos de proceso del bounded context sin contener reglas de dominio propias. Esta capa aloja los servicios de comando y consulta que coordinan la interacción entre el Domain Layer y la Infrastructure Layer, y es el único punto donde se invocan los adaptadores ACL para validar referencias cruzadas hacia otros bounded contexts antes de ejecutar operaciones sobre los aggregates.

`MeetingCommandService` coordina la creación, actualización y eliminación de reuniones, así como la gestión de participantes. Antes de crear o actualizar una reunión, valida la existencia del administrador responsable a través de `IRExternalProfileService` y la existencia del aula asignada a través de `IExternalClassroomService`. Al añadir un participante, valida la existencia del docente y detecta conflictos horarios consultando sus reuniones previas. `ReservationCommandService` coordina el ciclo de vida de las reservas; valida la existencia del docente reservante a través de `IExternalProfileService` y delega al método de dominio `CanReserve` la detección de solapamientos en el área solicitada.

| Clase | Tipo | Responsabilidad |
| --- | --- | --- |
| `MeetingCommandService` | Command Service | Implementa `IMeetingCommandService`. Coordina la creación, actualización y eliminación de `Meeting`, y la gestión de participantes (`AddTeacherToMeeting`, `RemoveTeacherFromMeeting`). Invoca `IRExternalProfileService` para validar administrador y docente, e `IExternalClassroomService` para validar el aula. Detecta conflictos horarios entre reuniones al agregar participantes o actualizar horarios. |
| `MeetingQueryService` | Query Service | Implementa `IMeetingQueryService`. Resuelve consultas de solo lectura sobre `Meeting` delegando a `IMeetingRepository`: listado general, por Id, por administrador y por docente. |
| `ReservationCommandService` | Command Service | Implementa `IReservationCommandService`. Coordina la creación, actualización y eliminación de `Reservation`. Valida la existencia del docente vía `IExternalProfileService`. Delega la verificación de solapamiento al método `CanReserve` del aggregate antes de persistir. |
| `ReservationQueryService` | Query Service | Implementa `IReservationQueryService`. Resuelve consultas de solo lectura sobre `Reservation`: listado general, por área, por área/mes/día y por Id. |
| `ExternalClassroomServices` | ACL Adapter (outbound) | Implementa `IExternalClassroomService`. Traduce la llamada `ValidateClassroomId` hacia `ISpacesAndResourceManagementFacade.ValidateClassroomIdExistence`, desacoplando el sub-módulo Meeting del BC Spaces & Resource Management. |
| `RExternalProfileServices` | ACL Adapter (outbound) | Implementa `IRExternalProfileService`. Traduce las llamadas de validación de docente y administrador hacia `IProfilesContextFacade`, desacoplando el sub-módulo Meeting del BC Profiles. |
| `ExternalProfileServices` | ACL Adapter (outbound) | Implementa `IExternalProfileService` (sub-módulo Reservation). Traduce la validación de existencia de docente hacia `IProfilesContextFacade`, desacoplando el sub-módulo Reservation del BC Profiles. |

#### 4.2.3.4. Infrastructure Layer

La Infrastructure Layer del contexto Reservation & Scheduling provee las implementaciones concretas de los contratos de repositorio definidos en el Domain Layer, utilizando Entity Framework Core como ORM sobre una base de datos MySQL, consistente con la decisión de infraestructura adoptada para el Web API de la plataforma EduSpace IoT (véase sección 4.1.3.3). Las implementaciones de repositorio extienden la clase base genérica `BaseRepository<T>` y sobrescriben las operaciones que requieren la carga de entidades relacionadas mediante `Include`/`ThenInclude` para materializar el grafo de objetos completo del aggregate.

`MeetingRepository` carga la colección de participantes (`MeetingParticipants`) junto con sus referencias a `TeacherProfile` en cada consulta, lo que garantiza que la Application Layer reciba siempre el aggregate `Meeting` con su estado completo. `ReservationRepository` implementa las consultas filtradas por área y por fecha que soportan la validación de solapamiento horario. El `AppDbContext` compartido del proyecto configura los `DbSet` para ambos aggregates y aplica las convenciones de nomenclatura en snake_case mediante Humanizer.

| Clase | Tipo | Tecnología / Responsabilidad |
| --- | --- | --- |
| `MeetingRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `IMeetingRepository`. Sobrescribe `FindByIdAsync` y `ListAsync` para incluir `MeetingParticipants` y `Teacher` mediante eager loading. Provee `FindAllByAdminIdAsync` y `FindAllByTeacherIdAsync` con filtros LINQ sobre los Value Objects `AdministratorId` y `TeacherId`. |
| `ReservationRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `IReservationRepository`. Provee `FindAllByAreaIdAsync` y `FindAllByAreaIdMonthAndDayAsync` con filtros LINQ sobre los campos del Value Object `ReservationDate`, permitiendo la detección diaria de solapamientos en el aggregate. |
| `AppDbContext` | DbContext (compartido) | Entity Framework Core. Incluye `DbSet<Meeting>` y `DbSet<Reservation>` junto con los del resto de bounded contexts. Configura los mappings, índices y conversiones de tipo requeridos para ambos aggregates mediante la API de configuración fluida. Aplica snake_case en nombres de columnas y tablas vía Humanizer. |

### 4.2.4. Bounded Context: Breakdown Management

El contexto de Breakdown Management concentra toda la responsabilidad relacionada con el registro, seguimiento y resolución de incidencias sobre recursos físicos de la institución. Su misión es permitir que el personal autorizado reporte fallas o averías en equipos y espacios, y que el estado de cada incidencia sea actualizado a lo largo de su ciclo de vida hasta su resolución. Este bounded context es el punto de entrada para la gestión reactiva del mantenimiento: recibe reportes de recursos dañados o fuera de servicio, los asocia a la entidad de recurso correspondiente en el BC Space & Resource Management mediante una referencia tipada, y expone su estado a la plataforma para que otros contextos puedan consultarlo.

Los eventos de dominio identificados durante el Design-Level EventStorming que delimitan este contexto incluyen `ReportCreated` (una nueva incidencia es registrada sobre un recurso) y `ReportResolutionNotified` (la incidencia es marcada como resuelta). El actor principal que interactúa con él es el Administrador, quien crea reportes ante una avería y los actualiza conforme avanza la gestión.

#### 4.2.4.1. Domain Layer

El Domain Layer del contexto Breakdown Management encapsula las reglas de negocio que gobiernan el ciclo de vida de un reporte de avería: qué constituye un reporte válido, qué estados puede adoptar y cómo se referencia el recurso afectado de forma tipada. Esta capa es independiente de toda infraestructura y define los contratos que las capas superiores deben respetar.

El aggregate raíz `Report` representa la entidad central del contexto. Contiene el tipo de incidencia (`KindOfReport`), una descripción libre (`Description`), la referencia tipada al recurso afectado (`ResourceId`) y la fecha de creación (`CreatedAt`). El estado del reporte es modelado por el Value Object `ReportStatus`, que define el ciclo de vida de la incidencia. La referencia al recurso externo es modelada por el Value Object `ResourceId`, que encapsula y valida el identificador entero del recurso correspondiente al BC Space & Resource Management.

Como nota de consistencia de naming: los archivos físicos de los Value Objects presentan naming inconsistente con sus clases — `Reportstatus.cs` (con 's' minúscula) y `Resourceid.cs` (con 'i' minúscula) — mientras que las clases declaradas en su interior utilizan correctamente `ReportStatus` y `ResourceId` en PascalCase.

El modelo conceptual del Strategic-Level (sección 4.1) introduce el evento `ReportResolutionNotified`. La implementación actual del BC contempla este evento como compromiso de diseño a materializar en una iteración posterior, una vez se integre la infraestructura de eventos de dominio.

| Clase | Tipo | Responsabilidad |
| --- | --- | --- |
| `Report` | Aggregate Root | Entidad raíz que registra una incidencia sobre un recurso físico. Atributos: `Id`, `KindOfReport`, `Description`, `ResourceId`, `CreatedAt`, `Status`. Se inicializa siempre con estado `EnProceso`. Expone el método `Update` para modificar tipo, descripción y estado. |
| `ReportStatus` | Value Object | Define el ciclo de vida de un reporte mediante dos estados: `EnProceso` (valor interno: `"in progress"`) y `Completado` (valor interno: `"completed"`). La factoría `FromString` lanza `ArgumentException` ante cualquier valor no reconocido. Esta iteración define el ciclo de vida en dos estados; iteraciones posteriores podrán ampliar el modelo. |
| `ResourceId` | Value Object | Referencia tipada al recurso afectado, perteneciente al BC Space & Resource Management. Encapsula un entero positivo (`Id`) e impone la invariante de que el valor sea mayor que cero. Se mapea como columna escalar mediante `HasConversion` en `AppDbContext`, a diferencia de otros Value Objects del proyecto que utilizan `OwnsOne`. |
| `IReportRepository` | Repository Interface | Contrato de persistencia para el aggregate `Report`. Hereda de `IBaseRepository<Report>` (operaciones genéricas: `AddAsync`, `Update`, `Remove`, `FindByIdAsync`, `ListAsync`). Además expone `FindAllAsync()` — método específico que duplica la funcionalidad del genérico heredado `ListAsync()` — y `FindAllByResourceIdAsync(int resourceId)` para consultar reportes por recurso afectado. |
| `IReportCommandService` | Service Interface | Contrato de aplicación para comandos de escritura. Operaciones: `Handle(CreateReportCommand)`, `Handle(UpdateReportCommand)`, `Handle(DeleteReportCommand)`. |
| `IReportQueryService` | Service Interface | Contrato de aplicación para consultas de solo lectura. Operaciones: `Handle(GetAllReportsQuery)`, `Handle(GetAllReportsByResourceIdQuery)`, `Handle(GetReportByIdQuery)`. |
| `CreateReportCommand` | Command | Transporta los datos necesarios para crear un reporte: `KindOfReport`, `Description`, `ResourceId`, `CreatedAt`. Valida en construcción que `KindOfReport` no sea nulo y que `ResourceId` sea mayor que cero. |
| `UpdateReportCommand` | Command | Transporta los datos para actualizar un reporte existente: `Id`, `KindOfReport`, `Description`, `Status` (string que será convertido a `ReportStatus` vía `FromString`). |
| `DeleteReportCommand` | Command | Identifica el reporte a eliminar por su `Id`. |
| `GetAllReportsQuery` | Query | Consulta sin parámetros que solicita la lista completa de reportes. |
| `GetAllReportsByResourceIdQuery` | Query | Consulta parametrizada por `ResourceId` para obtener los reportes asociados a un recurso específico. |
| `GetReportByIdQuery` | Query | Consulta por `Id` para obtener un reporte individual. |

#### 4.2.4.2. Interface Layer

La Interface Layer del contexto Breakdown Management expone un único controlador REST que sirve como puerto de entrada al bounded context. Este controlador atiende las operaciones de creación, consulta, actualización y eliminación de reportes de avería, traduciendo las solicitudes HTTP en comandos o consultas que son procesados por la Application Layer y devolviendo respuestas serializadas en JSON. La implementación actual no incluye decoradores de autorización por rol en los endpoints; el control de acceso queda pendiente para una iteración posterior.

Los recursos de transferencia (`CreateReportResource`, `UpdateReportResource`, `ReportResource`) y los ensambladores de transformación (`CreateReportCommandFromResourceAssembler`, `UpdateReportCommandFromResourceAssembler`, `ReportResourceFromEntityAssembler`) completan la capa, manteniendo la lógica de mapeo separada del controlador. Como detalle de implementación, el endpoint `POST /api/v1/reports` devuelve `200 OK` en lugar del `201 Created` semánticamente correcto para una operación de creación de recurso; la anotación Swagger del método declara `201` pero el código retorna `Ok(...)`.

| Clase | Tipo | Endpoints / Operaciones |
| --- | --- | --- |
| `ReportsController` | Controller | `POST /api/v1/reports` — crea un nuevo reporte de avería. `GET /api/v1/reports` — lista todos los reportes. `GET /api/v1/reports/{id}` — obtiene un reporte por su ID. `GET /api/v1/reports/resources/{resourceId}` — obtiene todos los reportes asociados a un recurso. `PUT /api/v1/reports/{id}` — actualiza tipo, descripción y estado de un reporte. `DELETE /api/v1/reports/{id}` — elimina un reporte. |
| `CreateReportResource` | Resource (entrada) | DTO de entrada para la creación: `KindOfReport`, `Description`, `ResourceId`, `CreatedAt`. |
| `UpdateReportResource` | Resource (entrada) | DTO de entrada para la actualización: `KindOfReport`, `Description`, `Status` (string). |
| `ReportResource` | Resource (salida) | DTO de salida con la representación completa del reporte: `Id`, `KindOfReport`, `Description`, `ResourceId`, `CreatedAt`, `Status`. |
| `CreateReportCommandFromResourceAssembler` | Assembler | Transforma `CreateReportResource` en `CreateReportCommand`. |
| `UpdateReportCommandFromResourceAssembler` | Assembler | Transforma `UpdateReportResource` y el `id` de ruta en `UpdateReportCommand`. |
| `ReportResourceFromEntityAssembler` | Assembler | Transforma el aggregate `Report` en `ReportResource` para la respuesta HTTP. |

#### 4.2.4.3. Application Layer

La Application Layer del contexto Breakdown Management orquesta los flujos de proceso sin contener reglas de dominio propias. Implementa el patrón Command/Query mediante dos servicios: `ReportCommandService`, responsable de los flujos de escritura, y `ReportQueryService`, responsable de los flujos de lectura. Ambos servicios dependen únicamente de las interfaces definidas en el Domain Layer (`IReportRepository`, `IUnitOfWork`) y no tienen referencias directas a la infraestructura.

El BC también define la posición de un servicio de salida (`ExternalProfileServices`) orientado a la integración con el BC Profiles para escenarios de notificación futura; su estado en la implementación actual se describe en la Infrastructure Layer.

| Clase | Tipo | Responsabilidad |
| --- | --- | --- |
| `ReportCommandService` | Command Service | Implementa `IReportCommandService`. Gestiona los tres flujos de escritura: (1) `Handle(CreateReportCommand)` — instancia un nuevo `Report`, lo persiste vía `IReportRepository.AddAsync` y confirma la unidad de trabajo. (2) `Handle(UpdateReportCommand)` — carga el `Report` por Id, invoca `Report.Update(command)` para aplicar las modificaciones e invoca `ReportStatus.FromString` para la transición de estado, luego confirma el cambio. Lanza `ArgumentException` si el reporte no existe o si el estado proporcionado no es válido. (3) `Handle(DeleteReportCommand)` — carga el `Report`, lo elimina del repositorio y confirma la unidad de trabajo. |
| `ReportQueryService` | Query Service | Implementa `IReportQueryService`. Gestiona los tres flujos de lectura: `Handle(GetAllReportsQuery)` delega en `IReportRepository.ListAsync()`; `Handle(GetAllReportsByResourceIdQuery)` delega en `FindAllByResourceIdAsync(resourceId)`; `Handle(GetReportByIdQuery)` delega en `FindByIdAsync(id)`. |

#### 4.2.4.4. Infrastructure Layer

La Infrastructure Layer del contexto Breakdown Management provee la implementación concreta del contrato de repositorio definido en el Domain Layer, utilizando Entity Framework Core como ORM sobre una base de datos MySQL, consistente con la decisión de infraestructura adoptada para toda la plataforma EduSpace IoT. La implementación de repositorio hereda de `BaseRepository<Report>` (infraestructura compartida del proyecto) y especializa las operaciones de consulta propias del BC.

La configuración del aggregate `Report` se centraliza directamente en `AppDbContext`, sin un archivo de configuración separado por bounded context (a diferencia del enfoque `IEntityTypeConfiguration<T>` que podría adoptarse por consistencia). Esta configuración define la clave primaria, las propiedades obligatorias y, de forma notable, dos conversiones de tipo mediante la API fluida de EF Core: `ReportStatus` se mapea como columna de cadena (`HasConversion` entre `ReportStatus` y `string`) y `ResourceId` se mapea como columna escalar entera (`HasConversion` entre `ResourceId` y `int`, con nombre de columna explícito `ResourceId`). Este último punto diferencia a `ResourceId` del patrón `OwnsOne` utilizado para otros Value Objects del proyecto, dado que su naturaleza de referencia externa hace preferible el almacenamiento escalar.

El BC define además la posición de la ACL outbound `ExternalProfileServices` hacia el BC Profiles, cuya implementación queda pendiente para integraciones futuras de notificación. El archivo `ExternalProfileServices.cs` existe como placeholder (stub vacío) que marca la frontera de integración.

| Clase | Tipo | Tecnología / Responsabilidad |
| --- | --- | --- |
| `ReportRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `IReportRepository`. Hereda de `BaseRepository<Report>`. Sobreescribe `FindByIdAsync` para consultar directamente sobre `DbSet<Report>`. Implementa `FindAllAsync()` para obtener todos los reportes (paralelo funcional de `ListAsync()` del base) y `FindAllByResourceIdAsync(int resourceId)` para filtrar por `ResourceId` mediante comparación de Value Object. |
| `AppDbContext` (configuración Report) | DbContext | Entity Framework Core. Define el `DbSet<Report>` del BC dentro del contexto compartido de la plataforma. Configura `ReportStatus` con `HasConversion<string>` (serialización a `"in progress"` / `"completed"`) y `ResourceId` con `HasConversion<int>` como columna escalar `ResourceId`, en lugar de `OwnsOne`. |
| `ExternalProfileServices` | ACL Stub (outbound) | Placeholder sin implementación. Marca la posición de la ACL outbound hacia el BC Profiles para futuros escenarios de notificación al resolver una incidencia. |

### 4.2.5. Bounded Context: IoT Monitoring

El contexto de IoT Monitoring concentra toda la responsabilidad relacionada con la captura, persistencia, evaluación y visualización de datos ambientales y de ocupación provenientes de los dispositivos ESP32 instalados en las aulas. Este bounded context es el punto de convergencia entre el mundo embebido y la lógica de negocio de la plataforma: recibe lecturas agregadas desde el Edge API, evalúa los umbrales configurados por el administrador y gestiona el ciclo de vida completo de las alertas generadas cuando se detecta una condición anormal. Los eventos de dominio que delimitan este contexto, identificados durante el Design-Level EventStorming, son `SensorReadingCaptured`, `EnvironmentalThresholdExceeded`, `OccupancyStatusChanged` y `AlertGenerated`. Los actores que interactúan directamente con él son el Administrador (quien configura umbrales y gestiona alertas), el Docente (quien consulta el dashboard ambiental en modo lectura) y el Edge API (que actúa como productor de lecturas agregadas).

#### 4.2.5.1. Domain Layer

El Domain Layer del contexto IoT Monitoring encapsula las reglas de negocio fundamentales que gobiernan el monitoreo ambiental: qué constituye una lectura válida, cuándo una condición ambiental viola un umbral configurado, y cuál es el ciclo de vida de una alerta desde su generación hasta su resolución. Esta capa es independiente de toda infraestructura y define los contratos que las capas superiores deben respetar.

Los tres aggregates principales son `SensorReading`, que representa la lectura agregada recibida desde el Edge API (con los valores de promedio, mínimo, máximo y conteo del minuto correspondiente); `Alert`, aggregate root con estado y ciclo de vida propio (`Active`, `Acknowledged`, `Dismissed`); y `MonitoringConfiguration`, que persiste los umbrales configurados por el administrador para cada sensor o espacio. Los eventos de dominio `EnvironmentalThresholdExceeded` y `AlertGenerated` se publican desde el aggregate `SensorReading` y `Alert` respectivamente cuando se cumplen las condiciones de negocio correspondientes. El evento `ThresholdConfigured` se publica al persistir o actualizar una configuración de umbrales. Las interfaces de repositorio abstraen la persistencia de cada aggregate, permitiendo que la Infrastructure Layer provea las implementaciones concretas sin contaminar el dominio.

| Clase | Tipo | Responsabilidad / Atributos clave |
| --- | --- | --- |
| `SensorReading` | Aggregate Root | Representa una lectura agregada recibida del Edge API. Atributos: `Id`, `sensorId`, `classroomId`, `averageValue`, `minValue`, `maxValue`, `readingCount`, `capturedAt`, `sensorType` (temperatura, humedad, ocupación). Publica `EnvironmentalThresholdExceeded` si el valor viola un umbral activo. |
| `Alert` | Aggregate Root | Gestiona el ciclo de vida de una alerta ambiental. Atributos: `Id`, `sensorId`, `triggerValue`, `thresholdViolated`, `status` (AlertStatus), `generatedAt`, `acknowledgedAt`, `dismissedAt`. Publica `AlertGenerated` al crearse. |
| `MonitoringConfiguration` | Aggregate Root | Almacena la configuración de umbrales por sensor o espacio. Atributos: `Id`, `classroomId`, `sensorType`, `thresholds` (colección de `Threshold`), `lastUpdatedAt`. Publica `ThresholdConfigured` al guardarse. |
| `AlertStatus` | Value Object | Enumeración de estados de una alerta: `Active`, `Acknowledged`, `Dismissed`. |
| `Threshold` | Value Object | Define un umbral de alerta. Atributos: `minValue`, `maxValue`, `severity`. Contiene la invariante de que `minValue` debe ser menor que `maxValue`. |
| `SensorType` | Value Object | Enumeración del tipo de sensor: `Temperature`, `Humidity`, `Occupancy`. |
| `EnvironmentalThresholdExceeded` | Domain Event | Publicado por `SensorReading` cuando el valor promedio de una lectura supera los límites configurados. Payload: `sensorReadingId`, `sensorType`, `triggerValue`, `thresholdViolated`, `classroomId`. |
| `AlertGenerated` | Domain Event | Publicado por `Alert` cuando una nueva alerta es creada en estado `Active`. Payload: `alertId`, `sensorId`, `classroomId`, `triggerValue`. |
| `ThresholdConfigured` | Domain Event | Publicado por `MonitoringConfiguration` al crear o actualizar umbrales. Payload: `configurationId`, `classroomId`, `sensorType`. |
| `ISensorReadingRepository` | Repository Interface | Contrato para persistir y consultar `SensorReading`. Operaciones: `save`, `findById`, `findByClassroomIdAndPeriod`. |
| `IAlertRepository` | Repository Interface | Contrato para persistir y consultar `Alert`. Operaciones: `save`, `findById`, `findActiveAlerts`, `findByClassroomId`. |
| `IMonitoringConfigurationRepository` | Repository Interface | Contrato para persistir y consultar `MonitoringConfiguration`. Operaciones: `save`, `findByClassroomIdAndSensorType`, `findAll`. |

#### 4.2.5.2. Interface Layer

La Interface Layer del contexto IoT Monitoring expone tres conjuntos de endpoints REST que sirven como puertos de entrada al bounded context. El primero atiende la ingesta de lecturas provenientes del Edge API; el segundo permite la consulta y actualización del estado de las alertas por parte del Administrador; y el tercero gestiona la configuración de umbrales. Esta capa traduce las solicitudes HTTP en comandos o consultas que son procesados por la Application Layer, devolviendo respuestas serializadas en JSON. Todos los endpoints que modifican estado requieren el rol `Admin`; los de solo lectura del dashboard están disponibles también para el rol `Teacher`.

Los controladores delegan la lógica de negocio completamente hacia la Application Layer y no contienen reglas de dominio; su responsabilidad se limita a la validación de formato de entrada, la resolución de autorización por atributo de rol y la construcción de la respuesta HTTP adecuada.

| Clase | Tipo | Endpoints / Operaciones |
| --- | --- | --- |
| `SensorReadingsController` | Controller | `POST /api/v1/sensor-readings` — ingesta de lectura agregada desde Edge API. `GET /api/v1/sensor-readings?classroomId={id}&from={date}&to={date}` — consulta histórico para dashboard (roles: Admin, Teacher). |
| `AlertsController` | Controller | `GET /api/v1/alerts` — lista alertas activas (roles: Admin, Teacher). `GET /api/v1/alerts/{id}` — detalle de alerta. `PATCH /api/v1/alerts/{id}/acknowledge` — cambia estado a `Acknowledged` (rol: Admin). `PATCH /api/v1/alerts/{id}/dismiss` — cambia estado a `Dismissed` (rol: Admin). |
| `MonitoringConfigurationsController` | Controller | `GET /api/v1/monitoring-configurations` — lista configuraciones existentes (rol: Admin). `POST /api/v1/monitoring-configurations` — crea configuración de umbrales (rol: Admin). `PUT /api/v1/monitoring-configurations/{id}` — actualiza umbrales (rol: Admin). `GET /api/v1/monitoring-configurations/{classroomId}` — obtiene configuración por aula (rol: Admin). |

#### 4.2.5.3. Application Layer

La Application Layer orquesta los flujos de proceso del bounded context IoT Monitoring sin contener reglas de dominio propias. Esta capa contiene los command handlers, query handlers y event handlers (policies) que coordinan la interacción entre el Domain Layer y la Infrastructure Layer. Los command handlers reciben comandos provenientes de la Interface Layer y los traducen en operaciones sobre los aggregates del dominio. Los query handlers atienden consultas de solo lectura y pueden acceder directamente a proyecciones optimizadas para la visualización en el dashboard. Los event handlers actúan como políticas reactivas: en particular, el handler `GenerateAlertOnThresholdExceededHandler` reacciona al evento de dominio `EnvironmentalThresholdExceeded` y orquesta la creación de una nueva `Alert`, manteniendo así la responsabilidad de detección y emisión de alerta dentro de la Application Layer y no en la Interface Layer.

Esta separación garantiza que la lógica de evaluación de umbrales y generación de alertas sea completamente testeable de forma aislada y no esté acoplada al mecanismo de transporte HTTP.

| Clase | Tipo | Responsabilidad |
| --- | --- | --- |
| `IngestSensorReadingCommandHandler` | Command Handler | Recibe el comando `IngestSensorReadingCommand` con los datos de la lectura agregada, crea una instancia de `SensorReading`, la persiste a través de `ISensorReadingRepository` y publica los eventos de dominio resultantes. |
| `AcknowledgeAlertCommandHandler` | Command Handler | Recibe `AcknowledgeAlertCommand`, carga el `Alert` correspondiente por su Id, invoca la transición de estado a `Acknowledged` y persiste el cambio. |
| `DismissAlertCommandHandler` | Command Handler | Análogo a `AcknowledgeAlertCommandHandler` para la transición al estado `Dismissed`. |
| `ConfigureThresholdCommandHandler` | Command Handler | Recibe `ConfigureThresholdCommand`, crea o actualiza una `MonitoringConfiguration` y persiste los cambios. Publica `ThresholdConfigured`. |
| `GenerateAlertOnThresholdExceededHandler` | Event Handler (Policy) | Reacciona al evento `EnvironmentalThresholdExceeded`. Crea una nueva instancia de `Alert` en estado `Active` y la persiste. Publica `AlertGenerated`. |
| `GetActiveAlertsQueryHandler` | Query Handler | Devuelve la lista de alertas en estado `Active`, opcionalmente filtrada por aula o tipo de sensor. Utiliza `IAlertRepository`. |
| `GetReadingsHistoryQueryHandler` | Query Handler | Devuelve el historial de lecturas para un aula en un rango de tiempo dado, utilizando `ISensorReadingRepository`. Empleado por el dashboard de monitoreo. |
| `GetMonitoringConfigurationQueryHandler` | Query Handler | Devuelve la configuración de umbrales activa para un aula y tipo de sensor. Utiliza `IMonitoringConfigurationRepository`. |

#### 4.2.5.4. Infrastructure Layer

La Infrastructure Layer del contexto IoT Monitoring provee las implementaciones concretas de los contratos definidos en el Domain Layer, utilizando Entity Framework Core como ORM sobre una base de datos MySQL, consistente con la decisión de infraestructura tomada para el Web API de la plataforma EduSpace IoT (véase sección 4.1.3.3). Las implementaciones de repositorio traducen las operaciones de dominio en consultas LINQ sobre el `DbContext` correspondiente, garantizando que el modelo de dominio permanezca desacoplado del motor de persistencia. Adicionalmente, esta capa aloja el adaptador de comunicación saliente con el servicio de correo electrónico, invocado cuando se genera una alerta para notificar al Administrador.

El `IoTMonitoringDbContext` define los `DbSet` para los tres aggregates persistibles y configura las relaciones, índices y conversiones de tipos necesarios mediante la API de configuración fluida de Entity Framework Core, siguiendo las convenciones de nomenclatura en snake_case aplicadas en el resto del proyecto mediante Humanizer.

| Clase | Tipo | Tecnología / Responsabilidad |
| --- | --- | --- |
| `SensorReadingRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `ISensorReadingRepository`. Gestiona la persistencia y consulta de instancias de `SensorReading`. |
| `AlertRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `IAlertRepository`. Gestiona persistencia, consulta por estado y filtrado por aula de instancias de `Alert`. |
| `MonitoringConfigurationRepository` | Repository (implementación) | Entity Framework Core + MySQL. Implementa `IMonitoringConfigurationRepository`. Gestiona la persistencia y consulta de configuraciones de umbrales. |
| `IoTMonitoringDbContext` | DbContext | Entity Framework Core. Define los `DbSet<SensorReading>`, `DbSet<Alert>` y `DbSet<MonitoringConfiguration>`. Configura mappings, índices y conversiones del Value Object `AlertStatus`. |
| `AlertEmailNotificationAdapter` | External Adapter | SendGrid (HTTP). Implementa la interfaz `IAlertNotificationService`. Se invoca desde `GenerateAlertOnThresholdExceededHandler` para enviar una notificación por correo electrónico al Administrador cuando se genera una alerta `Active`. |

---

# Conclusiones

## Conclusiones y recomendaciones

---

# Bibliografía

Birimisa, A. (2025, 19 febrero). _El consumo de energía en los Colegios y cómo el FM puede generar ahorros_. https://www.linkedin.com/pulse/el-consumo-de-energ%C3%ADa-en-los-colegios-y-c%C3%B3mo-fm-puede-birimisa-ncnpe/

Córdova Negrete, M. G., Domínguez Toala, G. del P., & Córdova Cabrera, D. J. (2025). Retos y perspectivas de la gestión administrativa en la educación superior: fortalecimiento institucional, calidad educativa y liderazgo académico en el contexto globalizado. _Multidisciplinary Journal of Sciences, Discoveries, and Society_, _2_(2), e-207. https://doi.org/10.71068/xzb5wn45

Expertos En Educación. (2025, 22 septiembre). _Gestión educativa en el Perú: claves, retos y soluciones_. VIU Universidad Online. https://www.universidadviu.com/pe/actualidad/nuestros-expertos/gestion-educativa-en-el-peru-claves-retos-y-soluciones

Diaz, H. (2024, 25 junio). _Infraestructura escolar: soluciones frente al déficit y los desafíos tecnológicos - Educared_. Educared. https://educared.fundaciontelefonica.com.pe/desafios/infraestructura-escolar-soluciones-frente-al-deficit-y-los-desafios-tecnologicos/

Valencia, C., & Almeida, V. (2024). La tecnología en la gestión educativa. _Revista de Investigación Latinoamericana En Competitividad Organizacional_, _6_(23), 9859863. https://dialnet.unirioja.es/descarga/articulo/9859863.pdf#:~:text=En%20resumen%2C%20la%20integraci%C3%B3n%20de%20la%20tecnolog%C3%ADa,a%20la%20mejora%20de%20la%20calidad%20educativa.

Shanganlall, A. (2025, 21 febrero). _Los 7 mayores retos que afectan a la gestión de la educación_. Classter. https://www.classter.com/es/blog/edtech-es/los-7-mayores-retos-que-afectan-a-la-gestion-de-la-educacion/

---

# Anexos

## Anexo A: Estructura para la sección Student Outcome

## Anexo B: Videos de Exposiciones

| Entrega | Título | URL |
| ------- | ------ | --- |
| AV1     |        |     |
