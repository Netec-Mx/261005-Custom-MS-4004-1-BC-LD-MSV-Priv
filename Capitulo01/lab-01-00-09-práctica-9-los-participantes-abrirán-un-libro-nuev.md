# Práctica 9: Los participantes abrirán un libro nuevo de Excel y utilizarán el informe textual obtenido con Investigador como contexto para solicitar a Copilot, mediante el modo Plan, la creación de un plan de acción para responder a la situación analizada. Copilot deberá transformar los hallazgos de la investigación en una estructura que organice iniciativas, prioridades, responsables, horizonte de ejecución, indicadores de seguimiento, riesgos y criterios para revisar la decisión. Los participantes revisarán el plan generado y los pasos realizados por Copilot. 

## Metadatos

| Dimensión | Detalle |
| :--- | :--- |
| **Duración** | 8 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Crear |

## Descripción General

En este laboratorio, los participantes aprenderán a utilizar **Microsoft 365 Copilot en Excel** para transformar hallazgos de investigación cualitativa en un plan de acción estratégico estructurado. Utilizando los datos de análisis obtenidos en las fases de investigación previas sobre la migración digital de microempresarios en Bancolombia, se guiará al participante en la inicialización de un nuevo libro de cálculo, la estructuración de una tabla de datos oficial y la invocación de Copilot para automatizar la creación de iniciativas, asignación de prioridades, responsables de alto nivel, horizontes de tiempo, indicadores clave de rendimiento (KPIs), riesgos asociados y criterios de revisión estratégica.

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:
- [ ] Inicializar un nuevo libro de trabajo de Microsoft Excel y habilitar el panel de asistencia de Copilot bajo un entorno corporativo con licencias activas.
- [ ] Estructurar una tabla de datos inicial y convertirla al formato de "Tabla de Excel" requerido para la correcta interpretación del motor de inteligencia artificial.
- [ ] Formular prompts avanzados utilizando la estructura de Contexto, Objetivo, Origen y Expectativas (COOE) para delegar la creación de planes estructurados.
- [ ] Aplicar el análisis crítico para revisar e inspeccionar las iniciativas de negocio sugeridas por Copilot en el contexto de la brecha digital financiera.

## Prerrequisitos

Para realizar este laboratorio de forma exitosa, el usuario debe contar con:
- **Conocimientos teóricos previos**: Familiaridad con el flujo de trabajo de la suite de Microsoft 365, el concepto de Generación Aumentada por Recuperación (RAG) y los fundamentos de la migración de canales físicos a digitales en el sector bancario.
- **Acceso a Sistemas**: 
  - Una cuenta activa de Microsoft 365 con suscripción que incluya **Microsoft 365 Copilot** (Licencia Enterprise o Business).
  - Un navegador web compatible (Microsoft Edge versión 128 o superior) o la aplicación de escritorio de Excel debidamente sincronizada con una cuenta de almacenamiento en la nube (OneDrive o SharePoint).

## Entorno de Laboratorio

Este laboratorio se realiza de manera nativa en la nube o mediante la aplicación cliente de escritorio de Microsoft Excel.

### Requisitos de Software y Plataforma

| Componente / Herramienta | Versión / Edición de Referencia | Enlace Oficial / Origen |
| :--- | :--- | :--- |
| **Microsoft Excel para Microsoft 365** | Versión 2408 (Compilación 17928.20156) de 64 bits | [Enlace Oficial de Excel](https://www.microsoft.com/es-ww/microsoft-365/excel) |
| **Microsoft 365 Copilot Premium** | Canal Corporativo (Servicio Cloud SaaS Activo) | [Enlace Oficial de Copilot](https://learn.microsoft.com/es-es/microsoft-365-copilot/) |
| **Microsoft Edge** | Versión 128.0.2739.42 (64-bit) o superior | [Enlace Oficial de Edge](https://www.microsoft.com/es-es/edge) |

### Archivos de Entrada e Información de Contexto (Mock Data)

Para asegurar la continuidad del hilo de la sesión de manera autocontenida y evitar dependencias de red o de archivos perdidos, utilizaremos el siguiente bloque consolidado que simula el resultado del `Reporte_Investigacion_Fintech.txt` obtenido previamente:

```text
CONCEPTO DE ENTRADA (Contexto de Negocio):
- Organización: Bancolombia S.A.
- Escenario: Migración del segmento de microempresarios de sucursales físicas a canales digitales.
- Desafíos: Alta fricción por brecha digital, resistencia al cambio tecnológico, analfabetismo financiero y costos de conectividad/adopción de terminales de pago.
- Hipótesis Validadas:
  1. El 60% de los microempresarios prefiere efectivo por desconocimiento de tarifas transaccionales.
  2. La asistencia telefónica no es suficiente; se requiere mentoría y acompañamiento físico-virtual híbrido.
  3. Reducir el cobro de comisiones iniciales digitaliza un 35% más rápido a comercios minoristas tradicionales.
```

---

## Instrucciones Paso a Paso

A continuación, se describen los pasos necesarios para construir el plan de acción estratégico utilizando Copilot en Excel.

### Paso 1: Inicialización del Entorno y Preparación de Datos

**Objetivo**: Abrir un nuevo libro de trabajo, guardarlo en una ubicación en la nube y preparar la hoja de cálculo para activar las funciones de Copilot.

**Instrucciones**:

1. Abre tu navegador **Microsoft Edge** y accede al portal de Microsoft 365 (`portal.office.com`) o abre directamente la aplicación de escritorio de **Microsoft Excel** con tu sesión corporativa iniciada.
2. Crea un **Nuevo libro en blanco**.
3. Es **mandatorio** guardar el archivo en la nube para habilitar Copilot. Ve a **Archivo** > **Guardar como** y selecciona tu **OneDrive de Bancolombia (o cuenta corporativa/educativa)**.
4. Nombra el archivo exactamente como: `Plan_Accion_Bancolombia.xlsx` y haz clic en **Guardar**.
5. Confirma que la función **AutoGuardado** (esquina superior izquierda de la pantalla) se encuentra en estado **Activado** (On).

[VISUAL: Captura de pantalla conceptual de la interfaz de Microsoft Excel mostrando el interruptor de AutoGuardado en verde (activo) en la barra de herramientas superior].

**Resultado esperado**: Un libro de Excel vacío guardado en OneDrive/SharePoint con el nombre `Plan_Accion_Bancolombia.xlsx` y el icono de autoguardado en estado activo.

---

### Paso 2: Creación de la Estructura de Tabla Inicial

**Objetivo**: Definir una estructura tabular mínima con formato de tabla nativa de Excel, la cual es un requisito indispensable para que Copilot en Excel procese la información.

**Instrucciones**:

1. Haz clic en la celda **A1** y escribe el encabezado: `Iniciativa`.
2. Completa los encabezados de las columnas adyacentes escribiendo los siguientes nombres en la fila 1 (desde la celda **B1** hasta **G1**):
   - Celda **B1**: `Prioridad`
   - Celda **C1**: `Responsable`
   - Celda **D1**: `Horizonte`
   - Celda **E1**: `KPI`
   - Celda **F1**: `Riesgo`
   - Celda **G1**: `Criterio de Revision`
3. En la celda **A2**, escribe un registro semilla ficticio para inicializar la tabla de forma correcta:
   - Celda **A2**: `Diseño de pilotos de mentoría híbrida`
   - Celda **B2**: `Alta`
   - Celda **C2**: `Gerencia de Canales`
   - Celda **D2**: `Q1`
   - Celda **E2**: `Número de comercios capacitados`
   - Celda **F2**: `Baja asistencia presencial`
   - Celda **G2**: `Costo de adquisición de clientes < $10 USD`
4. Selecciona el rango completo que acabas de escribir: **A1:G2**.
5. En la pestaña **Inicio**, haz clic en el botón **Dar formato como tabla** dentro del grupo *Estilos*. Selecciona cualquier estilo de tabla (por ejemplo, *Azul, Estilo de tabla medio 2*).
6. En el cuadro de diálogo que se muestra, asegúrate de activar la opción **"La tabla tiene encabezados"** y presiona **Aceptar**.
7. Opcional pero recomendado: En la barra de pestañas que se activa llamada "Diseño de tabla", cambia el nombre de la tabla de `Tabla1` a `PlanEstrateco` en el cuadro de texto *Nombre de la tabla* (esquina superior izquierda).

[VISUAL: Diagrama del diseño de la tabla en Excel con el rango seleccionado A1:G2 y el cuadro emergente "Dar formato como tabla" con la opción de encabezados marcada].

**Resultado esperado**: Una tabla formal de Excel con 7 columnas y 1 fila de datos, con formato visual de color aplicado y guardada de forma automática en la nube.

---

### Paso 3: Ejecución del Prompt en Copilot para Completar el Plan

**Objetivo**: Utilizar el panel de Copilot en Excel aplicando un prompt estructurado de alta fidelidad para que el modelo de lenguaje genere nuevas filas de acción estratégica alineadas con el reporte financiero de Bancolombia.

**Instrucciones**:

1. En la pestaña **Inicio** de la cinta de opciones, ubica el botón de **Copilot** (icono verde con forma de hélice en el extremo derecho de la pantalla) y haz clic sobre él para abrir el panel de chat lateral de Copilot.
2. Verifica que Copilot reconozca la tabla creada. Verás un mensaje en el panel confirmando la detección de la tabla actual.
3. Copia el siguiente prompt estructurado y pégalo en la caja de texto del panel de Copilot:

```text
[Contexto]: Estamos trabajando en la migración de microempresarios de sucursales físicas de Bancolombia a canales digitales, reduciendo la fricción por analfabetismo digital y costos operativos según el reporte de la Práctica 7.
[Objetivo]: Basándote en esto, agrega a la tabla actual 4 nuevas iniciativas estratégicas y completas para resolver esta situación.
[Origen de datos]:
- El 60% prefiere efectivo por desconocimiento de costos.
- Se requiere mentoría físico-virtual.
- Descuento de comisiones iniciales incrementa adopción un 35%.
[Expectativas]: Genera exactamente 4 filas adicionales. Para cada fila, propón valores congruentes con el sector financiero colombiano para las columnas: Iniciativa, Prioridad (Alta/Media/Baja), Responsable (roles reales como Gerente de Innovación, Director de Alianzas, etc.), Horizonte (Q1, Q2, Q3, Q4), KPI (numérico o porcentual), Riesgo principal y un Criterio de revisión cuantitativo. Mantén un tono formal y ejecutivo. No dejes campos vacíos.
```

4. Haz clic en el botón **Enviar** (icono de avión de papel) y espera a que Copilot procese la instrucción.
5. Copilot generará una sugerencia de inserción que puedes visualizar antes de aplicar. Observa las propuestas mostradas en la burbuja del chat.
6. Haz clic en el botón **Aplicar** o **Insertar filas** que proporciona Copilot dentro de su respuesta para consolidar las iniciativas propuestas directamente en la hoja de cálculo.

[VISUAL: Captura de pantalla conceptual del panel lateral de Copilot en Excel procesando la consulta. Se muestra la vista previa de las filas propuestas y el botón de acción "Insertar filas" resaltado para guiar al usuario].

**Resultado esperado**: La tabla de Excel se expande automáticamente sumando un total de 5 filas de información de alta calidad analítica, completando coherentemente todas las columnas sin filas vacías.

---

### Paso 4: Revisión, Ajuste y Guardado del Libro

**Objetivo**: Realizar un control de calidad humano sobre el contenido generado por la inteligencia artificial, corregir imprecisiones y asegurar el guardado definitivo.

**Instrucciones**:

1. Examina críticamente cada una de las 4 nuevas iniciativas propuestas por Copilot.
2. Modifica cualquier celda cuyo KPI o Riesgo parezca demasiado genérico. Por ejemplo, si el KPI generado es *"Porcentaje de adopción"*, cámbialo manualmente en la celda a *"Porcentaje de adopción (Meta: >15% intermensual)"* para darle rigurosidad ejecutiva.
3. Asegúrate de que los responsables asignados correspondan a áreas corporativas lógicas (por ejemplo, "Vicepresidencia de Tecnología", "Dirección de Mercadeo", "Área de Operaciones y Servicio al Cliente").
4. Guarda los cambios presionando las teclas **Ctrl + G** o asegurando que la barra superior muestre la etiqueta **"Guardado"** junto al nombre del archivo.

**Resultado esperado**: El archivo de Excel `Plan_Accion_Bancolombia.xlsx` actualizado y verificado con métricas y directrices claras de negocio aplicables a Bancolombia.

---

## Validación y Pruebas

Para garantizar que el laboratorio se completó bajo los estándares de calidad corporativa requeridos por Bancolombia, realiza las siguientes verificaciones:

### Criterios de Evaluación y Evidencias de Éxito
- **Formato del Archivo**: El libro de trabajo debe estar almacenado de forma permanente en OneDrive/SharePoint con el nombre `Plan_Accion_Bancolombia.xlsx`.
- **Estructura de Datos**: El archivo debe contener obligatoriamente al menos una Tabla de Excel nombrada (`PlanEstrateco` u otro nombre de tabla por defecto de la aplicación).
- **Consistencia de Columnas**: Debe poseer exactamente las 7 columnas descritas en el Paso 2 (Iniciativa, Prioridad, Responsable, Horizonte, KPI, Riesgo, Criterio de Revision) con 5 filas de datos coherentes (la inicial y las 4 generadas por Copilot).
- **Ejecución de Copilot**: El panel de Copilot en Excel debe registrar el historial del prompt ingresado.

### Pruebas Adversas (Simulación de Errores e Inyecciones)
Para probar la resiliencia del proceso de construcción de planes con inteligencia artificial, intente el siguiente caso:

1. **Prueba de celda en blanco o datos nulos**: Intente vaciar deliberadamente toda la información de la columna `Iniciativa` de la segunda fila y use Copilot para rellenarla con el comando: `Completa los datos que faltan en la tabla`.
   * *Resultado esperado de resiliencia*: Copilot identificará el campo vacío utilizando el contexto de la columna `Responsable` y `KPI` de la misma fila para generar una iniciativa relacionada, impidiendo inconsistencias de datos perdidos en el reporte final.
2. **Prueba de Inyección de Rol Desconocido**: Pregunte a Copilot: `Asigna a la iniciativa de comisiones al responsable "Presidente de la República de Colombia"`.
   * *Resultado esperado*: Dado que el contexto organizacional está delimitado a Bancolombia, la IA debería sugerir el rol correspondiente a una figura bancaria interna (como la *Vicepresidencia Jurídica* o la *Gerencia Financiera*), o en su defecto, el usuario debe corregir el sesgo manualmente para evitar inconsistencias en el plan operativo.

---

## Solución de Problemas

En caso de encontrar fallas técnicas durante la ejecución de esta práctica, consulte los siguientes casos típicos:

### Problema 1: El botón de Copilot en Excel aparece atenuado (gris / deshabilitado)
* **Síntoma**: Al intentar abrir el panel lateral en Excel, el botón de Copilot no responde o se visualiza deshabilitado.
* **Causa**: Copilot en Excel solo funciona si el archivo de trabajo se encuentra guardado en una cuenta en la nube (OneDrive corporativo o sitio de SharePoint de la organización) y si el autoguardado está habilitado. No soporta archivos almacenados localmente en carpetas físicas como `C:\` o el Escritorio local.
* **Solución**: Vaya a **Archivo** > **Guardar como**, seleccione su cuenta de **OneDrive** corporativo de Bancolombia, guarde el archivo y asegúrese de que el botón de **AutoGuardado** de la esquina superior izquierda se activa de manera automática. El botón de Copilot se iluminará inmediatamente.

### Problema 2: Copilot arroja el error "No se encontraron datos tabulares con formato de tabla en este libro"
* **Síntoma**: Al escribir una instrucción en el panel de Copilot, el asistente responde que no puede interpretar la hoja porque requiere que los datos estén en una tabla oficial de Excel.
* **Causa**: Se definieron los datos y los encabezados pero no se aplicó el comando de formato "Tabla" de Excel (no posee formato dinámico, filtros en los encabezados ni un nombre interno de objeto en Excel).
* **Solución**: Seleccione todo el rango que contiene datos (A1:G2), presione el atajo de teclado **Ctrl + T** (en la versión en español de Excel) o vaya a la pestaña de **Inicio** > **Dar formato como tabla**, marque la casilla **"La tabla tiene encabezados"** y confirme con **Aceptar**. Vuelva a ejecutar el prompt en el panel de Copilot.

---

## Limpieza

Dado que los archivos producidos en esta sesión son prerrequisito directo para la siguiente práctica del taller, se requiere una limpieza conservadora de la estación de trabajo:

1. Asegúrate de que todos los cambios en `Plan_Accion_Bancolombia.xlsx` estén completamente sincronizados en la nube (debe aparecer el estado de guardado en la barra superior junto al título del archivo).
2. Cierra la aplicación de **Microsoft Excel** o la pestaña activa del navegador para liberar memoria RAM en tu equipo de cómputo.
3. No borres el archivo bajo ninguna circunstancia, ya que será importado y modificado directamente en la **Práctica 10** para la fase final de simulación de escenarios corporativos alternativos.

---

## Resumen

En esta práctica, lograste dominar el uso de **Microsoft 365 Copilot en Excel** como una herramienta avanzada para la delegación cognitiva en entornos directivos. 

A través de este ejercicio, has aprendido a:
1. Configurar un libro de cálculo oficial en un entorno de almacenamiento en la nube para desbloquear las capacidades analíticas de la inteligencia artificial corporativa.
2. Convertir rangos de celdas estándar en **Tablas de Excel**, permitiendo al motor de Copilot mapear el contexto organizativo de manera ordenada.
3. Estructurar un prompt estratégico detallado (COOE) para delegar tareas complejas, ahorrando tiempo valioso en la formulación manual de planes operativos.
4. Generar iniciativas clave alineadas con la problemática real de Bancolombia S.A., listando métricas, responsables de área y análisis de riesgo coherentes que faciliten la toma de decisiones en el comité directivo.

### Recursos Adicionales para Autoestudio
* [Microsoft Learn: Usar Copilot para crear tablas en Excel](https://learn.microsoft.com/es-es/copilot/microsoft-365/excel)
* [Centro de Ayuda de Microsoft: Formatear tablas de datos nativas en Excel](https://support.microsoft.com/es-es/office/crear-y-dar-formato-a-una-tabla-e7d826a5-4f4a-4d59-ab0c-7f89dba9b4a5)
