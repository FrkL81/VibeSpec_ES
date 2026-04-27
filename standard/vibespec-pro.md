# VibeSpec Pro – Estándar de desarrollo colaborativo humano/IA (Nivel empresarial)

**Versión 1.0**
**Extensión de VibeSpec Lite**

---

## 1. Introducción

VibeSpec Pro extiende el estándar esencial (VibeSpec Lite) para cubrir el ciclo de vida completo en proyectos empresariales, de misión crítica o multi‑repositorio. Adopta la totalidad de los principios fundamentales y añade fases avanzadas de verificación, métricas de calidad y gobernanza del proceso humano‑IA.

Este documento asume que el equipo ya aplica los principios P1‑P7 y las checklists C1‑C6 definidas en VibeSpec Lite. No las repite; las complementa con las fases de planificación, funcionalidad, refactorización, depuración y despliegue, así como con un sistema de adopción por niveles y métricas de éxito.

---

## 2. Principios (recordatorio)

Los siete principios de VibeSpec (P1‑P7) son universales y rigen para este nivel. Se encuentran detallados en `vibespec-lite.md` y se resumen aquí:

- **P1** Intención explícita antes de ejecución
- **P2** Ciclo cerrado Humano‑IA con verificación obligatoria
- **P3** Contexto como activo de proyecto
- **P4** Trazabilidad y control de cambios
- **P5** Seguridad desde el diseño (Secure‑by‑Design)
- **P6** Gobernanza humana de las decisiones de diseño
- **P7** Mejora continua del propio proceso

---

## 3. El nuevo rol del programador (visión empresarial)

En el nivel Pro, el programador se consolida como **arquitecto de contexto, auditor de seguridad y estabilidad, curador de calidad y tomador de decisiones finales**. Además de las competencias descritas en Lite, asume responsabilidades ampliadas:

- **Gobernanza de IA empresarial**: cumplimiento normativo, autorización de despliegues, gestión de riesgos.
- **Diseño de ecosistemas de agentes**: configuración de MCP, Skills y agentes personalizados.
- **Supervisión de métricas y SLIs**: definición de indicadores para evaluar la efectividad del binomio humano‑IA.

---

## 4. Checklists complementarias (solo Pro)

Las checklists marcadas con asterisco (*) son exclusivas del nivel Pro y se aplican **sin excepción** tras cada interacción de la IA que genere artefactos en las fases que cubren.

### 4.1 Planificación / arquitectura

(Checklist P1‑P5 del estándar completo)

| # | Criterio | Método | Umbral | Acción correctiva |
| - | -------- | ------ | ------ | ----------------- |
| P1* | Intención documentada | Inspección de spec/prompt | Spec vinculada a la propuesta | Reconstruir documentación |
| P2* | Alternativas consideradas | Revisar historial | Análisis comparativo registrado | Solicitar alternativas |
| P3* | Alineación con constitución | Comparar con CONSTITUTION.md | Sin violaciones sin justificar | Rechazar propuesta |
| P4* | Viabilidad de contexto | Verificar prompt/archivos | Todos los sistemas relevantes mencionados | Enriquecer contexto |
| P5* | No sobrediseño | Revisión por pares | Solución más simple aprobada | Simplificar especificación |

### 4.2 Generación de código

(Idéntica a la checklist C1‑C6 de Lite; no se repite aquí.)

### 4.3 Implementación de funcionalidades

(Checklist F1‑F5 del estándar completo)

| # | Criterio | Método | Umbral | Acción correctiva |
| - | -------- | ------ | ------ | ----------------- |
| F1* | Especificación de aceptación cubierta | Mapeo criterio‑test | Todos los criterios tienen test | Implementar faltante |
| F2* | Integridad de la traza | Verificar referencia en commit | Vínculo a issue/spec | Añadir traza |
| F3* | Pruebas de regresión | Suite completa | Cero fallos | Corregir o documentar cambio |
| F4* | Documentación actualizada | Diff de docs | Refleja nueva funcionalidad | Actualizar docs |
| F5* | Revisión de deuda técnica | Revisión mantenibilidad | Aprobada o deuda registrada | Refactorizar o planificar |

### 4.4 Refactorización / optimización

(Checklist R1‑R4)

| # | Criterio | Método | Umbral | Acción correctiva |
| - | -------- | ------ | ------ | ----------------- |
| R1* | Comportamiento preservado | Suite de tests | Cero regresiones | Revertir o ajustar |
| R2* | Mejora objetiva | Comparar métricas | Métricas mejoran o se mantienen | Reconsiderar cambio |
| R3* | Sin nueva deuda | SAST + revisión | Cero nuevos avisos | Corregir antes de merge |
| R4* | Revisión de impacto | Notificar a afectados | Revisión recibida | Ampliar revisión |

### 4.5 Depuración / testing & validación

(Checklist D1‑D4)

| # | Criterio | Método | Umbral | Acción correctiva |
| - | -------- | ------ | ------ | ----------------- |
| D1* | Diagnóstico validado | Reproducción + evidencia | Causa raíz explica síntomas | Iterar diagnóstico |
| D2* | Cobertura de tests adecuada | Revisión tests + mutación | Casos borde cubiertos | Ampliar tests |
| D3* | No enmascaramiento | Revisar diff | Sin catch vacíos | Manejar error adecuadamente |
| D4* | Reintroducción prevenida | Test de regresión en commit | Test falla antes, pasa después | Añadir test de regresión |

### 4.6 Despliegue / integración en producción

(Checklist DP1‑DP5)

| # | Criterio | Método | Umbral | Acción correctiva |
| - | -------- | ------ | ------ | ----------------- |
| DP1* | Idempotencia y atomicidad | Ejecutar 2 veces en staging | Segunda ejecución sin errores | Corregir script |
| DP2* | Gestión de secretos | Escaneo automático | Cero secretos expuestos | Eliminar y rotar |
| DP3* | Plan de rollback definido | Simulación/documentación | Procedimiento probado | Diseñar rollback |
| DP4* | Monitorización post‑deploy | Revisar configuración de alertas | Alertas para KPIs nuevos | Configurar antes de deploy |
| DP5* | Aprobación de cambio en producción | Registro en tool de despliegue | Aprobación registrada | Obtener autorización |

---

## 5. Guía de implementación (Nivel Pro)

### 5.1 Adopción progresiva (recordatorio)

VibeSpec Pro corresponde al nivel 3 (Avanzado) de la ruta de adopción. El equipo debe haber consolidado los niveles Esencial (Lite) y Estructurado.

**Ruta de madurez:**

- **Nivel 1 – Esencial**: principios P1‑P2, checklist C1‑C6, contexto básico (`AGENTS.md`).
- **Nivel 2 – Estructurado**: incluye checklists de planificación y funcionalidad, especificaciones ligeras.
- **Nivel 3 – Avanzado (Pro)**: catálogo completo de checklists, trazabilidad obligatoria, métricas, MCP, gobernanza de desviaciones.

### 5.1.1 Specification-Driven Development (SDD) vs. Vibecoding
A nivel empresarial, VibeSpec rechaza el *vibecoding* (delegación informal y rápida sin revisión) a favor del **SDD**. El ciclo exigido es: la especificación detallada precede a la generación; el agente implementa basándose en la especificación, y el humano valida contra ella. La *spec* es el artefacto central.

### 5.2 Métricas de éxito

Se monitorizan, como mínimo, las siguientes métricas una vez alcanzado el nivel Pro:

- **Tasa de defectos escapados** originados en código generado por IA.
- **Tiempo de revisión por PR** (no debe dispararse).
- **Cobertura de pruebas** y su evolución.
- **Deuda técnica registrada** (tareas del checklist F5/R4 pendientes).
- **Adherencia al estándar**: porcentaje de interacciones con checklist documentada.

### 5.3 Flexibilidad documentada y gobernanza

El estándar es una línea base. Cualquier omisión de una checklist Pro debe registrarse como **desviación documentada** en el PR o issue correspondiente, explicando:

- Qué ítem se omite.
- Por qué es seguro en ese contexto.
- Fecha y responsable que la autoriza.

Las adiciones frecuentes de nuevos controles se consolidan en una revisión trimestral del estándar, que eleva la versión y se comunica al equipo.

---

## 6. Referencias conceptuales

- Principios de Secure‑by‑Design aplicados a outputs de IA.
- Human‑in‑the‑loop como requisito de sistemas de IA confiables.
- Spec‑Driven Development y trazabilidad spec‑tasks‑código.
- Model Context Protocol (MCP) para interoperabilidad de agentes.
- GitOps e Infraestructura como Código para despliegues seguros.

---

*Documento vivo. Última actualización: 2026‑04‑24. Consulte el repositorio para versiones posteriores.*
