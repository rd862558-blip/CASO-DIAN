# CASO-DIAN
En este grupo debe adjuntar todo el material para el desarrollo del trabajo 
# 🛡️ Threat Intel & Tactical Defense: Análisis de Incidente Crítico DIAN

**Estado del Repositorio:** `Activo / Fase de Mejora Continua`  
**Clasificación de la Información:** `TLP:GREEN / Ámbito Académico-Operativo`

Este repositorio centraliza la bitácora forense y el análisis táctico-estratégico de la reciente falla de infraestructura crítica que afectó a la Dirección de Impuestos y Aduanas Nacionales (DIAN) en Colombia. El objetivo principal no es solo documentar el evento, sino transformar la volumetría de incidentes (datos crudos) en inteligencia procesable (sabiduría) que permita la reestructuración de nuestras capacidades de ciberdefensa.

---

## 🎯 Contexto Operacional y Metodología (Qué, Por qué, Para qué, Cómo)

* **El Qué:** Disrupción severa de la tríada CID (Confidencialidad, Integridad, Disponibilidad) en los sistemas de recaudo y control aduanero del Estado.
* **El Por qué:** Identificación de brechas de seguridad perimetral, vulnerabilidades de ingeniería social (distorsión cognitiva) y dependencia excesiva de proveedores externos sin redundancia interna.
* **El Para qué:** Generar un marco de resiliencia institucional que anticipe amenazas persistentes avanzadas (APT) y evite el colapso de las comunicaciones críticas durante un ciberataque.
* **El Cómo:** Mediante el despliegue del ciclo de inteligencia y operaciones conjuntas (Blue/Red Team), evaluando la infraestructura bajo la lupa de marcos normativos nacionales e internacionales.

## 📂 Estructura del Análisis

La investigación documentada en este repositorio se divide en las siguientes áreas de foco:

### 1. Vectores de Infección y Psicología del Ataque
El eslabón más débil no fue el hardware, sino el factor humano. El análisis detalla cómo los atacantes utilizaron OSINT para perfilar objetivos con acceso privilegiado. Explotando la "vulnerabilidad de la pasión" y aplicando distorsión cognitiva, lograron envenenar la inteligencia desde dentro, evadiendo los controles tradicionales mediante ingeniería social dirigida (*spear-phishing*).

### 2. Tácticas de Persistencia en Ciberseguridad
Una vez dentro de la infraestructura de la entidad, el objetivo del adversario fue garantizar su supervivencia a largo plazo, incluso tras el reinicio de sistemas o la rotación de credenciales. Las investigaciones apuntan al uso de tácticas como:
> * **Modificación del Registro (Run Keys):** Inserción de ejecutables maliciosos en las llaves de arranque automático del sistema operativo.
> * **Tareas Programadas (Scheduled Tasks):** Creación de *scripts* silentes que se comunican con servidores de Comando y Control (C2) en horarios de bajo tráfico.
> * **Suscripciones a Eventos WMI:** Uso de instrumentación legítima de Windows para ejecutar código malicioso sin dejar rastros en el disco físico (ataques *fileless*).

### 3. Gestión de Infraestructura: SLA vs. ADLS
El incidente evidenció un colapso en la disponibilidad debido a la falta de protección integral y modular. Aquí diferenciamos dos conceptos críticos que fallaron:
* **SLA (Service Level Agreement):** El contrato vinculante con proveedores externos (ISP, Nube). La dependencia absoluta de este acuerdo paralizó la respuesta.
* **ADLS (Acuerdos de Niveles de Servicio Internos / OLA):** El compromiso operativo entre las dependencias tecnológicas internas de la organización. Su ausencia demostró que no existía un plan B de contención táctica propio.

## ⚖️ Marco Normativo y Doctrinario

El diseño, transición y operación de nuestras contramedidas se fundamenta estrictamente en la siguiente base legal y militar:

* **CONPES 3701, 3854, 3995:** Directrices nacionales para la gestión de riesgos digitales, confianza en el ciberespacio y protección de infraestructura crítica.
* **Ley 1621 de 2013:** Marco jurídico que ampara las actividades de inteligencia y salvaguarda los intereses estratégicos de la Nación.
* **Doctrina Militar (MEC 6-27.2 & Manual de Tallin 2.0):** Aplicación de los principios de la ciberdefensa en escenarios de guerra asimétrica, evaluación de la soberanía digital y el Código de Ética (principios del hacker ético).
* **Estándares ISO:** Alineación con las familias ISO 27001 (SGSI) para asegurar una gestión holística del riesgo.

---

*Nota para los investigadores: Todo commit y actualización en las ramas de este repositorio debe incluir la trazabilidad de las fuentes y mapear detalladamente los casos de estudio, priorizando siempre la supremacía y confiabilidad de la información.*
