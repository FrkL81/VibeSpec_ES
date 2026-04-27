# Plantillas de Prompting Estructurado

Patrones recomendados por VibeSpec para interactuar con agentes de IA minimizando la ambigüedad y maximizando el rigor técnico.

## 1. Plantilla: Debugging

```text
## CONTEXTO DEL ERROR
Mensaje de error: [pegar mensaje exacto]
Stack trace:[pegar stack trace]
Último cambio relevante: [qué se modificó recientemente]

## CÓDIGO INVOLUCRADO
[pegar el método o clase relevante]

## LO QUE YA INTENTÉ
[lista de lo ya probado, para evitar sugerencias redundantes]

## PREGUNTA
¿Cuál es la causa raíz y cuál es la corrección mínima necesaria?
No refactorices nada más allá del bug específico.
```

## 2. Plantilla: Refactorización

```text
## OBJETIVO DE LA REFACTORIZACIÓN
[Qué problema específico se quiere resolver: legibilidad, duplicación, acoplamiento]

## RESTRICCIONES
- No cambiar la interfaz pública.
- Mantener compatibilidad con [versión/plataforma].
- Conservar comentarios de documentación existentes.

## CÓDIGO A REFACTORIZAR
[código actual]

## FORMATO DE SALIDA
Código completo refactorizado, seguido de una lista de los cambios realizados y su justificación.
```

## 3. Plantilla: Generación de tests

```text
## MÉTODO A TESTEAR[código del método]

## FRAMEWORK
[xUnit / NUnit / pytest / Jest]

## CASOS A CUBRIR
- Happy path: [descripción]
- Edge cases:[lista de casos borde conocidos]
- Error cases: [qué errores debe manejar]

## RESTRICCIONES
Sin dependencias externas reales (usar mocks/stubs para todo lo externo).
