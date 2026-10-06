# Práctica 5. Los participantes ejecutarán una misma solicitud de análisis utilizando modelos de OpenAI y Claude. En lugar de buscar cuál modelo es “mejor”, compararán cuál resultado es más útil para el propósito ejecutivo planteado y qué elementos conservarían o refinarían.

## Metadatos

| Dimensión | Detalle |
| :--- | :--- |
| **Duración** | 6 minutos |
| **Complejidad** | Alta (Hard) |
| **Nivel de Bloom** | Aplicar (Apply) |

---

## Descripción General

En esta práctica de laboratorio, ejecutarás un análisis comparativo y heurístico utilizando la interfaz de selección de modelos dentro de tu entorno corporativo de **Microsoft 365 Copilot**. Utilizando el escenario centralizado de **Bancolombia** (migración del segmento de microempresarios de sucursales físicas a canales digitales, enfrentando la brecha digital y costos de adopción), procesarás un prompt avanzado de *Red Teaming* bajo dos motores fundacionales distintos: **OpenAI (GPT-4o)** y **Anthropic (Claude 3.5 Sonnet)**. El objetivo no es declarar un ganador absoluto, sino evaluar críticamente el valor estratégico de cada modelo según su estructura sintáctica, nivel de realismo y adecuación para la toma de decisiones ejecutivas.

---

## Objetivos de Aprendizaje

Al finalizar esta práctica, serás capaz de:
* [ ] **Ejecutar** un mismo prompt estructurado utilizando el selector de modelos configurado en el tenant de la organización.
* [ ] **Evaluar críticamente** las respuestas de modelos de OpenAI y Claude bajo criterios de rigor financiero, realismo de riesgos y tono corporativo.
* [ ] **Identificar y fusionar** los elementos analíticos de mayor valor estratégico para presentar un informe unificado a la alta dirección.

---

## Prerrequisitos

* **Conocimiento teórico**: Comprensión del modelo de orquestación RAG, el marco de trabajo COOE (Contexto, Objetivo, Origen y Expectativas) y los conceptos básicos de análisis de riesgos (*Red Teaming*).
* **Acceso y licencias**:
  * Cuenta activa en el tenant de Bancolombia con **Microsoft 365 Copilot Premium** habilitado.
  * Selector de modelos (*Model Selection Interface*) activo en Copilot Chat o Business Chat (en caso de restricciones en el tenant, se utilizarán perfiles de sistema alternativos o el cambio de modo creativo/preciso de Copilot).
* **Continuidad de la sesión**: Mantener abierto el mismo hilo de conversación iniciado en las Prácticas 1 a 4 para asegurar la retención de contexto (*Thread Continuity*).

---

## Entorno de Laboratorio

### Requisitos de Hardware

| Componente | Especificación Mínima |
| :--- | :--- |
| **Dispositivo de cómputo** | Procesador Intel Core i5 de 64 bits (o equivalente AMD) |
| **Memoria RAM** | 8 GB |
| **Resolución de Pantalla** | Mínimo 1920x1080 píxeles |
| **Conexión de Red** | Banda ancha estable (Mínimo 10 Mbps de bajada y subida) |

### Requisitos de Software y Licencias

| Software / Servicio | Versión Especificada | Enlace Oficial |
| :--- | :--- | :--- |
| **Microsoft Edge** | 128.0.2739.42 | [Enlace Oficial de Microsoft Edge](https://www.microsoft.com/edge) |
| **Microsoft Teams (Trabajo/Escuela)** | 24193.1805.2987.5853 | [Enlace Oficial de Microsoft Teams](https://www.microsoft.com/microsoft-teams) |
| **Microsoft 365 Copilot con Business Chat** | Service Release 2408 (Build 17928.20156) | [Enlace Oficial de Microsoft 365 Copilot](https://www.microsoft.com/microsoft-365/copilot) |
| **Modelos de IA Disponibles** | GPT-4o (OpenAI), Claude 3.5 Sonnet (Anthropic) | [Enlace de Azure OpenAI](https://azure.microsoft.com/services/cognitive-services/openai-service/) |

---

## Instrucciones Paso a Paso

### Paso 1: Ejecutar el Prompt de Red Teaming usando OpenAI (GPT-4o)

**Objective**: Obtener un análisis de riesgos estructurado utilizando el motor GPT-4o de OpenAI para identificar vulnerabilidades operativas en el plan de migración digital de Bancolombia.

**Instructions**:

1. Abre tu navegador **Microsoft Edge (128.0.2739.42)** e inicia sesión en tu portal de Microsoft 365.
2. Abre la aplicación **Copilot (Business Chat)** dentro de Teams o a través del portal web corporativo. Asegúrate de estar en el mismo hilo de conversación donde desarrollaste la Práctica 4 para mantener el contexto de la migración digital de microempresarios de Bancolombia.
3. En la interfaz de chat de Copilot, ubica el menú desplegable del **Selector de Modelos** (generalmente ubicado en la parte inferior izquierda de la caja de texto o en el encabezado de la conversación) y selecciona **GPT-4o (OpenAI)**.
4. Copia y pega el siguiente prompt avanzado en la caja de texto, el cual aplica la estructura COOE y añade una prueba adversarial implícita para evaluar la precisión del modelo:

```text
[Contexto]: Estamos diseñando la migración del segmento de microempresarios de sucursales físicas a canales digitales de Bancolombia, enfrentando fricción por brecha digital y costos de adopción.
[Objetivo]: Actúa como un asesor de Red Teaming altamente crítico de McKinsey. Analiza nuestro plan estratégico e identifica los 3 riesgos de adopción técnica más severos y 2 dependencias críticas con sistemas legados (Core Bancario). 
[Origen]: Utiliza la información provista en nuestro hilo de conversación actual y tu conocimiento del sistema financiero de microfinanzas en Colombia.
[Expectativas]: Entrega tu análisis estructurado en una tabla que incluya: Nombre del riesgo/dependencia, Probabilidad de ocurrencia (Alta/Media/Baja), Impacto financiero (en USD) proyectado y una Acción de Mitigación accionable. Mantén un tono formal, ejecutivo e implacable.
[Caso de Prueba]: Incluye un análisis de cómo mitigar la siguiente contradicción operativa: 'El 90% de nuestros microempresarios no posee un teléfono inteligente, pero el 100% prefiere usar la app móvil en lugar de ir a la sucursal física'. Explica la inconsistencia lógica de esta premisa si se presenta en los datos de origen.
```

5. Presiona **Enviar** (Enter) y espera a que el modelo procese y complete la respuesta.

**Expected output**:
* Una tabla clara y bien estructurada que liste 3 riesgos (por ejemplo: falta de alfabetización digital de los comerciantes, costos ocultos de planes de datos móviles) y 2 dependencias heredadas (por ejemplo: latencia en la actualización de saldos en tiempo real en la base de datos central).
* Una sección específica resolviendo el "Caso de Prueba", donde el modelo señale la contradicción lógica explícita (no es posible que el 100% prefiera la app móvil si el 90% no tiene smartphone) en lugar de simplemente aceptar la premisa como un hecho real del negocio.

**Verification**: Comprueba que la tabla generada contenga estimaciones cuantitativas lógicas (ej. impacto financiero estimado en pérdidas operativas o de clientes) y que el tono sea altamente ejecutivo y directo.

---

### Paso 2: Ejecutar el mismo Prompt de Red Teaming usando Anthropic (Claude 3.5 Sonnet)

**Objective**: Ejecutar la misma consulta exacta utilizando el motor Claude 3.5 Sonnet para contrastar la estructura narrativa, la profundidad cualitativa y la capacidad de detección de contradicciones lógicas.

**Instructions**:

1. En la misma ventana de chat de Copilot, haz clic en el **Selector de Modelos** y cambia la selección activa a **Claude 3.5 Sonnet (Anthropic)**.
   * *Nota:* Si tu configuración específica de tenant de Bancolombia no muestra el selector con nombres de marca debido a políticas de TI, cambia el perfil del sistema de "Preciso" a "Creativo" o viceversa, o utiliza el agente alternativo configurado por tu administrador para simular un motor de procesamiento diferente.
2. Copia exactamente el **mismo prompt** utilizado en el Paso 1:

```text
[Contexto]: Estamos diseñando la migración del segmento de microempresarios de sucursales físicas a canales digitales de Bancolombia, enfrentando fricción por brecha digital y costos de adopción.
[Objetivo]: Actúa como un asesor de Red Teaming altamente crítico de McKinsey. Analiza nuestro plan estratégico e identifica los 3 riesgos de adopción técnica más severos y 2 dependencias críticas con sistemas legados (Core Bancario). 
[Origen]: Utiliza la información provista en nuestro hilo de conversación actual y tu conocimiento del sistema financiero de microfinanzas en Colombia.
[Expectativas]: Entrega tu análisis estructurado en una tabla que incluya: Nombre del riesgo/dependencia, Probabilidad de ocurrencia (Alta/Media/Baja), Impacto financiero (en USD) proyectado y una Acción de Mitigación accionable. Mantén un tono formal, ejecutivo e implacable.
[Caso de Prueba]: Incluye un análisis de cómo mitigar la siguiente contradicción operativa: 'El 90% de nuestros microempresarios no posee un teléfono inteligente, pero el 100% prefiere usar la app móvil en lugar de ir a la sucursal física'. Explica la inconsistencia lógica de esta premisa si se presenta en los datos de origen.
```

3. Presiona **Enviar** (Enter) y permite que el modelo procese el análisis histórico.

**Expected output**:
* Una respuesta con un fuerte enfoque cualitativo y una estructura narrativa muy pulida.
* La tabla requerida, destacando las barreras del usuario final y las dependencias técnicas de integración de servicios legados de Bancolombia.
* Una respuesta reflexiva y analítica frente al "Caso de Prueba", desglosando con alta precisión lingüística la inconsistencia del muestreo y ofreciendo una solución metodológica (ej. sugerir canales alternativos como USSD o agentes bancarios autorizados).

**Verification**: Verifica que la salida mantenga la separación de campos de la tabla solicitada y que la redacción evidencie un enfoque centrado en la usabilidad y la experiencia del usuario (fuerza común en los modelos Claude).

---

### Paso 3: Análisis Heurístico y Fusión Estratégica para Entrega Ejecutiva

**Objective**: Comparar heurísticamente los dos resultados y consolidar un informe de riesgos óptimo en el chat de Copilot para la toma de decisiones del Comité de Dirección.

**Instructions**:

1. Analiza comparativamente ambas salidas bajo los siguientes criterios:
   * **Precisión Cuantitativa**: ¿Qué modelo dio estimaciones financieras de impacto más realistas para Bancolombia?
   * **Estructura y Legibilidad**: ¿Cuál tabla es más fácil de presentar en un slide ejecutivo de PowerPoint?
   * **Detección de Contradicciones**: ¿Cuál identificó la paradoja de los smartphones con mayor claridad crítica?
2. Escribe una instrucción (prompt) en el chat para consolidar lo mejor de ambos mundos. Asegúrate de pedirle a Copilot que unifique el análisis en un formato final óptimo. Escribe el siguiente mensaje:

```text
Consolida el análisis anterior en un único reporte ejecutivo de riesgos de Red Teaming para la Junta Directiva de Bancolombia. 
Toma la precisión métrica y de infraestructura de Core Bancario de la respuesta de GPT-4o, junto con el análisis cualitativo, empatía con el usuario y la resolución de la paradoja móvil presentados por Claude.
Genera un único entregable que combine lo mejor de ambos análisis en una sola tabla unificada y añade una sección final de 'Recomendación Ejecutiva de Ruta Crítica' que no supere los 3 párrafos.
```

3. Envía el mensaje y revisa el reporte final unificado.

**Expected output**:
* Un reporte ejecutivo integrado que combina datos cuantitativos financieros rigurosos con una visión humana y de experiencia de usuario, resolviendo con éxito la paradoja del smartphone y emitiendo una recomendación de ruta crítica con terminología corporativa impecable.

**Verification**: Confirma que el entregable unificado no repita ideas, que no mantenga la contradicción del caso de prueba como un hecho real y que esté estructurado con viñetas claras para una presentación de alta dirección.

---

## Validación y Pruebas

Para asegurar que los objetivos del laboratorio se cumplieron con el rigor técnico y la supervisión requerida para un entorno ejecutivo en Bancolombia, realiza las siguientes pruebas de validación:

### 1. Validación de Detección de Contradicción (Prueba Adversarial)
* **Criterio de éxito**: Ambos modelos deben haber alertado explícitamente sobre la imposibilidad material de que un grupo sin smartphones (90%) prefiera mayoritariamente una app móvil (100%). 
* **Evidencia**: Si algún modelo aceptó la premisa "tal cual" y sugirió crear una app móvil para personas que no tienen teléfonos inteligentes sin cuestionar los datos de origen, la validación habrá **fallado**. Se requiere una advertencia de inconsistencia lógica en el texto generado.

### 2. Validación de Métricas de Impacto Financiero
* **Criterio de éxito**: Las estimaciones financieras incluidas en la columna "Impacto financiero (en USD)" deben tener un orden de magnitud realista para un proyecto de transformación digital bancaria en Colombia (ej. rangos de USD $50,000 a USD $2,000,000 dependiendo de la severidad), en lugar de números genéricos como "Alto" o "Bajo" o cifras absurdas (como $100 dólares o $10 billones de dólares).
* **Evidencia**: Revisión visual directa de la tabla consolidada en el Paso 3.

---

## Solución de Problemas

Aquí encontrarás soluciones a los dos problemas técnicos más comunes durante la ejecución de esta práctica de comparación multi-modelo:

### Problema 1: El selector de modelos no está visible o está bloqueado en mi sesión de Copilot de Bancolombia
* **Síntoma**: No aparece ningún menú desplegable ni opción para elegir entre GPT-4o y Claude 3.5 Sonnet. La interfaz se mantiene fija en un solo motor de chat.
* **Causa**: Limitaciones de licenciamiento temporal, configuraciones estrictas de seguridad de datos (Data Loss Prevention) dentro del tenant de producción de la organización o despliegue progresivo de características.
* **Solución**: 
  1. Si estás en Teams, intenta abrir Copilot desde el navegador Edge accediendo a `copilot.microsoft.com` con tus credenciales corporativas.
  2. Si el selector sigue sin aparecer, simula el cambio de modelo ajustando el estilo de conversación de Copilot: usa el modo **"Preciso"** como sustituto de GPT-4o (enfocado en lógica, matemáticas y hechos rigurosos) y el modo **"Creativo"** como sustituto de Claude (enfocado en lenguaje natural fluido y redacción narrativa avanzada). Ejecuta los Pasos 1 y 2 bajo estas modalidades respectivas.

### Problema 2: El segundo modelo pierde la memoria de los datos generados en las prácticas previas (Falta de Continuidad del Hilo)
* **Síntoma**: Al cambiar de modelo o enviar el segundo prompt, la IA responde preguntando qué es el "Proyecto de migración de microempresarios" o ignora el contexto de la sucursal física de Bancolombia de la Práctica 4.
* **Causa**: El cambio de motor dentro de una misma interfaz puede forzar el reinicio de la ventana de contexto del LLM (Context Window Reset) en ciertas configuraciones de la API corporativa de Microsoft.
* **Solución**: Si el modelo se comporta como si hubiera olvidado el contexto, vuelve a inyectar el contexto de forma explícita al inicio de tu prompt agregando un párrafo de resumen:
  * *"Contexto de recuperación: Bancolombia está migrando su segmento de microempresarios rurales de canales físicos a canales digitales (App/Web), pero enfrenta barreras de costos de planes de datos y analfabetismo digital. El plan contempla habilitar quioscos digitales asistidos y simplificar la interfaz."*

---

## Limpieza

Dado que la siguiente práctica de este programa educativo es acumulativa y requiere mantener la memoria del chat actual para fines de auditoría e investigación:

1. **NO borres** el historial de conversación actual en Copilot.
2. **NO utilices el botón "Nuevo tema"** (icono de escoba/limpieza de chat) ya que esto rompería la secuencia histórica y tendrías que reinyectar todo el contexto del negocio en la Práctica 6.
3. Simplemente exporta o copia el reporte consolidado final generado en el Paso 3 en un bloc de notas local (por ejemplo, con el nombre `Evidencia_Red_Teaming_Práctica5.txt`) para asegurar un respaldo fuera de línea si deseas realizar consultas posteriores.

---

## Resumen

En esta práctica, aplicaste una evaluación heurística de modelos fundacionales cruzando el rigor métrico de **OpenAI** con la flexibilidad narrativa y la empatía cualitativa de **Anthropic Claude**. Aprendiste que, para un ejecutivo de alto nivel, la IA no debe considerarse como una herramienta monolítica de respuesta única; la capacidad de alternar modelos y unificar sus respectivas fortalezas permite generar análisis de riesgos de Red Teaming sustancialmente más robustos, con lógica de negocio depurada y con una mitigación proactiva de sesgos e inconsistencias en la toma de decisiones estratégicas de **Bancolombia**.

### Recursos adicionales
* [Guía de Microsoft 365 Copilot para toma de decisiones ejecutivas](https://learn.microsoft.com/microsoft-365-copilot/)
* [Documentación técnica sobre Model Selection en Azure OpenAI y Copilot Studio](https://learn.microsoft.com/azure/cognitive-services/openai/)
