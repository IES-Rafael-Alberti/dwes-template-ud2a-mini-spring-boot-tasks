# Aprendizaje — Mini Spring Boot Tasks

## Evolución de la API

### De v1 a v2

- ¿Qué control de la respuesta HTTP permite añadir `ResponseEntity`?
- ¿Qué cambió en el estado o las cabeceras devueltas?

### De v2 a v3

- ¿Qué aporta JPA/H2 frente a guardar tareas en memoria?
- ¿Qué responsabilidades aparecen en el repositorio y el manejador de errores?

### De v3 a v4

- ¿Qué lógica se trasladó a `TaskService` y por qué?
- ¿Qué responsabilidades conserva el controlador?

### De v4 a v4-extras

- Elige una ampliación (búsqueda, paginación, ETag, `HEAD` o `PUT`) y explica
  qué aporta a la API.

## Slice del grupo

| Campo | Decisión / evidencia |
|---|---|
| Operación implementada | |
| Ruta y método HTTP | |
| Clases modificadas | |
| Prueba que verifica el caso correcto | |
| Prueba del caso de error o recurso inexistente | |
| Comando de pruebas y resultado | |

## Decisiones técnicas

Explica brevemente cómo se reparten las responsabilidades entre controlador,
servicio y repositorio en vuestro slice. Enlaza los commits relevantes.
