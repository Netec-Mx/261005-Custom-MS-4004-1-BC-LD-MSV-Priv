# Lab 01-00-10: Práctica 10. Análisis Predictivo de Escenarios, Fórmulas y Visualización en Excel con Copilot

## Metadatos
| Dimensión | Detalle |
| :--- | :--- |
| **Duración** | 8 minutos |
| **Complejidad** | Difícil |
| **Nivel Bloom** | Crear |
| **Objetivos** | 1. Utilizar el modo de edición de Copilot en Excel para incorporar datos numéricos y estructurar escenarios evolutivos (Optimista, Base, Pesimista).<br>2. Generar fórmulas de cálculo automáticas y visualizaciones gráficas comparativas directamente en la hoja de cálculo.<br>3. Identificar riesgos y oportunidades clave basados en los gráficos de comportamiento proyectado. |

---

## Descripción General
En este laboratorio práctico, asumirá el rol de un Analista Financiero y de Estrategia Digital de Bancolombia. Utilizando el archivo generado en la práctica anterior (`Plan_Accion_Bancolombia.xlsx`), interactuará con **Microsoft 365 Copilot en Excel** para diseñar un modelo de simulación de escenarios (Optimista, Base y Pesimista) sobre la migración digital de microempresarios. 

A través de la funcionalidad de edición y comandos interactivos de Copilot, aplicará fórmulas automáticas para proyectar KPIs bajo diferentes niveles de fricción digital, automatizará la creación de gráficos comparativos y generará un análisis de sensibilidad cuantitativo para guiar las decisiones de la alta dirección.

---

## Objetivos de Aprendizaje
Al finalizar este laboratorio, usted será capaz de:
*   [ ] Configurar y formatear datos planos en tablas estructuradas de Excel compatibles con el motor de IA de Copilot.
*   [ ] Aplicar la estructura de prompts avanzados **COOE** (Contexto, Objetivo, Origen, Expectativas) en Excel para forzar la creación de columnas calculadas utilizando fórmulas nativas de Excel.
*   [ ] Generar visualizaciones dinámicas de tendencias de rendimiento entre escenarios sin intervención manual de menús.
*   [ ] Evaluar críticamente proyecciones asistidas por IA y diagnosticar puntos de riesgo financiero e inconsistencias en escenarios pesimistas.

---

## Prerrequisitos
*   **Conocimientos teóricos previos**: 
    *   Comprensión del marco de simulación de escenarios financieros (Base, Optimista, Pesimista).
    *   Entendimiento del problema de negocio: Migración de clientes microempresarios de sucursales físicas a canales digitales de Bancolombia (fricción por brecha digital, costos de adopción).
*   **Requisitos de acceso y archivos**:
    *   Archivo de trabajo `Plan_Accion_Bancolombia.xlsx` completado en la Práctica 9. *(En caso de no contar con él, en el Paso 1 se provee la estructura inicial para reconstruirlo rápidamente).*
    *   Licencia activa de **Microsoft 365 Copilot** con acceso a Excel en la Web o Excel de escritorio.

---

## Entorno de Laboratorio

### Requisitos de Hardware
| Componente | Especificación Mínima |
| :--- | :--- |
| **Dispositivo** | Laptop o PC de escritorio con procesador Intel Core i5 o superior (64 bits) |
| **Memoria RAM** | 8 GB o superior |
| **Conexión de Red** | Banda ancha estable (Mínimo 10 Mbps de bajada y subida) |
| **Resolución de Pantalla** | Mínimo 1920x1080 píxeles para facilitar la interfaz dividida de Excel y el panel de Copilot |

### Requisitos de Software y Licencias
| Software / Servicio | Versión Sugerida / Detalles de Licencia | Origen de Descarga |
| :--- | :--- | :--- |
| **Microsoft Edge** | Versión 128.0.2739.42 de 64 bits o superior | [Microsoft Edge Oficial](https://www.microsoft.com/edge) |
| **Microsoft Excel** | Microsoft 365 Apps para Empresas (Versión 2408 Compilación 17928.20156) o Excel Online | [Microsoft 365 Portal](https://portal.office.com) |
| **Licencia Copilot** | Licencia de **Microsoft 365 Copilot Premium** (SaaS) activa en el tenant organizacional | Asignado por Administrador M365 |

---

## Instrucciones Paso a Paso

### Paso 1: Preparación del archivo y validación de Tabla de Excel
Antes de solicitar operaciones complejas a Copilot en Excel, los datos deben estar estructurados rigurosamente en formato de **Tabla de Excel**. Si no se cumple esto, el botón de Copilot aparecerá deshabilitado.

1. Abra **Microsoft Edge** y acceda a su portal corporativo de OneDrive o SharePoint.
2. Abra el archivo `Plan_Accion_Bancolombia.xlsx` creado en la sesión anterior.
3. *Nota de contingencia (si no posee el archivo de la Práctica 9)*: Cree una hoja nueva e ingrese los siguientes datos EXACTAMENTE en el rango `A1:G4`:

| ID_Iniciativa | Iniciativa | KPI_Nombre | Metrica_Base | Meta_Q4 | Costo_Adopcion_USD | Friccion_Esperada |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| MIGR_01 | Talleres presenciales en sucursales | Tasa de Adopción Digital | 15.00% | 45.00% | 5000 | Baja |
| MIGR_02 | Subsidio de datos móviles App | Usuarios Activos Mensuales | 1200 | 3500 | 15000 | Media |
| MIGR_03 | Asistente Virtual en WhatsApp | Tasa de Retención del Canal | 60.00% | 85.00% | 8000 | Alta |

4. Seleccione todo el rango de datos (`A1:G4`).
5. Vaya a la pestaña **Inicio** -> sección Estilos -> haga clic en **Dar formato como tabla** y seleccione cualquier diseño. Asegúrese de marcar la opción "La tabla tiene encabezados".
6. En la pestaña **Diseño de tabla**, asigne el nombre de tabla `TablaPlanAccion` en el cuadro de texto del extremo izquierdo.

[VISUAL: Captura de pantalla de la cinta de opciones de Excel en la sección "Diseño de tabla", resaltando el campo "Nombre de la tabla" establecido como "TablaPlanAccion"].

7. Haga clic en el botón de **Copilot** en la pestaña *Inicio* (extremo derecho) para abrir el panel lateral de chat de Copilot en Excel.

---

### Paso 2: Creación de Escenarios Evolutivos mediante el Modo Edición (Fórmulas)
Aplicaremos el framework **COOE** para redactar un prompt avanzado que le ordene a Copilot agregar nuevas columnas con fórmulas estructuradas de Excel basadas en escenarios de negocio.

1. Copie el siguiente prompt estructurado en la caja de texto de Copilot:

```text
[Contexto]: Estamos simulando la migración digital de microempresarios de Bancolombia y necesitamos evaluar el impacto financiero de la fricción de adopción bajo escenarios controlados.
[Objetivo]: Crea tres nuevas columnas calculadas llamadas "Escenario_Pesimista", "Escenario_Base" y "Escenario_Optimista" basadas en la columna "Costo_Adopcion_USD".
[Origen]: Los datos provienen de la columna "Costo_Adopcion_USD" en TablaPlanAccion.
[Expectativas]: 
- La columna "Escenario_Pesimista" debe multiplicar "Costo_Adopcion_USD" por 1.40 (40% de incremento en costos por alta fricción).
- La columna "Escenario_Base" debe ser igual a "Costo_Adopcion_USD".
- La columna "Escenario_Optimista" debe multiplicar "Costo_Adopcion_USD" por 0.85 (15% de ahorro por adopción rápida).
- Usa fórmulas de Excel en lugar de valores estáticos para mantener el dinamismo de la tabla.
```

2. Haga clic en **Enviar** (o presione Enter).
3. Copilot procesará la solicitud y le mostrará una vista previa con el mensaje *"Se sugieren 3 nuevas columnas..."* y las fórmulas calculadas.
4. Haga clic en el botón **Aplicar** o **Insertar columnas** que se muestra en el panel flotante de Copilot.

[VISUAL: Panel flotante de Copilot en Excel mostrando el botón azul "Insertar columnas" con las fórmulas propuestas utilizando la sintaxis estructurada de tablas de Excel, por ejemplo `=[@Costo_Adopcion_USD]*1.4`].

---

### Paso 3: Generación de Fórmulas Dinámicas para KPIs de Rendimiento
Para medir la efectividad, proyectaremos las tasas y metas de los KPIs bajo los tres escenarios.

1. Envíe el siguiente prompt estructurado a Copilot:

```text
Escribe una fórmula en una nueva columna llamada "Meta_Escenario_Pesimista" que calcule la meta ajustada si la fricción digital causa un retroceso en el rendimiento. Si el "KPI_Nombre" contiene la palabra "Tasa", resta un 10.00% absoluto al valor de la columna "Meta_Q4". Si no contiene la palabra "Tasa", multiplica "Meta_Q4" por 0.80 (20% de reducción). Aplica esta regla usando fórmulas condicionales nativas de Excel.
```

2. Copilot analizará el prompt y sugerirá una fórmula que use la función `SI` (`IF`) combinada con `HALLAR` o `ESNUMERO`.
3. Revise la sugerencia en la tarjeta flotante de Copilot. Deberá verse similar a:
   `=SI(ESNUMERO(HALLAR("Tasa";[@KPI_Nombre])); [@Meta_Q4]-0.1; [@Meta_Q4]*0.8)`
4. Haga clic en **Insertar columna**.

---

### Paso 4: Generación Automática de Gráficos Comparativos mediante IA
Para presentar la información a la alta dirección de Bancolombia, requerimos de una visualización gráfica clara que compare los costos proyectados por escenario de cada iniciativa.

1. En el panel de chat de Copilot, escriba el siguiente comando de visualización:

```text
Genera un gráfico de columnas agrupadas que compare el costo de las tres iniciativas (columna "Iniciativa") en los tres escenarios de costos: "Escenario_Pesimista", "Escenario_Base" y "Escenario_Optimista". Asegúrate de que las leyendas muestren claramente el nombre de cada escenario.
```

2. Copilot procesará el conjunto de datos de la tabla de forma interna y generará una miniatura de un gráfico interactivo en su panel de chat.
3. Haga clic en **Agregar a una nueva hoja** o **Insertar en hoja actual** en la parte inferior de la miniatura que provee Copilot.

[VISUAL: Representación conceptual de un gráfico de columnas agrupadas con tres colores distintos en la leyenda (Rojo para Pesimista, Gris para Base, Verde para Optimista) correspondientes a cada una de las 3 iniciativas de migración de Bancolombia].

4. Cambie el nombre de la nueva pestaña que contiene el gráfico a `Visualizacion_Escenarios`.

---

### Paso 5: Análisis de Sensibilidad y Diagnóstico de Riesgos
Finalmente, utilizaremos la capacidad analítica de Copilot para evaluar las proyecciones y resumir los riesgos inherentes al peor escenario.

1. Envíe este prompt a Copilot para que analice los resultados que acaba de graficar y calcular:

```text
Actúa como un Consultor de Gestión de Riesgos de Bancolombia. Basándote exclusivamente en la información numérica de "TablaPlanAccion", analiza el "Escenario_Pesimista" de costos y rendimiento. 
Identifica:
1. Qué iniciativa presenta el riesgo financiero y operativo más crítico en el escenario pesimista, considerando tanto el costo inflado como el tipo de KPI.
2. Cuál es el impacto total acumulado en USD si el escenario pesimista se materializa para todas las iniciativas en lugar del escenario base.
3. Qué dos métricas operacionales o de adopción deberíamos monitorear semanalmente para activar un plan de mitigación inmediato.
Proporciona un informe ejecutivo conciso estructurado con viñetas.
```

2. Copilot leerá los datos directamente de la hoja de cálculo activa y escribirá un análisis detallado en el panel lateral de chat. 
3. Copie el texto entregado por Copilot y péguelo en una nota o en la celda `A7` debajo de su tabla principal para asegurar la persistencia física del análisis dentro del libro de trabajo.

---

## Validación y Pruebas

Para garantizar el cumplimiento de los estándares técnicos de este laboratorio, ejecute las siguientes verificaciones empíricas:

### Verificación del Modelo de Datos y Fórmulas
1. **Comprobación de la estructura dinámica de Excel**:
   * Posiciónese sobre cualquier celda de la columna `Escenario_Pesimista` (por ejemplo, celda `H2`).
   * Verifique en la barra de fórmulas de Excel que la celda no contenga un número estático (como `7000`), sino la referencia estructurada a la tabla:
     `=[@Costo_Adopcion_USD]*1.4` o su equivalente en inglés: `=[@Costo_Adopcion_USD]*1.4`.
2. **Evaluación de precisión de cálculos**:
   * Para la iniciativa `MIGR_02` (Subsidio de datos móviles App), el `Costo_Adopcion_USD` base es **15,000 USD**. El costo calculado bajo el `Escenario_Pesimista` debe ser estrictamente **21,000 USD** (15000 * 1.40).
   * La celda calculada en `Meta_Escenario_Pesimista` para la iniciativa `MIGR_01` (Tasa de Adopción Digital) debe ser **35.00%** (debido a que se restó un 10.00% absoluto al 45.00% original por contener la palabra "Tasa").
   * La celda calculada en `Meta_Escenario_Pesimista` para `MIGR_02` (Usuarios Activos Mensuales) debe ser **2,800** (3500 * 0.80).

### Prueba Adversaria de Robustez (Límites de la IA)
1. Inserte manualmente una nueva fila al final de su tabla con datos vacíos en `Costo_Adopcion_USD`.
2. Observe cómo Copilot autocompleta la fórmula dinámica mostrando un valor de `0` o `#¡VALOR!` (si ingresó un texto no numérico).
3. Envíe el siguiente prompt a Copilot: *"Calcula el escenario pesimista asumiendo que el costo de adopción de la nueva iniciativa es Desconocido"*.
4. **Comportamiento Esperado**: Copilot debe alertar que "Desconocido" es una cadena de texto y que no puede realizar multiplicaciones matemáticas directamente sobre ella sin antes depurar o ignorar el registro, demostrando el principio de preservación de integridad de datos financieros.

---

## Solución de Problemas

### Problema 1: El panel lateral de Copilot muestra un error indicando que "No se puede trabajar con los datos seleccionados" o el botón de Copilot aparece gris (deshabilitado)
* **Síntoma**: El botón de Copilot en la barra de herramientas superior está inactivo, o al intentar abrirlo, un banner indica que la hoja está bloqueada para el uso de IA.
* **Causa**: Copilot en Excel requiere que el archivo de trabajo se encuentre obligatoriamente guardado en la nube (OneDrive corporativo o SharePoint Online) y que los datos estén explícitamente definidos dentro de un objeto de **Tabla de Excel** con encabezados válidos y sin celdas combinadas.
* **Solución**:
  1. Asegúrese de que el archivo esté guardado en un directorio de Microsoft Teams, SharePoint o OneDrive de su cuenta empresarial activa.
  2. Seleccione el rango total de datos (`A1` hasta la última celda con contenido).
  3. Presione el atajo de teclado `Ctrl + T` (o `Ctrl + Q` en algunas versiones en inglés) para abrir la ventana de creación de tabla.
  4. Marque "La tabla tiene encabezados" y haga clic en **Aceptar**. Guarde los cambios y refresque la pestaña del explorador Web de Edge. El botón de Copilot se habilitará inmediatamente.

### Problema 2: El gráfico generado por Copilot no se inserta correctamente o agrupa de forma incorrecta los escenarios en el eje horizontal
* **Síntoma**: El gráfico de columnas muestra un solo bloque gigante o no diferencia las tres iniciativas propuestas, haciendo imposible una comparación limpia.
* **Causa**: Falta de claridad contextual en las cabeceras de columna o selección parcial de celdas al invocar la petición de IA.
* **Solución**:
  1. Haga clic en cualquier celda de datos dentro de `TablaPlanAccion` para restablecer el foco de Excel.
  2. Ejecute el siguiente prompt correctivo detallado en el panel de Copilot:
     ```text
     "Elimina el gráfico previo y vuelve a graficar. Crea un gráfico de columnas agrupadas. Define el eje X como 'Iniciativa' y añade las series individuales para 'Escenario_Pesimista', 'Escenario_Base' y 'Escenario_Optimista'. Ajusta el rango de origen a toda la tabla 'TablaPlanAccion'."
     ```
  3. Esto fuerza a la IA a reconstruir la consulta con la referencia estructural completa de los encabezados del libro de trabajo.

---

## Limpieza
Para dar por concluido el ciclo de trabajo de esta sesión práctica y asegurar el orden del entorno organizativo:

1. Guarde todos los cambios realizados en el archivo. El autoguardado de Excel Online debería indicar: **"Guardado en OneDrive"**.
2. Verifique que el archivo esté nombrado exactamente como `Plan_Accion_Bancolombia_Escenarios.xlsx` (Utilice la opción de **Archivo** -> **Guardar como** -> **Cambiar nombre** para actualizar el nombre del archivo final).
3. No es necesario eliminar las hojas de cálculo dinámicas o visualizaciones generadas, ya que servirán de evidencia para el proceso de auditoría y evaluación del docente.
4. Cierre la pestaña de Excel en Microsoft Edge y asegúrese de cerrar la sesión activa del navegador si está utilizando un dispositivo público o compartido.

---

## Resumen
En esta práctica de laboratorio, ha consolidado sus habilidades analíticas y de automatización mediante el uso de **Microsoft 365 Copilot en Excel** aplicado al negocio financiero. 

### Conceptos Clave Consolidados
*   **Modo Edición Orientado a Datos**: Aprendió que Copilot no solo edita de forma cosmética, sino que inserta fórmulas relacionales nativas de Excel que conservan la integridad lógica de las hojas de cálculo.
*   **Proyección bajo el marco COOE**: Estructuró prompts avanzados capaces de generar escenarios predictivos (Pesimista, Base y Optimista) basados en parámetros de fricción y costos operativos.
*   **Visualización Guiada por Lenguaje Natural**: Generó gráficos complejos directamente desde el motor de IA de Copilot sin necesidad de realizar selecciones manuales exhaustivas de rangos y formatos.
*   **Análisis Crítico de Riesgos**: Utilizó la IA para interrogar un modelo de datos plano y extraer conclusiones cuantitativas rápidas (ej. identificar sobrecostos máximos estimados en **21,000 USD** para la iniciativa crítica de subsidio de datos), traduciendo números áridos en un informe ejecutivo directamente utilizable por la alta dirección de Bancolombia.