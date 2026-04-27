# Ruta de adopción y métricas de madurez

## Niveles de adopción

| Nivel | Denominación | Perfil del equipo | Fases de checklist activas | Métrica de conformidad esperada |
| ----- | ------------ | ----------------- | -------------------------- | ------------------------------- |
| 1 | **VibeSpec Lite** | Principiante, proyecto pequeño | C1‑C6 | ≥ 90% de PRs |
| 2 | **VibeSpec Estructurado** | Equipo mediano, proyecto en crecimiento | Lite + P, F | ≥ 85% de PRs |
| 3 | **VibeSpec Pro** | Empresarial, misión crítica | Todas | ≥ 80% de PRs (por complejidad) |

## Cómo subir de nivel

1. Dominar el nivel actual durante al menos dos sprints.
2. Incorporar la nueva fase de checklist y medir el impacto (defectos,
   tiempo de revisión).
3. Automatizar todo lo posible antes de añadir más controles manuales.
4. Revisar y aprobar el ascenso en la retrospectiva del equipo.

## Métricas de éxito

| Métrica | Nivel Lite | Nivel Pro |
| ------- | ---------- | --------- |
| **% PRs con checklist completada** | > 90 % | > 80 % |
| **Tasa de defectos escapados** (código generado) | Medir para línea base | Reducir respecto a línea base |
| **Tiempo medio de revisión (min/PR)** | No debe duplicarse | Mantenerse < 150 % del valor sin IA |
| **Deuda técnica registrada vs resuelta** | Tomar conciencia | Ratio < 1.5 (se resuelve al menos el 40 % por sprint) |

## Indicadores de alerta temprana

- Más de un 20 % de PRs sin checklist → retroceder a fundamentos.
- Aumento de defectos en producción coincidiendo con adopción de IA →
  reforzar verificación.
- Fatiga de revisiones → automatizar checks repetitivos (linters,
  escáneres, tests).
