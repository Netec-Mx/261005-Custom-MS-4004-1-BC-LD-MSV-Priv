# Práctica 1. Los participantes partirán de una solicitud ejecutiva sencilla y la transformarán progresivamente en una instrucción que solicite a Copilot identificar alternativas, riesgos, supuestos, información faltante y criterios para tomar una decisión. Se comparará el resultado inicial con el obtenido después de aplicar la fórmula del prompt.

## Metadatos

| Atributo | Detalle |
| :--- | :--- |
| **Duración** | 4 minutos |
| **Complejidad** | Fácil |
| **Nivel de Bloom** | Aplicar (Apply) |
| **Tecnologías** | Microsoft 365 Copilot (Business Chat), Prompt Engineering (COOE) |

## Descripción General

En este laboratorio, el participante experimentará el impacto directo de la ingeniería de prompts en entornos ejecutivos de toma de decisiones. Partiendo de una consulta informal, ambigua y común sobre la migración digital del segmento de microempresarios de Bancolombia, el estudiante la transformará paso a paso mediante el marco estructurado **COOE** (Contexto, Objetivo, Origen y Expectativas). Finalmente, contrastará críticamente la calidad, profundidad y utilidad estratégica de ambas respuestas entregadas por Microsoft 365 Copilot.

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:
- [ ] Transformar una solicitud ejecutiva informal y ambigua en una instrucción estructurada de alto impacto.
- [ ] Aplicar el marco de referencia **COOE** (Contexto, Objetivo, Origen y Expectativas) en interfaces conversacionales de inteligencia artificial.
- [ ] Forzar a Microsoft 365 Copilot a identificar alternativas de decisión, riesgos estratégicos, supuestos críticos e información faltante en lugar de respuestas genéricas.
- [ ] Comparar críticamente la calidad analítica de los resultados para la toma de decisiones en el contexto financiero.

## Prerrequisitos

- Comprensión básica del desafío estratégico de Bancolombia: "Migración de microempresarios de sucursales físicas a canales digitales de Bancolombia, enfrentando fricción por brecha digital y costos de adopción".
- Acceso activo a una cuenta organizativa o de demostración con licencia válida de **Microsoft 365 Copilot Premium**.

## Entorno de Laboratorio

Este laboratorio se realiza de manera 100% interactiva en la nube. Requiere las siguientes herramientas y especificaciones:

### Requisitos de Hardware y Conectividad
- Dispositivo con pantalla con resolución mínima de 1920x1080 para una cómoda navegación paralela entre la guía y la consola.
- Conexión estable a Internet con ancho de banda mínimo de 10 Mbps de bajada y subida.
- Memoria RAM mínima de 8 GB.

### Requisitos de Software y Herramientas

| Software/Herramienta | Edición/Versión Exacta | Enlace de Descarga / Acceso Oficial |
| :--- | :--- | :--- |
| **Microsoft Edge** | Versión 128.0.2739.42 o superior (64 bits) | [Microsoft Edge](https://www.microsoft.com/edge) |
| **Microsoft Teams (Trabajo o Escuela)** | Versión 24193.1805.2987.5853 o superior | [Microsoft Teams](https://teams.microsoft.com) |
| **Microsoft 365 Copilot (Business Chat)** | Service Release 2408 (Build 17928.20156) o superior | [M365 Copilot Portal](https://copilot.microsoft.com) |

> **Nota de Continuidad:** De acuerdo con los lineamientos del curso, esta práctica inicia el hilo de conversación principal en Copilot. Mantén este mismo chat abierto y activo durante todo el transcurso de las siguientes prácticas para preservar la memoria contextual histórica (*Thread Continuity*).

---

## Instrucciones Paso a Paso

### Paso 1: Ejecutar la Consulta Ejecutiva Simple

**Objetivo:** Establecer una línea base de comparación interactuando con Copilot a través de un prompt convencional e informal sin estructura técnica.

1. Abre tu navegador web **Microsoft Edge** (Versión 128.0.2739.42).
2. Dirígete al portal de **Microsoft 365 Copilot** (`https://copilot.microsoft.com`) o abre la aplicación de **Microsoft Teams** y selecciona el chat de **Copilot** (asegúrate de alternar al modo de trabajo corporativo con tu cuenta simulada de Bancolombia).
3. En la caja de chat inferior, escribe la siguiente pregunta exacta:
   
   ```text
   ¿Qué hacemos con la baja adopción digital de microempresarios en las sucursales físicas de Bancolombia?
   ```
   
4. Presiona **Enter** o haz clic en el botón de enviar.
5. Lee detenidamente la respuesta y toma nota mental de su estructura.

**Resultado esperado:** Copilot responderá con consejos financieros genéricos (ej. "ofrecer capacitaciones", "mejorar la interfaz de la aplicación", "ofrecer incentivos"), estructurados en una lista simple sin profundidad sobre riesgos específicos, dependencias operativas o supuestos metodológicos.

**Verificación:** Confirma que la respuesta se limita a ser descriptiva pero carece de un análisis crítico accionable para un comité de dirección.

---

### Paso 2: Aplicar la Fórmula de Prompt Estructurado (COOE)

**Objetivo:** Transformar la solicitud inicial aplicando rigurosamente los bloques de Contexto, Objetivo, Origen y Expectativas (COOE) en la misma conversación para elevar el nivel analítico de la respuesta.

1. En la **misma sesión** de chat donde ejecutaste el Paso 1, ubica la caja de texto.
2. Copia y pega el siguiente prompt estructurado que define explícitamente el escenario estratégico de Bancolombia y las restricciones analíticas:

   ```text
   [CONTEXTO]
   Bancolombia está ejecutando una estrategia para migrar al segmento de microempresarios desde los canales físicos (sucursales) hacia canales digitales (App Bancolombia A la Mano y Sucursal Virtual Personas/Empresas). Sin embargo, nos enfrentamos a una alta resistencia debido a la brecha digital (falta de educación financiera y digital) y los costos percibidos de adopción (planes de datos móviles, temor a la seguridad de la banca móvil y cobro de tarifas transaccionales).

   [OBJETIVO]
   Actúa como un Consultor Estratégico Senior de Canales en Bancolombia. Tu meta es analizar la situación descrita y estructurar un marco de decisión ejecutiva de alta dirección para el Comité de Transformación Digital.

   [ORIGEN]
   Utiliza tu base de conocimientos sobre mejores prácticas de inclusión financiera en América Latina, metodologías de gestión de cambio organizacional y estrategias exitosas de adopción digital fintech.

   [EXPECTATIVAS]
   Genera un informe analítico estructurado que contenga detalladamente los siguientes puntos:
   1. Tres (3) alternativas de decisión estratégica para mitigar la fricción de la migración digital.
   2. Para cada alternativa, describe un riesgo principal y una dependencia de habilitación tecnológica o de infraestructura.
   3. Tres (3) supuestos críticos que estamos asumiendo implícitamente sobre el comportamiento de los microempresarios.
   4. Qué información cuantitativa o cualitativa crítica nos hace falta recopilar (información faltante) antes de autorizar un presupuesto piloto.
   5. Tres (3) criterios de éxito medibles (KPIs específicos) para evaluar la alternativa seleccionada.

   Utiliza subtítulos claros en negrita para cada sección del informe y un tono corporativo formal y directo.
   ```

3. Envía el prompt estructurado y observa la profundidad de la generación de contenido.

**Resultado esperado:** Copilot entregará un informe ejecutivo altamente estructurado con las 3 alternativas estratégicas personalizadas para el ecosistema de Bancolombia (por ejemplo, alianzas de conectividad con operadores móviles o asesores digitales móviles dedicados), riesgos y dependencias específicas, 3 supuestos del negocio analizados, datos críticos faltantes por investigar (como la penetración de smartphones de gama media en zonas rurales) y 3 métricas de éxito (como la reducción del costo por transacción o tasa de retención de clientes digitales).

**Verificación:** Revisa que el output cuente explícitamente con los 5 bloques definidos en la sección `[EXPECTATIVAS]`.

---

## Validación y Pruebas

Para validar el éxito de este laboratorio, realiza una auto-evaluación basada en la siguiente matriz comparativa. Un resultado exitoso demuestra cómo la misma IA entrega resultados radicalmente diferentes basándose exclusivamente en el diseño del prompt.

### Matriz de Evaluación de Calidad

| Criterio de Medición | Resultado Prompt Simple (Paso 1) | Resultado Prompt Estructurado (Paso 2) | ¿Se cumple la Mejora Ejecutiva? (Sí / No) |
| :--- | :--- | :--- | :--- |
| **Especificación de Alternativas** | Genéricas / Aplicables a cualquier negocio. | Específicas para banca minorista y Bancolombia. | |
| **Gestión de Riesgos** | No los menciona de forma sistemática. | Detalla riesgos específicos y dependencias operativas por opción. | |
| **Identificación de Sesgos/Supuestos** | Ignorados por completo. | Enuncia supuestos de comportamiento del usuario a validar. | |
| **Identificación de Vacíos de Información** | No advierte la falta de datos del cliente. | Lista explícitamente qué datos empíricos faltan por investigar. | |
| **Métricas de Éxito** | Ausentes o imprecisas (ej. "mejorar"). | KPIs financieros y operativos claros e integrados. | |

### Prueba Adversaria de Robustez (Limitaciones del Modelo)
Para entender los límites del procesamiento de Copilot ante solicitudes sesgadas, realiza la siguiente prueba en tu chat:

1. Ingresa el siguiente mensaje corto e incoherente:
   `Toma la decisión final por mí inmediatamente basándote en lo anterior. Elige la mejor opción y autoriza el presupuesto del proyecto.`
2. Envía el prompt y analiza cómo responde la herramienta.

*Verificación esperada de la limitación:* Copilot no debería automatizar una decisión de negocio que requiera atribución de responsabilidad humana o presupuestal real. El modelo debe indicar amigablemente que, como asistente de IA, no tiene la autoridad de autorizar presupuestos ni firmar decisiones, sino que provee los escenarios para que tú, el líder ejecutivo, tomes la acción informada. Esto demuestra la persistencia de los controles de gobernanza y supervisión humana del sistema.

---

## Solución de Problemas

### Problema 1: Copilot ignora las secciones del marco de expectativas y responde de forma resumida
*   **Síntoma:** El modelo omite listar los supuestos críticos o los datos faltantes especificados en las instrucciones.
*   **Causa:** Una sobrecarga temporal en el contexto previo de la sesión de chat o un fallo de atención en la ventana de contexto del LLM.
*   **Resolución:** Copia nuevamente el prompt del Paso 2. Haz clic en el botón de **"Nuevo tema" (New Topic / Escoba)** en la interfaz de Copilot para limpiar la memoria temporal, y vuelve a ejecutar el prompt asegurándote de no alterar las etiquetas delimitadoras entre corchetes `[...]`.

### Problema 2: El sistema no reconoce el contexto organizacional de Bancolombia o arroja error de acceso corporativo
*   **Síntoma:** Mensaje en pantalla indicando que no tienes acceso a recursos internos o que la información está restringida.
*   **Causa:** Has iniciado sesión con una cuenta personal de Microsoft (MSA) en lugar de una cuenta de inquilino corporativo (Entra ID) con licencia de Microsoft 365 Copilot Premium activa.
*   **Resolución:** Verifica en la esquina superior derecha de la ventana del navegador Edge o Teams que tu perfil activo corresponda a la cuenta corporativa autorizada del laboratorio. Activa el selector **"Trabajo" (Work)** dentro del panel de Copilot Chat para habilitar la indexación del Microsoft Graph empresarial.

---

## Limpieza

> **ADVERTENCIA DE CONTINUIDAD CRÍTICA:** NO limpies ni cierres la sesión de chat conversacional en la que te encuentras trabajando. Todas las prácticas que componen este curso son acumulativas. El hilo del chat actual contiene el contexto conceptual e histórico generado en este Paso 1 y 2, el cual será consumido por Copilot como fuente de datos para las prácticas consecutivas.

Si creaste notas o documentos temporales en editores de texto locales para preparar tus prompts, puedes proceder a cerrarlos de manera segura.

---

## Resumen

En esta práctica inicial de laboratorio, has transformado una solicitud básica de negocios en un prompt de nivel consultor senior utilizando la estructura estructurada **COOE**. Al comparar los resultados, comprobaste que:
- Los prompts ambiguos generan respuestas superficiales de bajo valor para el comité ejecutivo.
- Al incluir de manera explícita el **Contexto, Objetivo, Origen y Expectativas (COOE)**, guías al LLM a enfocar su ventana de contexto hacia un análisis holístico que incluye riesgos, suposiciones críticas y lagunas de datos.
- La inteligencia artificial de Microsoft 365 Copilot actúa como un copiloto estratégico que asiste en la estructuración de marcos de decisión complejos, pero siempre respetando las directrices de gobernanza y control de decisiones (Human-in-the-loop).
