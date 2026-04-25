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

* Mejorar la eficiencia operativa de las instituciones educativas un 25% en sus primeros 4 meses de uso del sistema.
* Se espera que al menos el 30% de nuestros clientes nos recomienden a otras instituciones dentro de los primeros 6 meses.
* Ofrecer la aplicación en múltiples idiomas incrementará la base de usuarios en un 25% en los primeros seis meses, permitiendo que más instituciones educativas de diferentes regiones utilicen la plataforma y contribuyendo a un crecimiento anual del 15%
*  Crear interfaz fácil de usar y visualmente atractiva que retenga al menos el 50% de usuarios después de los primeros 7 meses.
* Conseguir que más del 65% de usuarios pague la suscripción (anual o mensual) ofrecida. 

**User Assumptions:** 

**¿Quiénes serán nuestros usuarios?** 

Nuestros usuarios principales son: 

* Docentes y auxiliares entre las edades de 22 a 65 años que buscan una solución que facilite el monitoreo de ambientes y mejore la comunicación con los administradores.
* Administradores de instituciones educativas entre 35 a 60 años que necesitan una herramienta que permita gestionar eficazmente los espacios y recursos.

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

* Mejora en la gestión de los espacios y recursos, junto con una comunicación más eficiente entre los trabajadores.

**Los usuarios también pueden obtener estos beneficios adicionales:**

* Acceso rápido a la información en cualquier momento y desde cualquier dispositivo.

**El mayor riesgo para el usuario es:**

* Que la aplicación no se adapte correctamente a diferentes dispositivos o que no facilite la comunicación interna como se espera.

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
  * Incorporación de sensores que permitan detectar la presencia de personas, así como medir la temperatura y humedad en los ambientes educativos.


#### 1.2.2.3. Lean UX Hypothesis Statements

- Nosotros creemos que los usuarios necesitan una aplicación que les permita gestionar los espacios de su centro educativo de manera eficiente. Sabremos que es verdad cuando al menos el 50% de usuarios adquiera los planes de suscripción durante el primer mes.
- Nosotros creemos que al contar con una interfaz intuitiva, visualmente atractiva y sea fácil de usar reducirá la tasa de abandono del sistema. Sabremos que es verdad cuando al menos el 70% de los usuarios continúen utilizando la plataforma después del primer mes.
- Nosotros creemos que ofrecer la aplicación en múltiples idiomas incrementará la base de usuarios. Sabremos que es verdad cuando tengamos como mínimo un 30% de usuarios de otros países en el tercer mes.
- Nosotros creemos que el monitoreo en tiempo real mediante tecnologías IoT (presencia, temperatura, humedad y consumo energético) aportará valor a los usuarios en la gestión de los espacios. Sabremos que es verdad cuando los usuarios utilicen activamente estas funcionalidades y las consideren relevantes en la toma de decisiones operativas.

#### 1.2.2.4. Lean UX Canvas

## 1.3. Segmentos objetivo

**Administradores de instituciones educativas**

* Edad: 35 a 60 años
* Perfil: Directivos, coordinadores académicos, personal administrativo encargados de la gestión operativo de institución educativa.
* Uso de tecnología: Intermedio
* Necesidad principal: Optimizar la gestión de espacios, recursos y personal de manera centralizada.
* Beneficios buscados: Tener mayor control operativo, reducción de errores, ahorro de tiempo y mejora en la toma de decisiones.

**Características demográficas:** Profesionales entre 35 a 60 años, de género masculino y femenino, con formación en gestión educativa, administración o especialidades afines, que trabajan solamente en instituciones educativas.

**Características geográficas:** Principalmente ubicados en zonas urbanas de Perú, especialmente Lima Metropolitana, donde existen instituciones educativas con infraestructuras grandes y complejas.

**Docentes y auxiliares**

* Edad: 22 a 65 años
* Perfil: Profesores y personal de apoyo que utilizan los espacios educativos de las instituciones donde trabajan para desarrollar sus actividades diarias.
* Uso de tecnología: Básico a intermedio
* Necesidad principal: Acceder rápidamente a información sobre la disponibilidad de espacios y coordinar actividades sin complicaciones.
* Beneficios buscados: Acceso rápido a la información sobre los recursos y espacios disponibles, mejor comunicación y menos errores en la asignación de espacios.

**Características demográficas:** Profesionales del sector educativo entre 22 a 65 años, de género masculino y femenino, con formación académica en sus respectivas disciplinas (ciencias, literatura, entre otros), con experiencia en enseñanza.

**Características geográficas:** Principalmente ubicados en instituciones educativas con infraestructura compleja de zonas urbanas o semiurbanas de Perú, especialmente Lima Metropolitana.


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


Birimisa, A. (2025, 19 febrero). _El consumo de energía en los Colegios y cómo el FM puede generar ahorros_. https://www.linkedin.com/pulse/el-consumo-de-energ%C3%ADa-en-los-colegios-y-c%C3%B3mo-fm-puede-birimisa-ncnpe/

Córdova Negrete, M. G., Domínguez Toala, G. del P., & Córdova Cabrera, D. J. (2025). Retos y perspectivas de la gestión administrativa en la educación superior: fortalecimiento institucional, calidad educativa y liderazgo académico en el contexto globalizado. *Multidisciplinary Journal of Sciences, Discoveries, and Society*, *2*(2), e-207. https://doi.org/10.71068/xzb5wn45

Expertos En Educación. (2025, 22 septiembre). _Gestión educativa en el Perú: claves, retos y soluciones_. VIU Universidad Online. https://www.universidadviu.com/pe/actualidad/nuestros-expertos/gestion-educativa-en-el-peru-claves-retos-y-soluciones

Diaz, H. (2024, 25 junio). _Infraestructura escolar: soluciones frente al déficit y los desafíos tecnológicos - Educared_. Educared. https://educared.fundaciontelefonica.com.pe/desafios/infraestructura-escolar-soluciones-frente-al-deficit-y-los-desafios-tecnologicos/

Valencia, C., & Almeida, V. (2024). La tecnología en la gestión educativa. _Revista de Investigación Latinoamericana En Competitividad Organizacional_, _6_(23), 9859863. https://dialnet.unirioja.es/descarga/articulo/9859863.pdf#:~:text=En%20resumen%2C%20la%20integraci%C3%B3n%20de%20la%20tecnolog%C3%ADa,a%20la%20mejora%20de%20la%20calidad%20educativa.

Shanganlall, A. (2025, 21 febrero). _Los 7 mayores retos que afectan a la gestión de la educación_. Classter. https://www.classter.com/es/blog/edtech-es/los-7-mayores-retos-que-afectan-a-la-gestion-de-la-educacion/


---

# Anexos

## Anexo A: Estructura para la sección Student Outcome

## Anexo B: Videos de Exposiciones

| Entrega | Título | URL |
|---------|--------|-----|
| AV1 | | |
