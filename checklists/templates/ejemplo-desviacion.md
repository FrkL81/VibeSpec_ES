# Desviación del estándar VibeSpec — Ejemplo real

**Fecha:** 2026‑04‑10
**Solicitante:** @maria_dev
**Aprobador:** @tech_lead
**Fase y criterio omitido:** Planificación P5 – No sobrediseño
**Alcance:** PR #342 (prototipo de dashboard interno)

---

## Justificación

Se trata de un prototipo desechable para una demo interna con fecha de
caducidad explícita (2026‑04‑20). Incluye una capa de abstracción
adicional para acelerar la iteración, aunque técnicamente viola el
principio de "solución más simple". La alternativa simple habría
requerido reimplementar componentes manualmente en dos días, retrasando
la demo. Se acepta la desviación con el compromiso de eliminar el código
si el prototipo no se promociona a desarrollo real.

## Duración

- **¿Es permanente?** No
- **Fecha de caducidad:** 2026‑04‑20
- **Condición de re‑evaluación:** Si se decide promocionar el prototipo,
  se refactorizará eliminando la capa extra.

## Registro

- **Issue/PR:** #342
- **Comentario en PR:** <https://github.com/equipo/proyecto/pull/342#discussion>
