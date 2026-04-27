# VibeSpec Lite – Estándar esencial de desarrollo colaborativo humano/IA

**Versión 1.0**
**Para principiantes y proyectos pequeños. Extendido por VibeSpec Pro.**

---

## 1. Introducción

VibeSpec Lite es la puerta de entrada al desarrollo colaborativo con inteligencia artificial. Proporciona el conjunto mínimo de principios, prácticas y checklists para que un principiante o un equipo pequeño pueda empezar a trabajar con IA generativa de forma controlada, segura y con aprendizaje continuo, sin necesidad de adoptar la estructura completa del nivel empresarial.

---

## 2. Principios fundamentales

Estos siete principios son la constitución del proyecto. Deben estar visibles en el repositorio (`CONSTITUTION.md` o similar).

- **P1 – Intención explícita antes de ejecución**: Todo prompt debe declarar el resultado esperado, restricciones y contexto relevante.
- **P2 – Verificación humana obligatoria**: Ningún código generado se integra sin pasar la checklist C1‑C6.
- **P3 – Contexto como activo**: Mantén un archivo de instrucciones (`AGENTS.md`, `.cursor/rules`) con el estilo y restricciones del proyecto.
- **P4 – Trazabilidad básica**: Vincula cada cambio a la tarea o prompt que lo originó.
- **P5 – Seguridad desde el diseño**: El código generado debe cumplir las mismas reglas de seguridad que el manual.
- **P6 – Gobernanza humana**: Las decisiones de diseño (arquitectura, dependencias) las ratifica siempre un humano.
- **P7 – Mejora continua**: Registra lecciones aprendidas y ajusta el proceso.

---

## 3. Rol del programador en VibeSpec Lite

Incluso en el nivel esencial, el desarrollador asume tres funciones básicas:

- **Arquitecto de contexto**: redacta y mantiene el archivo de contexto del proyecto.
- **Auditor**: revisa cada fragmento generado con las checklists C1‑C6.
- **Curador**: decide qué código se conserva, cuál se descarta y qué necesita mejora.

**Regla de oro**: nunca hagas commit de código que no entiendas completamente.

---

## 4. Checklist de generación de código (obligatoria)

Esta checklist se aplica a **todo fragmento de código generado por IA** (función, clase, script, configuración).

| # | Criterio | Cómo comprobarlo | ¿Cómo sé que está bien? | Si falla… |
| - | -------- | ---------------- | ----------------------- | --------- |
| C1 | Legibilidad y estándares | Linter y revisión visual rápida | El linter no reporta errores; los nombres son claros. | Reformatear manualmente o con IA. |
| C2 | Corrección funcional | Ejecutar tests o probar manualmente | El código hace exactamente lo que se pidió. | Corregir con más contexto; no inventar. |
| C3 | Manejo de errores y casos límite | Revisar paths de error y probar con datos extremos | No hay excepciones tragadas; los errores se manejan. | Añadir manejo de errores. |
| C4 | Seguridad básica | Inspección visual de vulnerabilidades obvias (inyecciones, secretos) | No se ven passwords, URLs fake ni comandos peligrosos. | Reparar vulnerabilidad; si no sabes, pregunta a un compañero. |
| C5 | Dependencias seguras | Verificar que las bibliotecas nuevas son conocidas y aprobadas | No introduces librerías desconocidas, obsoletas o con licencia problemática. | Sustituir por alternativa confiable. |
| C6 | Sin alucinaciones | Ejecutar código y revisar referencias a funciones/APIs | El código no llama a funciones inexistentes ni usa URLs inventadas. | Sustituir las partes alucinadas por código real. |

---

## 5. Errores frecuentes y cómo evitarlos

- ❌ Aceptar el primer código sin leerlo.  
  ✅ Leer siempre, ejecutar los tests (o probarlo) y pasar la checklist.

- ❌ Hacer preguntas ambiguas (“arregla esto”, “optimiza el código”).  
  ✅ Ser específico: qué quieres, con qué restricciones y qué criterios de aceptación tienes.

- ❌ No mantener el archivo de contexto actualizado.  
  ✅ Al añadir una nueva regla o convención, inclúyela en `AGENTS.md`.

- ❌ Usar la IA como una caja negra que lo sabe todo.  
  ✅ Verifica, contrasta y aprende de cada interacción.

### 5.1 El riesgo principal: La "Ilusión de Competencia"
La facilidad de obtener código funcionando crea la falsa sensación de haber comprendido algo que no se ha interiorizado. **Mitigación:** Aplica la regla de "Explicar antes de aceptar". Si no puedes explicar en voz alta qué hace el código generado o cómo modificarlo, no lo integres.

---

## 6. Adopción progresiva: ruta de aprendizaje

### Semanas 1‑2: Fundamentos

- Aplica P1 y P2 en absolutamente todo.
- Completa la checklist C1‑C6 manualmente.
- Crea tu primer `AGENTS.md` con el estilo de código y restricciones del proyecto.
- Practica prompts específicos (usa la técnica “prompt → código → checklist”).

### Semanas 3‑4: Consolidación

- Incorpora checklists F1‑F4 (funcionalidades) si el proyecto crece.
- Comienza a escribir especificaciones ligeras (un párrafo con criterios de aceptación).
- Documenta una desviación si alguna vez decides omitir un paso (aprenderás a evaluar riesgos).

**Cuando domines Lite y tu proyecto requiera despliegues frecuentes, múltiples repositorios o cumplimiento normativo, da el salto a VibeSpec Pro.**

---

## 7. Referencia a VibeSpec Pro

Este documento se complementa con el estándar empresarial completo: `vibespec-pro.md`, que añade checklists de planificación, refactorización, depuración y despliegue, métricas de calidad y políticas de gobernanza. VibeSpec Lite es autónomo, pero siempre puedes consultar Pro para inspirar tu evolución.

---

*Documento vivo. Última actualización: 2026‑04‑24.*
