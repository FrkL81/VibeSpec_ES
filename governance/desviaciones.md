# Política de desviaciones de VibeSpec

Las desviaciones son omisiones documentadas de uno o más criterios de
verificación. Son lícitas y necesarias; el estándar no busca rigidez sino
**control consciente del riesgo**.

## 1. Principio rector

> *Una desviación no documentada es un incumplimiento.*  
> *Una desviación documentada con justificación técnica es una decisión
> profesional.*

## 2. Flujo de una desviación

1. **Identificar** el criterio que no se va a cumplir.
2. **Evaluar** el riesgo y las salvaguardas existentes.
3. **Documentar** usando la plantilla
   [`../checklists/templates/desviacion-template.md`](../checklists/templates/desviacion-template.md).
4. **Obtener aprobación** si la desviación es de nivel Pro. Para Lite,
   se permite auto‑aprobación con notificación al equipo.
5. **Adjuntar** el documento de desviación al PR o issue correspondiente.
6. **Registrar** el enlace en el registro de desviaciones del proyecto.

## 3. Niveles de aprobación

| Nivel del criterio omitido | ¿Quién aprueba? |
| -------------------------- | --------------- |
| Lite (C1‑C6) | Auto‑aprobación + notificar al canal del equipo |
| Pro (resto de fases) | Líder técnico, arquitecto o revisor designado |

## 4. Caducidad y re‑evaluación

- Si la desviación es **temporal**, debe tener fecha de caducidad y una
  condición de re‑evaluación.
- Las desviaciones **permanentes** deben revisarse trimestralmente en la
  revisión del estándar para decidir si se incorporan como regla, se
  ajusta el estándar o se eliminan las condiciones que obligaron a
  desviarse.

## 5. Auditoría

Las desviaciones acumuladas son un indicador de salud del proceso. Una
tasa alta de desviaciones sin mejora del estándar indica fricción. El
equipo debe revisar la colección completa cada trimestre y actuar.
