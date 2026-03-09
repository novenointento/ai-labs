# Prompt Template

Este documento sirve como plantilla para diseñar prompts estructurados y reutilizables.

El objetivo es tratar los prompts como si fueran código: versionados, documentados y mejorables.

---

# Prompt Name

Nombre corto y descriptivo del prompt.

Ejemplo:
Log Analysis Assistant

---

# Purpose

Explica qué problema resuelve este prompt.

Ejemplo:

Analizar logs de sistemas distribuidos para detectar posibles causas de errores y sugerir acciones correctivas.

---

# Recommended Models

Modelos con los que funciona bien este prompt.

Ejemplo:

* GPT-4 class models
* DeepSeek Coder
* Mistral
* Llama 3

---

# Prompt Structure

Este prompt sigue la estructura recomendada:

1. System prompt
2. Task
3. Context
4. Constraints
5. Output format

---

# System Prompt

Define el comportamiento del modelo.

Ejemplo:

You are a senior software engineer specialized in distributed systems and debugging complex infrastructures.

You explain technical issues clearly and provide actionable solutions.

---

# Task

Define la tarea concreta que debe realizar el modelo.

Ejemplo:

Analyze the provided system logs and identify potential root causes of failures.

---

# Context

Información adicional necesaria para la tarea.

Ejemplo:

Logs:

{{LOG_DATA}}

System description:

{{SYSTEM_DESCRIPTION}}

---

# Constraints

Reglas que debe seguir el modelo.

Ejemplo:

* Do not invent information that is not present in the logs
* Base the analysis only on the provided data
* If the root cause is uncertain, explain the possible alternatives

---

# Output Format

Define cómo debe estructurarse la respuesta.

Ejemplo:

Root Cause
Explanation
Suggested Fix

---

# Prompt Template

Plantilla final combinada.

You are a senior software engineer specialized in distributed systems.

Analyze the following logs and identify possible root causes.

Logs:
{{LOG_DATA}}

Explain:

1. Root cause
2. Explanation
3. Suggested fix

---

# Variables

Lista de variables utilizadas en el prompt.

{{LOG_DATA}}
Contenido de los logs a analizar.

{{SYSTEM_DESCRIPTION}}
Descripción del sistema si es necesario.

---

# Example Input

Logs:

ERROR: Node disconnected
Heartbeat missed
Connection timeout

---

# Example Output

Root Cause
The node was unable to maintain heartbeat communication with the cluster.

Explanation
This usually occurs when the node CPU is saturated or network connectivity is degraded.

Suggested Fix
Check CPU usage and verify cluster network connectivity.

---

# Notes

Observaciones sobre el comportamiento del prompt.

Ejemplo:

* funciona mejor con temperatura baja
* útil para logs de infraestructura
* puede requerir contexto adicional en sistemas complejos

---

# Version History

v1
Prompt inicial.

v2
Se añadió formato estructurado de respuesta.

v3
Mejora del system prompt para mayor precisión.
