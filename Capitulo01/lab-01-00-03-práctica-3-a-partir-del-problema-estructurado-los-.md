# Laboratorio 3: Ampliar el análisis y convertirlo en acción con Copilot y agentes

**Duración:** 30 min

## Descripción
En este laboratorio se profundiza el análisis del caso ejecutivo trasladando necesidades complejas a agentes especializados, contrastando hipótesis con evidencia externa, construyendo un plan de acción interactivo con escenarios en Excel y preparando al líder para la presentación defensiva mediante un agente especializado.

## Pasos para ejecutar la práctica

1. **Reconocer cuándo el caso deja de ser una tarea de prompting:**
   * Revisa las nuevas necesidades: investigar factores externos de mercado, validar supuestos con evidencia y preparar al líder para defender la recomendación.
   * Determina qué tareas se resuelven con el chat de Copilot y cuáles requieren agentes especializados como Investigador (Researcher) o Executive Briefing Agent.

2. **Profundizar una decisión con el agente Investigador (Researcher):**
   * Selecciona el agente **Investigador (Researcher)** en Microsoft 365 Copilot.
   * Envía la siguiente solicitud:
     ```text
     Investiga tendencias del mercado digital y financiero sobre la adopción de aplicaciones móviles en segmentos jóvenes, factores de abandono de experiencia de usuario (UX) e indicadores de referencia (benchmarks) de la industria.
     
     Restricción estricta de formato: Presenta los resultados EXCLUSIVAMENTE en formato de informe textual. Incluye tendencias encontradas, factores externos, indicadores clave y supuestos identificados. NO generes tablas, gráficos, visualizaciones ni proyecciones numéricas.
     ```

3. **Contrastar el análisis inicial con nueva evidencia:**
   * Lleva el informe obtenido en la investigación al chat principal con el siguiente prompt:
     ```text
     Con base en el siguiente informe de investigación [Pega el texto de la investigación], contrasta nuestro análisis inicial de alternativas de decisión.
     
     Indica:
     1. Qué elementos fortalecen cada alternativa.
     2. Qué elementos debilitan cada alternativa.
     3. Cuál es el supuesto crítico que, de resultar incorrecto, cambiaría drásticamente nuestra decisión.
     ```

4. **Convertir los hallazgos en un plan de acción con Copilot en Excel:**
   * Abre un libro nuevo en **Microsoft Excel**.
   * Activa el panel de Copilot en modo **Plan** y envía:
     ```text
     Usa el siguiente contexto de investigación [Pega el resumen del análisis] para crear un plan de acción estructurado. Organiza las columnas en: Iniciativa, Prioridad, Responsable, Horizonte de ejecución, Indicadores de seguimiento, Riesgo principal y Criterio de revisión.
     ```
   * Cambia al modo **Permitir la edición** en Copilot en Excel y envía:
     ```text
     Crea tres escenarios de evolución de adopción (Optimista, Conservador y Crítico) basados en los datos del plan, incorpora las fórmulas necesarias y genera un gráfico comparativo de los indicadores clave.
     ```

5. **Preparar al líder:**
   * Selecciona el agente **Investigador (Researcher)** en Microsoft 365 Copilot.
   * Envía el siguiente prompt de entrenamiento y simulación:
     ```text
     Prepárame para presentar y defender la recomendación ejecutiva de respuesta ante la caída de adopción digital ante el Comité Directivo.
     
     Genera:
     1. Los 3 mensajes principales de impacto.
     2. Anticipación de las 5 objeciones más difíciles que presentarán los directores.
     3. Respuestas estratégicas sustentadas para cada objeción.
     ```

## Resultado esperado
Un informe textual de investigación de tendencias, un análisis de supuestos revalidado con evidencia, un libro de Excel con plan de acción interactivo, escenarios y gráficos generados por Copilot, y una guía de preparación defensiva para el líder.
