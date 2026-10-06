# Lab 01-00-08: Práctica 8. Los participantes llevarán los hallazgos relevantes de la investigación al análisis original y solicitarán determinar qué elementos fortalecen, debilitan o no modifican cada alternativa. Finalmente identificarán qué supuesto tendría mayor capacidad de cambiar la decisión si resultara incorrecto.

## Metadatos

| Dimensión | Detalle |
| :--- | :--- |
| **Duración** | 9 minutos |
| **Complejidad** | Media |
| **Nivel de Taxonomía de Bloom** | Aplicar |

---

## Descripción General

En este laboratorio práctico de 9 minutos, los participantes aprenderán a integrar hallazgos de investigación externa en un análisis de decisiones estratégicas preexistente dentro del mismo hilo de conversación de Microsoft 365 Copilot. Utilizando el escenario de la migración digital de microempresarios de Bancolombia, importarán los datos del archivo de investigación generado en la práctica anterior y contrastarán críticamente las hipótesis originales con la realidad empírica del mercado. El ejercicio guiará al estudiante para categorizar el impacto de los nuevos datos sobre las alternativas estratégicas y realizar un análisis de sensibilidad conceptual para determinar el supuesto de mayor riesgo para el negocio.

---

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:
- **Integrar** datos e investigaciones externas en un hilo de chat continuo de Microsoft 365 Copilot para enriquecer análisis estratégicos previos.
- **Categorizar** el impacto de nueva información de mercado sobre alternativas predefinidas usando la taxonomía "Fortalece / Debilita / Neutral".
- **Realizar** un análisis de sensibilidad conceptual mediante prompting avanzado para aislar el supuesto más crítico de una decisión de negocio.
- **Evaluar** críticamente las respuestas del modelo para detectar sesgos de confirmación o lagunas de información que requieran supervisión humana.

---

## Prerrequisitos

Para realizar este laboratorio de manera exitosa, debes cumplir con los siguientes prerrequisitos:
- **Prácticas previas completadas**: Haber ejecutado la Práctica 7 y disponer de la sesión activa de Copilot Chat (Business Chat) donde se evaluaron las alternativas de decisión para Bancolombia.
- **Acceso a datos**: Contar con el archivo `Reporte_Investigacion_Fintech.txt` generado en la práctica anterior. En caso de no tenerlo a mano, se proporciona un extracto condensado dentro de este laboratorio para asegurar la continuidad de la experiencia.
- **Comprensión conceptual**: Entender el marco de decisión de Bancolombia (migración de microempresarios de sucursales físicas a canales digitales reduciendo la fricción por brecha digital y costos de adopción).

---

## Entorno de Laboratorio

Este laboratorio se ejecuta enteramente en un entorno SaaS en la nube a través de un navegador web moderno. No se requiere instalación local de software complejo.

### Hardware Requerido
| Componente | Especificación Mínima |
| :--- | :--- |
| **Dispositivo** | Computador de escritorio o laptop con arquitectura x64 |
| **Memoria RAM** | 8 GB o superior |
| **Conectividad** | Conexión a Internet de banda ancha estable (Mínimo 10 Mbps de subida y bajada) |
| **Pantalla** | Resolución de 1920x1080 para visualización óptima en doble ventana |

### Software y Licencias Requeridas
| Tecnología / Herramienta | Versión / Edición | Enlace Oficial / Origen |
| :--- | :--- | :--- |
| **Sistema Operativo** | Windows 11 Enterprise (23H2 x64) | [Microsoft Windows](https://www.microsoft.com/windows) |
| **Navegador Web** | Microsoft Edge (Versión 128.0.2739.42 o superior) | [Microsoft Edge](https://www.microsoft.com/edge) |
| **Plataforma de IA** | Microsoft 365 Copilot Premium (Business Chat activo) | [Microsoft 365 Copilot](https://www.microsoft.com/microsoft-365/copilot) |
| **Licencia de M365** | Licencia de Microsoft 365 Copilot para Empresas | Portal de Administración de Microsoft 365 |

---

## Instrucciones Paso a Paso

### Paso 1: Recuperar el Contexto de la Sesión y Cargar el Reporte

**Objetivo**: Garantizar la continuidad del hilo de conversación (Thread Continuity) en Copilot Chat e incorporar el conocimiento externo del `Reporte_Investigacion_Fintech.txt`.

> **Nota de Diseño (THOR)**: Si has cerrado la pestaña del navegador, abre nuevamente tu chat de Copilot en Teams o Microsoft Edge e inicia la interacción haciendo referencia al contexto previo de Bancolombia. Si mantienes el chat abierto de las prácticas 6 y 7, **no abras un nuevo chat**; mantén el hilo para conservar la memoria de la sesión.

#### Instrucciones

1. Abre tu navegador **Microsoft Edge** y accede a la interfaz de Copilot de tu organización (ya sea vía [copilot.microsoft.com](https://copilot.microsoft.com) en modo de protección de datos comerciales, o a través de Microsoft Teams > Aplicación Copilot).
2. Asegúrate de que estás interactuando con **Copilot Chat (Business Chat)** usando tu cuenta corporativa autorizada.
3. Si el archivo `Reporte_Investigacion_Fintech.txt` no está cargado, localízalo en tu sistema de archivos. El contenido clave del reporte que utilizaremos para alimentar al modelo es el siguiente:
   ```text
   -- CONTENIDO SINTETIZADO DE REPORTE_INVESTIGACION_FINTECH.TXT --
   - El 72% de los microempresarios bancarizados en LATAM abandonan las apps móviles autogestionadas durante los primeros 30 días si no reciben asistencia guiada inicial.
   - El miedo a la inseguridad y al fraude en transacciones móviles representa un freno de adopción mayor (85%) que el costo de las comisiones de retiro.
   - Las alianzas con comercios locales o Corresponsales Bancarios Digitalizados incrementaron la adopción digital en un 140% en segmentos de bajos ingresos.
   - Las interfaces simplificadas con comandos de voz y soporte offline reducen el error del usuario final en un 60%.
   - Los costos de conectividad a datos móviles representan un inhibidor crítico para el 45% del segmento objetivo.
   ```
4. Si tu configuración de inquilino de Copilot permite adjuntar archivos directamente, haz clic en el icono del clip (Adjuntar) y carga el archivo `Reporte_Investigacion_Fintech.txt`.
5. Si tu entorno tiene restringida la carga directa de archivos locales por políticas de Prevención de Pérdida de Datos (DLP) de Microsoft Purview, copia el texto delimitado del recuadro anterior para pegarlo directamente en el prompt del Paso 2.

#### Resultado Esperado
Copilot debe estar listo en la misma sesión de chat para procesar el nuevo prompt, conservando el contexto del caso de Bancolombia y las alternativas estratégicas definidas con anterioridad (Alternativa A: Corresponsales físicos guiados, Alternativa B: Migración por incentivos y app simplificada autogestionada, Alternativa C: Modelo híbrido de padrinos digitales temporales).

#### Verificación
Verifica que el icono de adjunto muestre el archivo cargado, o que tengas el texto del reporte copiado en tu portapapeles.

---

### Paso 2: Ejecutar el Prompt de Análisis de Impacto Cruzado

**Objetivo**: Contrastar la investigación externa con las tres alternativas de solución estratégica planteadas en el caso de Bancolombia para evaluar cómo afecta cada hallazgo a la viabilidad de las opciones.

#### Instrucciones

1. Copia de manera exacta el siguiente prompt avanzado estructurado bajo el marco de **Contexto, Objetivo, Origen y Expectativas (COOE)**. Si no pudiste subir el archivo en el Paso 1, sustituye la etiqueta `[Insertar Reporte]` con el contenido de texto del reporte provisto en el Paso 1.

```text
Contexto: Estamos trabajando en la estrategia de migración del segmento de microempresarios de sucursales físicas a canales digitales en Bancolombia, abordando la brecha digital y costos de adopción. Anteriormente evaluamos tres alternativas: 
- Alternativa A: Migración 100% asistida en sucursales/corresponsales físicos (alta cercanía, alto costo).
- Alternativa B: Incentivos financieros/tasas cero y auto-capacitación en App simplificada (bajo costo operativo, alto riesgo de deserción).
- Alternativa C: Modelo híbrido de "Padrinos Digitales" temporales (costo inicial medio, mitigación guiada de brecha).

Objetivo: Contrasta nuestro análisis previo y alternativas con la nueva evidencia empírica de mercado contenida en el siguiente reporte de investigación fintech. Clasifica rigurosamente el impacto de los nuevos hallazgos sobre cada una de las tres alternativas.

Origen (Datos de Investigación):
[Insertar el texto del reporte aquí si no pudiste adjuntar el archivo "Reporte_Investigacion_Fintech.txt"]

Expectativas de la respuesta:
1. Genera una tabla comparativa con 4 columnas:
   - Alternativa Estratégica.
   - Hallazgo Clave del Reporte de Impacto.
   - Categorización del Impacto (Usa exclusivamente: "Fortalece", "Debilita" o "Neutral").
   - Justificación Analítica (Explica de forma concisa el porqué de la categoría basándote estrictamente en los datos provistos).
2. Mantén un tono ejecutivo, directo y enfocado a la mitigación de riesgos operativos y financieros para Bancolombia.
```

2. Pega el prompt en la caja de texto de Copilot Chat y presiona **Enter** (o haz clic en el botón de enviar).
3. Espera a que el motor de Copilot realice el procesamiento y el post-procesamiento bajo las directivas de seguridad corporativas.

#### Resultado Esperado
Copilot devolverá una tabla analítica estructurada donde se evalúan los puntos de contacto entre la investigación y las alternativas de Bancolombia. 
- La *Alternativa B (Autogestionada con incentivos)* debe verse claramente **debilidada** debido al hallazgo de que el 72% abandona las apps sin asistencia guiada.
- La *Alternativa A (Asistida en corresponsales)* y la *Alternativa C (Padrinos Digitales)* deben verse **fortalecidas** debido a la necesidad validada de soporte humano y el incremento del 140% de adopción en corresponsales digitales.

#### Verificación
Comprueba que la respuesta contenga exactamente la tabla con las cuatro columnas solicitadas y que la clasificación de impacto mantenga coherencia lógica estricta con los datos del reporte.

---

### Paso 3: Realizar el Análisis de Sensibilidad Conceptual

**Objetivo**: Identificar el supuesto o hipótesis estratégica más vulnerable (aquel que, de ser incorrecto, cambiaría drásticamente la dirección de la toma de decisiones del Comité de Bancolombia).

#### Instrucciones

1. En el mismo hilo de chat de Copilot, escribe la siguiente instrucción de seguimiento para realizar el análisis de sensibilidad:

```text
Con base en la tabla comparativa que acabas de estructurar y el contexto financiero de Bancolombia, realiza un análisis de sensibilidad conceptual:
1. Identifica de manera unívoca el SUPUESTO CRÍTICO de negocio que tiene la mayor capacidad de alterar radicalmente la decisión del Comité Directivo si resultara ser falso o incorrecto en la práctica.
2. Explica qué sucedería si este supuesto falla (el "peor escenario") y cómo afectaría la viabilidad de la opción híbrida (Alternativa C).
3. Propón una métrica de monitoreo estratégico temprano (un indicador clave de desempeño o KPI) que permita alertar a la gerencia si este supuesto clave está fallando.
4. Indica qué grado de incertidumbre queda aún en este análisis y qué información adicional requerimos recopilar con urgencia mediante supervisión humana o investigación de campo directa.
```

2. Envía la instrucción en el chat y observa cómo Copilot procesa y prioriza los riesgos analíticos del caso.

#### Resultado Esperado
Copilot responderá con una sección bien definida que aísla un supuesto crítico (comúnmente relacionado con la *efectividad del soporte humano/padrinos* o la *capacidad de absorción digital del microempresario*). 
- El peor escenario para la Alternativa C debe ilustrar cómo el costo del "Padrino Digital" puede transformarse en un gasto hundido si el cliente no logra la autonomía operativa tras la ventana de acompañamiento.
- Debe incluir una métrica clara (ej. *Tasa de retención digital tras el retiro del soporte del padrino* o *Tasa de deserción en los primeros 30 días*).
- Se debe visibilizar la necesidad de validación humana en campo debido a la incertidumbre sobre el comportamiento real de los microempresarios locales de Bancolombia frente al temor al fraude.

#### Verificación
Verifica que el modelo no asuma una decisión idealizada perfecta; la respuesta debe reconocer explícitamente las limitaciones de los datos disponibles y la necesidad de supervisión humana y pruebas piloto directas antes del despliegue masivo.

---

## Validación y Pruebas

Para asegurar el éxito del laboratorio y evaluar la calidad del entregable, verifica que se cumplan los siguientes puntos de control de calidad:

### Criterios de Evaluación y Evidencias

1. **Continuidad del Hilo de Chat**: El estudiante debió realizar todo el proceso en un solo hilo de conversación de Copilot. Esto se comprueba si el modelo alude a los análisis de alternativas anteriores sin necesidad de volver a introducirlos por completo.
2. **Estructura de Datos en Tabla**: El output del Paso 2 debe poseer estrictamente el formato de tabla de 4 columnas solicitado, sin omisiones en los nombres de las alternativas evaluadas.
3. **Mapeo de Categoría de Impacto**: 
   * La *Alternativa B (Autogestionada)* debe aparecer clasificada con un impacto de tipo **"Debilita"** apoyándose en la estadística de abandono del 72% provista en el reporte.
   * Si el modelo clasifica la Alternativa B como "Fortalece", la prueba se considera fallida debido a inconsistencia lógica en el razonamiento de la IA.
4. **Análisis de Incertidumbre y Sensibilidad**: La respuesta al Paso 3 debe señalar explícitamente un indicador clave de desempeño (KPI) medible de forma numérica y alertar sobre al menos una limitación de datos (brecha de conocimiento) que no cubre el reporte general de LATAM para la realidad específica de las sucursales de Bancolombia.

### Caso de Prueba Adversario (Detección de Sesgos / Alucinación Controlada)

Como método de control de calidad bajo la directiva de supervisión humana, verifica de forma crítica el output del modelo buscando lo siguiente:
- **Caso Adversario**: ¿Menciona el modelo datos de Bancolombia que no le proporcionaste (por ejemplo, cifras reales de sucursales físicas o presupuestos de TI específicos)? Si Copilot genera números financieros precisos no provistos en los prompts o en el reporte, se trata de una **alucinación**.
- **Acción Correctiva**: Escribe en el chat: *"Corrige el análisis anterior. Limítate estrictamente a los datos del reporte provisto y al contexto conceptual planteado, eliminando cualquier cifra que no haya sido introducida explícitamente en esta conversación."*

---

## Solución de Problemas

A continuación, se describen dos de los problemas más habituales al ejecutar este laboratorio específico y los pasos de mitigación recomendados:

### Problema 1: Copilot pierde el hilo del contexto anterior (Falta de Memoria de Sesión)
- **Síntoma**: Al procesar el prompt del Paso 2, Copilot responde pidiendo que se vuelvan a definir las alternativas estratégicas originales o se comporta como si estuviera en un chat completamente nuevo, ignorando la estructura de Bancolombia.
- **Causa**: Se ha alcanzado el límite de tokens del contexto (*context window*) de la sesión actual, o se abrió accidentalmente un nuevo chat o se refrescó el navegador limpiando el historial activo del LLM.
- **Solución**: No inicies un nuevo hilo desde cero si puedes evitarlo. Si es inevitable porque la sesión expiró, recupera el contexto histórico pegando un prompt de alineación rápida antes del Paso 2:
  ```text
  "Reiniciaremos el análisis estratégico de Bancolombia. Como contexto inicial rápido, recuerda que evaluamos tres alternativas para migrar microempresarios de sucursales físicas a canales digitales: Alternativa A (Asistida en sucursal/corresponsal, costo alto), Alternativa B (Autogestionada mediante App e incentivos, costo bajo) y Alternativa C (Híbrida con Padrinos Digitales temporales, costo medio). Confirma si tienes claro este escenario."
  ```
  Una vez que el modelo confirme su entendimiento, procede inmediatamente con el Paso 2 de este laboratorio.

### Problema 2: Error de bloqueo por políticas de seguridad de datos (DLP / Purview) al subir el archivo TXT
- **Síntoma**: Al intentar cargar el archivo `Reporte_Investigacion_Fintech.txt` mediante el icono del clip de la interfaz de chat, aparece un mensaje de advertencia indicando que el archivo no puede compartirse externamente o que el formato no está permitido por directivas de seguridad.
- **Causa**: Políticas rigurosas de prevención de pérdida de datos de la organización aplicadas al tenant empresarial de Microsoft 365 Copilot, que restringen la subida de archivos planos locales a chats de IA.
- **Solución**: Evita subir el archivo físico. Copia el contenido plano estructurado del reporte (provisto en el bloque de código del Paso 1) y pégalo directamente en la caja de prompt dentro de la sección delimitada por la etiqueta `Origen (Datos de Investigación)`. Copilot lo procesará con el mismo nivel de precisión contextual y respetando el cifrado en tránsito de los datos.

---

## Limpieza

Para este laboratorio de análisis estratégico en Copilot Chat, las tareas de limpieza son mínimas pero importantes para la gobernanza de datos de la organización:

1. **Guardar el Historial de Discusión**: Si deseas conservar este valioso análisis para la Práctica 9 y Práctica 10 (las cuales son acumulativas), no borres la conversación del chat.
2. **Exportar**: Copia las respuestas clave (especialmente la tabla comparativa y el análisis de sensibilidad) y pégalas en un documento de Microsoft Word local o bloc de notas etiquetado como `Analisis_Sensibilidad_Bancolombia.txt` para tener un respaldo seguro.
3. **Cierre seguro**: Si estás utilizando un equipo de cómputo compartido, asegúrate de cerrar la sesión de tu cuenta corporativa de Microsoft 365 en el navegador Microsoft Edge y borrar las cookies de navegación recientes. No se han creado bases de datos locales ni contenedores que requieran desinstalación o detención manual.

---

## Resumen

En esta **Práctica 8**, has completado con éxito la integración de hallazgos de investigación externa en un análisis de alternativas previamente diseñado, aplicando un enfoque riguroso de evaluación conceptual.

**Logros Clave**:
- **Consolidación de Datos**: Lograste vincular información proveniente de investigación fintech externa con las realidades estratégicas de la migración digital de Bancolombia.
- **Clasificación Semántica**: Utilizaste a Copilot para clasificar sistémicamente la influencia de cada dato (Fortalece / Debilita / Neutral), aportando objetividad al análisis y eliminando sesgos internos de planificación.
- **Aislamiento de Supuestos Críticos**: Identificaste la hipótesis de mayor riesgo del proyecto y definiste una métrica de alerta temprana (KPI), demostrando cómo un líder ejecutivo puede apoyarse en la IA para robustecer la toma de decisiones basada en el valor del negocio financiero.

Este entregable enriquecido en tu hilo de chat actual será el insumo directo para la **Práctica 9**, donde estructuraremos el Plan de Acción Operativo resultante en Microsoft Excel.

### Referencias Adicionales
* [Documentación oficial de Microsoft sobre prompts contextuales en Business Chat](https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-prompts)
* [Guía de Microsoft Purview para la protección de datos e información en Copilot](https://learn.microsoft.com/es-es/purview/protect-data-copilot)