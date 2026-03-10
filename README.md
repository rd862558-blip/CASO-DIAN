# 🛡️ Threat Intel Dossier: Colapso de Infraestructura Crítica (Caso DIAN / IFX)

> **Clasificación:** `TLP:AMBER` | **Estado:** `Fase 5 - Mejora Continua` | **Dominio:** `Ciberdefensa Estatal`

Este repositorio centraliza la bitácora táctico-estratégica sobre la disrupción sistémica que afectó a la Dirección de Impuestos y Aduanas Nacionales (DIAN) en Colombia, producto del compromiso a la cadena de suministro tecnológica (IFX Networks). El objetivo es trascender el reporte técnico para consolidar inteligencia procesable que obligue a la reestructuración de la doctrina de defensa digital del Estado.

---

## 🎯 1. Coordenadas de la Misión (Qué, Por qué, Para qué, Cómo)

* **El Qué:** Disrupción severa de la infraestructura crítica nacional mediante un ataque de ransomware a la cadena de suministro.
* **El Por qué:** Identificación de una falla sistémica en la contención perimetral, dependencia absoluta de terceros y obsolescencia en los planes de contingencia (BCP/DRP).
* **El Para qué:** Generar sabiduría operativa que permita blindar el ecosistema digital estatal, anticipando amenazas avanzadas (APT) y recuperando la soberanía de los datos.
* **El Cómo:** A través de una autopsia forense cruzando telemetría técnica, la matriz MITRE ATT&CK y el escrutinio del marco normativo y militar vigente.

---

## 🧠 2. Epistemología del Ataque: De los Datos a la Sabiduría

El análisis de este incidente exige superar la simple recolección de eventos. Hemos aplicado el ciclo de inteligencia para transformar el ruido en capacidad de anticipación, evaluando la asimetría en el **Ciclo OODA** (Observar, Orientar, Decidir, Actuar). Mientras el Estado "observaba" la caída, el adversario ya estaba "actuando".

1.  **Datos:** Recolección cruda de IoCs, logs de red y firmas del *ransomware* desplegado en los servidores.
2.  **Información:** Correlación del vector de acceso, confirmando el compromiso de la infraestructura hiperconvergente del proveedor externo.
3.  **Conocimiento:** Mapeo de las Tácticas, Técnicas y Procedimientos (TTPs). Entendimiento del movimiento lateral y las tácticas de doble extorsión.
4.  **Sabiduría:** La internalización estratégica de que el perímetro ya no existe. La defensa debe asumir la brecha desde el diseño (Zero Trust) y no depender exclusivamente de un SLA externo.

---

## 💥 3. Radiografía de la Falla: Tríada CID y el Espejo de Keralty

El ataque evidenció la fragilidad de la Tríada de Seguridad. Para dimensionar el riesgo, cruzamos el evento con el ataque a la infraestructura de salud de **Keralty/Sanitas**:

* **Disponibilidad (Colapso en Cascada):** La paralización aduanera demostró una arquitectura monolítica. La fricción crítica se dio entre el **SLA** (Acuerdo de Nivel de Servicio - el contrato de papel con IFX) y la absoluta inexistencia de un **ADLS** (Acuerdo de Nivel de Servicio Operativo interno), dejando a la entidad sin capacidad técnica de respuesta autónoma.
* **Confidencialidad e Integridad (Doble Extorsión):** Al igual que en Keralty, el secuestro de datos tributarios es solo la primera fase. La amenaza de exposición o manipulación de esta inteligencia financiera equivale a alterar coordenadas de artillería en la doctrina militar: genera *inteligencia envenenada*.

---

## 🕷️ 4. Vectores y Persistencia (Mapeo MITRE ATT&CK)

La vulneración no ocurrió por fuerza bruta criptográfica, sino explotando el eslabón humano.

* **Acceso Inicial & Psicología:** Mediante reconocimiento OSINT, los atacantes perfilaron administradores clave. Utilizando la "vulnerabilidad de la pasión" y la **distorsión cognitiva**, ejecutaron campañas de *spear-phishing*. Manipularon el sentido de urgencia para que los propios operadores eludieran los protocolos de seguridad.
* **Persistencia Táctica:** Una vez dentro, el adversario aseguró su supervivencia a largo plazo mediante:
    * `Registry Run Keys` (Modificación de llaves de auto-arranque).
    * `Scheduled Tasks` (Scripts de balizamiento C2 silentes).
    * `WMI Event Subscription` (Ejecución de código *fileless* o sin archivos).

---

## ⚖️ 5. Cerco Normativo y Doctrinario

La respuesta frente a esta degradación de comunicaciones debe alinearse estrictamente con el marco legal e institucional:

* **Legislación y Política Pública:** La exfiltración compromete la **Ley 1621 de 2013** (Seguridad e Inteligencia de la Nación). Asimismo, evidencia fallas en la adopción de los **CONPES 3701, 3854 y 3995** respecto a la resiliencia de infraestructura crítica y confianza digital.
* **Estándares ISO:** El incidente subraya la urgencia de auditar la cadena de suministro bajo la **ISO 27000** (SGSI) y la **ISO 27032** (Directrices de Ciberseguridad).
* **Doctrina Militar (MEC 6-27.2 & Manual de Tallin 2.0):** Desde una óptica de ciberdefensa conjunta, el ataque plantea un desafío a la soberanía digital del Estado. La actuación del analista debe regirse por el Código de Ética de la FAC y los principios del hacker ético para restaurar la supremacía de la información.

---

## 🛡️ 6. El Analista Híbrido: Los 3 Súper Poderes y Contención

El software no detiene a un adversario motivado; lo hace un operador con criterio. El equipo de respuesta debe dominar **"Los 3 Súper Poderes"**: *Adaptabilidad* (para mutar la defensa), *Resiliencia Operativa* (para mantener el control bajo fuego) y *Proactividad Purple Team* (para pensar como el atacante).

### Ciclo Operativo de Recuperación (5 Fases)
1.  **Análisis:** Autopsia forense y aislamiento de los entornos comprometidos.
2.  **Diseño:** Reestructuración hacia redes divergentes y microsegmentadas.
3.  **Transición:** Activación real (no teórica) de laboratorios y simulacros de los planes BCP y DRP.
4.  **Operación:** Despliegue de patrullas de *Threat Hunting* continuo en la red activa.
5.  **Mejora Continua:** Centralización inmutable de scripts, IoCs y tácticas mitigadas en este repositorio, asegurando la trazabilidad operativa y el aprendizaje institucional.

> *"La supremacía de la información no se garantiza firmando contratos con proveedores, sino asumiendo el control táctico de nuestra propia infraestructura."*
