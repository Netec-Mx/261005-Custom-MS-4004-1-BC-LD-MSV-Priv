# Práctica 1

## Descripción General

Los participantes partirán de una solicitud ejecutiva sencilla y la transformarán progresivamente en una instrucción que solicite a Copilot identificar alternativas, riesgos, supuestos, información faltante y criterios para tomar una decisión. Se comparará el resultado inicial con el obtenido después de aplicar la fórmula del prompt.

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

