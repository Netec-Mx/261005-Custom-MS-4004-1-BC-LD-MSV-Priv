# Lab 01-00-03: Práctica 3. A partir del problema estructurado, los participantes solicitarán a Copilot tres alternativas de actuación. Para cada alternativa deberán obtener beneficio esperado, riesgos, dependencias, supuesto crítico, información faltante e indicadores que permitirían evaluar posteriormente su efectividad. Después modificarán criterios o restricciones para observar cómo cambia la recomendación.

## Metadatos

| Metadato | Valor |
| :--- | :--- |
| **Duración** | 8 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Aplicar (Apply) |

---

## Descripción General

En este laboratorio práctico, los participantes simularán el rol de un consultor de estrategia corporativa trabajando para Bancolombia. Utilizando el mismo hilo de conversación consolidado en la Práctica 2, solicitarán a Microsoft 365 Copilot la formulación de tres alternativas estratégicas diferenciadas para abordar la migración del segmento de microempresarios hacia canales digitales. 

Cada alternativa se analizará bajo seis dimensiones de viabilidad (beneficios, riesgos, dependencias, supuestos, información faltante y métricas de éxito). Posteriormente, los participantes ejecutarán un análisis de sensibilidad introduciendo restricciones operativas extremas (reducción del 40% de presupuesto y tiempo límite de implementación de 3 meses). Esto permitirá evaluar críticamente cómo Copilot reconfigura prioridades y adapta recomendaciones ejecutivas bajo presión corporativa simulada.

---

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:
* [ ] Solicitar y estructurar tres alternativas estratégicas detalladas utilizando Copilot en Microsoft 365, desglosando viabilidad técnica, operativa y financiera.
* [ ] Diseñar indicadores clave de rendimiento (KPIs) y documentar vacíos de información o dependencias críticas para la toma de decisiones.
* [ ] Ejecutar un análisis de sensibilidad en tiempo real mediante la modificación interactiva de restricciones de presupuesto y de tiempo de comercialización (*Time-to-Market*).
* [ ] Evaluar críticamente el cambio de comportamiento, lógica y priorización del modelo de lenguaje de Copilot ante escenarios de alta presión de recursos.

---

## Prerrequisitos

* **Conocimiento previo**: Conceptos de estructuración de problemas corporativos, análisis de sensibilidad y comprensión del marco de migración digital para microempresarios en banca.
* **Acceso requerido**:
  * Cuenta activa de Microsoft 365 con licencia habilitada para **Microsoft 365 Copilot Premium (incluyendo Business Chat)**.
  * Mantener abierto el mismo navegador y la misma sesión de chat (Thread Continuity) utilizada durante la Práctica 2 para conservar el historial y contexto de Bancolombia.

---

## Entorno de Laboratorio

### Requisitos de Hardware

| Componente | Requisito Mínimo |
| :--- | :--- |
| **Dispositivo de cómputo** | Laptop o PC de escritorio con Procesador de 64 bits Intel Core i5 o superior (o equivalente AMD) |
| **Memoria RAM** | Mínimo 8 GB de memoria RAM disponibles |
| **Resolución de pantalla** | 1920x1080 píxeles para facilitar la visualización del chat en paralelo |
| **Conectividad a Internet** | Conexión de banda ancha estable (Mínimo 10 Mbps de bajada y subida) |

### Requisitos de Software y Licencias

| Software / Servicio | Versión Exacta | Licencia / Configuración | Enlace de Descarga / Acceso |
| :--- | :--- | :--- | :--- |
| **Microsoft Edge** | Versión 128.0.2739.42 (64-bit) | Estándar de sistema operativo | [Microsoft Edge](https://www.microsoft.com/edge) |
| **Microsoft 365 Copilot (Business Chat)** | Service Release 2408 (Build 17928.20156) | Copilot Premium para empresas | [Portal Microsoft 365](https://portal.office.com) |

### Configuración Inicial

1. Abre el navegador **Microsoft Edge (128.0.2739.42)**.
2. Accede a [https://copilot.microsoft.com](https://copilot.microsoft.com) e inicia sesión con las credenciales corporativas autorizadas de Bancolombia o del tenant de prueba asignado.
3. Localiza el chat activo donde se completó la Práctica 2. Asegúrate de **no iniciar un nuevo chat** para garantizar la continuidad del hilo de conversación (*Thread Continuity*).

---

## Instrucciones Paso a Paso

### Paso 1: Generación de las tres alternativas estratégicas multidimensionales

**Objetivo**: Solicitar a Microsoft 365 Copilot tres rutas estratégicas mutuamente excluyentes y exhaustivas para la migración del segmento de microempresarios de Bancolombia, desglosando cada opción en los parámetros críticos de decisión.

**Instrucciones**:

1. En el chat activo, ubícate en la caja de redacción del prompt de Copilot.
2. Copia y pega el siguiente prompt avanzado diseñado bajo la estructura de Contexto, Objetivo, Origen y Expectativas:

```text
[CONTEXTO]
Actúas como un Consultor de Estrategia de Canales Digitales de primer nivel para Bancolombia. Continuamos abordando el reto del segmento de microempresarios que experimenta alta fricción, costos de adopción y brecha digital al migrar desde sucursales físicas hacia canales digitales.

[OBJETIVO]
Tomando como base la estructura del problema consolidada en la práctica anterior en este chat, propón exactamente TRES alternativas de actuación estratégica diferenciadas para Bancolombia. 

[ORIGEN]
Utiliza el contexto de brecha de adopción y los puntos de dolor estructurados previamente en nuestro historial de conversación.

[EXPECTATIVAS DE ESTRUCTURA Y RESPUESTA]
Para cada una de las tres alternativas estratégicas de actuación, debes proporcionar de manera estructurada los siguientes apartados bajo títulos en negrita en formato Markdown:

1. **Nombre de la Alternativa:** (Nombre innovador, conciso y de enfoque bancario).
2. **Beneficio Esperado:** (Impacto cualitativo y cuantitativo esperado en la migración de microempresarios).
3. **Riesgos Asociados:** (Menciona al menos dos riesgos financieros o de adopción tecnológica).
4. **Dependencias Clave:** (Sistemas de TI, alianzas o normativas regulatorias necesarias).
5. **Supuesto Crítico:** (La hipótesis de negocio o comportamiento que DEBE ser cierta para que la alternativa funcione).
6. **Información Faltante:** (Qué métricas o datos internos específicos de Bancolombia requerimos y hoy no tenemos en este chat para validar la opción).
7. **Indicadores de Efectividad (KPIs):** (Dos indicadores clave de rendimiento medibles para evaluar el éxito posterior a la implementación).

Por favor, genera la respuesta directamente en formato estructurado para ser presentada ante el comité de innovación.
```

3. Presiona **Enter** para enviar el prompt a Copilot.
4. Lee detalladamente la propuesta generada. Asegúrate de que las alternativas sean realistas y adaptadas a la geografía de Bancolombia (por ejemplo: migración apoyada en corresponsales bancarios, aplicaciones móviles simplificadas de bajo consumo de datos móviles, o micro-capacitaciones digitales integradas en plataformas existentes como Nequi o Bancolombia A la Mano).

**Resultado esperado**:
Copilot proporcionará una respuesta estructurada en Markdown con tres opciones diferenciadas de negocio. Un fragmento del resultado esperado lucirá similar a esto:

```markdown
### Alternativa 1: Red de Mentores de Barrio y Corresponsales Bancarios Digitales
* **Beneficio Esperado:** Incremento del 25% en la tasa de adopción digital al apalancarse en la confianza de líderes de comunidad locales y corresponsales ya establecidos.
* **Riesgos Asociados:** Riesgo de suplantación de identidad por fraude y resistencia inicial del corresponsal por carga laboral.
* **Dependencias Clave:** Red de corresponsales físicos de Bancolombia e integración de un módulo de educación digital simple en terminales físicas.
...
```

**Verificación**:
Valida que la respuesta de Copilot contenga exactamente **tres alternativas** y que cada una incluya los **7 puntos estructurados** solicitados.

---

### Paso 2: Análisis de sensibilidad ante restricciones operativas críticas

**Objetivo**: Evaluar la resiliencia y capacidad adaptativa de las recomendaciones de Copilot mediante la simulación de un cambio drástico en las condiciones de presupuesto y plazos corporativos dictados por la dirección del banco.

**Instrucciones**:

1. En la misma ventana de chat, introduce el siguiente prompt de análisis de sensibilidad que impone restricciones de tiempo y costos financieros:

```text
[CONTEXTO]
La junta directiva de Bancolombia ha modificado de forma imprevista las directrices estratégicas de este año debido a una contracción en el presupuesto corporativo y a la necesidad de obtener retornos rápidos ante competidores Neobancos en el mercado colombiano.

[RESTRICCIONES CRÍTICAS]
Debes ajustar y evaluar las tres alternativas estratégicas generadas en el paso anterior bajo estas dos nuevas restricciones estrictas:
1. Reducción inmediata del 40% en el presupuesto inicial asignado para inversión técnica y de mercadeo.
2. El tiempo máximo de implementación para el lanzamiento del primer piloto viable se reduce a solo 3 meses.

[OBJETIVO]
Realiza un análisis estratégico rápido respondiendo a los siguientes tres puntos:
- ¿Cuál de las tres alternativas presentadas anteriormente debe ser descartada de inmediato y por qué no es viable bajo estas nuevas restricciones?
- ¿Cómo deben rediseñarse, simplificarse o fusionarse las dos alternativas restantes para poder cumplir con el recorte del 40% del presupuesto y el límite de 3 meses? Explica las modificaciones clave.
- Presenta una propuesta consolidada recomendada para ser ejecutada inmediatamente por el equipo, indicando su viabilidad bajo esta alta presión.

Estructura tu respuesta con viñetas ejecutivas orientadas a la alta dirección financiera del banco.
```

2. Envía el prompt.
3. Analiza críticamente el cambio de prioridades que realiza la IA. Observa si descarta las alternativas que dependían de pesados desarrollos tecnológicos a largo plazo o de la implementación de hardware físico costoso.

**Resultado esperado**:
Copilot devolverá un análisis de sensibilidad detallado en el que:
* Identifica y descarta justificadamente una de las alternativas (por ejemplo, aquella que involucra subsidiar hardware o rediseñar la arquitectura base de la App principal por su alto costo y tiempo de desarrollo).
* Ofrece estrategias de mitigación para las opciones viables (por ejemplo, apalancarse en soluciones ya construidas o canales existentes de menor costo como mensajería interactiva por WhatsApp corporativo de Bancolombia).
* Recomienda una sola opción rápida y de bajo costo para implementar el piloto en 90 días.

**Verificación**:
Confirma que la respuesta se comprometa directamente con los valores de las restricciones suministradas en el prompt (la reducción del **40% de presupuesto** y el límite de **3 meses**).

---

## Validación y Pruebas

Para asegurar la calidad y consistencia lógica del análisis obtenido por Copilot, realiza la siguiente prueba de control contra sesgos y alucinaciones comunes de modelos de lenguaje grande (Adversarial Testing):

1. En el mismo chat, ingresa este prompt de validación de robustez ante escenarios regulatorios colombianos imprevistos:

```text
Para la alternativa de contingencia priorizada que elegiste bajo el límite de 3 meses, asume por un momento que la Superintendencia Financiera de Colombia emite una nueva circular de ciberseguridad que prohíbe de manera absoluta el registro de nuevos usuarios financieros mediante el uso de datos biométricos de huella facial a través de dispositivos móviles personales durante los próximos 6 meses. 

Evalúa críticamente: ¿Se bloquea tu propuesta por esta regulación colombiana? Si la respuesta es sí, propón un ajuste operativo ágil de autenticación que mantenga el presupuesto bajo el límite del 40% de reducción y el plazo de lanzamiento de 3 meses.
```

2. **Evaluación de la Respuesta**:
   * **Precisión y Viabilidad**: Evalúa si la respuesta de Copilot propone soluciones realistas del mercado colombiano (como autenticación mediante OTP - *One Time Password* vía SMS, o registro simplificado asistido a través de la red de corresponsales que cuenta con hardware homologado).
   * **Gobernanza**: Asegura que el modelo no sugiera ignorar la regulación o subestimar el riesgo de ciberseguridad.

---

## Solución de Problemas

A continuación se describen dos fallos comunes que pueden presentarse durante la sesión práctica y cómo corregirlos inmediatamente:

### Problema 1: Pérdida del contexto histórico de Bancolombia (La IA responde con generalidades)
* **Síntoma**: Al solicitar las alternativas, Copilot proporciona respuestas genéricas de bancos globales (como Chase o Bank of America) o sugiere canales físicos e infraestructuras que no pertenecen a Bancolombia.
* **Causa**: Se cerró accidentalmente el navegador o se abrió un "Nuevo chat" en la barra lateral de Microsoft Copilot, provocando la pérdida de memoria de la sesión (Thread Continuity).
* **Solución**: No inicies un nuevo hilo de chat. Copia el mapa del problema o resumen estratégico estructurado al final de la Práctica 2 y pégalo al inicio de tu prompt en el Paso 1 diciendo: *"Utiliza el siguiente contexto del problema de Bancolombia para responder a mi solicitud: [Pegar el resumen estructurado de la Práctica 2]..."*.

### Problema 2: Resistencia a descartar alternativas caras (Sesgo de persistencia de la IA)
* **Síntoma**: Al realizar el análisis de sensibilidad en el Paso 2, Copilot afirma de manera vaga que *"las tres alternativas propuestas siguen siendo válidas buscando eficiencias"*, ignorando el impacto real de la reducción presupuestal del 40%.
* **Causa**: El modelo presenta un sesgo de anclaje con las ideas que generó inicialmente en el Paso 1 y evita tomar decisiones ejecutivas difíciles de eliminación.
* **Solución**: Envía un prompt correctivo de control al chat diciendo: *"El presupuesto del 40% menos y el tiempo de 3 meses son restricciones reales, estrictas y obligatorias de la junta directiva. No es posible ejecutar las tres opciones. Obligatoriamente debes descartar una de ellas. Argumenta técnicamente cuál de ellas no tiene ninguna posibilidad física o financiera de realizarse en solo 90 días"*.

---

## Limpieza

1. Selecciona y copia el texto completo de las alternativas consolidadas y el análisis de sensibilidad prioritario del Paso 2.
2. Abre un editor de texto o archivo temporal y guarda esta información bajo el nombre de archivo estándar **`Reporte_Investigacion_Fintech.txt`** (puedes guardarlo localmente o en tu OneDrive). Este archivo y su contenido se utilizarán como base de entrada de contexto para las Prácticas 8 y 9.
3. **Advertencia de Continuidad**: **No limpies el chat de Microsoft 365 Copilot**, mantén la pestaña activa del navegador abierta, ya que las prácticas de toma de decisiones del siguiente módulo se construirán sobre esta base.

---

## Resumen

En esta práctica número 3, has aprendido a utilizar Microsoft 365 Copilot Premium como un asesor ejecutivo de alto nivel, aplicando un análisis de sensibilidad automatizado sobre decisiones de negocio. 

Al estructurar los prompts con el marco de Contexto, Objetivo, Origen y Expectativas, lograste que Copilot generara tres alternativas detallando sus riesgos, dependencias y supuestos. Al retar la propuesta con limitaciones reales de presupuestos (reducción de un 40%) y tiempo (*Time-to-Market* de 3 meses), demostraste cómo los modelos fundacionales pueden procesar lógicas complejas bajo presión de parámetros, facilitando a los ejecutivos de Bancolombia la simulación rápida de escenarios y la agilización del ciclo de planificación estratégica corporativa.

### Recursos Adicionales
* [Guía de Microsoft 365 Copilot para Ejecutivos](https://learn.microsoft.com/es-es/microsoft-365-copilot/overview)
* [Uso de Inteligencia Artificial para el Modelado de Escenarios de Sensibilidad y Negocios en Microsoft WorkLab](https://www.microsoft.com/en-us/worklab)