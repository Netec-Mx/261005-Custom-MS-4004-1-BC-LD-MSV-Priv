# Práctica 2: El instructor proporcionará directamente en el escenario la información necesaria sobre comportamiento del segmento, experiencia del cliente, restricciones operativas y objetivos esperados. Los participantes construirán un prompt utilizando Contexto + Objetivo + Origen + Expectativas para solicitar a Copilot que organice la situación sin generar todavía una recomendación. El resultado deberá separar qué se sabe, qué se está suponiendo y qué sería necesario validar. (

## Metadatos

| Campo | Detalle |
|:---|:---|
| **Duración** | 6 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Aplicar (Apply) |
| **Módulo** | 1.0 — Prompting Avanzado para Líderes Ejecutivos |
| **Práctica** | 2 de 10 (secuencial y acumulativa) |
| **Modalidad** | Individual con discusión grupal al cierre |

## Descripción General

En esta práctica, cada participante escuchará un escenario ejecutivo presentado verbalmente por el instructor —centrado en la migración del segmento de microempresarios de sucursales físicas a canales digitales de Bancolombia— y construirá un prompt estructurado bajo el marco **COOE (Contexto + Objetivo + Origen + Expectativas)** en Microsoft 365 Copilot Chat. El propósito del prompt es que Copilot **organice** la situación de negocio sin emitir recomendaciones, separando explícitamente lo que se sabe con certeza, lo que se está suponiendo y lo que requiere validación antes de tomar decisiones. Esta actividad desarrolla la competencia de formulación precisa de instrucciones para obtener respuestas analíticas de alta utilidad ejecutiva.

## Objetivos de Aprendizaje

Al completar esta práctica, serás capaz de:

- [ ] Construir un prompt ejecutivo completo y bien estructurado aplicando el marco **Contexto + Objetivo + Origen + Expectativas (COOE)** en Microsoft 365 Copilot Chat.
- [ ] Solicitar a Microsoft 365 Copilot que organice una situación de negocio compleja sin generar recomendaciones de acción, obteniendo una clasificación tripartita de la información (hechos, supuestos, pendientes).
- [ ] Interpretar y evaluar críticamente el resultado generado por Copilot verificando que la respuesta separe correctamente hechos confirmados, supuestos implícitos y elementos pendientes de validación.
- [ ] Identificar al menos una oportunidad concreta de refinamiento iterativo en el prompt construido para mejorar la precisión de la respuesta en un contexto ejecutivo real.

## Prerrequisitos

### Conocimientos Previos

| Requisito | Descripción |
|:---|:---|
| Marco COOE | Haber completado la Práctica 1 del Módulo 1.0 o conocer la estructura de prompting Contexto + Objetivo + Origen + Expectativas. |
| Interacción básica con Copilot | Haber realizado al menos una consulta previa en Microsoft 365 Copilot Chat (según prerrequisitos generales del curso). |
| Comprensión del escenario base | Familiaridad con el escenario del curso: *Migración del segmento de microempresarios de sucursales físicas a canales digitales de Bancolombia, enfrentando fricción por brecha digital y costos de adopción.* |

### Acceso y Configuración

| Requisito | Detalle |
|:---|:---|
| Cuenta corporativa | Sesión activa con cuenta `@bancolombia.com.co` en el tenant de Bancolombia. |
| Licencia | Microsoft 365 Copilot Premium activa y asignada (Service Release 2408, Build 17928.20156). |
| Sesión de Copilot Chat | Chat abierto en `https://m365.cloud.microsoft/chat` (modo **Work**) o en Microsoft Teams (Trabajo o Escuela) versión 24193.1805.2987.5853. |
| Bloc de notas | Papel físico o aplicación de notas digital para capturar los elementos del escenario dictado por el instructor. |

## Entorno de Laboratorio

### Hardware Mínimo

| Componente | Especificación |
|:---|:---|
| Procesador | Intel Core i5 (64 bits) o equivalente AMD |
| Memoria RAM | 8 GB mínimo |
| Pantalla | Resolución mínima 1920×1080 |
| Conectividad | Banda ancha ≥ 10 Mbps bajada/subida |

### Software Requerido

| Herramienta | Versión Exacta | Función en la Práctica |
|:---|:---|:---|
| Microsoft Edge | 128.0.2739.42 | Navegador principal para acceder a Copilot Chat |
| Microsoft 365 Copilot Chat (Business Chat, modo Work) | Service Release 2408 (Build 17928.20156) | Plataforma de interacción con el LLM mediante prompts COOE |
| Microsoft Teams (Trabajo o Escuela) | 24193.1805.2987.5853 | Canal alternativo de acceso a Copilot Chat |

> **Nota sobre licencias:** Microsoft 365 Copilot Chat (Business Chat en modo Work) es un componente de la licencia **Microsoft 365 Copilot Premium**. No debe confundirse con la versión gratuita de Copilot (anteriormente Bing Chat) ni con Copilot en aplicaciones individuales como Word o Excel. La funcionalidad de modo Work permite a Copilot acceder a datos del tenant corporativo a través de Microsoft Graph, lo cual es esencial para esta práctica.

### Configuración Inicial

Antes de iniciar, verifica que cumples con las siguientes condiciones:

1. Tienes abierta **una sola pestaña** de Microsoft 365 Copilot Chat en `https://m365.cloud.microsoft/chat` con el selector de modo en **Work** (icono de maletín).
2. Si utilizaste Copilot Chat en la Práctica 1, **mantén el mismo hilo de conversación abierto** para conservar la continuidad del contexto (Thread Continuity).
3. Tienes listo tu bloc de notas (físico o digital) para registrar los datos del escenario que el instructor proporcionará verbalmente.

## Instrucciones Paso a Paso

### Paso 1: Capturar los elementos del escenario proporcionado por el instructor

**Objetivo:** Registrar de forma estructurada los cuatro bloques de información del escenario ejecutivo que el instructor presentará verbalmente, organizándolos según las categorías que alimentarán cada componente del marco COOE.

**Instrucciones:**

1. Escucha atentamente al instructor mientras presenta el escenario ejecutivo. El escenario incluirá información sobre las siguientes cuatro dimensiones:

   - **Comportamiento del segmento:** Datos sobre cómo los microempresarios de Bancolombia interactúan actualmente con los canales de la entidad.
   - **Experiencia del cliente:** Puntos de dolor, fricciones y percepciones del microempresario al usar (o intentar usar) canales digitales.
   - **Restricciones operativas:** Limitaciones de presupuesto, infraestructura tecnológica, capacidad de atención en sucursales o regulaciones que condicionan la migración.
   - **Objetivos esperados:** Metas organizacionales que Bancolombia busca alcanzar con la migración digital del segmento.

2. En tu bloc de notas, crea cuatro secciones con los encabezados anteriores y registra **al menos 2 datos específicos por sección** mientras el instructor habla.

3. Marca con un asterisco (*) cualquier dato que te parezca ambiguo o incompleto — esto será útil al construir la sección de "supuestos" en tu prompt.

4. Si el instructor comparte cifras o porcentajes específicos, regístralos textualmente; serán los **hechos** de tu prompt.

> **Escenario de referencia proporcionado por el instructor:**
>
> A continuación se presenta el escenario completo que el instructor dictará. Durante la sesión presencial, los participantes deben capturarlo de oído. Para efectos de esta guía de laboratorio, se incluye como referencia:
>
> ---
>
> #### Escenario: Migración Digital del Segmento Microempresarios — Bancolombia
>
> **Comportamiento del segmento:**
> - El 68% de los microempresarios de Bancolombia realizan sus transacciones principales (pagos a proveedores, consultas de saldo, solicitudes de crédito) exclusivamente en sucursales físicas.
> - El 42% de estos clientes posee un smartphone con acceso a datos móviles, pero solo el 15% ha descargado la app Bancolombia.
> - La frecuencia promedio de visita a sucursal es de 3.2 veces por semana, con un tiempo promedio de espera de 38 minutos por visita.
>
> **Experiencia del cliente:**
> - En encuestas de satisfacción (NPS), el segmento de microempresarios reporta un puntaje de 23 (zona de mejora), siendo la principal queja el tiempo de espera en sucursales y la percepción de que "la app es complicada para lo que necesito".
> - El 31% de los microempresarios que intentaron usar la app la desinstalaron en los primeros 14 días, citando dificultad para encontrar funciones de pago a proveedores.
> - Los asesores comerciales en sucursal reportan que dedican aproximadamente el 40% de su tiempo a transacciones operativas que podrían realizarse digitalmente.
>
> **Restricciones operativas:**
> - El presupuesto aprobado para iniciativas de migración digital en el segmento microempresarios para el año fiscal actual es de COP $2,800 millones, lo cual cubre capacitación en campo, rediseño parcial de UX y campañas de comunicación.
> - La regulación de la Superintendencia Financiera exige que cualquier canal digital mantenga un esquema de autenticación fuerte (doble factor) para transacciones superiores a COP $500,000, lo cual añade fricción al proceso de adopción.
> - Bancolombia tiene 412 sucursales con presencia del segmento microempresarial, pero solo 38 cuentan con "embajadores digitales" dedicados a acompañar la migración.
>
> **Objetivos esperados:**
> - Reducir la dependencia de sucursales físicas del segmento en un 30% en 18 meses (medido por reducción de transacciones presenciales).
> - Incrementar la adopción activa de la app Bancolombia entre microempresarios del 15% actual al 45% en 12 meses.
> - Mantener o mejorar el NPS del segmento durante el proceso de migración (meta: pasar de 23 a al menos 35).
> - Liberar al menos el 25% del tiempo de los asesores comerciales en sucursal para actividades de venta consultiva y profundización de relaciones.
>
> ---

**Resultado esperado:** Un registro organizado en cuatro secciones con datos concretos del escenario, donde al menos algunos elementos están marcados como potencialmente ambiguos o incompletos.

**Verificación:** Confirma que tienes al menos 8 datos registrados (mínimo 2 por cada una de las 4 dimensiones) antes de avanzar al Paso 2. Si te falta información de alguna dimensión, levanta la mano para que el instructor la repita.

---

### Paso 2: Construir el prompt COOE en Microsoft 365 Copilot Chat

**Objetivo:** Redactar un prompt completo y estructurado bajo el marco COOE que instruya a Copilot a organizar la situación de negocio sin generar recomendaciones, produciendo una salida con tres secciones diferenciadas.

**Instrucciones:**

1. Dirígete a tu pestaña abierta de Microsoft 365 Copilot Chat en `https://m365.cloud.microsoft/chat`. Verifica que el selector de modo esté en **Work** (icono de maletín en la parte superior del campo de texto).

2. Si continuaste desde la Práctica 1 en el mismo hilo, escribe un separador contextual antes de tu nuevo prompt para que Copilot entienda que se trata de una nueva solicitud dentro del mismo hilo:

   ```text
   --- Nueva solicitud (Práctica 2) ---
   ```

3. Construye tu prompt siguiendo **obligatoriamente** las cuatro secciones del marco COOE. Utiliza la siguiente estructura como guía, pero **personaliza el contenido** con los datos específicos que capturaste en el Paso 1:

   ```text
   **CONTEXTO:**
   Soy un líder ejecutivo de Bancolombia responsable de evaluar la viabilidad de migrar al segmento de microempresarios desde sucursales físicas hacia canales digitales. Actualmente, el 68% de los microempresarios realizan sus transacciones principales exclusivamente en sucursales físicas. Solo el 15% ha descargado la app Bancolombia, aunque el 42% posee smartphone con datos móviles. La frecuencia de visita a sucursal es de 3.2 veces por semana con un tiempo de espera promedio de 38 minutos. El NPS del segmento es 23 (zona de mejora). El 31% de quienes descargaron la app la desinstalaron en los primeros 14 días. Los asesores en sucursal dedican el 40% de su tiempo a transacciones operativas digitalizables. El presupuesto aprobado es de COP $2,800 millones para el año fiscal. La Superintendencia Financiera exige autenticación de doble factor para transacciones superiores a COP $500,000. De 412 sucursales con presencia del segmento, solo 38 cuentan con embajadores digitales. Los objetivos son: reducir dependencia de sucursales en 30% en 18 meses, llevar la adopción de la app del 15% al 45% en 12 meses, mejorar NPS de 23 a 35, y liberar el 25% del tiempo de asesores para venta consultiva.

   **OBJETIVO:**
   Necesito que organices toda la información anterior de forma estructurada, SIN generar recomendaciones ni propuestas de acción todavía. Quiero entender con claridad qué elementos de esta situación son hechos confirmados, cuáles son supuestos que estamos dando por ciertos sin evidencia suficiente, y qué información adicional necesitaríamos obtener antes de tomar cualquier decisión estratégica.

   **ORIGEN:**
   La información que te estoy proporcionando proviene de un briefing ejecutivo interno presentado por el equipo de estrategia digital y el área comercial de Bancolombia. Incluye datos de encuestas de satisfacción (NPS), métricas operativas de sucursales, estadísticas de uso de la app y restricciones presupuestarias y regulatorias comunicadas por las áreas de planeación financiera y cumplimiento normativo.

   **EXPECTATIVAS:**
   Presenta tu respuesta organizada en exactamente tres secciones claramente diferenciadas:
   1. **Lo que sabemos con certeza** — Hechos respaldados por datos cuantitativos o fuentes verificables mencionadas en el contexto.
   2. **Lo que estamos asumiendo** — Supuestos implícitos o explícitos que se están tomando como ciertos pero que no cuentan con evidencia directa en la información proporcionada.
   3. **Lo que necesitamos validar** — Preguntas críticas o datos faltantes que deberían investigarse antes de proceder con cualquier decisión estratégica.

   Usa viñetas dentro de cada sección. No incluyas recomendaciones, planes de acción ni sugerencias de siguiente paso. Tu rol es exclusivamente organizar y clasificar la información.
   ```

4. **Antes de enviar**, revisa tu prompt verificando los siguientes criterios:

   | Criterio | Verificación |
   |:---|:---|
   | ¿El Contexto incluye datos específicos (cifras, porcentajes, plazos)? | ✅ / ❌ |
   | ¿El Objetivo indica explícitamente que NO se deben generar recomendaciones? | ✅ / ❌ |
   | ¿El Origen identifica de dónde proviene la información? | ✅ / ❌ |
   | ¿Las Expectativas definen el formato exacto de salida (3 secciones con nombres)? | ✅ / ❌ |
   | ¿Se usa lenguaje directivo sin ambigüedades ("presenta", "no incluyas", "tu rol es")? | ✅ / ❌ |

5. Una vez verificados todos los criterios, presiona **Enter** o haz clic en el botón de enviar para ejecutar el prompt en Copilot Chat.

**Resultado esperado:** El prompt queda enviado a Microsoft 365 Copilot Chat y Copilot comienza a generar una respuesta estructurada.

**Verificación:** Confirma que tu prompt contiene las cuatro secciones COOE etiquetadas explícitamente y que la instrucción de no generar recomendaciones está presente antes de enviarlo.

---

### Paso 3: Analizar y evaluar la respuesta de Copilot

**Objetivo:** Interpretar críticamente la respuesta generada por Copilot, verificando que cumple con la estructura solicitada y que la clasificación de información (hechos, supuestos, pendientes) es precisa y útil para un contexto de toma de decisiones ejecutivas.

**Instrucciones:**

1. Lee la respuesta completa de Copilot. Identifica si la salida contiene **exactamente tres secciones** con los nombres solicitados:
   - "Lo que sabemos con certeza" (o equivalente semántico)
   - "Lo que estamos asumiendo" (o equivalente semántico)
   - "Lo que necesitamos validar" (o equivalente semántico)

2. Aplica la siguiente **rúbrica de evaluación** a la respuesta de Copilot. Marca cada criterio como cumplido (✅) o no cumplido (❌):

   | # | Criterio de Evaluación | ✅/❌ | Observaciones |
   |:---|:---|:---|:---|
   | 1 | La respuesta contiene exactamente 3 secciones diferenciadas | | |
   | 2 | La sección de "hechos" incluye solo datos con respaldo cuantitativo proporcionado en el prompt (ej.: 68%, NPS 23, COP $2,800M) | | |
   | 3 | La sección de "supuestos" identifica al menos 2 inferencias no respaldadas directamente por los datos (ej.: que los microempresarios *quieren* migrar, que el presupuesto es *suficiente*) | | |
   | 4 | La sección de "pendientes de validación" plantea al menos 3 preguntas o brechas de información relevantes y no triviales | | |
   | 5 | La respuesta NO contiene recomendaciones, planes de acción ni sugerencias de siguiente paso | | |
   | 6 | El lenguaje es apropiado para un contexto ejecutivo (conciso, profesional, sin jerga técnica innecesaria) | | |
   | 7 | La respuesta no inventa datos ni cifras que no fueron proporcionados en el prompt | | |

3. Si el criterio **#5** no se cumple (Copilot generó recomendaciones a pesar de la instrucción explícita), registra este hallazgo como una **limitación del modelo** y no como un error de tu prompt. Este es un comportamiento conocido de los LLM: tienden a generar sugerencias de acción por defecto, incluso cuando se les instruye lo contrario.

4. Si el criterio **#7** no se cumple (Copilot inventó datos o cifras — fenómeno conocido como *alucinación*), marca específicamente qué dato fue fabricado. Este hallazgo es especialmente relevante en contextos ejecutivos donde una cifra falsa podría influir en una decisión de negocio.

5. Registra en tu bloc de notas un resumen de tu evaluación con el conteo de criterios cumplidos (ej.: "5 de 7 criterios cumplidos").

**Resultado esperado:** Una evaluación documentada de la respuesta de Copilot con al menos 5 de 7 criterios cumplidos. La respuesta de Copilot debería verse estructuralmente similar a este ejemplo de referencia (el contenido variará según cada interacción):

> **Lo que sabemos con certeza:**
> - El 68% de los microempresarios realizan transacciones exclusivamente en sucursales físicas.
> - Solo el 15% ha descargado la app, aunque el 42% tiene smartphone con datos.
> - El NPS del segmento es 23 (zona de mejora).
> - El 31% de los usuarios que descargaron la app la desinstalaron en 14 días.
> - El presupuesto aprobado es COP $2,800 millones.
> - Solo 38 de 412 sucursales tienen embajadores digitales.
> - La regulación exige doble factor para transacciones > COP $500,000.
> - Los asesores dedican el 40% de su tiempo a transacciones operativas.
>
> **Lo que estamos asumiendo:**
> - Que los microempresarios que poseen smartphone (42%) tienen la disposición y las competencias digitales para usar la app bancaria.
> - Que la desinstalación de la app se debe principalmente a problemas de usabilidad (UX) y no a otros factores como desconfianza o preferencia consciente por el canal presencial.
> - Que el presupuesto de COP $2,800M es suficiente para cubrir simultáneamente capacitación, rediseño UX y campañas.
> - Que la meta de pasar de 15% a 45% de adopción en 12 meses es alcanzable con los recursos disponibles.
> - Que liberar tiempo de asesores se traducirá efectivamente en venta consultiva y no en reducción de plantilla.
>
> **Lo que necesitamos validar:**
> - ¿Cuál es el perfil demográfico y nivel de alfabetización digital de los microempresarios del segmento?
> - ¿Existen datos sobre por qué el 58% que tiene smartphone no ha descargado la app?
> - ¿Cuál es el costo por microempresario de la capacitación en campo vs. el ahorro esperado por transacción migrada?
> - ¿Qué resultados han tenido las 38 sucursales con embajadores digitales vs. las 374 sin ellos?
> - ¿Existe un benchmark interno o externo de tasas de adopción digital en segmentos similares en la banca colombiana?
> - ¿Cómo se medirá el impacto de la autenticación de doble factor en la tasa de abandono del flujo digital?

**Verificación:** Has completado la rúbrica de 7 criterios y tienes documentados los hallazgos clave, incluyendo cualquier caso de recomendación no solicitada o alucinación detectada.

---

### Paso 4: Identificar oportunidades de refinamiento y compartir con el grupo

**Objetivo:** Reflexionar sobre la calidad del prompt construido, identificar al menos una mejora concreta y preparar una síntesis para la discusión grupal.

**Instrucciones:**

1. Basándote en tu evaluación del Paso 3, identifica **al menos una oportunidad de refinamiento** de tu prompt original. Considera las siguientes preguntas guía:

   | Pregunta de Reflexión | Tu Respuesta |
   |:---|:---|
   | ¿La sección de Contexto incluyó todos los datos relevantes o omitiste alguno? | |
   | ¿La instrucción de "no generar recomendaciones" fue suficientemente enfática? ¿Copilot la respetó? | |
   | ¿Podrías haber sido más específico en las Expectativas sobre el nivel de detalle deseado? | |
   | ¿El Origen fue lo suficientemente preciso para que Copilot calibrara la confiabilidad de los datos? | |
   | ¿Habrías obtenido mejor resultado separando la instrucción en dos prompts secuenciales? | |

2. Redacta en tu bloc de notas una frase que resuma tu principal aprendizaje sobre la construcción de prompts COOE. Ejemplo: *"Descubrí que cuando no especifico el número mínimo de elementos por sección, Copilot tiende a ser superficial en los supuestos."*

3. **(Opcional — si el tiempo lo permite):** Si identificaste que Copilot generó recomendaciones a pesar de tu instrucción, envía un **prompt de corrección** en el mismo hilo:

   ```text
   En tu respuesta anterior incluiste recomendaciones o sugerencias de acción. Por favor, revisa tu respuesta y elimina cualquier elemento que sea una recomendación, plan de acción o sugerencia. Mantén únicamente la clasificación en las tres secciones solicitadas: lo que sabemos, lo que asumimos y lo que necesitamos validar.
   ```

4. Prepárate para compartir con el grupo los siguientes elementos cuando el instructor lo solicite:
   - Tu prompt completo (puedes leerlo o compartir pantalla).
   - El resultado de tu rúbrica de evaluación (cuántos criterios de 7 se cumplieron).
   - Tu principal hallazgo o aprendizaje sobre prompting COOE.

**Resultado esperado:** Al menos una oportunidad de mejora documentada y una síntesis lista para compartir en la discusión grupal.

**Verificación:** Puedes articular en una frase qué cambiarías en tu prompt para obtener un resultado más preciso en una segunda iteración.

## Validación y Pruebas

Para considerar esta práctica como completada exitosamente, verifica los siguientes criterios medibles:

### Criterios de Éxito Obligatorios

| # | Criterio | Evidencia Requerida | Cumplido |
|:---|:---|:---|:---|
| 1 | El prompt enviado contiene las 4 secciones COOE etiquetadas explícitamente | Texto del prompt visible en el hilo de Copilot Chat | ✅/❌ |
| 2 | La respuesta de Copilot contiene 3 secciones diferenciadas (hechos, supuestos, pendientes) | Respuesta visible en pantalla con las 3 secciones | ✅/❌ |
| 3 | La sección de "hechos" no contiene información inventada por el modelo | Verificación cruzada con los datos del escenario del instructor | ✅/❌ |
| 4 | La sección de "supuestos" identifica al menos 2 inferencias no respaldadas | Conteo de supuestos en la respuesta | ✅/❌ |
| 5 | La sección de "pendientes" plantea al menos 3 preguntas de validación no triviales | Conteo y evaluación de relevancia | ✅/❌ |
| 6 | La rúbrica de 7 criterios del Paso 3 está completada | Registro en bloc de notas | ✅/❌ |

### Prueba Adversaria (Limitaciones de IA)

Realiza la siguiente verificación adicional para evaluar la robustez de la respuesta de Copilot frente a información ausente o contradictoria:

**Prueba de alucinación por omisión:** Revisa si la respuesta de Copilot en la sección "Lo que sabemos con certeza" incluye algún dato cuantitativo que **no** fue proporcionado en tu prompt original. Por ejemplo:
- ¿Copilot mencionó una tasa de adopción digital del sector bancario colombiano que tú no proporcionaste?
- ¿Copilot atribuyó una cifra de ahorro por transacción digital que no estaba en el escenario?
- ¿Copilot citó alguna fuente documental interna (correo, archivo de SharePoint) que no existe o no fue mencionada?

Si detectas cualquiera de estos casos, documéntalo como un **hallazgo de alucinación** con el siguiente formato:

| Dato fabricado por Copilot | ¿Estaba en el prompt original? | Impacto potencial en decisión ejecutiva |
|:---|:---|:---|
| [Dato específico] | No | [Alto/Medio/Bajo] |

> **Reflexión crítica:** En un entorno ejecutivo real, un dato fabricado por el modelo que se presente como "hecho confirmado" podría influir en una decisión de inversión de miles de millones de pesos. La supervisión humana de las respuestas de Copilot no es opcional: es una responsabilidad del líder que utiliza la herramienta.

## Solución de Problemas

### Problema 1: Copilot genera recomendaciones a pesar de la instrucción explícita de no hacerlo

**Síntomas:** La respuesta de Copilot incluye una cuarta sección con títulos como "Recomendaciones", "Próximos pasos sugeridos", "Acciones propuestas" o frases como "Se recomienda que…", "Una posible estrategia sería…" al final de la respuesta o integradas dentro de las tres secciones solicitadas.

**Causa:** Los modelos de lenguaje grande (LLM) están entrenados con un sesgo hacia la generación de contenido útil y orientado a la acción. Incluso con instrucciones explícitas de restricción, el modelo puede "completar" la respuesta con sugerencias porque su distribución de probabilidad favorece patrones de respuesta que incluyen recomendaciones en contextos de análisis de negocio. Esto no es un error del prompt del usuario sino una limitación inherente del comportamiento del modelo.

**Solución:**

1. Envía un prompt de corrección en el mismo hilo de conversación:
   ```text
   Tu respuesta anterior incluye recomendaciones que no solicité. Necesito que regeneres únicamente las tres secciones pedidas (Lo que sabemos, Lo que asumimos, Lo que necesitamos validar) eliminando cualquier sugerencia de acción, recomendación o propuesta. Limítate estrictamente a clasificar la información.
   ```
2. Si el problema persiste, refuerza la restricción añadiendo al final de tu prompt original la frase: `RESTRICCIÓN ABSOLUTA: Bajo ninguna circunstancia incluyas recomendaciones, sugerencias, planes de acción o próximos pasos. Si sientes la necesidad de sugerir algo, conviértelo en una pregunta de validación y colócalo en la sección 3.`
3. Documenta el hallazgo en tu rúbrica como una limitación conocida del modelo, no como un fallo de tu prompt.

---

### Problema 2: Copilot responde con un formato genérico sin respetar las tres secciones solicitadas

**Síntomas:** La respuesta de Copilot se presenta como un texto corrido, una lista plana sin secciones diferenciadas, o utiliza encabezados diferentes a los solicitados (por ejemplo, "Análisis", "Resumen", "Conclusiones" en lugar de "Lo que sabemos", "Lo que asumimos", "Lo que necesitamos validar").

**Causa:** Cuando el prompt es muy extenso (como ocurre con prompts COOE completos con datos detallados), el modelo puede perder la instrucción de formato si esta se encuentra al final del prompt y la ventana de atención prioriza el contenido inicial. También puede ocurrir si el modo de Copilot Chat no está configurado en **Work** o si la sesión tiene un contexto previo que interfiere con las instrucciones actuales.

**Solución:**

1. Verifica que el selector de modo de Copilot Chat esté en **Work** (icono de maletín), no en "Web" ni en otro modo.
2. Envía un prompt de reformateo en el mismo hilo:
   ```text
   Reorganiza tu respuesta anterior utilizando exactamente estos tres encabezados en negrita, cada uno seguido de viñetas:

   **1. Lo que sabemos con certeza**
   **2. Lo que estamos asumiendo**
   **3. Lo que necesitamos validar**

   No agregues ninguna sección adicional.
   ```
3. Si el problema persiste, considera iniciar un **nuevo hilo de conversación** y colocar las instrucciones de formato **al inicio** del prompt (antes de la sección de Contexto), ya que los LLM tienden a dar mayor peso a las instrucciones que aparecen primero.

## Limpieza

Esta práctica **no requiere eliminación de recursos** ya que no se crearon archivos, agentes ni configuraciones permanentes. Sin embargo, sigue estas indicaciones para mantener la continuidad del curso:

1. **NO cierres el hilo de conversación** de Microsoft 365 Copilot Chat. Las prácticas posteriores (3 a 10) se ejecutarán en el mismo hilo para mantener la continuidad contextual (Thread Continuity).
2. **Conserva tus notas** del Paso 1 (datos del escenario) y del Paso 3 (rúbrica de evaluación). Serán referencia para las prácticas subsiguientes donde se construirán prompts más complejos sobre el mismo escenario.
3. Si tomaste capturas de pantalla de tu prompt o de la respuesta de Copilot, guárdalas en una carpeta local con el nombre `Lab_01-00-02_Practica2` para referencia futura.

## Resumen

En esta práctica aplicaste el marco de prompting **COOE (Contexto + Objetivo + Origen + Expectativas)** para construir una instrucción estructurada que solicita a Microsoft 365 Copilot organizar una situación de negocio compleja sin generar recomendaciones prematuras. Los aprendizajes clave incluyen:

- **La estructura COOE es un habilitador de precisión:** Al etiquetar explícitamente cada sección del prompt, se reduce la ambigüedad y se incrementa la probabilidad de obtener una respuesta con el formato y contenido deseados.
- **La restricción de "no recomendar" requiere refuerzo explícito:** Los LLM tienen un sesgo inherente hacia la generación de sugerencias; la supervisión humana y la iteración son necesarias para mantener el control sobre el tipo de respuesta.
- **Separar hechos de supuestos es un acto de rigor analítico:** En contextos ejecutivos, la diferencia entre un dato confirmado y una suposición puede significar la diferencia entre una decisión acertada y un error de millones de pesos.
- **La verificación de alucinaciones es responsabilidad del líder:** Copilot puede presentar información fabricada como si fuera un hecho; el ejecutivo debe siempre validar las cifras contra las fuentes originales.

### Conexión con la Siguiente Práctica

En la **Práctica 3**, utilizarás el mismo hilo de conversación para avanzar al siguiente nivel: solicitar a Copilot que, a partir de la organización de información lograda en esta práctica, genere alternativas de decisión estratégica con análisis de riesgos y dependencias. La clasificación tripartita (hechos/supuestos/pendientes) que obtuviste aquí será el insumo directo para esa solicitud.

### Recursos Adicionales

| Recurso | Enlace |
|:---|:---|
| Microsoft Learn: Introducción a Microsoft 365 Copilot | https://learn.microsoft.com/es-es/microsoft-365-copilot/overview |
| Microsoft Learn: Datos, privacidad y seguridad para Microsoft 365 Copilot | https://learn.microsoft.com/es-es/microsoft-365-copilot/copilot-privacy |
| Microsoft Learn: Escribir prompts eficaces para Microsoft 365 Copilot | https://learn.microsoft.com/es-es/microsoft-365-copilot/microsoft-365-copilot-usage-activity |
| Microsoft WorkLab: Guía de IA para líderes y ejecutivos | https://www.microsoft.com/en-us/worklab |
