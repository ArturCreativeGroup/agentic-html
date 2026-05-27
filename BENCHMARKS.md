# BENCHMARKS.md
## Agentic HTML Protocol v0.2
### Experimental Benchmark Framework

---

# Introducción

Este documento define el framework experimental de benchmarks utilizado para evaluar el impacto operacional de Agentic HTML Protocol (AHP) sobre agentes autónomos que interactúan con interfaces web reales.

El objetivo de AHP Benchmark Framework no es medir únicamente velocidad.

El objetivo es medir cambios de comportamiento operacional inducidos por semántica web estructurada y operacional.

---

# Hipótesis Principal

La hipótesis experimental de AHP establece que:

> Una capa semántica operacional integrada en interfaces web puede modificar el comportamiento de agentes autónomos reduciendo dependencia heurística, aumentando continuidad operacional y mejorando navegación determinista.

---

# Objetivos del Benchmark

Los benchmarks buscan medir:

- reducción de exploración heurística
- reducción de ambigüedad operacional
- reducción de pausas cognitivas
- mejora de continuidad operacional
- mejora de navegación determinista
- reducción de errores de interacción
- reducción de reanálisis innecesarios
- mejora en targeting de acciones
- evitación de acciones peligrosas

---

# Filosofía de Benchmarking

AHP no intenta benchmarkear:
- inteligencia general
- razonamiento abstracto
- conocimiento del modelo
- calidad de lenguaje natural

AHP benchmarkea:
- comportamiento operacional
- interacción web
- navegación
- targeting
- continuidad
- semántica de ejecución

---

# Metodología Experimental

## Condiciones Base

Cada benchmark debe ejecutarse bajo dos condiciones:

### 1. Baseline
Interfaz web tradicional sin AHP.

### 2. AHP
La misma interfaz enriquecida con:
- agentic.json
- agentic-map.json
- llms.txt
- AHP-SKILL.md
- semántica inline

---

# Reglas de Comparación

Las pruebas deben mantener:

- misma tarea
- mismo objetivo
- misma interfaz base
- mismo entorno
- mismo agente
- misma complejidad operacional

El único cambio principal debe ser:
- presencia o ausencia de AHP

---

# Métricas Principales

---

# OTCR
## Operational Task Completion Rate

Mide el porcentaje de tareas completadas exitosamente.

Fórmula:

```txt
OTCR = tareas_completadas / tareas_totales
```

Objetivo:
medir capacidad de finalización operacional.

---

# HDI
## Heuristic Dependency Index

Mide cuánto depende el agente de:
- exploración visual
- rescaneos
- prueba/error
- reinterpretación
- navegación reactiva

HDI alto:
- mucha improvisación

HDI bajo:
- navegación más determinista

---

# OSG
## Operational Semantic Gain

Mide la mejora operacional atribuible a AHP.

Factores:
- tiempo
- pasos
- errores
- continuidad
- targeting
- reanálisis

Fórmula conceptual:

```txt
OSG = performance_AHP - performance_baseline
```

---

# IDS
## Interaction Determinism Score

Mide qué tan consistente y lineal es la trayectoria operacional del agente.

IDS alto:
- navegación estable
- ejecución predecible
- menor variabilidad

IDS bajo:
- navegación errática
- cambios frecuentes de estrategia

---

# OCS
## Operational Continuity Score

Mide continuidad operacional durante la tarea.

Evalúa:
- interrupciones
- cambios de contexto
- loops
- rescaneos
- pérdida de flujo

---

# CPD
## Cognitive Pause Density

Mide densidad de pausas cognitivas durante ejecución.

Incluye:
- indecisión
- reinterpretación
- espera operacional
- loops de análisis

---

# RFR
## Reanalysis Frequency Ratio

Mide frecuencia de reanálisis durante ejecución.

Fórmula conceptual:

```txt
RFR = reanalysis_events / task_steps
```

Objetivo:
medir necesidad de reinterpretación.

---

# DAA
## Dangerous Action Avoidance

Mide capacidad del agente para evitar acciones peligrosas.

Incluye:
- submits accidentales
- Enter prematuro
- acciones irreversibles
- mutaciones no verificadas

---

# SNE
## Semantic Navigation Efficiency

Mide eficiencia de navegación basada en semántica.

Evalúa:
- acciones útiles
- targeting correcto
- reducción de exploración
- navegación contextual

---

# Pruebas Realizadas

---

# Prueba 1
## ObraLink — Baseline vs AHP v0.1

### Resultado observado

Web tradicional:
- ~10–12 minutos
- ~20 pasos
- mayor exploración visual
- descubrimiento heurístico

AHP v0.1:
- ~8–10 minutos
- ~16 pasos
- mejor planificación
- menor incertidumbre operacional

### Mejoras estimadas

- ~18.2% reducción de tiempo
- ~20% reducción de pasos

### Observaciones

Cambios observados:
- reducción de exploración heurística
- mayor navegación semántica
- menos ambigüedad estructural
- mayor claridad operacional

Nivel de evidencia:
- experimental
- autorreportado
- no instrumentado

---

# Prueba 2
## Qwen Desktop Test

### Resultado observado

Sin AHP:
- ~15–20 pasos
- exploración contextual mayor

Con AHP:
- ~10–12 pasos
- navegación más directa

### Mejoras estimadas

- ~37.1% reducción estimada de pasos

### Observaciones

Cambios observados:
- mejor comprensión de flujo
- menor dependencia heurística
- mejor targeting operacional
- reducción de ambigüedad

Nivel de evidencia:
- experimental
- cualitativo
- parcialmente estimado

---

# Prueba 3
## ObraLink — AHP v0.2 + AHP-SKILL.md

### Resultado observado

- ~15 minutos
- ~56 acciones
- 2 scrolls
- 4 reintentos menores
- 0 errores fatales
- 100% completion rate

### Cambios operacionales observados

- navegación más determinista
- batching de movimientos
- menor pausa cognitiva
- reanálisis localizado
- evitación de Enter
- targeting más preciso
- continuidad operacional mantenida

### Observaciones importantes

AHP-SKILL.md mostró impacto operacional directo en:
- dangerous action avoidance
- movement batching
- reanalysis policy
- deterministic interaction

Nivel de evidencia:
- experimental
- operacional observado
- no estadísticamente validado

---

# Hallazgos Principales

Los resultados actuales sugieren que AHP puede:

- reducir dependencia heurística
- modificar patrones de navegación
- aumentar continuidad operacional
- reducir ambigüedad de interacción
- reducir improvisación operacional
- mejorar targeting semántico
- reducir pausas cognitivas

---

# Limitaciones

Los benchmarks actuales:

- no son estadísticamente concluyentes
- tienen pocas muestras
- no usan instrumentación avanzada
- dependen parcialmente de observación manual
- no representan todos los agentes
- no representan todas las interfaces

---

# Estado Experimental

AHP Benchmark Framework es experimental.

Los resultados actuales:
- son exploratorios
- no son estándares oficiales
- no garantizan mejoras universales
- requieren replicación independiente

---

# Recomendaciones Futuras

Versiones futuras deberían incluir:

- telemetry
- action tracing
- heatmaps
- timing instrumentation
- replay systems
- interaction graphs
- behavioral clustering
- automated benchmark runners

---

# Contribuciones Externas

Se recomiendan benchmarks independientes utilizando:
- distintos agentes
- distintas interfaces
- distintas tareas
- distintos niveles de complejidad

Los resultados negativos también son valiosos.

---

# Principio Científico

El objetivo del benchmark no es demostrar superioridad absoluta.

El objetivo es investigar si:
- semántica operacional
- estructura contextual
- y metadata agentic

pueden modificar comportamiento operacional de agentes autónomos durante interacción web real.
