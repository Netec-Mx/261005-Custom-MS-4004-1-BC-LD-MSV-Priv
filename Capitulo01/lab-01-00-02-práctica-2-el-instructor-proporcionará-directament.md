# Práctica 2: Copilot como apoyo para analizar y desafiar una decisión

**Duración:** 30 min

## Descripción
Escenario: Un equipo ejecutivo debe decidir cómo responder ante una disminución en la adopción de una experiencia digital por parte de un segmento de clientes. Existen diferentes hipótesis sobre las causas y distintas alternativas de intervención, pero antes de comprometer recursos el líder necesita estructurar el problema, evaluar las opciones y determinar qué información adicional necesita.

## Pasos para ejecutar la práctica

1. **Construir el problema antes de buscar la respuesta:**
   * Copia y envía el siguiente prompt a Copilot Chat para estructurar la situación sin solicitar aún recomendaciones:
     ```text
     Actúa como un Consultor de Estrategia Ejecutiva.
     
     Contexto: Registro de una caída del 18% en la adopción de la aplicación móvil en el segmento de clientes jóvenes durante el último trimestre. Las hipótesis internas señalan lentitud en la interfaz y falta de funcionalidades clave, pero existen restricciones presupuestales y operativas para el presente año.
     Objetivo: Estructurar y organizar la problemática sin generar recomendaciones o soluciones aún.
     Origen: Información del escenario operativo y métricas de adopción presentadas.
     Expectativas: Presenta un análisis dividido estrictamente en tres apartados:
     - Qué se sabe (hechos y datos confirmados)
     - Qué se está suponiendo (hipótesis no validadas)
     - Qué sería necesario validar (vacíos de información crítica)
     ```

2. **Construir y comparar alternativas de decisión:**
   * A partir del problema organizado, envía el siguiente prompt para evaluar opciones:
     ```text
     Con base en el problema estructurado anteriormente, genera exactamente tres alternativas de actuación estratégicas.
     
     Para cada una de las alternativas detalla obligatoriamente:
     1. Beneficio esperado
     2. Riesgos principales
     3. Dependencias operativas o de equipo
     4. Supuesto crítico para que funcione
     5. Información faltante
     6. Indicadores (KPIs) para evaluar posteriormente su efectividad
     ```

3. **Utilizar la IA para cuestionar, no solamente para recomendar:**
   * Desafía la alternativa preferida utilizando el siguiente prompt de postura crítica:
     ```text
     Adopta una postura crítica e imparcial frente a la alternativa de mayor impacto propuesta.
     
     Identifica:
     1. Las 3 razones principales por las que esta decisión podría fracasar estrepitosamente.
     2. Señales tempranas (alertas) que indicarían que debemos reconsiderar la decisión inmediatamente.
     3. Las 5 preguntas difíciles que un Comité Ejecutivo debería realizar antes de aprobar recursos.
     ```

4. **Comparar modelos según el tipo de tarea:**
   * Alterna el modelo de lenguaje disponible en la interfaz de Copilot (por ejemplo, entre modelos de OpenAI y Claude) y vuelve a ejecutar la solicitud de análisis del paso 3. Compara qué enfoque genera información más profunda y útil para la toma de decisiones ejecutiva.

## Resultado esperado
Un marco completo de decisión ejecutiva que incluye la estructuración del problema entre hechos y supuestos, una matriz comparativa de tres alternativas con sus riesgos e indicadores, un análisis crítico de puntos de falla y una comparación analítica de respuestas según el modelo de IA utilizado.
