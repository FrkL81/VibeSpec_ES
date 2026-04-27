# VibeSpec Check — Lista maestra de verificación

Aplica el bloque correspondiente después de cada ciclo Humano↔IA.

---

## Generación de código (Lite + Pro)

| # | Criterio | Cómo comprobarlo | Umbral de aceptación | Si falla… |
| - | -------- | ---------------- | -------------------- | --------- |
| C1 | Legibilidad y estándares | Linter + revisión visual | Sin errores de estilo | Reformatear |
| C2 | Corrección funcional | Ejecutar tests o probar | Hace lo pedido | Corregir con más contexto |
| C3 | Manejo de errores | Revisar paths de error | Sin catch vacíos | Añadir manejo de errores |
| C4 | Seguridad básica | Inspección visual de secretos/vulns | Sin passwords, URLs falsas, inyecciones | Reparar vulnerabilidad |
| C5 | Dependencias seguras | Verificar contra lista blanca | Sin librerías desconocidas u obsoletas | Sustituir dependencia |
| C6 | Sin alucinaciones | Ejecutar y revisar APIs | Sin funciones inexistentes | Sustituir partes alucinadas |

---

## Planificación / Arquitectura (Pro)

| # | Criterio | Cómo comprobarlo | Umbral de aceptación | Si falla… |
| - | -------- | ---------------- | -------------------- | --------- |
| P1 | Intención documentada | Inspeccionar spec/prompt | Existe spec vinculada | Reconstruir documentación |
| P2 | Alternativas consideradas | Revisar historial | Análisis comparativo registrado | Solicitar alternativas |
| P3 | Alineación con constitución | Comparar con CONSTITUTION.md | Sin violaciones sin justificar | Rechazar propuesta |
| P4 | Viabilidad de contexto | Verificar prompt/archivos | Todos los sistemas relevantes mencionados | Enriquecer contexto |
| P5 | No sobrediseño | Revisión por pares | Solución más simple aprobada | Simplificar especificación |

---

## Implementación de funcionalidades (Pro)

| # | Criterio | Cómo comprobarlo | Umbral de aceptación | Si falla… |
| - | -------- | ---------------- | -------------------- | --------- |
| F1 | Criterios de aceptación cubiertos | Mapeo criterio‑test | Todos los criterios tienen test | Implementar faltante |
| F2 | Traza completa | Verificar referencia en commit | Vínculo a issue/spec | Añadir traza |
| F3 | Sin regresiones | Suite completa | Cero fallos | Corregir o documentar cambio |
| F4 | Documentación actualizada | Diff de docs | Refleja nueva funcionalidad | Actualizar docs |
| F5 | Deuda técnica evaluada | Revisión de mantenibilidad | Aprobada o deuda registrada | Refactorizar o planificar |

---

## Refactorización / Optimización (Pro)

| # | Criterio | Cómo comprobarlo | Umbral de aceptación | Si falla… |
| - | -------- | ---------------- | -------------------- | --------- |
| R1 | Comportamiento preservado | Suite de tests | Cero regresiones | Revertir o ajustar |
| R2 | Mejora objetiva | Comparar métricas (complejidad, duplicación) | Métricas mejoran o se mantienen | Reconsiderar cambio |
| R3 | Sin nueva deuda | SAST + revisión | Cero nuevos avisos | Corregir antes de merge |
| R4 | Revisión de impacto | Notificar a afectados | Revisión recibida | Ampliar revisión |

---

## Depuración / Testing & Validación (Pro)

| # | Criterio | Cómo comprobarlo | Umbral de aceptación | Si falla… |
| - | -------- | ---------------- | -------------------- | --------- |
| D1 | Diagnóstico validado | Reproducción + evidencia | Causa raíz explica síntomas | Iterar diagnóstico |
| D2 | Cobertura adecuada | Revisión de tests + mutación | Casos borde cubiertos | Ampliar tests |
| D3 | No enmascaramiento | Revisar diff | Sin catch vacíos | Manejar error adecuadamente |
| D4 | Test de regresión | Incluir test específico en commit | Test falla antes, pasa después | Añadir test de regresión |

---

## Despliegue / Integración en producción (Pro)

| # | Criterio | Cómo comprobarlo | Umbral de aceptación | Si falla… |
| - | -------- | ---------------- | -------------------- | --------- |
| DP1 | Idempotencia y atomicidad | Ejecutar 2 veces en staging | Segunda ejecución sin errores | Corregir script |
| DP2 | Gestión de secretos | Escaneo automático | Cero secretos expuestos | Eliminar y rotar |
| DP3 | Plan de rollback definido | Simulación o documento | Procedimiento probado | Diseñar rollback |
| DP4 | Monitorización post‑deploy | Revisar alertas/config | Alertas para KPIs nuevos | Configurar antes de deploy |
| DP5 | Aprobación de cambio en producción | Registro en tool de despliegue | Aprobación registrada | Obtener autorización |

---

## Uso de esta lista

1. Copia la tabla correspondiente a tu fase y pégala en el PR, issue o
   descripción de la tarea.
2. Marca cada ítem como superado (✅) o fallido (❌).
3. Para cada ❌, añade un comentario con la acción correctiva tomada.
4. Si decides omitir un ítem, documenta la desviación con la plantilla
   `templates/desviacion-template.md`.
