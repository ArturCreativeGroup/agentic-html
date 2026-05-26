# Agentic HTML Protocol

## ¿Qué es esto?

Agentic HTML Protocol es un proyecto experimental que explora cómo las interfaces web podrían exponer intención operacional, contexto semántico y reglas de interacción para agentes IA.

La idea principal es investigar si una interfaz puede describirse no solo para navegadores y humanos, sino también para sistemas capaces de interpretar acciones, relaciones, workflows y contexto de manera más explícita.

---

## ¿Por qué existe?

Actualmente la mayoría de agentes IA interpretan interfaces web mediante:

* parsing HTML
* heurísticas
* inferencia contextual
* navegación probabilística
* análisis visual

Eso funciona, pero también genera:

* ambigüedad
* consumo innecesario de contexto
* inferencias incorrectas
* workflows inconsistentes
* navegación poco precisa

Agentic HTML Protocol nace como una investigación experimental para explorar una posible capa semántica-operacional que permita describir interfaces de manera más comprensible para agentes IA.

---

## Idea principal

La hipótesis principal es que una interfaz web puede ofrecer una capa semántica y operacional más explícita para agentes IA, reduciendo ambigüedad y mejorando comprensión contextual.

En lugar de depender únicamente del DOM visual, una interfaz podría declarar:

* intención
* acciones
* workflows
* relaciones
* políticas
* contexto operacional

Ejemplo:

```
<section
  agentic-role="form"
  agentic-purpose="capture-qualified-lead"
  agentic-policy="requires-human-confirmation">
</section>
```

---

## Archivos principales del protocolo

El protocolo actualmente propone algunos archivos experimentales:

| Archivo             | Propósito                                 |
| ------------------- | ----------------------------------------- |
| `agentic.json`      | Configuración principal del protocolo     |
| `agentic-map.json`  | Representación operacional de la interfaz |
| `agentic-skills.md` | Instrucciones operacionales para agentes  |
| `llms.txt`          | Contexto resumido para modelos IA         |

---

## Atributos experimentales

Actualmente se están explorando atributos como:

```
agentic-role
agentic-purpose
agentic-action
agentic-policy
agentic-context
agentic-flow
agentic-entity
```

Estos atributos buscan describir:

* intención
* relaciones
* workflows
* acciones disponibles
* restricciones operacionales
* entidades de la interfaz

---

## Ejemplo

Ejemplo simple:

```
<button
  agentic-action="submit-form"
  agentic-policy="requires-human-confirmation">
  Enviar solicitud
</button>
```

Más ejemplos disponibles en:

```
/examples
```

---

## Benchmark preliminar

Primera prueba experimental realizada sobre una demo funcional del protocolo:

### HTML completo

~10.446 tokens aproximados

### Archivos core del protocolo

* `agentic.json`
* `agentic-map.json`
* `agentic-skills.md`
* `llms.txt`

Total aproximado:

~2.235 tokens

### Resultado preliminar observado

Reducción aproximada:
~78,6%

⚠️ Importante:

Este benchmark es experimental y no debe considerarse un resultado generalizable todavía.

Actualmente representa únicamente:

* una prueba exploratoria
* un entorno controlado
* un dataset reducido

---

## Estado actual del proyecto

Actualmente el proyecto incluye:

* documentación experimental
* parser semántico inicial
* generación de `agentic-map.json`
* generación experimental de `agentic-skills.md`
* detección de entidades
* detección de workflows
* detección de acciones
* inferencia contextual básica
* benchmark preliminar

---

## Objetivos de investigación

Las áreas actualmente en investigación incluyen:

* representación operacional de interfaces
* reducción de ambigüedad
* workflows semánticos
* navegación agentic
* relationship graphs
* policies para agentes IA
* extracción semántica contextual
* benchmark de comprensión de interfaces

---

## Limitaciones actuales

* Extracción semántica experimental
* Dataset pequeño
* Sin validación multi-modelo
* Relationship graph en desarrollo
* Inferencia de workflows todavía inestable
* Sin especificación formal
* Sin benchmark a gran escala
* Sin validación en producción
* Parser todavía propenso a sobreinferencia
* Cobertura limitada de tipos de interfaces

---

## Roadmap

### v0.1

* Documentación inicial
* Protocolo experimental
* Atributos base
* Parser experimental
* Benchmark preliminar

### v0.2

* Relationship graph engine
* Workflow inference mejorado
* Semantic scoring
* Validación estructural
* Benchmarks comparativos

### v0.3

* Plataforma de benchmarks
* Validación multi-modelo
* Datasets públicos
* Tooling semántico
* Navegación agent-ready

### v0.4

* Refinamiento del protocolo
* Semantic operational graphs
* Reasoning layers
* Protocol validator
* Ecosistema experimental

---

## Estado experimental

Agentic HTML Protocol es actualmente:

* una investigación experimental
* un laboratorio conceptual
* una exploración técnica

NO:

* un estándar oficial
* un reemplazo de HTML
* una especificación final
* una tecnología validada en producción

El objetivo actual es:
investigar, experimentar y validar hipótesis relacionadas con interfaces preparadas para agentes IA.

---

## Filosofía

Human First. Agent Ready.

La idea central del proyecto no es reemplazar la experiencia humana de la web, sino explorar cómo las interfaces podrían comunicar intención y contexto de manera más explícita para sistemas IA sin perder claridad para
