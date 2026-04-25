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

### 1.1.2. Perfiles de integrantes del equipo

## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

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
    <td align= "center"><div>EduSpace</div><img src="https://github.com/user-attachments/assets/aa72b842-fa31-4a24-b10b-7d3444705e3d" alt="logo-eduspace" width="50"/>  </td>
    <td align= "center"><div>Siemens Smart Infrastructure</div> <img src="/assets/images/siemens_logo.png" alt="logo-siemens" width="50"/> </td>
    <td align= "center"><div>Cisco Spaces</div> <img src="/assets/images/cisco_logo.png" alt="logo-cisco" width="50"/> </td>
    <td align= "center"><div>Honeywell Building Tech</div><img src="/assets/images/honeywell_logo.png" alt="logo-honeywell" width="50"/> </td>
    <td align= "center"><div>Spacewell</div> <img src="/assets/images/spacewell_logo.png" alt="logo-spacewell" width="50"/> </td> 
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

* Alto nivel de automatización y precisión en sus sistemas
* Soluciones integrales a gran escala (energía, seguridad, infraestructura)
* Amplia experiencia y posicionamiento en el mercado
* Uso de tecnologías avanzadas como IA, Big Data y analítica predictiva
##### **Fortalezas de Smart Campus IoT:**
* Especialización en el sector educativo
* Integración con procesos académicos (aulas, horarios, docentes)
* Bajo costo de implementación
* Flexibilidad y escalabilidad modular
* Enfoque en analítica aplicada a la toma de decisiones académicas
##### **Estrategias**
* Diferenciar la propuesta mediante un enfoque específico en educación.
* Posicionar la solución como una herramienta de gestión académica basada en datos.
* Priorizar la simplicidad y accesibilidad frente a soluciones complejas y costosas.
##### **Tácticas**
* Desarrollar dashboards orientados a indicadores académicos (uso de aulas, eficiencia).
* Comunicar el valor del sistema en términos de mejora del aprendizaje y optimización de recursos.
* Implementar módulos iniciales simples que puedan escalar progresivamente.

#### **Frente a las debilidades de los competidores**

Se identificaron las siguientes debilidades en los competidores:

* Alto costo de implementación
* Complejidad técnica e infraestructura pesada
* Falta de enfoque en el sector educativo
* Limitada adaptación a procesos académicos específicos
##### **Debilidades de Smart Campus IoT:**
* Menor precisión frente a soluciones industriales
* Dependencia de sensores de bajo costo
* Limitada validación en escenarios reales
##### **Estrategias**
* Aprovechar la falta de especialización educativa de los competidores.
* Enfocar la solución en necesidades concretas de instituciones educativas.
* Diseñar un sistema fácil de implementar y mantener.
##### **Tácticas**
* Desarrollar funcionalidades específicas como monitoreo por horario académico y score de aula.
* Realizar pilotos en instituciones educativas para validar el sistema.
* Optimizar el uso de sensores accesibles manteniendo precisión suficiente para el contexto educativo.

## 2.2. Entrevistas

### 2.2.1. Diseño de entrevistas

Las entrevistas permitirán recolectar información cualitativa sobre cómo se gestionan actualmente los espacios académicos, recursos e infraestructura en instituciones educativas, identificando problemas, necesidades y oportunidades para validar la propuesta de EduSpace.

#### Segmento 1: Administradores de instituciones educativas

Objetivo: Comprender cómo los administradores gestionan aulas y recursos, qué dificultades enfrentan y qué valor perciben en una solución basada en monitoreo en tiempo real.

* ¿Cómo verifican si las aulas están siendo utilizadas correctamente?
* ¿Qué herramientas utilizan para el control de espacios y recursos?
* ¿Cómo monitorean el consumo de energía o mantenimiento de aulas?
* ¿Qué dificultades enfrentan en la gestión de aulas?
* ¿Qué tan frecuente es el desperdicio de recursos (luces, equipos encendidos)?
* ¿Tienen visibilidad en tiempo real de lo que ocurre en las aulas?
* ¿Qué tan importante sería contar con datos en tiempo real sobre uso de aulas?
* ¿Te sería útil recibir alertas sobre ineficiencias o problemas?
* ¿Qué opinas de un sistema que monitoree aulas en tiempo real?
* ¿Qué funcionalidades considerarías más importantes?
* ¿Qué te generaría más valor: ahorro de costos, control o mejora académica?
* ¿Implementarías una solución así en tu institución? ¿Por qué?
* ¿Qué barreras ves para su implementación? (costo, tecnología, cultura, etc.)

#### Segmento 2: Docentes y auxiliares

Objetivo: Comprender cómo perciben el uso de aulas, condiciones del entorno y problemas que afectan el desarrollo de clases.

* ¿Has tenido problemas con temperatura, ruido o equipos?
* ¿Qué te gustaría mejorar en las aulas?
* ¿Te sería útil conocer el estado de un aula antes de ingresar?
* ¿Qué opinas de un sistema que monitoree las condiciones del aula?
* ¿Te ayudaría saber si un aula está disponible o en buenas condiciones?
* ¿Qué funcionalidad te sería más útil como docente?
* ¿Crees que un sistema así mejoraría tu experiencia al enseñar?

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

En este capítulo, el equipo presenta las decisiones de diseño estratégico para la solución EduSpace IoT, aplicando los principios de Domain-Driven Design (DDD). El objetivo de este nivel de diseño es identificar y definir los bounded contexts que conforman el sistema, comprender cómo interactúan entre sí y establecer una arquitectura clara que soporte tanto las funcionalidades existentes de gestión de espacios como las nuevas capacidades de monitoreo IoT. Las secciones a continuación abarcan las sesiones de Design-Level EventStorming, el proceso de Candidate Context Discovery, el modelado de Domain Message Flows, los Bounded Context Canvases, el Context Mapping y los diagramas de Arquitectura de Software.

### 4.1.1. Design-Level EventStorming

Tomando como base el Big Picture EventStorming realizado en el Capítulo II, el equipo llevó a cabo una serie de sesiones de Design-Level EventStorming con el objetivo de modelar cada bounded context con mayor nivel de detalle. A diferencia de la sesión de Big Picture, que se enfocó en comprender el dominio del negocio a alto nivel, el Design-Level EventStorming profundiza en la mecánica interna de cada contexto, incorporando Commands, Aggregates, Policies y Read Models junto a los Domain Events.

Las sesiones se realizaron de forma colaborativa utilizando LucidChart como herramienta de modelado, y abarcaron los seis bounded contexts identificados durante la sesión de Big Picture: Identity & Access Management, Space & Resource Management, Reservation & Scheduling, Breakdown Management y el nuevo contexto de IoT Monitoring. Se prestó especial atención al contexto de IoT Monitoring, al ser la incorporación principal de esta iteración e introducir nuevos actores como el dispositivo ESP32 y el Edge API.

A continuación se presentan los diagramas resultantes para cada bounded context.

![Design Level Event Storming](/assets/images/design-level-event-storming.png)

#### 4.1.1.1. Candidate Context Discovery

A partir del Design-Level EventStorming realizado, el equipo llevó a cabo el proceso de Candidate Context Discovery con el objetivo de identificar y delimitar los bounded contexts del sistema. Para ello se aplicó la técnica look-for-pivotal-events, que consiste en identificar los eventos clave del negocio que marcan cambios de estado significativos entre diferentes partes del proceso, y que naturalmente señalan las fronteras entre contextos.

Como resultado del análisis, se identificaron seis bounded contexts. A continuación se presenta cada uno con su justificación:

| # | Bounded Context | Eventos pivote que delimitan su frontera | Justificación |
|---|----------------|------------------------------------------|---------------|
| 1 | **Identity, Access & Profile Management** | `AdminAccountCreated`, `TeacherAccountCreated`, `SessionStarted` | Agrupa todo lo relacionado con la autenticación, control de acceso y gestión de perfiles de usuario. Es el contexto de entrada obligatorio para cualquier usuario y concentra tanto las credenciales de acceso como la información personal asociada a cada cuenta. |
| 2 | **Space & Resource Management** | `ClassroomRegistered`, `SharedAreaRegistered`, `ResourceAddedToClassroom`, `TeacherAssignedToClassroom` | Agrupa la configuración y administración de todos los espacios físicos e inventario de recursos de la institución. Es el contexto core del negocio original. |
| 3 | **Reservation & Scheduling** | `SharedAreaReserved`, `ReservationConfirmed`, `MeetingScheduled`, `TeacherInvitedToMeeting` | Gestiona la planificación y reserva de espacios compartidos y reuniones. Se separa de Space & Resource Management porque opera sobre disponibilidad y tiempo, no sobre el registro de espacios. |
| 4 | **Breakdown Management** | `BreakdownReported`, `ReportStatusUpdated` | Concentra el ciclo de vida completo de los reportes de averías, desde su creación por un docente hasta su resolución por el administrador. |
| 5 | **IoT Monitoring** | `SensorReadingCaptured`, `EnvironmentalThresholdExceeded`, `OccupancyStatusChanged`, `AlertGenerated` | Contexto nuevo incorporado en esta iteración. Gestiona la captura, procesamiento y visualización de datos provenientes de los dispositivos IoT instalados en las aulas, así como la generación de alertas automáticas. Se delimita como contexto independiente debido a que introduce nuevos actores (ESP32, Edge API), un flujo de datos completamente distinto al resto del sistema y requisitos técnicos propios del mundo embebido. |

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
