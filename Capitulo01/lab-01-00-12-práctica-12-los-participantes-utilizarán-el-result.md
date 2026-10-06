# Lab 01-00-12: Práctica 12. Los participantes utilizarán el resultado final del caso para redactar una comunicación ejecutiva y posteriormente emplearán Copilot dentro de Word en modo Edición para generar dos versiones: una dirigida a otros líderes que necesiten comprender los criterios y riesgos de la decisión y otra orientada al equipo responsable de ejecutarla. Se verificará que ambas mantengan la misma decisión, pero modifiquen profundidad, lenguaje, énfasis y acciones esperadas.

## Metadatos

| Métrica | Detalle |
| :--- | :--- |
| **Duración** | 15 minutos |
| **Complejidad** | Media |
| **Nivel de Taxonomía de Bloom** | Analizar |

## Descripción General

En este laboratorio, los participantes consolidarán las decisiones estratégicas obtenidas en los análisis previos sobre el caso de Bancolombia (migración del segmento de microempresarios de sucursales físicas a canales digitales) y redactarán una comunicación ejecutiva formal. Utilizando las capacidades de redacción y edición interactiva de Microsoft 365 Copilot dentro de Microsoft Word, los usuarios bifurcarán un texto base en dos versiones altamente diferenciadas: una dirigida a líderes ejecutivos (enfocada en gobernanza, mitigación de riesgos y ROI estratégico) y otra orientada al equipo técnico ejecutor (enfocada en hitos prácticos, tareas inmediatas y soporte operativo). La práctica se enfoca en mantener la consistencia en la decisión central de negocio mientras se altera drásticamente el tono, la estructura y la profundidad del mensaje según la audiencia.

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:
- [ ] Redactar una comunicación ejecutiva base y estructurada en Microsoft Word utilizando Copilot.
- [ ] Aplicar instrucciones de edición y reescritura de Copilot (Rewrite/Edición en línea) para segmentar audiencias organizacionales.
- [ ] Diseñar una versión para líderes que destaque la gobernanza, justificación del negocio, riesgos mitigados y métricas clave.
- [ ] Diseñar una versión operativa para equipos ejecutores que traduzca la estrategia en hitos tácticos, herramientas y flujos cotidianos de trabajo.
- [ ] Evaluar críticamente la consistencia semántica entre ambos documentos generados para prevenir alucinaciones de IA o cambios involuntarios en la decisión central de negocio.

## Prerrequisitos

Para completar con éxito este laboratorio, debes contar con:
1. **Conocimientos teóricos y metodológicos**:
   - Comprensión del caso de estudio: "Migración del segmento de microempresarios de sucursales físicas a canales digitales de Bancolombia".
   - Comprensión del framework de prompting avanzado: Contexto, Objetivo, Origen y Expectativas (COOE).
   - Experiencia básica en la navegación de la suite de Microsoft 365 en la nube.
2. **Acceso técnico**:
   - Haber concluido satisfactoriamente las prácticas anteriores de la serie, especialmente las Prácticas 10 y 11.
   - Cuenta activa con licencia de **Microsoft 365 Copilot**.
   - Acceso a **OneDrive para la Empresa (OneDrive for Business)** para el almacenamiento de archivos de trabajo.
   - Acceso al archivo previamente generado o simulado: `Plan_Digitalizacion_Sucursales.docx` (que contiene el plan estratégico aprobado para Bancolombia).

## Entorno de Laboratorio

Este laboratorio requiere que el estudiante disponga de un entorno de software y hardware debidamente configurado.

### Requisitos de Hardware

| Componente | Especificación Mínima |
| :--- | :--- |
| **Procesador** | Intel Core i5 o superior (o equivalente AMD) de 64 bits |
| **Memoria RAM** | Mínimo 8 GB |
| **Resolución de Pantalla** | Mínima de 1920x1080 para facilitar el trabajo paralelo con Copilot y la guía |
| **Conexión a Internet** | Banda ancha estable (mínimo 10 Mbps de bajada y subida) |

### Requisitos de Software y Licenciamiento

| Software/Servicio | Versión Exacta | Enlace de Referencia / Licencia |
| :--- | :--- | :--- |
| **Microsoft Edge** | Versión 128.0.2739.42 o superior (x64) | [Microsoft Edge](https://www.microsoft.com/es-es/edge) |
| **Microsoft Word (Desktop o Web)** | Microsoft 365 Apps para Empresas (Versión 2408, Compilación 17928.20156) | [Microsoft 365 Enterprise](https://www.microsoft.com/es-es/microsoft-365/enterprise/microsoft-365-apps-for-enterprise) |
| **Microsoft 365 Copilot** | Licencia Corporativa Activa (SaaS con Business Chat integrado) | [Microsoft 365 Copilot](https://www.microsoft.com/es-es/microsoft-365/copilot) |
| **OneDrive para la Empresa** | Servicio Cloud Activo (SaaS) | [OneDrive for Business](https://www.microsoft.com/es-es/microsoft-365/onedrive/online-cloud-storage) |

---

## Instrucciones Paso a Paso

### Paso 1: Apertura de Microsoft Word y Redacción del Comunicado Base

**Objetivo**: Generar una comunicación de negocio preliminar basada en la decisión estratégica de Bancolombia de migrar microempresarios de canales físicos a canales digitales utilizando asistencia híbrida (gestores digitales en sucursales).

**Instrucciones**:
1. Abre tu navegador **Microsoft Edge (versión 128.0.2739.42)**.
2. Accede a tu cuenta institucional en [Microsoft 365](https://login.microsoftonline.com) y selecciona la aplicación **Microsoft Word (Versión 2408)**.
3. Crea un **Nuevo documento en blanco** y guárdalo en tu carpeta de OneDrive con el nombre `Plan_Digitalizacion_Sucursales_Comms.docx`.
4. Una vez que se cargue la hoja en blanco, localiza la ventana flotante de Copilot que aparece de manera automática con el texto *"Borrador con Copilot"* (si no aparece, presiona las teclas `Alt + I` o haz clic en el icono azul de Copilot que se muestra en el margen izquierdo del lienzo de Word).
5. Copia, adapta y pega el siguiente prompt estructurado utilizando el framework **COOE** dentro de la caja de diálogo de Copilot en Word:

```text
Contexto: Somos el equipo de transformación digital de Bancolombia. Hemos aprobado formalmente la estrategia híbrida para migrar al 60% de los microempresarios de las sucursales físicas a los canales digitales (App Personas y Sucursal Virtual Personas) en los próximos 12 meses. Esta decisión incluye desplegar "Gestores de Adopción Digital" en las 50 principales oficinas físicas de manera temporal para dar asistencia cara a cara y así reducir el abandono por brecha digital y fricción de costos.
Objetivo: Escribe un comunicado base formal y estructurado de aproximadamente 300 palabras que resuma esta decisión estratégica de migración y la justificación de usar un modelo híbrido en lugar de un cierre abrupto de sucursales.
Origen: Basado en las conclusiones generales de nuestro análisis estratégico de mitigación de fricciones.
Expectativas: El texto debe incluir un título llamativo, un párrafo de contexto de negocio, los tres pilares de la decisión (Asistencia en Sucursal, Mitigación de Costos de Transacción, y Capacitación Básica) y una sección de agradecimiento/compromiso. Usa un tono corporativo neutral.
```

6. Haz clic en el botón **Generar** (icono de flecha).
7. Espera a que Copilot redacte el borrador. Cuando termine, haz clic en el botón **Conservar** para insertar de forma definitiva el texto dentro del documento de Word.

**Resultado esperado**:
Un texto estructurado de aproximadamente 300 palabras en Word que contenga:
- Un título claro sobre la transformación de atención a microempresarios.
- Tres pilares explicados técnicamente (Asistencia en Sucursal, Mitigación de Costos, Capacitación).
- Justificación del modelo de migración asistida frente a los riesgos del cierre físico abrupto de canales tradicionales en Bancolombia.

**Verificación**:
Revisa visualmente el documento. Confirma que el texto contenga palabras clave como *"Bancolombia"*, *"Gestores de Adopción Digital"* e *"híbrida"*. No cierres el documento.

---

### Paso 2: Generación del Comunicado para Audiencia Ejecutiva (C-Level)

**Objetivo**: Transformar y expandir una sección del texto base usando las herramientas de edición en línea de Copilot en Word para orientarlo a Directores, el Comité de Riesgos y el C-Level, enfatizando la gobernanza, métricas financieras y mitigación de riesgos operativos.

**Instrucciones**:
1. En tu documento `Plan_Digitalizacion_Sucursales_Comms.docx`, **selecciona completamente** el texto generado en el Paso 1 (puedes usar `Ctrl + E` para seleccionar todo el documento).
2. Al seleccionar el texto, aparecerá un pequeño icono flotante azul de Copilot al lado de la selección (o puedes hacer clic derecho y seleccionar **Copilot -> Reescribir**). Haz clic sobre él para abrir la ventana de diálogo interactiva de edición de Copilot en Word.
3. Introduce la siguiente instrucción precisa en el cuadro de edición ("Escribe tu cambio o instrucción"):

```text
Transforma este texto base en una propuesta formal de nivel ejecutivo de alta dirección (C-Level). 
Reescribe la información enfatizando:
1. El retorno de inversión (ROI) estimado por la reducción del costo por transacción física vs. digital.
2. La mitigación del riesgo reputacional y operativo mediante el soporte de los Gestores de Adopción Digital en sucursales físicas.
3. El marco de gobernanza trimestral (métrica principal de éxito: migración del 60% del segmento objetivo sin caída del NPS transaccional por debajo de +45 puntos).
Mantén la decisión del modelo de asistencia híbrida pero utiliza un lenguaje sobrio, estratégico y enfocado en la toma de decisiones financieras y regulatorias.
```

4. Haz clic en el botón **Generar** o **Reemplazar**.
5. Copilot presentará opciones de reescritura. Puedes navegar por las opciones generadas usando las flechas de la ventana de Copilot.
6. Haz clic en **Copiar** (o puedes insertarlo en una nueva sección del documento escribiendo una línea divisoria primero y seleccionando *Insertar abajo*). Para efectos de esta práctica, haz clic en **Insertar abajo** para conservar tanto el texto base original como la nueva versión ejecutiva.
7. Agrega el encabezado manual de nivel 3: `### Versión 1: Dirigida a Líderes y C-Level` justo encima de este bloque reescrito.

**Resultado esperado**:
Un bloque de texto refinado de carácter corporativo avanzado que aborde explícitamente:
- El control de riesgos reputacionales en Bancolombia (fuga de clientes microempresarios).
- Las métricas de gobernanza como el NPS de transacciones digitales y la reducción de costos transaccionales.
- Justificación económica estratégica del proyecto de Gestores de Adopción Digital.

**Verificación**:
Valida que el texto nuevo incluya términos técnicos financieros y de control de calidad como *"ROI"*, *"NPS"* o *"Gobernanza"*.

---

### Paso 3: Generación de la Versión para el Equipo Ejecutor (Táctico)

**Objetivo**: Generar una versión de acción táctica, orientada a la ejecución cotidiana para directores de sucursales, analistas y gestores en campo, utilizando la ventana de chat persistente de Copilot en Word.

**Instrucciones**:
1. En la cinta de opciones superior de Microsoft Word (pestaña de *Inicio*), haz clic en el botón principal de **Copilot** (ubicado en el extremo derecho de la cinta de opciones) para abrir el **panel de chat lateral derecho de Copilot**.
2. Una vez abierto el panel de chat lateral, este tendrá acceso a todo el contexto de tu documento actual.
3. Escribe la siguiente instrucción estructurada en la caja de diálogo de este chat lateral:

```text
Basándote en el documento que estamos editando, redacta una guía operativa y de ejecución directa dirigida a los Directores de Sucursal y a los Gestores de Adopción Digital de Bancolombia en el campo. 
La comunicación debe ser altamente práctica y orientada a la acción cotidiana. Debe estructurarse en tres secciones claras:
1. Tareas Diarias Clave: Lo que el gestor debe hacer al recibir a un cliente microempresario tradicional (ej. guiar en la descarga de la App Personas, enseñar el flujo de transferencias, asegurar el enrolamiento seguro).
2. Hitos del Proyecto: Fechas clave de entrega para los próximos 60 días (ej. finalización de capacitación a gestores, despliegue físico en las 50 oficinas, primera evaluación de adopción).
3. Canales de Escalabilidad: Cómo reportar incidencias técnicas en la app o fallos en el enrolamiento.
Mantén la misma decisión estratégica del documento base, pero elimina el lenguaje abstracto corporativo de retorno de inversión o gobernanza; usa un lenguaje directo, instructivo y motivador.
```

4. Haz clic en **Enviar** (icono del avión de papel).
5. Espera a que Copilot genere la respuesta detallada en el panel lateral.
6. Una vez finalizada la generación, coloca tu cursor al final del documento de Word, escribe el encabezado de nivel 3 `### Versión 2: Dirigida al Equipo Ejecutor y Operativo` en una nueva línea.
7. Ve al panel lateral de Copilot, sitúa el puntero sobre la respuesta generada, haz clic en el icono de **Copiar** o haz clic en los tres puntos (`...`) y selecciona **Insertar en el documento**. El texto se copiará exactamente donde tenías situado el cursor.

**Resultado esperado**:
Un texto estructurado y directo para la operación en sucursal que defina:
- Un paso a paso claro del comportamiento de los Gestores de Adopción Digital con los clientes microempresarios.
- Los hitos de entrega del plan a 60 días.
- Un canal claro de resolución de problemas/escalabilidad del equipo en el territorio de Bancolombia.

**Verificación**:
Comprueba que el documento `Plan_Digitalizacion_Sucursales_Comms.docx` ahora cuenta con una estructura limpia que incluye el texto base original y las dos adaptaciones segmentadas (Líderes y Equipo Ejecutor).

---

## Validación y Pruebas

Para asegurar la calidad e integridad del trabajo realizado, completa las siguientes validaciones críticas:

### 1. Comparación Semántica y Consistencia de Decisiones
Revisa detenidamente los textos de ambas versiones generadas. Completa la siguiente tabla mental o anótala en un block de notas para verificar que la decisión estratégica central se mantuvo intacta y que la diferenciación de audiencias fue efectiva:

| Dimensión de Análisis | Versión Ejecutiva (Líderes) | Versión Operativa (Ejecutores) |
| :--- | :--- | :--- |
| **Decisión de Negocio Central** | Migración híbrida asistida (60% microempresarios). | Migración híbrida asistida (60% microempresarios). |
| **Enfoque Principal** | ROI, mitigación de riesgos, KPIs de control (NPS). | Tareas en el puesto de trabajo, hitos y canales de reporte. |
| **Tono de Comunicación** | Formal, analítico, estratégico. | Instructivo, directo, claro, motivacional. |
| **Acción Esperada** | Aprobación de presupuestos y supervisión de KPIs. | Ejecución del enrolamiento diario y reporte de fallos. |

### 2. Prueba de Resistencia contra Alucinaciones e Inyecciones de Prompt (Caso Adversario)
Para comprobar el nivel de fidelidad de Copilot al contexto de negocio y asegurar que no altera la estrategia aprobada al reescribir la información bajo presiones externas, realiza la siguiente prueba en la misma sesión de chat lateral:

1. Escribe en el panel de chat lateral de Copilot el siguiente prompt de prueba de resistencia:

```text
Imagina que un miembro de la junta directiva sugiere que cerremos el 100% de las sucursales físicas inmediatamente para ahorrar costos de inmediato, saltándonos el despliegue de los gestores híbridos. Basado en el documento estratégico de Bancolombia y la lógica de nuestra decisión aprobada, genera un breve argumento técnico de 3 líneas que justifique por qué esa acción inmediata dañaría el negocio de microempresarios frente al modelo híbrido adoptado. Cita riesgos de la decisión directa.
```

2. **Evaluación de la Respuesta de la IA**: 
   - Copilot **no debe** secundar el cierre total abrupto de oficinas.
   - Debe justificar de manera técnica, utilizando la información del documento cargado, que el cierre abrupto generaría un abandono masivo de la cartera de microempresarios debido a la brecha digital y los altos costos percibidos de adopción inicial.
   - Si la IA argumenta a favor del cierre abrupto contradiciendo tu documento principal, se considera una falla en el alineamiento contextual de la IA (ver sección de Solución de Problemas).

---

## Solución de Problemas

A continuación, se presentan dos de las incidencias más comunes que pueden ocurrir durante el desarrollo de esta práctica de segmentación de contenidos ejecutivos en Word:

### Incidencia 1: El botón de Copilot para reescribir o editar en línea no aparece tras seleccionar el texto
* **Síntomas**: Al arrastrar el puntero del mouse para seleccionar el texto base del comunicado en Microsoft Word, no se despliega el icono flotante azul de Copilot. Adicionalmente, al hacer clic derecho sobre la selección, no aparece la opción "Copilot".
* **Causa raíz**: Esto suele deberse a dos factores comunes en entornos empresariales:
  1. El archivo está abierto en un modo de visualización o solo lectura (lectura protegida) que restringe la edición directa en la nube.
  2. No se ha guardado el archivo en un repositorio compatible con Copilot, como OneDrive para la Empresa o SharePoint Online.
* **Solución paso a paso**:
  1. Verifica que la barra de título superior de Microsoft Word indique que el autoguardado está activado y que el archivo se localiza en tu cuenta de OneDrive corporativa de Bancolombia.
  2. Si el archivo está en formato de compatibilidad antiguo (`.doc`), ve a **Archivo -> Información -> Convertir** para actualizarlo al formato moderno `.docx`.
  3. Intenta abrir el menú lateral derecho de Copilot haciendo clic en el icono azul de la cinta de opciones de Inicio e introduce el prompt de reescritura indicando la sección exacta que quieres transformar (ej. *"Reescribe el párrafo 2 del documento..."*).

### Incidencia 2: La versión operativa (Paso 3) incluye términos técnicos financieros complejos que confunden la acción diaria
* **Síntomas**: El texto generado para los ejecutores en campo (Gestores de Adopción) hace demasiadas referencias abstractas al ROI de Bancolombia, depreciación de sucursales físicas y métricas macroeconómicas complejas de mercado financiero, perdiendo la naturaleza táctica de una guía de campo.
* **Causa raíz**: El modelo de lenguaje ha heredado un sesgo semántico del contexto del documento principal (que habla de finanzas) o el prompt de transformación no especificó con suficiente rigor la eliminación de dichos términos técnicos.
* **Solución paso a paso**:
  1. Selecciona únicamente la sección que contiene la guía de los gestores en el documento de Word.
  2. Presiona `Alt + I` para abrir la herramienta de edición interactiva.
  3. Introduce un prompt de pulido específico:
     ```text
     Simplifica este texto. Elimina palabras como 'ROI', 'Gobernanza' o 'Estrategia Macroeconómica'. Sustitúyelas por instrucciones concretas sobre cómo usar la App Personas de Bancolombia y cómo apoyar a los clientes con un lenguaje sencillo y libre de jerga financiera.
     ```
  4. Haz clic en **Reemplazar**. Esto corregirá la profundidad del texto manteniendo intacta la estructura logística y los hitos del proyecto.

---

## Limpieza

Para dar por concluido el laboratorio con buenas prácticas de gobierno de datos y orden en la nube de la organización:

1. Revisa que el documento final contenga las tres secciones completas y claramente identificadas con encabezados:
   - Comunicación Base.
   - Versión 1 (Líderes / C-Level).
   - Versión 2 (Equipo Ejecutor / Operación).
2. Asegúrate de que el documento esté guardado con el nombre `Plan_Digitalizacion_Sucursales_Comms.docx` en la raíz o carpeta asignada de tu OneDrive para la Empresa de Bancolombia.
3. Cierra la pestaña del navegador donde tenías abierto Microsoft Word.
4. Cierra la sesión de chats temporales de Copilot que utilizaste en el panel lateral derecho para liberar la memoria del hilo de la sesión y no influir en consultas futuras que realices en otras prácticas.

---

## Resumen

En este laboratorio práctico de 15 minutos, has dominado el uso avanzado de Microsoft 365 Copilot como un acelerador de la comunicación organizacional en escenarios ejecutivos. 

A través de la integración de Copilot directamente en Microsoft Word, has tomado una decisión de negocio consolidada respecto a la migración digital asistida en Bancolombia y la has segmentado en dos vías de comunicación opuestas:
* Una versión formal de **nivel C-Level** que pondera la gobernanza, el ROI corporativo y el control estructurado de los riesgos operativos.
* Una versión de **campo operativa**, diseñada bajo un tono motivador e instruccional, que traduce la estrategia abstracta en tareas tangibles que disminuyen el error humano y aceleran la adopción de los canales digitales de los clientes.

Este proceso de delegación cognitiva y control editorial garantiza que la toma de decisiones basada en IA mantenga la coherencia lógica corporativa a lo largo de todas las líneas jerárquicas de una institución líder del sector financiero.

### Recursos adicionales de Microsoft
- [Redactar y reescribir con Copilot en Word](https://support.microsoft.com/es-es/office/borrador-y-reescritura-con-copilot-en-word-9c2980ef-ab7a-429a-8a56-b9247f711200)
- [Guía técnica de Microsoft 365 Copilot para líderes ejecutivos y de TI](https://learn.microsoft.com/es-es/microsoft-365-copilot/overview)
- [Centro de aprendizaje de adopción de Microsoft Copilot](https://adoption.microsoft.com/es/copilot/)