# Práctica 7: Los participantes utilizarán Investigador (Researcher) para explorar tendencias relacionadas con comportamiento y adopción de servicios financieros digitales, experiencia del cliente y otros factores pertinentes al escenario. La solicitud deberá indicar qué decisión se está evaluando y qué información se necesita para reducir incertidumbre. El resultado deberá presentarse exclusivamente como un informe textual, identificando tendencias, factores externos, indicadores de referencia, supuestos y datos relevantes encontrados durante la investigación, sin generar tablas, gráficos, visualizaciones ni proyecciones. 

## Metadatos

| Dimensión | Detalle |
| :--- | :--- |
| **Duración** | 14 minutos |
| **Complejidad** | Media |
| **Nivel de Bloom** | Crear |

## Descripción General

En esta práctica de laboratorio, los participantes asumirán el rol de un Investigador de Estrategia Digital en Bancolombia. El objetivo es utilizar el agente especializado **Investigador** (*Researcher*) de Microsoft 365 Copilot para recopilar y sintetizar datos críticos del mercado latinoamericano y colombiano sobre la adopción de banca digital en el segmento de microempresarios. 

Para reducir la incertidumbre en la toma de decisiones ejecutivas respecto a la migración de sucursales físicas a canales digitales, se construirá un prompt de alta fidelidad aplicando la técnica de **Negative Prompting** (restricción absoluta de formatos). El agente recopilará la información y la estructurará exclusivamente en texto plano, sin tablas ni gráficos, para generar el archivo base `Reporte_Investigacion_Fintech.txt` que se utilizará de forma acumulativa en las prácticas posteriores.

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:
- **Utilizar** de manera efectiva el agente especializado 'Investigador' (Researcher) en Copilot para extraer tendencias y benchmarks del sector fintech.
- **Aplicar** técnicas avanzadas de *Negative Prompting* en un entorno ejecutivo para excluir formatos específicos (tablas, gráficos) y asegurar la entrega de un informe puramente textual.
- **Identificar y sintetizar** factores externos, indicadores de adopción y supuestos de comportamiento de clientes financieros de bajos recursos.
- **Generar y estructurar** un archivo de texto plano (`Reporte_Investigacion_Fintech.txt`) que sirva como fuente de verdad contextual para flujos de automatización posteriores.

## Prerrequisitos

- **Conocimientos Teóricos:**
  - Comprensión de la estructura de prompts corporativos (Contexto, Objetivo, Origen y Expectativas).
  - Familiaridad con el escenario estratégico de Bancolombia (migración digital de microempresarios frente a la brecha digital).
- **Acceso a Sistemas:**
  - Una cuenta activa con licencia corporativa de **Microsoft 365 Copilot Premium** con el agente "Investigador" (*Researcher*) habilitado en el inquilino (*tenant*) de la organización.
  - Conectividad a Internet activa sin bloqueos de red hacia servicios de Microsoft AI.

## Entorno de Laboratorio

### Requisitos de Hardware

| Componente | Requisito Mínimo |
| :--- | :--- |
| **Procesador** | Intel Core i5 de 64 bits (o equivalente AMD) |
| **Memoria RAM** | 8 GB o superior |
| **Resolución de Pantalla** | Mínima de 1920x1080 para visualización paralela de la guía y la consola |
| **Conexión de Red** | Banda ancha estable (mínimo 10 Mbps de subida y bajada) |

### Requisitos de Software y Licencias

| Software / Servicio | Versión Certificada | Origen / URL Oficial |
| :--- | :--- | :--- |
| **Microsoft Edge** | Versión 128.0.2739.42 (64-bit) o superior | [https://www.microsoft.com/edge](https://www.microsoft.com/edge) |
| **Microsoft 365 Copilot con Business Chat** | Service Release 2408 (Build 17928.20156) o superior | [https://copilot.microsoft.com](https://copilot.microsoft.com) |
| **Agente Investigador (Researcher)** | Integrado en Copilot Premium | Activado en la barra lateral de Agentes de Microsoft 365 |
| **Editor de Texto** | Bloc de notas (Notepad) o VS Code | Herramienta nativa del sistema operativo |

## Instrucciones Paso a Paso

### Paso 1: Acceder al Agente Investigador (Researcher) en Copilot

**Objetivo:** Inicializar la sesión de trabajo directamente en el agente especializado "Investigador" (*Researcher*) de Microsoft 365 Copilot para garantizar búsquedas externas exhaustivas y síntesis web avanzada.

1. Abre el navegador **Microsoft Edge** en tu equipo.
2. Navega al portal de chat corporativo accediendo a la URL oficial: [https://copilot.microsoft.com](https://copilot.microsoft.com) e inicia sesión con tus credenciales asignadas de Bancolombia si se te solicita. Asegúrate de estar en la pestaña de chat de **Trabajo** (*Work*).
3. En la interfaz principal de Copilot, ubica el panel lateral derecho correspondiente a **Agentes** (*Agents*) o utiliza la biblioteca de agentes del sistema.
4. Busca y haz clic sobre el agente especializado denominado **Investigador** o **Researcher** (este agente cuenta con la capacidad innata de realizar múltiples pasadas de búsqueda, sintetizar fuentes externas de confianza y estructurar respuestas complejas).

[VISUAL: Interfaz de chat de Microsoft 365 Copilot Business Chat, mostrando en el panel lateral de "Agentes" el icono activo de "Investigador" (Researcher), confirmando que las consultas se procesarán a través de este perfil especializado.]

*Resultado esperado:* La ventana del chat se actualizará mostrando un indicador o encabezado que confirma que estás interactuando activamente con el agente **Investigador (Researcher)**. El historial del hilo de conversación se iniciará limpio.

*Verificación:* Valida que en la parte superior del chat o justo arriba de la caja de prompts aparezca la etiqueta **Investigador** o **Researcher** con su correspondiente icono distintivo.

---

### Paso 2: Formular el Prompt Estructurado de Investigación (Negative Prompting)

**Objetivo:** Redactar y enviar un prompt avanzado que aplique la estructura corporativa de objetivos de negocio e incorpore *Negative Prompting* para forzar una salida estrictamente textual estructurada, evitando la generación de tablas o diagramas visuales que dificulten el procesamiento en texto plano de las siguientes prácticas.

1. Copia de forma exacta el siguiente prompt estructurado en la caja de entrada de texto del Agente Investigador:

```text
[Contexto]: Bancolombia está evaluando la viabilidad y los riesgos de migrar a su segmento de microempresarios desde el modelo tradicional de atención en sucursales físicas hacia canales 100% digitales. Identificamos fricciones severas debido a la brecha digital (analfabetismo tecnológico) y los costos de adopción (planes de datos, dispositivos móviles).

[Objetivo]: Investiga y recopila de fuentes externas fidedignas (informes del Banco Mundial, estudios de GSMA, reportes de la Superintendencia Financiera de Colombia o literatura Fintech de los últimos 2 años) tendencias del mercado financiero digital en Latinoamérica, con especial énfasis en Colombia, relativas a los microempresarios.

[Información Requerida]:
Redúceme la incertidumbre estratégica respondiendo con precisión:
1. Tendencias de adopción digital y comportamiento transaccional en microempresarios tradicionales.
2. Factores externos (sociales, económicos, cobertura de conectividad rural/urbana) que actúen como barreras y facilitadores.
3. Indicadores de referencia (benchmarks) de tasas de éxito en procesos de migración digital financiera en segmentos similares.
4. Supuestos críticos de uso que la organización debe asumir (ej. uso compartido de smartphones, dependencia del efectivo).

[Restricciones de Formato - NEGATIVE PROMPTING CRÍTICO]:
El resultado final debe presentarse EXCLUSIVAMENTE como un informe textual continuo y altamente descriptivo, organizado jerárquicamente con títulos y párrafos detallados.
- NO generes tablas de datos bajo ninguna circunstancia.
- NO utilices gráficos, diagramas de flujo de caracteres ni representaciones visuales.
- NO uses listas de cotejo vacías o viñetas que solo presenten números sin desarrollo narrativo de los mismos.
- Cualquier indicador numérico o métrica debe estar redactado de manera fluida y explicativa dentro del cuerpo de los párrafos.
```

2. Haz clic en el botón de **Enviar** (icono de avión de papel) o presiona `Enter`.
3. Espera a que el Agente Investigador complete sus ciclos de búsqueda en la web y compile el informe definitivo. (Este proceso puede tardar unos segundos adicionales debido al análisis profundo de fuentes que realiza el agente).

*Resultado esperado:* El Agente Investigador devolverá un texto de alta calidad técnica estructurado únicamente con títulos (Markdown `#`, `##`), párrafos bien articulados y citas contextuales embebidas en el texto. No debe mostrarse ninguna estructura de tabla de Markdown (caracteres `|` o `--`).

*Verificación:* Revisa minuciosamente el texto generado en pantalla para asegurar que no se haya filtrado ninguna tabla o gráfico. Confirma que se listen de manera descriptiva las tendencias de Latinoamérica/Colombia, los factores externos, los indicadores de adopción y los supuestos de smartphones de manera fluida.

---

### Paso 3: Guardar el Reporte como Archivo de Trabajo

**Objetivo:** Consolidar el resultado en el sistema de archivos local utilizando el nombre de archivo estándar de trabajo para garantizar la persistencia de los datos en las prácticas posteriores.

1. Desplázate al inicio de la respuesta proporcionada por el Copilot Researcher.
2. Haz clic sobre el botón de **Copiar** situado en la base del bloque de respuesta de Copilot, o selecciona manualmente todo el texto generado desde el título inicial hasta el párrafo final.
3. En tu sistema operativo local, abre el **Bloc de notas** (*Notepad.exe*) o tu editor de texto plano favorito (como VS Code).
4. Pega el texto copiado mediante la combinación de teclas `Ctrl + V` (Windows) o `Cmd + V` (macOS).
5. Guarda el archivo con el siguiente nombre exacto dentro de tu directorio de trabajo del taller:
   - Nombre: `Reporte_Investigacion_Fintech.txt`
6. Cierra el editor de texto.

*Resultado esperado:* Creación física de un archivo de texto plano `.txt` que contiene la síntesis de investigación rica en contexto e indicadores cualitativos y cuantitativos narrados, libre de formato tabular.

*Verificación:* Navega a través del explorador de archivos local hasta la ubicación donde guardaste el archivo. Haz doble clic en `Reporte_Investigacion_Fintech.txt` y valida que el contenido se visualice de manera legible y estructurada, con un tamaño de archivo superior a 2 KB (lo que indica un reporte robusto y detallado).

---

## Validación y Pruebas

Para garantizar que los resultados de esta práctica cumplen con los estándares corporativos rigurosos, ejecuta los siguientes pasos de control de calidad:

### Evaluación del Contenido y Cumplimiento de Reglas
Abre tu archivo `Reporte_Investigacion_Fintech.txt` y verifica que cumpla con los siguientes criterios cualitativos:
- **Ausencia de Tablas:** El archivo no contiene caracteres divisores de tabla (`|` o similar). Si detectas una sola celda o fila estructurada como tabla, el resultado no cumple la restricción de Negative Prompting.
- **Métricas Embebidas:** Las métricas encontradas (por ejemplo, penetración de smartphones en Colombia o porcentaje de uso de efectivo en comercios pequeños) están explicadas narrativamente (Ejemplo correcto: *"Aproximadamente el sesenta por ciento de los comercios sigue operando de forma prioritaria con dinero en efectivo..."*).
- **Consistencia de Escenario:** El reporte describe la situación de microempresarios de escala similar a los de Bancolombia, abordando de manera directa la brecha digital y la infraestructura de conectividad móvil en la región.

### Caso de Prueba Adversario (Adversarial Testing)
Para evaluar la resistencia del agente y la correcta aplicación de instrucciones por parte del alumno, realiza el siguiente ejercicio rápido utilizando la misma sesión activa:

1. Escribe en el chat con el Agente Investigador el siguiente prompt conflictivo:
   ```text
   Resume las tendencias que encontraste anteriormente y colócalas en una tabla comparativa de 3 columnas para facilitar una presentación rápida a la gerencia.
   ```
2. **Resultado Esperado del Test Adversario:** Dado que este prompt viola deliberadamente la restricción de diseño original (que exige que toda la información se mantenga puramente en texto sin tablas para los laboratorios subsiguientes), el estudiante deberá observar cómo el agente genera la tabla. 
3. **Acción de Mitigación del Estudiante:** Inmediatamente después de observar la tabla, ingresa el siguiente prompt de corrección para restaurar el formato de datos requerido:
   ```text
   No está permitido el uso de tablas para este pipeline de datos. Reescribe ese último resumen convirtiendo cada fila de la tabla en un párrafo descriptivo independiente. Asegúrate de eliminar la tabla.
   ```
4. **Verificación final:** Valida que el agente haya eliminado la estructura tabular antes de continuar.

---

## Solución de Problemas

A continuación se describen los dos incidentes más comunes que pueden ocurrir durante el desarrollo de esta práctica de laboratorio, junto con sus causas raíz y soluciones paso a paso:

### Incidente 1: El Agente "Investigador" (Researcher) no está visible en el tenant de la organización o está deshabilitado por políticas de TI

- **Síntoma:** No encuentras la opción de seleccionar el agente "Investigador" o "Researcher" en la barra lateral de Copilot ni en la biblioteca de agentes corporativa de Bancolombia.
- **Causa Raíz:** Restricciones de licenciamiento temporal, políticas estrictas de seguridad de la información aplicadas al subconjunto de agentes, o retraso en la propagación de actualizaciones del inquilino (*tenant*) de Microsoft 365.
- **Solución:**
  1. En lugar de usar el agente especializado, utiliza el chat principal de **Microsoft 365 Copilot (Business Chat)** en el modo de trabajo.
  2. Asegúrate de que el selector de "Web" esté activado (para habilitar búsquedas en tiempo real).
  3. Modifica la primera línea de tu prompt agregando un sistema de instrucción explícito: 
     `"Actúa como un agente de investigación web senior. Realiza múltiples búsquedas profundas en internet..."`. Esto emulará las capacidades de recolección de información del agente especializado.

### Incidente 2: El reporte generado incluye tablas o listas con formatos de cuadrícula, violando la regla de Negative Prompting

- **Síntoma:** El reporte de salida de Copilot despliega una tabla de markdown o un formato de rejilla con líneas divisorias verticales u horizontales.
- **Causa Raíz:** El Modelo de Lenguaje Grande (LLM) priorizó la legibilidad visual estándar sobre la instrucción negativa debido a la sobrecarga de contexto en el prompt o la falta de peso asignado a las restricciones.
- **Solución:**
  1. No copies ese resultado. En la misma caja de conversación, introduce la siguiente instrucción de refinamiento:
     `"Tu respuesta anterior violó la regla de exclusión. Convierte inmediatamente todas las tablas y elementos gráficos de tu respuesta previa en párrafos descriptivos completos. NO uses formato de tabla de Markdown."`
  2. Una vez corregido el texto y comprobado que solo contiene prosa estructurada por títulos, procede con el guardado en el archivo `Reporte_Investigacion_Fintech.txt`.

---

## Limpieza

1. **Guardado Seguro:** Asegúrate de que el archivo `Reporte_Investigacion_Fintech.txt` esté guardado correctamente en tu disco local. Este archivo será la entrada fundamental para los flujos de trabajo de las Prácticas 8 y 9.
2. **Preservación del Contexto (Thread Continuity):** **NO cierres ni borres** el hilo de chat actual de Microsoft 365 Copilot en tu navegador Edge. Los próximos laboratorios requieren mantener esta misma conversación abierta para conservar el contexto histórico y la memoria del escenario acumulada por la IA.
3. Cierra únicamente las pestañas auxiliares que no utilices y el Bloc de Notas una vez hayas confirmado que los datos se guardaron correctamente.

---

## Resumen

En esta práctica, has aprendido a utilizar el agente especializado **Investigador** (Researcher) de Microsoft 365 Copilot para recopilar datos del entorno fintech de forma segura y gobernada. 

Has dominado la técnica de **Negative Prompting**, una habilidad avanzada de ingeniería de prompts que te permite limitar de manera estricta los formatos de salida generados por los modelos de IA. Esta técnica es fundamental en entornos corporativos donde la salida de una fase de automatización (en este caso, la investigación de campo en formato de texto plano) actúa directamente como el insumo de análisis o programación para las fases posteriores del proyecto (Prácticas 8, 9 y 10), garantizando la compatibilidad absoluta y la eliminación de ruidos en la transmisión de datos semánticos.
