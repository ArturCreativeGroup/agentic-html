# AHP-SKILL.md
## Agentic HTML Protocol v0.2
### Capa Semántica Operacional para Agentes Web Autónomos

---

# Propósito

Este documento define las guías de comportamiento operacional para agentes autónomos que interactúan con sitios web que implementan Agentic HTML Protocol (AHP).

A diferencia de capas semánticas estructurales que únicamente describen contenido, AHP-SKILL.md introduce semántica orientada al comportamiento y ejecución operacional con el objetivo de reducir ambigüedad, exploración heurística e interacciones inseguras.

Esta especificación es experimental.

---

# Filosofía Principal

## Human First, Agent Ready

Las interfaces deben seguir siendo centradas en humanos mientras exponen contexto operacional para agentes autónomos.

AHP no intenta reemplazar:
- HTML
- estándares de accesibilidad
- APIs
- sistemas de autenticación
- sistemas de seguridad
- MCP
- permisos del navegador

AHP añade una capa semántica operacional que ayuda a los agentes a:
- comprender intención
- navegar de forma determinista
- reducir interpretación heurística
- minimizar ambigüedad operacional
- ejecutar acciones de manera más segura

---

# Principios Operacionales

## 1. Navegación Determinista

Los agentes deben priorizar:
- flujos declarados
- rutas semánticas
- acciones explícitas
- objetivos estables

Los agentes deben evitar:
- exploración aleatoria
- rescaneos excesivos
- adivinación heurística
- navegación reactiva puramente visual

---

## 2. Continuidad Operacional

Los agentes deben mantener una ejecución operacional lineal siempre que sea posible.

Comportamiento recomendado:
1. analizar
2. planificar
3. ejecutar
4. verificar
5. continuar

Evitar:
- interrupciones innecesarias
- reinterpretación repetida
- rescaneos recursivos
- bucles de cambio de contexto

---

## 3. Targeting Semántico

Los agentes deben priorizar:
- acciones declaradas semánticamente
- zonas estables de interfaz
- áreas centrales clicables
- entidades operacionales explícitas

Evitar:
- targeting en bordes
- anclas visuales inestables
- elementos decorativos
- zonas ambiguas de interacción

---

## 4. Ejecución Agrupada

Los agentes deben agrupar acciones compatibles cuando sea operacionalmente seguro.

Ejemplos:
- click + escribir + blur
- seleccionar + confirmar
- abrir + inspeccionar + resumir

Beneficios:
- menor cambio de contexto
- menor fragmentación operacional
- mejor continuidad
- menor densidad de pausas cognitivas

---

# Política de Acciones Peligrosas

## Acciones de Alto Riesgo

Los agentes deben tratar las siguientes acciones como potencialmente peligrosas:

- submit
- purchase
- delete
- confirm
- send
- transfer
- accept
- publish
- overwrite
- authenticate
- mutaciones irreversibles

---

## Confirmación Humana Requerida

Las acciones marcadas con:

```html
agentic-policy="requires-human-confirmation"
```

no deben ejecutarse autónomamente sin aprobación explícita del usuario.

---

## Restricción de Envíos Autónomos

Los agentes deben evitar:
- presionar Enter dentro de formularios
- envíos implícitos
- diálogos de confirmación automáticos
- triggers ocultos de envío

Estrategia recomendada:
- targeting explícito de botones
- confirmación controlada
- verificación visible de acciones

---

# Política de Reanálisis

## Reanalizar SOLO ante fallo

Los agentes no deben reinterpretar continuamente la interfaz.

El reanálisis es recomendado únicamente cuando:
- la ejecución falla
- el targeting falla
- ocurre un desajuste de estado
- no puede localizarse una entidad requerida
- aparece una contradicción semántica

---

## Reanálisis Localizado

Cuando el reanálisis sea necesario:
- inspeccionar únicamente la zona afectada
- preservar el contexto global
- evitar reiniciar completamente el flujo operacional

---

# Guía de Navegación

## Modelo Recomendado

Secuencia recomendada:

1. Leer estructura semántica
2. Identificar entidades operacionales
3. Identificar acción objetivo
4. Verificar restricciones de política
5. Ejecutar interacción agrupada
6. Verificar estado resultante

---

## Comportamiento de Scroll

El scroll debe ser:
- intencional
- direccional
- mínimo
- preservando contexto

Evitar:
- scroll exploratorio
- rescaneo repetido del viewport
- patrones oscilatorios de movimiento

---

# Targeting de Interacción

## Zonas Recomendadas de Click

Preferir:
- clicks centrados
- interiores estables de botones
- zonas explícitas de inputs

Evitar:
- clicks en bordes
- áreas animadas
- regiones visualmente inestables
- capas superpuestas

---

# Seguridad Operacional

## Datos Sensibles

Los agentes deben evitar manejo autónomo de:
- contraseñas
- información bancaria
- confirmaciones legales
- verificación de identidad
- biometría
- información médica

A menos que exista autorización explícita del operador humano.

---

## Acciones Externas

Los agentes deben verificar antes de:
- abrir descargas
- abandonar el dominio actual
- activar pagos
- enviar correos
- modificar datos persistentes

---

# Comportamiento Orientado a Benchmarks

AHP v0.2 introduce comportamientos operacionales destinados a mejorar:

- OTCR
- HDI
- IDS
- OCS
- CPD
- DAA

El protocolo no garantiza mejoras.

Las mejoras observadas siguen siendo experimentales.

---

# Flujo Operacional Recomendado

## Secuencia Operacional Estándar

1. Inspeccionar `agentic.json`
2. Inspeccionar `agentic-map.json`
3. Inspeccionar `AHP-SKILL.md`
4. Construir plan operacional
5. Ejecutar navegación determinista
6. Minimizar exploración heurística
7. Reanalizar únicamente si es necesario
8. Verificar estado final
9. Reportar observaciones operacionales

---

# No Objetivos

AHP NO intenta:
- reemplazar navegadores
- reemplazar APIs
- reemplazar estándares de accesibilidad
- forzar ejecución autónoma
- crear interfaces ocultas solo para máquinas
- eliminar humanos del flujo de interacción

---

# Estado Experimental

AHP v0.2 es un protocolo experimental de investigación.

Las observaciones operacionales actuales:
- son exploratorias
- no están validadas estadísticamente
- no son estándares web oficiales
- no deben interpretarse como garantías universales de rendimiento

Se recomiendan benchmarks y experimentos independientes adicionales.

---

# Principio Humano

El objetivo de la semántica operacional no es reemplazar humanos.

El objetivo es reducir ambigüedad entre:
- interfaces
- humanos
- y sistemas inteligentes

La comprensión humana sigue siendo prioritaria.
