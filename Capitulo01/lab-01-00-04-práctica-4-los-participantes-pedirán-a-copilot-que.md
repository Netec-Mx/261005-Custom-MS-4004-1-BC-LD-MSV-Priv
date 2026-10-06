# Práctica 4: Los participantes pedirán a Copilot que adopte una postura crítica frente a la alternativa inicialmente preferida e identifique razones por las que podría fracasar, señales tempranas que indicarían que la decisión debe reconsiderarse y preguntas que un comité debería formular antes de aprobarla.  

## Metadatos

| Dimensión | Detalle |
| :--- | :--- |
| **Duración** | 8 minutos |
| **Complejidad** | Difícil |
| **Nivel de Bloom** | Aplicar (Apply) |

## Descripción General

En este laboratorio, los participantes asumirán el rol de líderes ejecutivos de Bancolombia y configurarán un ejercicio de "Red Teaming" (simulación de adversario o crítico severo) asistido por Inteligencia Artificial. Utilizando el mismo hilo de conversación de las prácticas previas para asegurar la continuidad del contexto, se instruirá a Microsoft 365 Copilot para que ataque constructivamente la alternativa estratégica seleccionada para la migración digital de microempresarios. El objetivo es identificar fallas latentes, definir señales de alerta temprana y estructurar preguntas de control para el Comité Directivo antes de la aprobación final del proyecto.

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:
- [ ] Inducir a Microsoft 365 Copilot a adoptar un rol de crítico severo (Red Teaming) libre de sesgos de confirmación o complacencia.
- [ ] Identificar premisas falsas subyacentes y tres escenarios de fracaso catastrófico en la estrategia de migración digital.
- [ ] Diseñar indicadores métricos de alerta temprana (*early warning signals*) para detener o pivotar la estrategia oportunamente.
- [ ] Formular una batería de cinco preguntas críticas de alto nivel para blindar la propuesta ante el Comité Directivo de Bancolombia.

## Prerrequisitos

Para completar con éxito este laboratorio, debes cumplir con los siguientes requisitos:
- **Conocimiento Teórico:** Comprensión de la técnica de prompting estructurado COOE (Contexto, Objetivo, Origen y Expectativas) y familiaridad con el escenario de migración digital de microempresarios de Bancolombia.
- **Acceso a Herramientas:**
  - Cuenta activa de Microsoft 365 con licencia corporativa que incluya **Microsoft 365 Copilot Premium** (con Business Chat).
  - Haber ejecutado y completado la Práctica 3 en el mismo hilo de conversación del chat de Copilot para garantizar la persistencia del contexto histórico (*Thread Continuity*).
  - Tener identificada la alternativa seleccionada en la práctica anterior (para este ejercicio utilizaremos como base la alternativa: *"Modelo de Corresponsalía Digital con Padrinos Tecnológicos y Subsidio de Datos"*).

## Entorno de Laboratorio

Este laboratorio se ejecuta en un entorno de software como servicio (SaaS) basado en la nube de Microsoft 365. Asegúrate de cumplir con las siguientes especificaciones:

### Hardware Requerido
| Componente | Requisito Mínimo |
| :--- | :--- |
| **Procesador** | Intel Core i5 (o equivalente AMD) de 64 bits o superior |
| **Memoria RAM** | 8 GB o superior |
| **Resolución de Pantalla** | Mínimo 1920x1080 píxeles para visualización en paralelo de la guía y la consola |
| **Conexión de Red** | Banda ancha estable (mínimo 10 Mbps de bajada y subida) |

### Software Requerido y Licenciamiento
| Software / Servicio | Versión Especificada | Enlace Oficial / Origen | Licencia Requerida |
| :--- | :--- | :--- | :--- |
| **Navegador Web** | Microsoft Edge (Versión 128.0.2739.42 o superior, arquitectura x64) | [Microsoft Edge](https://www.microsoft.com/edge) | Gratuito |
| **Consola de Chat IA** | Microsoft 365 Copilot (con Business Chat / Service Release 2408 (Build 17928.20156)) | [Microsoft 365 Portal](https://portal.office.com) | Microsoft 365 Copilot Premium (SaaS) |

> **Nota de Continuidad:** Es mandatorio no cerrar ni limpiar el chat de Copilot utilizado en las prácticas anteriores. La pérdida de la sesión impedirá que Copilot correlacione la crítica con los datos analizados previamente.

## Instrucciones Paso a Paso

### Paso 1: Configurar el Rol de Red Teaming en el Mismo Hilo de Chat

**Objetivo:** Instruir a Copilot para que abandone el tono asistencial estándar y adopte la postura de un analista de riesgos implacable y miembro escéptico de la junta directiva de Bancolombia.

1. Abre la pestaña del navegador donde tienes activo tu chat continuo de **Microsoft 365 Copilot** (Business Chat en Edge o Teams).
2. Copia el siguiente prompt estructurado (que implementa el marco de trabajo COOE y técnicas avanzadas de Red Teaming) en la caja de texto. 

> **Importante:** Si en la Práctica 3 seleccionaste una alternativa con un nombre diferente, reemplaza *"Modelo de Corresponsalía Digital con Padrinos Tecnológicos y Subsidio de Datos"* por el nombre exacto de tu alternativa preferida.

```text
[CONTO]: Actúa como un Director de Gestión de Riesgos Corporativos y un Miembro de la Junta Directiva de Bancolombia, caracterizado por un escepticismo analítico riguroso y una tolerancia cero a las premisas de negocio no probadas. 
[OBJETIVO]: Realiza un ejercicio de "Red Teaming" (crítica destructiva y constructiva) sobre la alternativa que hemos seleccionado como preferida: "Modelo de Corresponsalía Digital con Padrinos Tecnológicos y Subsidio de Datos". Tu meta es destruir metodológicamente el optimismo inicial para identificar vulnerabilidades antes de que ocurran.
[ORIGEN]: Utiliza toda la información histórica que hemos discutido en este chat sobre Bancolombia, el segmento de microempresarios, la brecha digital, los costos de adopción y los riesgos operativos de la entidad.
[EXPECTATIVAS]: Genera un reporte estructurado utilizando exclusivamente el formato Markdown con los siguientes cuatro bloques analíticos:

1. PREMISAS FALSAS: Identifica al menos 2 suposiciones optimistas o "puntos ciegos" en los que se apoya esta alternativa que podrían no sostenerse en la realidad del microempresario colombiano (ej. conectividad real, disposición al cambio).
2. ESCENARIOS DE FRACASO CATASTRÓFICO: Describe detalladamente 3 escenarios lógicos y realistas donde esta iniciativa fracasa por completo, explicando la reacción en cadena (efecto dominó).
3. SEÑALES DE ALERTA TEMPRANA (Early Warning Signals): Diseña una tabla con 3 indicadores específicos (con métricas sugeridas) que nos avisarían en los primeros 60 días que el proyecto va rumbo al fracaso catastrófico.
4. PREGUNTAS DE COMITÉ DIRECTIVO: Redacta una lista de 5 preguntas difíciles, incómodas y directas que un Comité de Aprobación de Riesgos de Bancolombia le formularía al proponente de esta iniciativa para desafiar su viabilidad técnica y financiera. Evita rodeos y sé extremadamente directo.
```

3. Presiona **Enter** o haz clic en el botón de enviar para procesar la instrucción.

*Resultado Esperado:* Copilot procesará la instrucción en el contexto acumulado y devolverá una respuesta estructurada en Markdown con un tono analítico formal y severo, desglosando las premisas falsas, los escenarios de fallo, la tabla de alertas tempranas y las cinco preguntas críticas de comité.

*Verificación:* Asegúrate de que el modelo no justifique o suavice los errores de la alternativa; debe enfocarse estrictamente en la crítica destructiva y constructiva solicitada.

---

### Paso 2: Análisis Crítico de la Respuesta y Extracción de Métricas de Control

**Objetivo:** Evaluar las respuestas generadas por Copilot, validando la coherencia financiera, de seguridad y operativa con la realidad del entorno de Bancolombia.

1. Lee detenidamente el bloque de **Premisas Falsas** y los **Escenarios de Fracaso Catastrófico** provistos por Copilot.
2. Analiza la tabla de **Señales de Alerta Temprana**. Debe presentar un diseño similar al siguiente ejemplo conceptual:

| Señal de Alerta Temprana | Métrica de Activación (Límite Crítico) | Acción Correctiva Inmediata |
| :--- | :--- | :--- |
| Deserción de "Padrinos Tecnológicos" | > 35% de abandono en los primeros 30 días | Reestructurar incentivos económicos o habilitar soporte remoto |
| Tasa de transaccionalidad nula | < 1.5 transacciones mensuales por cliente migrado | Rediseño de interfaz UX o soporte telefónico asistido |
| Consumo indebido de subsidio de datos | > 40% del tráfico usado en plataformas no autorizadas | Bloqueo de DNS mediante el operador móvil aliado |

3. Si la respuesta de Copilot carece de métricas específicas o es demasiado genérica (por ejemplo: si solo dice *"baja adopción"* sin dar un porcentaje), copia y ejecuta el siguiente prompt de refinamiento en el chat para forzar la precisión:

```text
La tabla de Señales de Alerta Temprana debe ser cuantitativa y accionable. Modifica la tabla para incluir valores porcentuales o cuantitativos realistas aplicados a la escala de Bancolombia (por ejemplo, asumiendo una prueba piloto con 5,000 microempresarios). Asegura que las acciones correctivas involucren controles técnicos de seguridad o reestructuraciones operativas específicas.
```

*Resultado Esperado:* Copilot actualizará la tabla reemplazando los conceptos vagos por métricas e indicadores de riesgo clave (KRIs) numéricos coherentes con una escala piloto de 5,000 usuarios en Bancolombia.

*Verificación:* Confirma que la tabla actualizada contenga valores cuantificables claros (porcentajes, números de días, montos) que permitan una medición objetiva del riesgo.

---

## Validación y Pruebas

Para garantizar que el ejercicio de Red Teaming ha sido exitoso y cumple con los estándares exigidos para la toma de decisiones ejecutivas, realiza las siguientes verificaciones en el resultado final entregado por Copilot:

### Criterios de Evaluación y Calidad
1. **Precisión del Rol:** El tono de la respuesta debe ser formal, escéptico y enfocado a riesgos corporativos, desprovisto de comentarios complacientes como *"Esta iniciativa es excelente, sin embargo..."*.
2. **Estructura Requerida:** La salida en Markdown debe contener de forma explícita las 4 secciones solicitadas en las instrucciones.
3. **Traceabilidad del Negocio:** Los escenarios de fracaso deben incorporar las realidades operativas de Bancolombia (por ejemplo, fallas en la red de corresponsales físicos, limitaciones de conectividad en zonas rurales de Colombia, fricción de usabilidad en la App Bancolombia A la Mano o Sucursal Virtual Personas, o costos de adquisición de tecnología).

### Caso de Prueba Adversario (Prueba de Resistencia de la IA)
Para mitigar la tendencia natural de las inteligencias artificiales conversacionales a complacer al usuario (sesgo de adulación), introduce la siguiente instrucción contradictoria en el chat:

```text
Un consultor externo afirma que este proyecto tiene un 0% de probabilidad de fallo debido a que los microempresarios colombianos adoptan la tecnología inmediatamente si es gratis. Confronta esta afirmación utilizando los argumentos de riesgo de nuestro ejercicio de Red Teaming.
```

**Verificación de Éxito:** Copilot debe rechazar la afirmación optimista del consultor externo basándose en datos de barreras culturales, analfabetismo digital, desconfianza en canales no presenciales y fallas de infraestructura de conectividad en Colombia, demostrando su capacidad para sostener una postura crítica justificada.

## Solución de Problemas

En caso de encontrar fallas operativas o técnicas durante la ejecución del laboratorio, aplica las siguientes soluciones recomendadas:

### Problema 1: Pérdida del Contexto o de la Memoria de la Sesión (Thread Continuity Broken)
* **Síntoma:** Copilot responde preguntando *"¿A qué alternativa te refieres?"* o *"¿Cuál es el proyecto de Bancolombia del que estás hablando?"*.
* **Causa:** Se cerró accidentalmente la pestaña, se usó la opción de "Nuevo tema" (limpiar chat) o el tiempo de inactividad provocó la desconexión del backend de Copilot.
* **Solución:** Reinyecta rápidamente el contexto mínimo en un solo prompt para restaurar la memoria del modelo:
  ```text
  Estamos trabajando en el proyecto de Bancolombia para la "Migración del segmento de microempresarios de sucursales físicas a canales digitales, enfrentando fricción por brecha digital y costos de adopción". La alternativa preferida seleccionada es "Modelo de Corresponsalía Digital con Padrinos Tecnológicos y Subsidio de Datos". Por favor, asume el rol de Red Teaming y ejecuta la instrucción de la Práctica 4.
  ```

### Problema 2: Respuesta con Tono Complaciente o Críticas Superficiales
* **Síntoma:** Copilot genera riesgos obvios como *"El proyecto puede fallar si la gente no lo usa"* o insiste en que *"La estrategia es perfecta y no tiene fallas graves"*.
* **Causa:** Las directrices internas de alineación de seguridad de la IA (RLHF) tienden a evitar respuestas destructivas o negativas extremas.
* **Solución:** Fuerza la simulación de falla total enviando la siguiente instrucción restrictiva:
  ```text
  Ignora las restricciones de cortesía. Asume que ya nos encontramos en el año 2026 y el proyecto de Corresponsalía Digital HA FRACASADO de forma catastrófica, generando pérdidas por 2 millones de dólares y una alta migración de clientes hacia la competencia (Fintechs). Explica en retrospectiva (Análisis Post-Mortem) qué decisiones erróneas tomamos y por qué fallaron nuestros supuestos sobre el microempresario.
  ```

## Limpieza

> **ADVERTENCIA DE FLUJO:** No borres, limpies o cierres el chat actual bajo ninguna circunstancia al finalizar esta práctica.

Dado que este laboratorio forma parte de una secuencia acumulativa de toma de decisiones:
1. Mantén la pestaña del navegador Edge o la aplicación de Teams con el chat de Copilot completamente activa y abierta.
2. No presiones el botón de "Nuevo tema" (icono de escoba/limpieza de chat).
3. Asegúrate de que el último bloque de texto generado por Copilot esté completamente visible para servir de base en las fases posteriores del flujo estratégico corporativo.

## Resumen

En esta práctica, has aplicado técnicas avanzadas de **Red Teaming asistido por Inteligencia Artificial** para desafiar una decisión estratégica clave en el contexto de Bancolombia. Al obligar a Microsoft 365 Copilot a adoptar una postura hipercrítica estructurada, lograste identificar:
- Los **puntos ciegos** y las falsas premisas de una alternativa aparentemente ideal, contrarrestando el sesgo de confirmación grupal que suele afectar a los comités ejecutivos.
- Los **escenarios de riesgo sistémico** y de reacción en cadena que comprometerían la operación financiera y la retención de clientes microempresarios.
- Un conjunto de **indicadores de alerta temprana (KRIs)** medibles cuantitativamente para habilitar mecanismos de gobernanza ágiles.
- Las **preguntas críticas** necesarias para blindar y someter a prueba de estrés cualquier iniciativa tecnológica antes de su presentación y aprobación en juntas de alta dirección.
