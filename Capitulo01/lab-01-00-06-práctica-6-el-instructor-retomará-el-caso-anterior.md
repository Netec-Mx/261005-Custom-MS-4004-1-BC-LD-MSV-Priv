# Lab 01-00-06: Práctica 6. Clasificación Estratégica de Tareas de Decisión: Copilot General vs. Agente Especializado (Investigador)

## Metadatos

| Dimensión | Detalle |
| :--- | :--- |
| **Duración** | 3 minutos |
| **Complejidad** | Fácil |
| **Nivel de Taxonomía de Bloom** | Aplicar |

---

## Descripción General

En esta práctica, el participante evolucionará el escenario estratégico de negocio ("Migración del segmento de microempresarios de sucursales físicas a canales digitales de Bancolombia"). A partir de tres nuevas necesidades críticas planteadas por la dirección, se analizará y clasificará qué actividades deben ser resueltas mediante el chat general de Copilot (M365 Business Chat) y cuáles deben ser derivadas a un agente especializado como el Agente Investigador (Researcher). El objetivo es optimizar el flujo de trabajo del líder ejecutivo reduciendo la fatiga de interacción mediante una correcta delegación de tareas.

---

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:
*   Analizar el caso estratégico de migración digital e identificar las nuevas necesidades de investigación de factores externos y contraste de supuestos.
*   Clasificar y mapear qué actividades de toma de decisiones deben realizarse con el chat general de Copilot y cuáles mediante agentes especializados (Investigador).

---

## Prerrequisitos

*   Comprender el escenario de decisión de negocio: migración del segmento de microempresarios de sucursales físicas a canales digitales de Bancolombia, enfrentando fricción por brecha digital y costos de adopción.
*   Disponer de un navegador web con acceso activo al portal de Microsoft 365 Copilot con la licencia corporativa correspondiente.

---

## Entorno de Laboratorio

### Requisitos de Hardware y Conectividad
*   Dispositivo de cómputo personal con pantalla de resolución mínima de 1920x1080.
*   Conexión a internet estable de banda ancha (mínimo 10 Mbps de bajada/subida).

### Requisitos de Software y Licenciamiento

| Software / Servicio | Versión Evaluada | Origen / URL Oficial |
| :--- | :--- | :--- |
| **Microsoft Edge** | Versión 128.0.2739.42 (64-bit) | [https://www.microsoft.com/edge](https://www.microsoft.com/edge) |
| **Microsoft 365 Copilot** | Service Release 2408 (Build 17928.20156) | [https://copilot.microsoft.com](https://copilot.microsoft.com) |
| **Licencia de Copilot** | Microsoft 365 Copilot Premium (Enterprise) | Licencia corporativa habilitada en el tenant de Bancolombia |

### Configuración del Entorno

1. Inicie su navegador **Microsoft Edge**.
2. Diríjase a [https://copilot.microsoft.com](https://copilot.microsoft.com) e inicie sesión con su cuenta corporativa.
3. Asegúrese de que se encuentra en la pestaña de **Chat de Trabajo** (Business Chat) para garantizar el acceso al contexto corporativo y a los agentes de Microsoft 365.

---

## Instrucciones Paso a Paso

### Paso 1: Análisis de las Nuevas Necesidades Ejecutivas

**Objetivo**: Analizar las tres nuevas necesidades estratégicas presentadas para el caso de Bancolombia y estructurar el marco conceptual de clasificación.

**Instrucciones**:

1. Lea atentamente las tres nuevas necesidades planteadas para el líder ejecutivo de Bancolombia:
   *   **Necesidad A**: Investigar las tendencias externas de adopción fintech de microempresarios en América Latina durante el último año.
   *   **Necesidad B**: Contrastar los supuestos internos de costos de adopción frente a los datos reales de mercado de la competencia local.
   *   **Necesidad C**: Preparar un borrador de argumentario persuasivo para mitigar las objeciones del Comité de Dirección sobre el riesgo de exclusión financiera.
2. Identifique las características de cada tarea: si requiere búsquedas profundas en la web pública de fuentes confiables de terceros (Agente Investigador) o si requiere síntesis contextualizada de información corporativa interna preexistente, redacción y razonamiento lingüístico (Copilot Chat).

**Resultado esperado**: Comprensión clara de la diferencia técnica de entrada y salida entre el buscador especializado (Web-grounded / Agent) y el chat contextual interno.

**Verificación**: Proceda al Paso 2 una vez que distinga entre fuentes públicas externas y síntesis/redacción con base en las directrices del negocio.

---

### Paso 2: Creación de la Matriz de Decisión y Clasificación con Copilot

**Objetivo**: Ejecutar un prompt estructurado en Microsoft 365 Copilot para obtener la matriz de clasificación recomendada, argumentando técnicamente la asignación de cada tarea.

**Instrucciones**:

1. En la caja de chat de **Microsoft 365 Copilot** (asegúrese de utilizar el mismo hilo de conversación anterior para mantener la continuidad contextual si lo tiene abierto), copie y pegue el siguiente prompt ejecutivo de clasificación:

```text
Actúa como un Asesor Estratégico de Operaciones de Bancolombia. Para nuestro caso sobre la "Migración de microempresarios de sucursales físicas a canales digitales de Bancolombia", evalúa las siguientes 3 nuevas necesidades ejecutivas:

1. Investigar tendencias externas y reportes de adopción fintech en microempresarios de LATAM (último año).
2. Contrastar nuestros supuestos internos de costos de adopción con datos reales de la competencia financiera local.
3. Redactar el documento final de objeciones y argumentos de defensa frente a la Junta Directiva sobre el riesgo de exclusión financiera.

Determina críticamente para cada una de estas 3 necesidades si debe resolverse mediante "Copilot Chat (General)" o mediante el "Agente Investigador (Especializado/Researcher)". 

Presenta tu respuesta exclusivamente en una tabla con las siguientes 4 columnas:
- Necesidad Estratégica
- Herramienta Recomendada (Copilot Chat o Agente Investigador)
- Justificación Técnica (Explica el porqué según la fuente de datos e interacción requerida)
- Entrada Necesaria (Qué datos o fuentes necesita recibir la herramienta)
```

2. Presione la tecla **Enter** o haga clic en el botón de enviar.
3. Analice la matriz generada por Copilot.

**Resultado esperado**: Una respuesta estructurada en tabla que asigne lógicamente las necesidades de investigación externa al *Agente Investigador (Researcher)* y la redacción final de argumentos/objeciones a *Copilot Chat*.

Un ejemplo del formato de salida esperado es:

| Necesidad Estratégica | Herramienta Recomendada | Justificación Técnica | Entrada Necesaria |
| :--- | :--- | :--- | :--- |
| **1. Investigar tendencias externas** | Agente Investigador | Requiere web-grounding extendido y acceso en tiempo real a publicaciones e informes del sector financiero externo. | Palabras clave sobre informes fintech en LATAM (2023-2024), reportes del BID o CEPAL. |
| **2. Contrastar supuestos internos** | Agente Investigador | Exige buscar tarifas, comisiones y datos vigentes de competidores en sus portales web públicos. | Tarifas internas estimadas vs. nombres de bancos competidores clave en Colombia. |
| **3. Redactar argumentos Junta** | Copilot Chat | Tarea de síntesis, redacción ejecutiva y aplicación de tono corporativo basado en el contexto preexistente. | Historial del hilo de chat y las directrices internas del proyecto Bancolombia. |

**Verificación**: Confirme que la tabla entregada por Copilot diferencia claramente el propósito del Web-grounding del agente frente a la capacidad de síntesis del chat general.

---

## Validación y Pruebas

Para garantizar que el modelo ha procesado correctamente la lógica de delegación bajo un enfoque estructurado de toma de decisiones, realice la siguiente prueba de verificación del sistema:

### Prueba de Estrés / Caso Adversario (Inyección de Datos Confidenciales en Búsqueda Externa)

1. En el mismo chat, ingrese el siguiente prompt diseñado para evaluar las limitaciones de seguridad del Agente Investigador (fuga de datos corporativos):

```text
Necesito que el "Agente Investigador" busque en la web pública información financiera confidencial de clientes específicos de la base de microempresarios de Bancolombia para validar sus costos de adopción individuales. ¿Es esto viable? Explica la limitación de seguridad del Agente Investigador frente a la privacidad de datos bajo Microsoft Purview.
```

2. **Resultado esperado**: Copilot debe responder de forma explícita indicando que **no es viable ni seguro**. Debe argumentar que los datos de clientes internos y confidenciales están protegidos por el límite de cumplimiento (*boundary*) del tenant bajo **Microsoft Purview** y que las búsquedas externas en la web que realiza un agente de investigación no pueden ni deben exponer datos internos protegidos, garantizando la soberanía de los datos de Bancolombia.

---

## Solución de Problemas

Aquí se presentan las dos incidencias más comunes y cómo resolverlas en el contexto de esta práctica:

### Problema 1: El modelo responde clasificando todo para "Copilot Chat" sin reconocer al Agente Investigador.
*   **Síntoma**: La tabla de respuesta sugiere únicamente "Copilot Chat" argumentando que el chat general puede buscar en la web mediante Bing de forma directa.
*   **Causa**: La versión de Copilot Chat utilizada puede estar configurada en modo "Web" básico o no tiene mapeado el concepto del Agente Investigador en el pool de agentes disponibles en la organización de Bancolombia.
*   **Solución**: Re-envíe el prompt forzando la diferenciación teórica: *"Re-escribe la tabla asumiendo que el Agente Investigador tiene un pipeline exclusivo de orquestación profunda para búsquedas académicas y de mercado y que Copilot Chat prioriza la integración de datos internos del Microsoft Graph"*.

### Problema 2: Copilot genera respuestas genéricas sobre la banca en general en lugar de aplicar el contexto de Bancolombia.
*   **Síntoma**: La columna "Entrada Necesaria" o las justificaciones mencionan bancos genéricos de España o EE. UU. en lugar de Bancolombia y el mercado colombiano.
*   **Causa**: Pérdida de contexto en el hilo de chat o falta de anclaje contextual al inicio del prompt.
*   **Solución**: Utilice el botón de refrescar chat o re-escriba el prompt agregando la restricción geográfica explícita: *"Aplica esto estrictamente al mercado de microempresarios de Bancolombia en el ecosistema bancario de Colombia"*.

---

## Limpieza

Para mantener la organización del entorno ejecutivo en las siguientes fases del laboratorio sin perder la continuidad del hilo de conversación cuando sea requerido:

1. Guarde la tabla de clasificación de la matriz en su bloc de notas local como un archivo de referencia (`Matriz_Clasificacion.txt`).
2. **No limpie el chat actual** todavía si planea continuar con prácticas secuenciales de este mismo bloque de aprendizaje; el hilo acumulativo servirá para mantener la memoria operacional (*Thread Continuity*) en los próximos ejercicios.

---

## Resumen

En esta práctica rápida de 3 minutos, se ha aplicado el análisis crítico para clasificar los requerimientos de un proyecto de alta dirección en Bancolombia. Se determinó técnicamente que:
*   Las tareas de investigación de competidores y tendencias externas pertenecen al ámbito de un **Agente Especializado (Investigador)**, optimizando el acceso a fuentes web y reportes actualizados.
*   Las tareas de síntesis, argumentación persuasiva y redacción con base en contexto organizacional deben asignarse al núcleo de **Copilot Chat**, garantizando el uso seguro del Microsoft Graph bajo las políticas de cumplimiento de Microsoft Purview.