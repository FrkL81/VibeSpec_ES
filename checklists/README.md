# VibeSpec Check — Listas de verificación colaborativas humano/IA

Esta carpeta contiene las listas de verificación oficiales de VibeSpec.
Están diseñadas para ser aplicadas tras **cada interacción** de la IA que
produzca un artefacto (código, configuración, plan, documentación).

## Estructura

- **`vibespec-check.md`** → Lista maestra con todas las fases.
- **`templates/`** → Plantillas reutilizables en Markdown para integrar en
  tus issues, PRs o herramientas de gestión.
- **`templates/desviacion-template.md`** → Cómo documentar que has omitido
  deliberadamente una verificación.
- **`templates/ejemplo-desviacion.md`** → Un caso real de desviación bien
  documentada.

## Niveles

| Fase | Lite | Pro |
| ---- | ---- | --- |
| Generación de código (C1‑C6) | ✅ Obligatorio | ✅ |
| Planificación (P1‑P5) | Opcional | ✅ Obligatorio |
| Implementación (F1‑F5) | Opcional (recomendado si el proyecto crece) | ✅ |
| Refactorización (R1‑R4) | Opcional | ✅ |
| Depuración (D1‑D4) | Opcional | ✅ |
| Despliegue (DP1‑DP5) | — | ✅ |

La columna "Lite" muestra el núcleo mínimo para empezar.
La columna "Pro" añade las fases exigidas en entornos empresariales.
