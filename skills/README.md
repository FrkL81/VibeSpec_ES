# 🧠 VibeSpec Skills — Guía de integración para Agentes IA

Las "Skills" de VibeSpec son instrucciones (system prompts) que transforman tu IDE o CLI en un participante activo del estándar. En lugar de que tú tengas que recordar hacer el checklist, la IA te obligará a hacerlo.

## ⚙️ Cómo instalar las Skills base

Dependiendo de tu entorno de desarrollo, copia el contenido de `vibespec-lite.md` o `vibespec-pro.md` en el archivo de configuración correspondiente de tu proyecto:

- **Cursor IDE:** Pégalo en un archivo llamado `.cursorrules` en la raíz.
- **Windsurf (Cascade):** Añádelo a tus "Memories" o reglas de proyecto.
- **Claude Code (CLI):** Guárdalo en un archivo `CLAUDE.md`.
- **GitHub Copilot:** Guárdalo en `.github/copilot-instructions.md`.
- **Sistemas modulares (ej. Antigravity):** Guárdalo en tu carpeta `.agent/skills/`.

---

## 🛠️ Tutorial: Cómo crear Skills personalizadas (Desviaciones)

A veces, un proyecto requiere "desviarse" temporal o permanentemente del estándar (por ejemplo, omitir la validación de tests en un prototipo rápido, tal como permite VibeSpec). Para evitar que la IA te exija pasos innecesarios y genere fricción, debes crear una **Skill de Desviación**.

### Pasos para crear una Skill de Desviación

1. **Documenta la desviación humana:** Crea tu archivo en `checklists/templates/desviacion-template.md` (ej. omitir el paso F1 - Tests).
2. **Duplica la Skill base:** Copia tu archivo `vibespec-lite.md` o `vibespec-pro.md`.
3. **Inyecta el contexto de la desviación:** Añade una sección de "EXCEPCIONES ACTIVAS" en las instrucciones del prompt.

### Ejemplo de Skill adaptada para un prototipo rápido:

```markdown
# VibeSpec Pro - Proyecto: Prototipo Dashboard
... [Instrucciones base de VibeSpec Pro] ...

EXCEPCIONES ACTIVAS (DESVIACIONES APROBADAS):
- **Omitir F1 y D2 (Cobertura de Tests):** Estamos en fase de prototipado rápido hasta el 2026-05-01. NO generes pruebas unitarias a menos que se te pida explícitamente, y NO incluyas los puntos F1 ni D2 en el checklist de verificación final.
- **Omitir P5 (No Sobrediseño):** Se permite utilizar capas de abstracción extra para acelerar la maquetación.

[Resto de las reglas de ejecución...]
```

Al enseñarle a la IA las desviaciones aprobadas, mantienes el control arquitectónico sin perder la velocidad del vibecoding.
