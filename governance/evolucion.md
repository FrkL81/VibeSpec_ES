# Evolución y versionado del estándar VibeSpec

## Filosofía

VibeSpec es un estándar vivo. La tecnología, las herramientas y las
prácticas de la industria cambian; el estándar debe adaptarse sin perder
estabilidad. La evolución sigue el principio **P7 – Mejora continua del
propio proceso**.

## Ciclo de revisión

- **Revisión menor (trimestral)**: el equipo evalúa las desviaciones
  acumuladas, las métricas de adopción y las lecciones aprendidas.
  Propone ajustes a los criterios, umbrales o checklists.
- **Revisión mayor (anual)**: se actualiza la versión principal del
  estándar, se incorporan nuevas fases si la industria las ha consolidado
  y se publica para la comunidad.

## Proceso de cambio

1. **Propuesta**: cualquier miembro del equipo abre un issue en el
   repositorio explicando el cambio sugerido, su motivación y evidencias
   (datos, incidentes, referencias).
2. **Discusión**: período de comentarios de al menos dos semanas para
   cambios menores, un mes para mayores.
3. **Adopción**: si hay consenso, se actualiza el documento
   correspondiente (`vibespec-lite.md`, `vibespec-pro.md` o
   `vibespec-check.md`), se incrementa la versión y se comunica al
   equipo.
4. **Registro**: el cambio queda documentado en un `CHANGELOG.md` en la
   raíz del repositorio.

## Versionado

Se sigue un esquema **MAJOR.MINOR**:

- **MAJOR**: cambio estructural (nueva fase de checklist, nuevo
  principio, redefinición del rol).
- **MINOR**: ajustes de criterios, redacción, umbrales, ejemplos.

Las "Skills" también deben versionarse junto con el estándar, ya que un
cambio en la checklist de Markdown debe reflejarse en el prompt del agente.

**Versión actual:** `1.0` (abril 2026).

## Compatibilidad

Una versión MAJOR puede requerir recalificación del nivel de madurez del
equipo. Las versiones MINOR son retrocompatibles (los checklists
existentes siguen siendo válidos, con criterios añadidos o refinados).
