# VibeSpec 🧠

![CodeBlast Header](assets\banner-dark_ES.png)

**El estándar de desarrollo agéntico para mitigar la deuda técnica cognitiva.**

[![Licencia](https://img.shields.io/badge/Licencia-CC%20BY%204.0-blue.svg)](LICENSE.md)

🌍[VibeSpec Repository in English](https://github.com/FrkL81/VibeSpec_EN)

---

## 🧭 ¿Qué es VibeSpec?

**VibeSpec** es el estándar abierto para la colaboración entre humanos y
sistemas de inteligencia artificial en el desarrollo de software. Nace
en 2026, cuando la programación ya no consiste en escribir código sino en
**dirigir intención**, y los agentes de IA se han convertido en
compañeros de equipo.

Define **principios, roles, listas de verificación y métricas** que
permiten a cualquier equipo —independientemente de su tamaño, nivel de
experiencia o herramienta elegida—:

- Traducir ideas en especificaciones ejecutables (**Spec‑Driven
  Development**)
- Mantener el control humano sobre la calidad y la seguridad
- Aprender a colaborar con agentes de IA de forma progresiva
- Escalar desde un prototipo rápido hasta un sistema de misión crítica

---

## 🚀 ¿Por qué VibeSpec?

| Situación actual | Con VibeSpec |
| ---------------- | ------------ |
| Cada herramienta tiene su propio vocabulario y flujo | **[Glosario unificado](standard/glosario.md)** que mapea conceptos comunes a todas las plataformas |
| El “vibe coding” produce código sin revisión que llega a producción | **Checklists obligatorias** que evitan riesgos sin frenar la creatividad |
| No está claro qué rol juega el desarrollador con la IA | **Nuevo rol del programador** como arquitecto, auditor y tomador de decisiones |
| Falta de trazabilidad en las decisiones de la IA | **Traza completa** desde la intención hasta el despliegue |
| Curva de aprendizaje empinada y desorganizada | **Ruta de adopción Lite → Pro** con métricas de madurez |

---

## 📁 Estructura del repositorio

```text
vibespec\
├── checklists\
│   ├── templates\
│   │   ├── ejemplo-desviacion.md
│   │   ├── template-markdown.md
│   │   └── template-yaml.yaml
│   ├── README.md
│   └── vibespec-check.md
├── governance\
│   ├── adopcion.md
│   ├── desviaciones.md
│   ├── evolucion.md
│   └── README.md
├── skills\
│   ├── README.md
│   ├── vibespec-lite.md
│   └── vibespec-pro.md
├── standard\
│   ├── glosario.md
│   ├── plantillas-prompts.md
│   ├── vibespec-lite.md
│   └── vibespec-pro.md
├── LICENSE.md
├── README.md
└── TRADEMARK.md
```

---

## ⚡ Empieza en 2 minutos

1. **Elige tu nivel**  
   - Si eres principiante o estás en un proyecto pequeño → [`standard/vibespec-lite.md`](standard/vibespec-lite.md)  
   - Si trabajas en un entorno empresarial o de alta criticidad → [`standard/vibespec-pro.md`](standard/vibespec-pro.md)

2. **Descarga la checklist maestra**  
   [`checklists/vibespec-check.md`](checklists/vibespec-check.md) y pégala en tu próximo PR.

3. **Crea tu archivo de contexto**  
   Añade un `AGENTS.md` o `.cursor/rules` con las instrucciones que la IA debe seguir.

4. **Instala la Skill de VibeSpec** en tu agente (Cursor, Windsurf, Claude Code) para automatizar los recordatorios.

---

## 🎯 Principios fundamentales

1. **Intención explícita** antes de ejecución  
2. **Verificación humana obligatoria** en cada ciclo  
3. **Contexto como activo** versionable del proyecto  
4. **Trazabilidad y control de cambios** de todas las decisiones  
5. **Seguridad desde el diseño** (Secure‑by‑Design)  
6. **Gobernanza humana** de las decisiones arquitectónicas  
7. **Mejora continua** del propio proceso  

[Ver desarrollo completo →](standard/vibespec-lite.md#2-principios-fundamentales)

---

## 🧑‍🚀 El nuevo rol del programador

El desarrollador ya no es un tecleador de código: es el **arquitecto de
contexto**, el **auditor de seguridad y estabilidad**, el **curador de
calidad** y el **tomador de decisiones finales**. La IA propone, pero la
responsabilidad —técnica, legal y ética— sigue siendo humana.

---

## 📊 Métricas de madurez

| Nivel | Checklist activa | Conformidad esperada |
| ----- | ---------------- | -------------------- |
| **Lite** | C1‑C6 | ≥ 90 % PRs |
| **Estructurado** | Lite + Planificación + Funcionalidad | ≥ 85 % PRs |
| **Pro** | Todas las fases (incluye despliegue) | ≥ 80 % PRs |

[Guía de adopción progresiva →](governance/adopcion.md)

---

## 🤝 Contribuir

VibeSpec es un estándar vivo. Si encuentras un área de mejora, un nuevo
riesgo que cubrir o quieres compartir una plantilla útil:

1. Abre un *issue* describiendo la propuesta.
2. Comenta y debate durante dos semanas (cambios menores) o un mes (cambios mayores).
3. Si hay consenso, se integra en la siguiente revisión.

Consulta [`governance/evolucion.md`](governance/evolucion.md) para el
proceso completo.

---

## 📜 Licencia

El contenido del estándar está bajo **Creative Commons BY 4.0**.  
Los fragmentos de código, bajo **MIT**.  
La marca **VibeSpec™** tiene una política de uso en [`TRADEMARK.md`](TRADEMARK.md).

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

---

## 💖 Apoyo y Donaciones

VibeSpec es un estándar gratuito y abierto, creado para resolver un
problema real: poner orden en el caos de la programación con IA.

Si este estándar te ahorra horas de revisión, te ayuda a desplegar con
seguridad o te da un marco para enseñar a tu equipo, **considera
invitarnos un café** a través del siguiente enlace:

[![Apoyar en Gumroad](https://img.shields.io/badge/Apoyar_en-Gumroad-ff90e8?style=for-the-badge&logo=gumroad&logoColor=black)](https://frkl81.gumroad.com/l/VibeSpecES)

Cada contribución nos permite mantener, mejorar y compartir VibeSpec con
la comunidad.

---

*Diseñado con precisión de estándar y pasión por el código limpio.*

*Creado por Franklin A. Lara P. ([@FrkL81](https://github.com/FrkL81))*
